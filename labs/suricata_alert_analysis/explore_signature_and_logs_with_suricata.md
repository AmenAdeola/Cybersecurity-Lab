# Explore Signatures and Logs with Suricata

## Objective

Learn how Suricata uses signatures to inspect network traffic, generates alerts, and record events in security logs.
------------

# Suricata Rule Structure

The custom rule examined during the lab: alert http $HOME_NET any -> $EXTERNAL_NET any any (msg:"GET on wire"; flow:established,to_server; content:"GET"; http_method; sid:12345; rev:3;)
---------------------

# Components of a Suricata Rule

## Action: Alert
Determines what action Suricata takes when all rule conditions are satisfied.

### Common Actions

Action | Purpose|
-------|--------|
Alert| Generate an alert|
pass| Allow traffic and ignore matching rules
drop|Block traffic and generate an alert|
reject| Block traffic and send a reset message|

---------------

## Header: http $HOME_NET any -> $EXTERNAL_NET any 
Determines the traffic that rule applies to.

### Header Components

Component |Value|
----------|-----|
Protocol|http|
Source Network| $HOME_NET|
Source Prot|any
Direction | ->
Destination Network| $EXTERNAL_NET
Destination Port|any

### Variables

Variable|Description|
--------|-----------|
$HOME_NET|Internal network
$EXTERNAL_NET|External network

In this lab: $HOME_NET = 172.21.224.0/20

---------------------

## Rule Options: msg; "GET on wire"; flow:established, to_server; content:"GET"; http_method; sid:12345; rev:3;

### Rule Option Breakdown

Option|Purpose|
------|-------|
msg|Alert message displayed when triggered|
flow| Defines traffic direction and connection state|
content| Text pattern to search for|
http_method|Restricts match to HTTP method field|
sid|Unique Signature ID|
rev|Rule revision number|

-----------
# Running Suricata

Command:
sudo suricata -r sample.pcap -S custom.rules -k none

### Command Options

Option|Purpose|
------|-------|
-r|Read traffic from packet capture|
-S|Load custom rule file|
-k none| Disable checksum verification
-----------------
# Log Files Generated

Location: /var/log/suricata/

Key log files:
File|Purpose|
----|-------|
fast.log|Quick alert summary|
eve.json|Detailed event log

---------------

# Fast Log Analysis
Command: cat /var/log/suricata/fast.log

Example alert: [1:12345:3] GET on wire

### Fast Log Contains
-  Timestamp
-  Alert Message
-  Signature ID
-  Source Information
-  Destination Information

### Characteristics
-   Easy to read
-   Quick verification
-   no Limited details
-   no Deprecated format
--------------------
# Eve JSON Analysis

Command: cat /var/log/suricata/eve.json

The Eve log stores detailed events in JSON format.
-------------------

# Parsing JSON Output

Command: jq . /var/log/suricata/eve.json | less

Purpose: Display JSON events in a readable format

-------------------------

## Event Severity
The first alert contained: severity = 3

----------------------

# Extract Specific Fields

Command: jq -c "[.timestamp,.flow_id,.alert.signature,.proto,.dest_ip]" /var/log/suricata/eve.json

Extracted Fields: 

Field | Description|
------|------------|
timestamp|Event time|
flow_id|Unique flow identifier
alert.signature|Alert message|
proto| Network protocol|
dest_ip|Destination IP|
--------------

## Example Output
["2022-11-23T12:38:34.624866+0000",14500150016149,"GET on wire","TCP","142.250.1.139"]

--------------------

# Flow ID
Definition:
A unique identifier assigned to a network flow.

### Why It Matters
Allows analysts to correlate:
-  Related packets
-  Related alerts
-  Related events

across Suricata logs.
------------------------
# Search by Flows ID
Command:jq "select(.flow_id==X)" /var/log/suricata/eve.json

# Key findings
-  Suricata uses signature-based detection to identify network activity.
-  Rules consist of an action, header, and rule options.
-  fast.log provides quick alert summaries.
-  eve.json provides detailed structured event data
-  jq helps parse and extract JSON fields.
-  flow_id enables event correlation during investigations.

------------------------

# Skills Demonstrated
-  Suricata IDS
-  Detection Rule Analysis
-  Signature-Based Detection
-  Alert Analysis
-  JSON Parsing
-  Log Investigation
-  Event Correlation
  
