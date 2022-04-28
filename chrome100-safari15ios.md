# Browsers versions

- Chrome: 100.0.4896.127
- Safari iOS: 15.2

# Signaling state
```
new => have-local-offer => stable => have-remote-offer => stable
```

# Results

- [x] Chrome video on Safari
- [X] Chrome audio on Safari
- [ ] Safari video on Chrome
- [ ] Safari audio on Chrome

<details>
<summary>Chrome SDP (local)</summary>

```
v=0
o=mozilla...THIS_IS_SDPARTA-99.0.1 752759619129555288 0 IN IP4 0.0.0.0
s=-
t=0 0
a=fingerprint:sha-256 AA:F3:72:F3:34:B3:B2:72:69:20:86:FD:8C:B8:59:B1:57:C2:E0:B3:C3:46:5D:16:9C:2C:34:50:DA:1A:CF:C6
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
a=ice-pwd:3b75a8e760c5295e5bcf309404f5f633
a=ice-ufrag:15845c69
a=mid:0
a=msid:{dce4a3ba-1188-4439-bfd0-b1bc321dd7db} {f5c0c9ed-c34e-4a6d-b797-3a44af9509c7}
a=rtcp-mux
a=rtpmap:109 opus/48000/2
a=rtpmap:9 G722/8000/1
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:101 telephone-event/8000/1
a=setup:actpass
a=ssrc:223177853 cname:{34a7cae5-2831-4db5-bf62-b85c9ec6640f}
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
a=ice-pwd:3b75a8e760c5295e5bcf309404f5f633
a=ice-ufrag:15845c69
a=mid:1
a=msid:{dce4a3ba-1188-4439-bfd0-b1bc321dd7db} {60841dc1-8487-40f8-9d9c-9b10047b0cd5}
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
a=ssrc:1012011086 cname:{34a7cae5-2831-4db5-bf62-b85c9ec6640f}
a=ssrc:523234647 cname:{34a7cae5-2831-4db5-bf62-b85c9ec6640f}
a=ssrc-group:FID 1012011086 523234647
```
  
</details>

<details>
<summary>Safari SDP (remote)</summary>

```
v=0
o=- 4065081228854667603 2 IN IP4 127.0.0.1
s=-
t=0 0
a=group:BUNDLE 0 1
a=msid-semantic: WMS
m=audio 49582 UDP/TLS/RTP/SAVPF 109 9 0 8 101
c=IN IP4 192.168.100.19
a=rtcp:9 IN IP4 0.0.0.0
a=candidate:1617124397 1 udp 2122262783 2803:c180:2102:7cc1:4d9d:d54:842b:87ca 50653 typ host generation 0 network-id 2 network-cost 10
a=candidate:3463870814 1 udp 2122194687 192.168.100.19 49582 typ host generation 0 network-id 1 network-cost 10
a=ice-ufrag:FLcl
a=ice-pwd:RmdqlPitfwbq0giexmaMpiWZ
a=ice-options:trickle
a=fingerprint:sha-256 FE:F0:5E:1F:E4:0E:18:43:22:71:78:C5:1A:55:17:ED:5F:0A:7B:1F:A7:00:D2:90:5B:51:EA:36:3A:43:7D:8A
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
a=ice-ufrag:FLcl
a=ice-pwd:RmdqlPitfwbq0giexmaMpiWZ
a=ice-options:trickle
a=fingerprint:sha-256 FE:F0:5E:1F:E4:0E:18:43:22:71:78:C5:1A:55:17:ED:5F:0A:7B:1F:A7:00:D2:90:5B:51:EA:36:3A:43:7D:8A
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
a=fmtp:98 apt=97
```
  
</details>
