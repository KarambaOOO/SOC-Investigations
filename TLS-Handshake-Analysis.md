# TLS Handshake Analysis

## Objective

Analyze the TLS handshake process and understand how secure HTTPS connections are established.

## Tools

- Wireshark
- Windows 11
- Home Network

## Investigation

Captured HTTPS traffic and filtered TLS packets using Wireshark.

Observed the complete TLS handshake sequence:

1. Client Hello
2. Server Hello
3. Certificate Exchange
4. Key Exchange
5. Finished Messages
6. Encrypted Application Data

## Findings

### Client Hello

The client initiated the connection and proposed:

- Supported TLS versions
- Cipher suites
- Extensions
- Server Name Indication (SNI)

### Server Hello

The server selected:

- TLS version
- Cipher suite
- Security parameters

### Certificate Exchange

The server presented its digital certificate.

Verified:

- Certificate Authority (CA)
- Domain name
- Certificate validity period

### Encrypted Communication

After successful negotiation:

- Session keys were established
- Application data became encrypted
- Traffic contents were no longer readable without decryption keys

## Security Importance

TLS provides:

- Confidentiality
- Integrity
- Authentication

This protects users against eavesdropping and man-in-the-middle attacks.

## Conclusion

Successfully analyzed the TLS handshake process using Wireshark and identified the key stages required to establish a secure HTTPS connection.
