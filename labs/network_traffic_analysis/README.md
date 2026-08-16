# Network Traffic Analysis

## objective

Analyze DNS an ICMP traffic captured with tcgdump to determine why users could not access the website yummyrecipesforme.com.

## skills Demonstrated

-  Network Traffic Analysis
-  DNS Troubleshooting
-  ICMP Analysis
-  Packet Inspection
-  Root Cause Identification


## Tools Used
-  tcpdump

## Protocls Analyzed

-  DNS
-  UDP
-  ICMP
-  IP

## Key finding

DNS requests sent to UDP port 53 received ICMP "udp port 53 unreachable" responses, preventing successful resolution of the website domain name.
