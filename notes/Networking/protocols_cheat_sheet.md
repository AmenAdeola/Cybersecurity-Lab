
# Networking Protocols cheat Sheet

| Protocol  | Purpose | Easy way to remember 
|-----------|---------|----------------------|
| DNS       | Translates domain names into IP addresses| Internet phone book 
| IP        | Provides addressing and routing| Delivers packets
| TCP       | Reliable data delivery | Reliable
| UDP       | Fast data delivery |  Fast 
| ICMP      | Reports errors and diagnostics | Troubleshooting
| HTTPS     | Secure web communication | Secure browsing
| DHCP      | Automatically assigns IP addresses | Automatic IP assignment
| ARP       | Maps an IP address to a MAC address| finds physical addresses
| FTP       | Transfers files between systems | File transfer 
| SSH       | Secure remote administration | Secure remote access 


| Protocol | Port | Purpose |
|---|---:|---|
| HTTP | 80 | Unencrypted web traffic |
| HTTPS | 443 | Encrypted web traffic |
| DNS | 53 | Name resolution |
| SSH | 22 | Secure remote administration |
| FTP | 20/21 | File transfer |
| SMTP | 25 | Email transfer |
| POP3 | 110 | Retrieve email |
| IMAP | 143 | Synchronize email |
| DHCP | 67/68 | Dynamic IP configuration |
| RDP | 3389 | Remote desktop |
| SMB | 445 | File and printer sharing |
| NTP | 123 | Time synchronization |  

## Transport  

- TCP: connection-oriented, reliable, ordered.
- UDP: connectionless, lower overhead, no delivery guarantee.
- ICMP: diagnostics and error reporting.

## Secure Alternatives

- HTTPS instead of HTTP
- SFTP or SCP instead of FTP
- SSH instead of Telnet
- Secure email configurations rather than unencrypted legacy protocols

Ports identify expected services, but applications can use non-standard ports. Validate the protocol and payload when possible.





 
