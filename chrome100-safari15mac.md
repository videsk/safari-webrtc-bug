# Browsers versions

- Chrome: 100.0.4896.127
- Safari MacOS: 15.1 (17612.2.9.1.20)

# Signaling state
```
new => have-local-offer => stable => have-remote-offer => stable
```

# Results

- [x] Chrome video on Safari
- [X] Chrome audio on Safari
- [X] Safari video on Chrome
- [X] Safari audio on Chrome

# SDP

<details>
<summary>Firefox SDP (local)</summary>

```
v=0
o=- 1199995653041531788 2 IN IP4 127.0.0.1
s=-
t=0 0
a=group:BUNDLE 0 1
a=extmap-allow-mixed
a=msid-semantic: WMS SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX
m=audio 9 UDP/TLS/RTP/SAVPF 111 63 103 104 9 0 8 106 105 13 110 112 113 126
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:R8cd
a=ice-pwd:YOZZdgKdJrG9tndNv9GmXgNv
a=ice-options:trickle
a=fingerprint:sha-256 F1:BC:90:CF:BC:31:D2:5C:E4:7A:BD:69:99:60:4B:86:35:C7:1A:F9:FF:2C:01:28:1E:9D:3A:C0:EF:89:D5:24
a=setup:actpass
a=mid:0
a=extmap:1 urn:ietf:params:rtp-hdrext:ssrc-audio-level
a=extmap:2 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:3 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=extmap:4 urn:ietf:params:rtp-hdrext:sdes:mid
a=sendrecv
a=msid:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX 656b320a-1642-46d0-8231-c250ec363def
a=rtcp-mux
a=rtpmap:111 opus/48000/2
a=rtcp-fb:111 transport-cc
a=fmtp:111 minptime=10;useinbandfec=1
a=rtpmap:63 red/48000/2
a=fmtp:63 111/111
a=rtpmap:103 ISAC/16000
a=rtpmap:104 ISAC/32000
a=rtpmap:9 G722/8000
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:106 CN/32000
a=rtpmap:105 CN/16000
a=rtpmap:13 CN/8000
a=rtpmap:110 telephone-event/48000
a=rtpmap:112 telephone-event/32000
a=rtpmap:113 telephone-event/16000
a=rtpmap:126 telephone-event/8000
a=ssrc:2343465030 cname:A49hdNFq/VnyhJEj
a=ssrc:2343465030 msid:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX 656b320a-1642-46d0-8231-c250ec363def
a=ssrc:2343465030 mslabel:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX
a=ssrc:2343465030 label:656b320a-1642-46d0-8231-c250ec363def
m=video 9 UDP/TLS/RTP/SAVPF 96 97 98 99 100 101 127 121 125 107 108 109 124 120 123 119 35 36 41 42 114 115 116
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:R8cd
a=ice-pwd:YOZZdgKdJrG9tndNv9GmXgNv
a=ice-options:trickle
a=fingerprint:sha-256 F1:BC:90:CF:BC:31:D2:5C:E4:7A:BD:69:99:60:4B:86:35:C7:1A:F9:FF:2C:01:28:1E:9D:3A:C0:EF:89:D5:24
a=setup:actpass
a=mid:1
a=extmap:14 urn:ietf:params:rtp-hdrext:toffset
a=extmap:2 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:13 urn:3gpp:video-orientation
a=extmap:3 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=extmap:5 http://www.webrtc.org/experiments/rtp-hdrext/playout-delay
a=extmap:6 http://www.webrtc.org/experiments/rtp-hdrext/video-content-type
a=extmap:7 http://www.webrtc.org/experiments/rtp-hdrext/video-timing
a=extmap:8 http://www.webrtc.org/experiments/rtp-hdrext/color-space
a=extmap:4 urn:ietf:params:rtp-hdrext:sdes:mid
a=extmap:10 urn:ietf:params:rtp-hdrext:sdes:rtp-stream-id
a=extmap:11 urn:ietf:params:rtp-hdrext:sdes:repaired-rtp-stream-id
a=sendrecv
a=msid:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX 31592c6b-4bf4-4a59-b32b-6f8d9492d901
a=rtcp-mux
a=rtcp-rsize
a=rtpmap:96 VP8/90000
a=rtcp-fb:96 goog-remb
a=rtcp-fb:96 transport-cc
a=rtcp-fb:96 ccm fir
a=rtcp-fb:96 nack
a=rtcp-fb:96 nack pli
a=rtpmap:97 rtx/90000
a=fmtp:97 apt=96
a=rtpmap:98 VP9/90000
a=rtcp-fb:98 goog-remb
a=rtcp-fb:98 transport-cc
a=rtcp-fb:98 ccm fir
a=rtcp-fb:98 nack
a=rtcp-fb:98 nack pli
a=fmtp:98 profile-id=0
a=rtpmap:99 rtx/90000
a=fmtp:99 apt=98
a=rtpmap:100 VP9/90000
a=rtcp-fb:100 goog-remb
a=rtcp-fb:100 transport-cc
a=rtcp-fb:100 ccm fir
a=rtcp-fb:100 nack
a=rtcp-fb:100 nack pli
a=fmtp:100 profile-id=2
a=rtpmap:101 rtx/90000
a=fmtp:101 apt=100
a=rtpmap:127 H264/90000
a=rtcp-fb:127 goog-remb
a=rtcp-fb:127 transport-cc
a=rtcp-fb:127 ccm fir
a=rtcp-fb:127 nack
a=rtcp-fb:127 nack pli
a=fmtp:127 level-asymmetry-allowed=1;packetization-mode=1;profile-level-id=42001f
a=rtpmap:121 rtx/90000
a=fmtp:121 apt=127
a=rtpmap:125 H264/90000
a=rtcp-fb:125 goog-remb
a=rtcp-fb:125 transport-cc
a=rtcp-fb:125 ccm fir
a=rtcp-fb:125 nack
a=rtcp-fb:125 nack pli
a=fmtp:125 level-asymmetry-allowed=1;packetization-mode=0;profile-level-id=42001f
a=rtpmap:107 rtx/90000
a=fmtp:107 apt=125
a=rtpmap:108 H264/90000
a=rtcp-fb:108 goog-remb
a=rtcp-fb:108 transport-cc
a=rtcp-fb:108 ccm fir
a=rtcp-fb:108 nack
a=rtcp-fb:108 nack pli
a=fmtp:108 level-asymmetry-allowed=1;packetization-mode=1;profile-level-id=42e01f
a=rtpmap:109 rtx/90000
a=fmtp:109 apt=108
a=rtpmap:124 H264/90000
a=rtcp-fb:124 goog-remb
a=rtcp-fb:124 transport-cc
a=rtcp-fb:124 ccm fir
a=rtcp-fb:124 nack
a=rtcp-fb:124 nack pli
a=fmtp:124 level-asymmetry-allowed=1;packetization-mode=0;profile-level-id=42e01f
a=rtpmap:120 rtx/90000
a=fmtp:120 apt=124
a=rtpmap:123 H264/90000
a=rtcp-fb:123 goog-remb
a=rtcp-fb:123 transport-cc
a=rtcp-fb:123 ccm fir
a=rtcp-fb:123 nack
a=rtcp-fb:123 nack pli
a=fmtp:123 level-asymmetry-allowed=1;packetization-mode=1;profile-level-id=4d001f
a=rtpmap:119 rtx/90000
a=fmtp:119 apt=123
a=rtpmap:35 H264/90000
a=rtcp-fb:35 goog-remb
a=rtcp-fb:35 transport-cc
a=rtcp-fb:35 ccm fir
a=rtcp-fb:35 nack
a=rtcp-fb:35 nack pli
a=fmtp:35 level-asymmetry-allowed=1;packetization-mode=0;profile-level-id=4d001f
a=rtpmap:36 rtx/90000
a=fmtp:36 apt=35
a=rtpmap:41 AV1/90000
a=rtcp-fb:41 goog-remb
a=rtcp-fb:41 transport-cc
a=rtcp-fb:41 ccm fir
a=rtcp-fb:41 nack
a=rtcp-fb:41 nack pli
a=rtpmap:42 rtx/90000
a=fmtp:42 apt=41
a=rtpmap:114 red/90000
a=rtpmap:115 rtx/90000
a=fmtp:115 apt=114
a=rtpmap:116 ulpfec/90000
a=ssrc-group:FID 3833826596 1114541102
a=ssrc:3833826596 cname:A49hdNFq/VnyhJEj
a=ssrc:3833826596 msid:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX 31592c6b-4bf4-4a59-b32b-6f8d9492d901
a=ssrc:3833826596 mslabel:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX
a=ssrc:3833826596 label:31592c6b-4bf4-4a59-b32b-6f8d9492d901
a=ssrc:1114541102 cname:A49hdNFq/VnyhJEj
a=ssrc:1114541102 msid:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX 31592c6b-4bf4-4a59-b32b-6f8d9492d901
a=ssrc:1114541102 mslabel:SEjpN1Aw0j0oQTV9bdSuy3EzFbGMzRtJqsYX
a=ssrc:1114541102 label:31592c6b-4bf4-4a59-b32b-6f8d9492d901
```

