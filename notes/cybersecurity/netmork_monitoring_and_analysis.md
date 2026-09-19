# Network Monitoring and Analysis

## Definitions

Concept | Definition
--------|-----------|
Network Traffic| Data transmitted between devices across a network
Network Monitoring | Continuous observation of network activity to identify normal and abnormal behavior
Network Analysis | Inspection and interpretation of network communications
Traffic Flow | Movement of data between source and destination systems
Baseline| Expected or normal network behavior used for comparison
Data Exfiltration | Unauthorized transfer of data outside of an organization<s environment
Packet| Small unit of data transmitted over a network
Packet Capture (PCAP)| Recorded network traffic saved for analysis
Protocol Analyzer | Tool used to capture and inspect packets

## Why Security Analysis Monitor Networks

Purpose | Example|
--------|--------|
Detect Suspicious Activity| Unexpected outbound traffic
Detect Intrusions| Unauthorized Communications
Detect Data Exfiltration| Large transfers of sensitive data
Investigate incidents| Analyze malicious communications
Establish Baseline | Understand normal traffic patterns
Support Threat Hunting | Search indicators of compromise


## Network Traffic Analysis Workflow

Network -> Traffic Capture -> Packet Inspection -> Traffic Analysis -> Anomaly Detection -> Incident Investigation -> Response

## Network Protocol Analyzers

Tool | Description|
-----|------------|
Wireshark | Graphical network protocol analyzer
tcpdump | Command-line packet and analysis tool
Protocol Analyzer | Tool used to inspect network communications

## Packet Structure

Packet
|--- Header
|
------ Payload

## Packet Header

Contains routing and communication information.

Field| Purpose|
-----|--------|
Source IP address | Sender of the packet
Destination IP Address | Receiver of the packet
Source Port | Sending service
Destination Port | Receiving service
Protocol | Network protocol used
TTL | Time To Live
Packet Length |Packet size

## Packet Payload
Contains the actual transmitted data.

Examples:
-  HTTP content
-  DNS data
-  Application data
-  File transfers

## Common Protocols

Protocol | Purpose|
---------|--------|
IPv4| Internet commnunication
TCP | Reliable communications
UDP | Fast connectionless commnunications
ICMP| Ping requests and responses
DNS| Domain name resolution
HTTP| Web traffic
HTTPS| Secure web traffic
SSH | Secure remote access

## IPv4 Header Fields

Field | Purpose|
------|--------|
Version | IP protocol version
Header Length | Length of the header
Type of Service (ToS)| Traffic prioritization
Total Length | Total packet size
Identification | Packet identifier
Flags| Fragmentation control
TTL | Packet lifetime
Protocol | Next-layer protocol
Header Checksum| Error detection
Source IP | Sender address
Destination IP | Destination address

## Indicators of Network Activity

Indicator| Example|
---------|--------|
Source IP | 192.168.1.1
Destination IP| 8.8.8.8
Protocol|TCP
Destination Port | 80
DNS Query | opensource.google.com
HTTP Request| GET request
ICMP Traffic | Ping request

## Data Exfiltration

Definition
Unauthorized movement of sensitive information outside an organization
Example:
-  Uploading confidential files
-  Sending sensitive information through email
-  Malware transmitting customer data
-  Unauthorized cloud uploads

### Indicators

Indicator | Example
----------|--------|
Large outbound transfers| Unusual volume of network traffic
Unknown destination IPs|Connections to unrecognized hots
Suspicious DNS queries | Communication with malicious domains
Off-hours traffic| Unexpected activity outside business hours

## Packet Analysis Process

Step| Purpose|
----|--------|
Capture traffic| Collect network packets
Inspect Headers | Review addressing information
Review Payload Data | Examine content
Identify Trends | Connect events and indicators
Investigate | Determine whether a threat exists

## Wireshark Display Filters

Filter | Purpose|
-------|--------|
ip.addr == IP |Source or destination IP
ip.src == IP | Source IP only
ip.dst ==IP | Destination IP only
eth.addr == MAC| Specific MAC address
udp.port == 53| DNS traffic
tcp,port == 80 | HTTP traffic
tcp contains "text" | Search packet payload

## Key Takeaways

-  Network monitoring helps detect abnormal activity and security incidents.
-  Packet analysis allows analysts to understand system communications.
-  Protocol analyzers such as Wireshark and tcpdump are essential investigation tools.
-  Packet headers reveal routing and protocol information
-  Packet payloads contain transmitted data.
-  Data exfiltration is a major indicator of compromise
-  Packet captures support incident response, threat hunting, and forensic investigations.


