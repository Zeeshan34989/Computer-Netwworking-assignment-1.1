# QUIC (HTTP/3) Analysis (https://quic.rocks)

1. **Website Name:** quic.rocks

2. **Initial QUIC Handshake Packet:**
   The Initial packet carries the QUIC handshake, including the embedded TLS ClientHello.

3. **TLS ClientHello inside QUIC:**
   Found inside the Initial QUIC packet (carried over UDP port 443).

4. **QUIC Version Used:**
   QUIC v1 (draft-29 compatible).

5. **0-RTT or 1-RTT Keys First Used:**
   The first `1-RTT Protected` packet appears after the handshake, allowing secure communication.

6. **First Packet with HTTP/3 Application Data:**
   The first HTTP/3 stream data is carried inside QUIC packet #15.

   **Difference from HTTP/1.1 over TCP:**
   - HTTP/3 runs on QUIC (UDP).
   - No head-of-line blocking (lost packet doesn’t block whole connection).
   - TLS is integrated inside QUIC instead of a separate handshake.
