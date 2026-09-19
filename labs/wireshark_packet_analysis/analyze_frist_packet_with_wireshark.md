# Analyze Network Traffic with Wirehsark

## Objective

Use Wireshark to inspect captures, identify protocols, analyze packet headers, and investigate network communications.

------------

# Packet Structure

## Layers Observed
''' text
Frame -> Ethernet II -> IPv4 -> TCP/UDP/ICMP -> Application Data
'''

--------------
# Packet Analysis

## Frame Layer

Information collected:
-  Arrival Time
-  Frame Length
-  Capture Details

Example: 
'''Text
74 bytes on wire
'''
------------

## Ethernet II Layer

Information collected
-  Source MAC Address
-  Destination MAC Address
-  EtherType

Example filter
''' text
eth.addr == 42:01:ac:15:e0:02
'''

Purpose:
Identify traffic sent or received by a specific network interface.

------------
## Internet Protocol (IPv4)

Information collected:
-  Source IP Address
-  Destination IP Address
-  Time TO Live (TTL)
-  Protocol

Example:
''' text
TTL = 64
'''
Purpose:
Identify communication endpoints
----------
## ICMP Traffic

Protocol observed:
''' text
ICMP
'''
Purpose:
Used by ping requests and responses to test connectivity between hosts
------------

## TCP Traffic

Destination Port:
''' text
80
'''
Purpose:
Identify HTTP communcations.
------------

# Wireshark Display Filters Used
## MAC Address Filter
'''text
eth.addr == 42:01:ac:15:e0:02
Displays packets associated with the specified MAC address
----------
## DNS Filter
'''text
udp.port ==53
'''
Displays DNS traffic.
-----------
## HTTP Filter
'''text 
tcp.port ==80
'''
Displays HTTP traffic
-----------

## Search Payload content
'''text
tcp contains "curl"
Searches packet payload data for the specified string
------------
# DNS Investigation 
## Domain Queried
''' text
opensource.google.com
'''

## Resolved IP Address
'''text
142.250.1.139
'''
Purpose:
Analyze domain resolution activity and map domains to IP address.
----------------

# Key Findings
-  ICMP traffic was observed during ping operations.
-  DNS requests were identified through TCP port 80.
-  Packet headers provided source and destination addressing information
-  Display filters improved investigation efficiency by isolation relevant traffic

---------------
# Security Relevance

Packet analysis allows security teams to:
-  Investigate suspicious network activity
-  Identify Indicators of Compromise (IOCs)
-  Wireshark Filtering
-  DNS Investigation
-  Network Traffic Analysis
-  Incident Investigation
