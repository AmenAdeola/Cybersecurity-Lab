# Entry 3: Wireshark Packet Analysis

##Date: September 2026 

Entry Number: 03

## Description

In this activity, I used Wireshark to examine network packets from a packet capture file. The objective was to understand how traffic is organized into protocol layers and how analysts use packet evidence to investigate network activity. I reviewed packet headers, addressing information, protocols, ports, DNS, ICMP, TCP, and HTTP traffic.

## Tools Used
-  Wireshark
-  Packet capture file (PCAP)
-  Wireshark display filters
-  IPv4
-  TCP
-  UDP
-  ICMP
-  DNS
-  HTTP

## The 5 W's

### Who
The packet capture contained network communications between a source system and one or more destination systems. The traffic was examined from the perspective of a cybersecurity analyst.

### What
Wireshark was used to inspect source and destination MAC and IP addresses, protocols, ports, packet lengths, TCP flags, DNS queries and responses, ICMP echo traffic, HTTP requests, and readable payload data.

### When
The activity was completed in September 2026. The exact date should be verified from the original lab records or screenshots. Individual packet timestamps were available in the PCAP.

### Where
The activity was performed in a controlled lab environment using Wireshark and a packet capture file.

### Why
The activity developed practical packet-inspection skills used to validate alerts, identify affected systems, collect indicators, and reconstruct network events.


### Packet Structure

Frame
↓ Ethernet II
↓ Internet Protocol Version 4
↓ TCP, UDP, or ICMP
↓ Application data 

## Important Packet Fields

-  Frame number, arrival time, and length
-  Source and destination MAC addresses
-  Source and destination IP addresses
-  TTL and protocol
-  Source and destination ports
-  TCP flags
-  DNS query and response information
-  HTTP method, URI, host, and payload

### ICMP Analysis
icmp 
ICMP echo request and echo reply traffic can validate connectivity. Unusual volume, timing, or destinations may require additional analysis, but ICMP alone does not confirm malicious activity.

### DNS Analysis
dns udp.port == 53 
DNS queries and responses can connect domain names with returned IP addresses. Analysts review queried domains, source systems, response codes, frequency, and reputation.

### TCP Analysis

SYN → SYN-ACK → ACK 
-  SYN initiates a connection.
-  ACK acknowledges data.
-  FIN closes a connection normally.
-  RST resets a connection.
-  PSH requests prompt delivery of data.

### HTTP Analysis
http tcp.port == 80
tcp contains "curl"
tcp contains "GET" 
Unencrypted HTTP traffic may expose requested resources, hostnames, user-agent strings, query parameters, or other readable content. HTTPS should be used for sensitive communications.

### Display Filters
ip.addr == 142.250.1.139
ip.src == 142.250.1.139
ip.dst == 142.250.1.139
eth.addr == 42:01:ac:15:e0:02
udp.port == 53
tcp.port == 80
tcp contains "curl" 
The example values must be kept only if they match the original lab capture.

### Investigation Workflow
Open PCAP → review packet list → identify protocols → apply filters → inspect addressing and ports → examine payloads → correlate packets → document findings 

## Findings
-  Wireshark organizes network evidence into protocol layers.
-  Ethernet fields describe local-network delivery.
-  IPv4 headers identify communicating systems.
-  ICMP supports connectivity analysis.
-  DNS maps queried domains to IP addresses.
-  TCP flags provide connection-state context.
-  HTTP traffic can expose readable application information.
-  Display filters isolate investigation-relevant traffic.

### Detection Assessment
The presence of ICMP, DNS, TCP, or HTTP traffic does not automatically indicate malicious activity. The analyst must consider authorization, destination reputation, timing, volume, the network baseline, and related endpoint or authentication evidence.


### Potential Response Actions

-  Record source and destination IP addresses, ports, and protocols.
-  Identify relevant domains and affected internal assets.
-  Search SIEM and endpoint logs for related activity.
-  Check indicators using approved threat-intelligence sources.
-  Preserve the PCAP as evidence.
-  Escalate according to incident-response procedures when the evidence supports malicious activity.
-  Document the analysis and decision.

### Lessons Learned

-  Each protocol layer provides different evidence.
-  Display filters make large captures manageable.
-  DNS and HTTP may reveal valuable investigative context.
-  TCP flags help explain connection behaviour.
-  Packet evidence requires environmental context before an incident can be confirmed.

## Skills Demonstrated

-  Wireshark
-  Packet capture analysis
-  Network traffic analysis
-  IPv4
-  TCP and UDP
-  ICMP
-  DNS
-  HTTP
-  Display filtering
-  Packet-header interpretation
-  Incident-investigation reasoning