</details>

<details>
<summary>Safari SDP (remote)</summary>

```
v=0
o=- 6127579574041048960 2 IN IP4 127.0.0.1
s=-
t=0 0
a=group:BUNDLE 0 1
a=extmap-allow-mixed
a=msid-semantic: WMS
m=audio 9 UDP/TLS/RTP/SAVPF 111 63 103 9 0 8 105 13 110 113 126
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:dmpN
a=ice-pwd:tQZ3XslR2Pm1s7EbAT6vEtph
a=ice-options:trickle
a=fingerprint:sha-256 DB:18:18:48:26:AE:F3:AF:8C:13:F6:45:C9:54:C5:2B:D0:14:A7:25:11:5C:3F:93:73:3A:D8:41:9C:5C:09:4E
a=setup:active
a=mid:0
a=extmap:1 urn:ietf:params:rtp-hdrext:ssrc-audio-level
a=extmap:2 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:3 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=extmap:4 urn:ietf:params:rtp-hdrext:sdes:mid
a=recvonly
a=rtcp-mux
a=rtpmap:111 opus/48000/2
a=rtcp-fb:111 transport-cc
a=fmtp:111 minptime=10;useinbandfec=1
a=rtpmap:63 red/48000/2
a=fmtp:63 111/111
a=rtpmap:103 ISAC/16000
a=rtpmap:9 G722/8000
a=rtpmap:0 PCMU/8000
a=rtpmap:8 PCMA/8000
a=rtpmap:105 CN/16000
a=rtpmap:13 CN/8000
a=rtpmap:110 telephone-event/48000
a=rtpmap:113 telephone-event/16000
a=rtpmap:126 telephone-event/8000
m=video 9 UDP/TLS/RTP/SAVPF 96 97 98 99 108 109 124 120 114 115 116
c=IN IP4 0.0.0.0
a=rtcp:9 IN IP4 0.0.0.0
a=ice-ufrag:dmpN
a=ice-pwd:tQZ3XslR2Pm1s7EbAT6vEtph
a=ice-options:trickle
a=fingerprint:sha-256 DB:18:18:48:26:AE:F3:AF:8C:13:F6:45:C9:54:C5:2B:D0:14:A7:25:11:5C:3F:93:73:3A:D8:41:9C:5C:09:4E
a=setup:active
a=mid:1
a=extmap:14 urn:ietf:params:rtp-hdrext:toffset
a=extmap:2 http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time
a=extmap:13 urn:3gpp:video-orientation
a=extmap:3 http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01
a=extmap:5 http://www.webrtc.org/experiments/rtp-hdrext/playout-delay
a=extmap:6 http://www.webrtc.org/experiments/rtp-hdrext/video-content-type
a=extmap:7 http://www.webrtc.org/experiments/rtp-hdrext/video-timing
a=extmap:8 http://www.webrtc.org/experiments/rtp-hdrext/color-space
a=extmap:4 urn:ietf:params:rtp-hdrext:sdes:mid
a=extmap:10 urn:ietf:params:rtp-hdrext:sdes:rtp-stream-id
a=extmap:11 urn:ietf:params:rtp-hdrext:sdes:repaired-rtp-stream-id
a=recvonly
a=rtcp-mux
a=rtcp-rsize
a=rtpmap:96 VP8/90000
a=rtcp-fb:96 goog-remb
a=rtcp-fb:96 transport-cc
a=rtcp-fb:96 ccm fir
a=rtcp-fb:96 nack
a=rtcp-fb:96 nack pli
a=rtpmap:97 rtx/90000
a=fmtp:97 apt=96
a=rtpmap:98 VP9/90000
a=rtcp-fb:98 goog-remb
a=rtcp-fb:98 transport-cc
a=rtcp-fb:98 ccm fir
a=rtcp-fb:98 nack
a=rtcp-fb:98 nack pli
a=fmtp:98 profile-id=0
a=rtpmap:99 rtx/90000
a=fmtp:99 apt=98
a=rtpmap:108 H264/90000
a=rtcp-fb:108 goog-remb
a=rtcp-fb:108 transport-cc
a=rtcp-fb:108 ccm fir
a=rtcp-fb:108 nack
a=rtcp-fb:108 nack pli
a=fmtp:108 level-asymmetry-allowed=1;packetization-mode=1;profile-level-id=42e01f
a=rtpmap:109 rtx/90000
a=fmtp:109 apt=108
a=rtpmap:124 H264/90000
a=rtcp-fb:124 goog-remb
a=rtcp-fb:124 transport-cc
a=rtcp-fb:124 ccm fir
a=rtcp-fb:124 nack
a=rtcp-fb:124 nack pli
a=fmtp:124 level-asymmetry-allowed=1;packetization-mode=0;profile-level-id=42e01f
a=rtpmap:120 rtx/90000
a=fmtp:120 apt=124
a=rtpmap:114 red/90000
a=rtpmap:115 rtx/90000
a=fmtp:115 apt=114
a=rtpmap:116 ulpfec/90000
```

</details>
