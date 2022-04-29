# Webkit SDP transceivers bug

The context is when trying to send tracks between peers async. That means sending tracks from peer 1 and when complete the signaling process to `stable`, sending the tracks to peer 2.

```
new => have-local-offer => stable => have-remote-offer => stable
```

**The bug only happens when the peer 1 is any browser in any OS except iOS and the second one Safari/Firefox/Chrome on iOS, and send tracks async.**

# How to reproduce it

1. Get user media with audio and video
2. Create RTCPeerconnection on both peers following the [perfect negotiation](https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API/Perfect_negotiation).
3. Execute `peer1.addTrack(track, cameraStream);`
4. Wait to receive the tracks of peer1 on peer2
5. Add mute/unmute listener to both track `track.addEventListener('mute', event => console.log(event.track.kind, 'muted', event));` and `track.addEventListener('unmute', event => console.log(event.track.kind, 'unmuted', event));`
6. Execute `peer2.addTrack(track, stream);`
7. Expect receive tracks **muted**

Point 7 is where weird things happen. You will receive the tracks as muted, only before transceivers exchange and the direction of `RTCRtpSender` and `RTCRtpReceiver` will be `recvonly`. After transceivers, the tracks will be changed to unmuted, and both transceivers `RTCRtpTransceiver` will change direction value to `sendrecv`, but tracks still empty (no audio, no video).

A human-readable example is the case when Alice calls Bob. Previous to Bob answering the call we show a preview of Alice's camera, when Bob answer we send the Bob tracks. That use case could be complex if you don't create a new RTCPeerconnection on Alice and Bob, that means starting the signaling process again, which is inefficient.

---

If you try send track synchronous between peers works perfect and transceivers direction is `sendrecv`. So, the first conclusion is meanwhile the signaling process is in the process the transceivers' direction will be set as `sendrecv` if you send tracks at the same time, not asynchronous.

# SDP examples
- Chrome 100 and Safari 15.2 iOS ([here](chrome100-safari15ios.md)) ❌
- Chrome 100 and Safari 15.1 macOS ([here](chrome100-safari15mac.md)) ✅
- Firefox 99 and Safari 15.2 iOS ([here](firefox99-safari15ios.md)) ❌
- Firefox 99 and Safari 14.1 macOS ([here](firefox99-safari14mac.md)) ✅

Also, was tested Chrome and Firefox in iOS with the same results as failed examples.

# Conclusion

Only happens in iOS when sending tracks between peers asynchronous, first from not iOS peer and then from the iOS peer.
