# Browsers versions

- Firefox: 99.0.1
- Safari MacOS: 14.1.1 (16611.2.7.1.4)

# Signaling state
```
new => have-local-offer => stable => have-remote-offer => stable
```

# Results

- [x] Firefox video on Safari
- [X] Firefox audio on Safari
- [X] Safari video on Firefox
- [X] Safari audio on Firefox

# SDP

<details>
<summary>Firefox SDP (local)</summary>

```
v=0
o=mozilla...THIS_IS_SDPARTA-99.0.1 1894599345761206733 0 IN IP4 0.0.0.0
s=-
t=0 0
a=fingerprint:sha-256 A6:0B:F8:39:47:AC:8D:DF:6D:AD:C7:FB:29:03:15:8F:4B:CF:88:11:71:10:84:36:DA:3D:8F:52:60:84:99:B9
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
a=ice-pwd:255a1defbdcce24aae6351a1ec30f31a
a=ice-ufrag:c4988b6e
a=mid:0
a=msid:{e9831e41-993d-4d46-b2d5-8dad29da04d8} {543609a8-3426-4339-af46-bd37814de188}
a=rtcp-mux
a=rtpmap:109 opus/48000/2
a=rtpmap:9 G722/8000/1
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:101 telephone-event/8000/1
a=setup:actpass
a=ssrc:2902092287 cname:{ddc71945-f6ae-4608-9930-01c67ab35f58}
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
a=ice-pwd:255a1defbdcce24aae6351a1ec30f31a
a=ice-ufrag:c4988b6e
a=mid:1
a=msid:{e9831e41-993d-4d46-b2d5-8dad29da04d8} {761844fc-f8b2-4f68-ac7d-35b28e582050}
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
a=ssrc:1131712597 cname:{ddc71945-f6ae-4608-9930-01c67ab35f58}
a=ssrc:2143080264 cname:{ddc71945-f6ae-4608-9930-01c67ab35f58}
a=ssrc-group:FID 1131712597 2143080264
```

</details>

<details>
<summary>Safari SDP (remote)</summary>

```
v=0
o=- 8790664378260512967 2 IN IP4 127.0.0.1
s=-
t=0 0
a=group:BUNDLE 0 1
a=msid-semantic: WMS
m=audio 9 UDP/TLS/RTP/SAVPF 109 9 0 8 101
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:A1/z
a=ice-pwd:vSrOGfBKc1s/eKHjsuVGIkYC
a=ice-options:trickle
a=fingerprint:sha-256 19:32:2C:7A:53:03:FA:5D:66:99:2F:26:3A:A7:6F:1D:E6:10:E5:18:EB:58:2D:4D:56:D5:E1:F0:FD:51:34:37
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
m=video 9 UDP/TLS/RTP/SAVPF 120 124 126 127 97 98
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:A1/z
a=ice-pwd:vSrOGfBKc1s/eKHjsuVGIkYC
a=ice-options:trickle
a=fingerprint:sha-256 19:32:2C:7A:53:03:FA:5D:66:99:2F:26:3A:A7:6F:1D:E6:10:E5:18:EB:58:2D:4D:56:D5:E1:F0:FD:51:34:37
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
