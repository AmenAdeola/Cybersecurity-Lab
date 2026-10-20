# Network Traffic Analysis

## objective

## Overview

A security investigation that uses network evidence to identify affected protocols, probable attack activity, and remediation actions. Analyze DNS an ICMP traffic captured with tcgdump to determine why users could not access the website yummyrecipesforme.com.

## skills Demonstrated

-  Network Traffic Analysis
-  DNS Troubleshooting
-  ICMP Analysis
-  Packet Inspection
-  Root Cause Identification
- Protocol analysis
- Incident investigation
- Security reporting

## Tools and Technologies
-  tcpdump
- Wireshark concepts
- TCP/IP
- DNS
- ICMP
- HTTP
  
## Protocls Analyzed

-  DNS
-  UDP
-  ICMP
-  IP

## Key finding

DNS requests sent to UDP port 53 received ICMP "udp port 53 unreachable" responses, preventing successful resolution of the website domain name.


## Outcome
The report connects observed traffic with the incident scenario and recommends defensive actions. 
