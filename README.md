# CombPort
_Fast transmission through Any means, Any platform, Any network, Any data_

## Preface
:partying_face: At present, no unsupported platforms have been found. There is always a transmission method that can run on the platform! :hugs:

Sometimes I am really frustrated with file transfer between different devices without a good solution, so I created the CombPort project with the aim of providing the best transfer service backend for any device.

## Approach
**The identifier marked with "*" does not support WASM.**

### Network
+ [Matchbox](https://github.com/johanhelsing/matchbox)

+ *USB (With [nusb](https://github.com/kevinmehall/nusb))

+ *[WebRTC](https://github.com/webrtc-rs/webrtc) (DataChannel)

_I am considering whether it is necessary to add non P2P connection methods._

### Compression

+ [Snappy](https://github.com/BurntSushi/rust-snappy)

+ [LZ4](https://github.com/rusty-shell/rust-compress)

+ [DEFLATE](https://github.com/rusty-shell/rust-compress)

### Custom Protocol (if needed)

+ *[QUIC](https://github.com/quinn-rs/quinn)

+ *[AP-KCP](https://github.com/black-binary/ap-kcp)