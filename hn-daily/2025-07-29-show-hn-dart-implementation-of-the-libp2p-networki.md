# Show HN: Dart implementation of the libp2p networking stack

**Posted by stephanfebs on 2025-07-29**

I created a Dart port of the LibP2P stack. My goal was to have a native Dart implementation. Since there is no native QUIC library available, I also developed my own UDP transport called Dart-UDX.

In addition to the core stack, my GitHub repository includes implementations of GossipSub, DHT, and UDX.