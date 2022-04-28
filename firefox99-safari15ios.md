# Browsers versions

- Firefox: 99.0.1
- Safari iOS: 15.2

# Signaling state
```
new => have-local-offer => stable => have-remote-offer => stable
```

# Results

- [x] Firefox video on Safari
- [X] Firefox audio on Safari
- [ ] Safari video on Firefox
- [ ] Safari audio on Firefox

# SDP

<details>
<summary>Firefox SDP (local)</summary>

```
v=0
o=mozilla...THIS_IS_SDPARTA-99.0.1 5389392510466966347 0 IN IP4 0.0.0.0
s=-
t=0 0
a=fingerprint:sha-256 D1:58:BA:AE:37:BC:8B:EF:D0:54:38:D0:AA:B6:1C:93:D2:3D:30:82:75:01:C4:51:7D:2E:2D:A6:44:62:18:71
a=group:BUNDLE 0 1
a=ice-options:trickle
a=msid-semantic:WMS *
m=audio 9 UDP/TLS/RTP/SAVPF 109 9 0 8 101
c=IN IP4 0.0.0.0
a=sendrecv
a=extmap:1 urn:ietf:params:rtp-hdrext:ssrc-audio-level
a=extmap:2/recvonly urn:ietf:params:rtp-hdrext:csrc-audio-level
a=extmap:3 urn:ietf:params:rtp-hdrext:sdes:mid
a=fmtp:109 maxplaybackrate=48000;stereo=1;useinbandfec=1
a=fmtp:101 0-15
a=ice-pwd:26f252f12c5fbf0af234a5e9b568b917
a=ice-ufrag:166e73e0
a=mid:0
a=msid:{62bb28ce-30d3-4707-8bf6-dec72f328137} {5745f07a-729e-44e3-8f3e-d3a32bbab9a1}
a=rtcp-mux
a=rtpmap:109 opus/48000/2
a=rtpmap:9 G722/8000/1
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:101 telephone-event/8000/1
a=setup:actpass
a=ssrc:666131314 cname:{4f06cf33-9c46-48a4-a154-45539154b8f6}
m=video 9 UDP/TLS/RTP/SAVPF 120 124 121 125 126 127 97 98
c=IN IP4 0.0.0.0
a=sendrecv
a=extmap:3 urn:ietf:params:rtp-hdrext:sdes:mid
a=extmap:4 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:5 urn:ietf:params:rtp-hdrext:toffset
a=extmap:6/recvonly http://www.webrtc.org/experiments/rtp-hdrext/playout-delay
a=extmap:7 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=fmtp:126 profile-level-id=42e01f;level-asymmetry-allowed=1;packetization-mode=1
a=fmtp:97 profile-level-id=42e01f;level-asymmetry-allowed=1
a=fmtp:120 max-fs=12288;max-fr=60
a=fmtp:124 apt=120
a=fmtp:121 max-fs=12288;max-fr=60
a=fmtp:125 apt=121
a=fmtp:127 apt=126
a=fmtp:98 apt=97
a=ice-pwd:26f252f12c5fbf0af234a5e9b568b917
a=ice-ufrag:166e73e0
a=mid:1
a=msid:{62bb28ce-30d3-4707-8bf6-dec72f328137} {4e85b132-d62c-4a9c-8824-989f5c1dbd91}
a=rtcp-fb:120 nack
a=rtcp-fb:120 nack pli
a=rtcp-fb:120 ccm fir
a=rtcp-fb:120 goog-remb
a=rtcp-fb:120 transport-cc
a=rtcp-fb:121 nack
a=rtcp-fb:121 nack pli
a=rtcp-fb:121 ccm fir
a=rtcp-fb:121 goog-remb
a=rtcp-fb:121 transport-cc
a=rtcp-fb:126 nack
a=rtcp-fb:126 nack pli
a=rtcp-fb:126 ccm fir
a=rtcp-fb:126 goog-remb
a=rtcp-fb:126 transport-cc
a=rtcp-fb:97 nack
a=rtcp-fb:97 nack pli
a=rtcp-fb:97 ccm fir
a=rtcp-fb:97 goog-remb
a=rtcp-fb:97 transport-cc
a=rtcp-mux
a=rtcp-rsize
a=rtpmap:120 VP8/90000
a=rtpmap:124 rtx/90000
a=rtpmap:121 VP9/90000
a=rtpmap:125 rtx/90000
a=rtpmap:126 H264/90000
a=rtpmap:127 rtx/90000
a=rtpmap:97 H264/90000
a=rtpmap:98 rtx/90000
a=setup:actpass
a=ssrc:2421420840 cname:{4f06cf33-9c46-48a4-a154-45539154b8f6}
a=ssrc:1588910798 cname:{4f06cf33-9c46-48a4-a154-45539154b8f6}
a=ssrc-group:FID 2421420840 1588910798
```

