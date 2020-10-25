## Flow P2P Module Features

Flow is a low-level, stateless, concurrent networking library that easily allows you to incorporate fundamental features any modern p2p application needs such as:

1) cryptographic primitives (Ed25519, PoW, AES-256),
2) message serialization/deserialization schemes (byte-order little endian, protobuf, msgpack),
3) network timeout/error management (on dial, on receive message, on send buffer full),
4) network-level atomic operations (receive-then-lock),
5) and NAT traversal support (NAT-PMP, UPnP).

Flow additionally comes bundled with a high-level `protocol` package comprised of a large number of production-ready, high-level protocol building blocks such as:
1) handshake protocol implementations (Elliptic-Curve Diffie Hellman),
2) peer routing/discovery protocol implementations (S/Kademlia),
3) message broadcasting protocol implementations (S/Kademlia),
4) overlay network protocol implementations (S/Kademlia),
5) cryptographic identity schemes (Ed25519 w/ EdDSA signatures),
6) and authenticated encryption schemes (AES-256 GCM AEAD).

## Componenet
Application layer can define component by themself
## Session establishment
There is only ONE open/privacy connection between same pair nodes;
## Message&Broadcasting
- P2P by default encodes messages as bytes in little-endian order, and provides utility classes to assist with serializing/deserializing arbitrary Go/rust types into bytes efficiently.

The Flow stack is writed in Golang and Rust.
