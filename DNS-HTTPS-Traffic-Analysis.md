# DNS and HTTPS Traffic Analysis

## Objective

Analyze network traffic and identify DNS requests, HTTPS connections and TLS handshakes using Wireshark.

## Tools

- Wireshark
- Windows 11
- Home Network

## Investigation

### DNS Analysis

Observed DNS requests resolving domain names into IP addresses.

Examples:
- google.com
- youtube.com
- github.com

Verified successful name resolution before HTTPS connections were established.

### HTTPS Analysis

Identified encrypted HTTPS traffic between client and server.

Observed:
- TCP 3-Way Handshake
- HTTPS Sessions
- Encrypted Application Data

### TLS Handshake

Analyzed TLS negotiation process.

Observed:

- Client Hello
- Server Hello
- Certificate Exchange
- Key Agreement
- Encrypted Communication

## Findings

- DNS is used to resolve hostnames before communication begins.
- HTTPS protects application traffic using TLS encryption.
- TLS handshake establishes a secure communication channel.

## Conclusion

Successfully analyzed DNS resolution and HTTPS communication flow using Wireshark in a home lab environment.