</details>

<details>
<summary>Safari SDP (remote)</summary>

```
v=0
o=- 5137614179833741010 2 IN IP4 127.0.0.1
s=-
t=0 0
a=group:BUNDLE 0 1
a=msid-semantic: WMS
m=audio 9 UDP/TLS/RTP/SAVPF 109 9 0 8 101
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:pWez
a=ice-pwd:0b4U1AtXv9xcBCm363UwAJOV
a=ice-options:trickle
a=fingerprint:sha-256 B0:F0:0D:4A:BF:F4:9A:82:25:1B:C2:85:A6:44:71:BA:08:DB:6A:13:8D:2B:70:6F:AC:E9:F6:8A:7B:04:06:7D
a=setup:active
a=mid:0
a=extmap:1 urn:ietf:params:rtp-hdrext:ssrc-audio-level
a=extmap:3 urn:ietf:params:rtp-hdrext:sdes:mid
a=recvonly
a=rtcp-mux
a=rtpmap:109 opus/48000/2
a=fmtp:109 minptime=10;useinbandfec=1
a=rtpmap:9 G722/8000
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:101 telephone-event/8000
m=video 9 UDP/TLS/RTP/SAVPF 120 124 121 125 126 127 97 98
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:pWez
a=ice-pwd:0b4U1AtXv9xcBCm363UwAJOV
a=ice-options:trickle
a=fingerprint:sha-256 B0:F0:0D:4A:BF:F4:9A:82:25:1B:C2:85:A6:44:71:BA:08:DB:6A:13:8D:2B:70:6F:AC:E9:F6:8A:7B:04:06:7D
a=setup:active
a=mid:1
a=extmap:5 urn:ietf:params:rtp-hdrext:toffset
a=extmap:4 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:7 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=extmap:6 http://www.webrtc.org/experiments/rtp-hdrext/playout-delay
a=extmap:3 urn:ietf:params:rtp-hdrext:sdes:mid
a=recvonly
a=rtcp-mux
a=rtcp-rsize
a=rtpmap:120 VP8/90000
a=rtcp-fb:120 goog-remb
a=rtcp-fb:120 transport-cc
a=rtcp-fb:120 ccm fir
a=rtcp-fb:120 nack
a=rtcp-fb:120 nack pli
a=rtpmap:124 rtx/90000
a=fmtp:124 apt=120
a=rtpmap:121 VP9/90000
a=rtcp-fb:121 goog-remb
a=rtcp-fb:121 transport-cc
a=rtcp-fb:121 ccm fir
a=rtcp-fb:121 nack
a=rtcp-fb:121 nack pli
a=fmtp:121 profile-id=0
a=rtpmap:125 rtx/90000
a=fmtp:125 apt=121
a=rtpmap:126 H264/90000
a=rtcp-fb:126 goog-remb
a=rtcp-fb:126 transport-cc
a=rtcp-fb:126 ccm fir
a=rtcp-fb:126 nack
a=rtcp-fb:126 nack pli
a=fmtp:126 level-asymmetry-allowed=1;packetization-mode=1;profile-level-id=42e01f
a=rtpmap:127 rtx/90000
a=fmtp:127 apt=126
a=rtpmap:97 H264/90000
a=rtcp-fb:97 goog-remb
a=rtcp-fb:97 transport-cc
a=rtcp-fb:97 ccm fir
a=rtcp-fb:97 nack
a=rtcp-fb:97 nack pli
a=fmtp:97 level-asymmetry-allowed=1;packetization-mode=0;profile-level-id=42e01f
a=rtpmap:98 rtx/90000
a=fmtp:98 apt=9
```

</details>
