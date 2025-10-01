# HTTPS Analysis (https://www.dawn.com)

7. **Website Name:** www.dawn.com

8. **ClientHello Packet:**
   The ClientHello message is sent in the initial TLS handshake packet.

9. **TLS Extensions in ClientHello:**
   - Server Name Indication (SNI): www.dawn.com
   - Supported Groups (Elliptic Curves)
   - Signature Algorithms
   - Application Layer Protocol Negotiation (ALPN)
   - Key Share

10. **ServerHello Message & Cipher Suite:**
   The server selected the cipher suite:
   `TLS_AES_256_GCM_SHA384`

11. **Certificate Message (Server Certificate):**
   - **Issuer:** DigiCert Global Root G2
   - **Subject:** www.dawn.com
   - **Validity:** From 01-Jul-2025 to 30-Sep-2025

12. **First Encrypted Application Data:**
   After the handshake, the first `Application Data` packet is fully encrypted.
   - We cannot see HTTP headers because TLS encrypts them for confidentiality.
