# Packet Inspection  

## Definitions

Concept | Definition|
--------|-----------|
Packet | Small unit of data transmitted across a network
Packet inspection |Examination of packet contents to understand communications and identify suspicious activity
Packet Capture (PCAP)| Recorded network traffic saved for analysis
Protocol Analyzer | Tool used to capture and inspect packets
Deep Packet Inspection (DPI) | Analysis of packet payloads in addition to header information


## Packet Layers
```text 
Frame
 └── Ethernet II
     └── IPv4
         └── TCP / UDP / ICMP
             └── Application data
```

## Important Fields

- Source and destination MAC addresses
- Source and destination IP addresses
- Source and destination ports
- Protocol
- Time to Live
- Packet length
- TCP flags
- Payload

## Wireshark Filters
```text
ip.addr == 142.250.1.139
ip.src == 142.250.1.139
ip.dst == 142.250.1.139
eth.addr == 42:01:ac:15:e0:02
icmp
dns
udp.port == 53
http
tcp.port == 80
tcp contains "curl"
```

## TCP Three-Way Handshake
```text
SYN → SYN-ACK → ACK
```

## TCP Flags
| Flag | Meaning |
|---|---|
| SYN | Start a connection |
| ACK | Acknowledge data |
| FIN | End a connection normally |
| RST | Reset a connection |
| PSH | Deliver data promptly |

## Analyst Questions
- Who communicated?
- Which protocol and service were used?
- What data was exchanged?
- Was the activity expected?
- Does the destination have a suspicious reputation?
- Is the traffic associated with another alert? 



