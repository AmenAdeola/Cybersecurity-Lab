# Network attacks Cheat sheet

Attack Type | Main Protocol | How it works | Impact |
------------|---------------|--------------|--------|
IP Spoofing | IP            | Forges the sources IP address of packets| Hides attacker identify and enables other attacks|
ARP Poisoning| ARP          | Associates the attacker's MAC address with a legitimate IP address.| Traffic interception and redirection|
Man-in-the-middle (MITM)/On-Path Attack| TCP/IP | Positions the attacker between two communicating systems| Data interception and manipulation|
Packet Sniffing |Multiple |Capture network traffic traversing the network| Information disclosure|
Session Hijacking| TCP/HTTP/HTTPS| Takes over a valid authenticated session| Unauthorized account access|
MAC Flooding| Ethernet| Floods a switch with fake MAC addresses.|Forces the switch to broadcast traffic, enabling sniffing.|
DNS Spoofing | DNS| Sends falsified DNS responses to victims| Redirects users to malicious websites|
DHCP Spoofing | DHCP | Rogue DHCP server provides malicious network settings| Traffic redirection and interception|
Evil Twin Attack| WI-FI| Create a fake wireless access point that mimics a legitimate one| Credential theft and traffic interception|
Rogue Access Point | WI-FI|Unauthorized wireless access point connected to network.|Bypass of network security controls|


| Attack | Description | Defensive focus |
|--------|-------------|-----------------|
| Packet sniffing | Captures network traffic | Encryption, switched networks, secure protocols |
| IP spoofing | Forges a source IP address | Ingress/egress filtering, authentication |
| MAC spoofing | Impersonates a network interface | Port security, NAC, monitoring |
| MITM | Intercepts or alters communication | TLS, certificate validation, secure Wi-Fi |
| DNS poisoning | Manipulates name-resolution results | DNSSEC, trusted resolvers, monitoring |
| ARP spoofing | Sends false ARP information | Dynamic ARP inspection, segmentation |
| Session hijacking | Takes over an authenticated session | Secure cookies, MFA, session controls |
| Rogue access point | Unauthorized wireless access point | Wireless monitoring, approved configurations |
| Evil twin | Fake Wi-Fi mimics a legitimate network | Certificate validation, VPN, user awareness |
| Port scanning | Enumerates open services | Reduce exposed services, detection, filtering |  


## Analyst Questions 

- Which hosts communicated?
- Was the source address expected?
- Which protocol and port were involved?
- Did certificates or DNS responses change?
- Are there repeated authentication or session anomalies?
- Does packet evidence match endpoint and SIEM evidence?
