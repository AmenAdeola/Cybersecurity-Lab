# Capture and Filter Network Traffic with Tcpdump

## Objective

Use tcpdump to identify network interfaces, inspect live network traffic, capture packets into a PCAP file, and analyze captured network data.

--------------
# Task 1 - Identify Network Interfaces

## List Available Network Interfaces 

Command:
''' bash
sudo ifconfig
'''

Purpose:
Display available network interfaces and network configuration information.

Interfaces Identified:

''' text
eth0 -> Ethernet Interface
lo -> Loopback Interface
'''
-------

## List Interfaces with tcpdump
Command:
''' bash
sudo tcpdump -D
'''

Purpose:
Display available interfaces that can be used for packet capture.

-------
# Task 2 - Inspect Live Network Traffic

Command:
''' bash
sudo tcpdump -i eth0 -v -c5
'''

Options Used:
Option| Purpose|
------|--------|
-i eth0| Capture traffic from interface eth0
-v | Display verbose packet information|
-c5 | Capture 5 packets and exit|
-------------------

## Packet Details Observed
### Packet Timestamp

Example:
''' text
22:24:18.910372
'''

Purpose:
Shows when the packet was captured.
----------

### Protocol

Example:
''' text
IP
'''

Purpose:
Identifies the network protocol
---------
### IP header Information
Example:
''' text
tos 0x0
ttl 64
id 5802
flags [DF]
proto TCP (6)
length 134
'''

Information Provided
-  Type of Service (TOS)
-  Time To Live (TTL)
-  Packet Identifier
-  Flags
-  Protocol Type
-  Packet Length

-------------

## Communication Information
Example:
'''text
source_host.5000 > destination_host.59788
'''
Purpose:
Identify systems communicating and the ports used.
----------

## TCP Flags
Example:
''' text
Flags [P.]
'''

Meaning:
Flag| Purpose|
----|--------|
P | Push Flag
. | ACK Flag

This indicates data transmission with acknowledgement.
--------------

# Task 3 - Capture Traffic into a PCAP File

Command:
''' bash
sudo tcpdump -i eth0 -nn -c9 prot 80 -w capture.pcap &
'''

Options Used:

Option| Purpose|
------|--------|
-i eth0| Capture from eth0|
-nn | Disable hostname and port name resolution|
-c9| Capture 9 packets|
prot 80| Capture HTTP traffic only|
-w capture.pcap| Save packets to PCAP file|
&| Run command in background|

------------
## Generate HTTP Traffic

Command:
''' bash
curl opensource.google.com
'''

Purpose:
Generate HTTP traffic that tcpdump can capture
----------

## Verify Capture File

Command:
''' bash
ls -l capture.pcap
'''
Purpose:
Verify that the packet capture file was created successfully.
-------------

# Task 4 - Read Captured Traffic

## Read Packet Headers

Command:
''' bash
sudo tcpdump -nn -r capture.pcap -v
'''

Options:
 Option | Purpose|
 -------|--------|
 -nn | Disable name resolution|
 -r | Read packets from file|
 -v |Display detailed packet information

 ---------
 ## Read Extended Packet Data
 Command:

 ''' bash
 sudo tcpdump -nn -r capture.pcap -x
 '''

 Options: 
 Option | Purpose|
 -------|--------|
 -nn| Disable name resolution
 -r| Read packets from file
 -x | Display packet contents in hexadecimal and ASCII

 Purpose:
 Inspect packet payloads and identify patterns during investigations.
 -----------

 Key Findings
 -  Network interfaces can be identified using both ifconfig and tcpdump
 -  Tcpdump can capture live traffic directly from a network interface
 -  Packet captures can be saved to PCAP files for later analysis.
 -  Traffic can be filtered by protocol, interface, ansd port.
 -  Security analysis can inspect packet headers and payloads using verbose and hexadecimal outup.

---------------

# Security Relevance

Tcpdump is commonly used during:
-  Incident Response
-  Threat Hunting
-  Malware Analysis
-  Network Troubleshooting
-  Packet Forensics
-  Security Monitoring

---------------

# Skills Demonstrated
-  Tcpdump
-  Packet Capture
-  Packet Analysis
-  Traffic Filtering
-  Linux Networking
-  Cybersecurity Investigations
 
