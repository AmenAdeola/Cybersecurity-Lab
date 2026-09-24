# Detection tools and Techniques

## Intrusion Detection Systems (IDS)

Detection Tool | Description | Purpose|
---------------|-------------|--------|
HIDS (Host-Based Intrusion Detection System)|Monitors activity on a single host or endpoint| Detect suspicious activity on a device|
NIDS (Network-Based Intrusion Detection System) | Monitors traffic across a network segment|Detect malicious network activity|
IPS (Intrusion Prevention System)|Detects and blocks malicious activity | Prevent attacks in real time

### HIDS (Host-based IDS)
Definition: 
Monitors activity occurring on individual hosts or endpoints.

Monitors
-  System logs
-  File modifications
-  User activity
-  Processes
-  Registry changes
-  Operating system events

Examples:
Example | Detection|
--------|----------|
Unauthorized file modification|Detected
Suspicious process execution | Detected
Privilege escalation | Detected
Malware activity | Detected

Advantage: High visibility into endpoint activity
Limitation: Limited visibility outside the host

### NIDS (Network-Based IDS)
Definition:
Monitors network traffic moving between devices

Monitors
-  Packets
-  Connections
-  Protocol activity
-  Network flows

Examples:
Example | Detection|
--------|----------|
Port scanning | Detected
Malware traffic|Detected
Data exfiltration|Detected
Command-and-control traffic | Detected

Advantage: Monitors multiple systems simultaneously
Limitation: Cannot see activity occurring only on hosts


## Detection Techniques

### Signature-Based Analysis

Definition: Detects threats by comparing activity to known attack patterns

Process: Known Threat -> Signature Match -> Alert generated

Examples:
Threat | Detection|
-------|----------|
Known malware hash | Signature match
Known exploit pattern | Signature match
Known malicious domain| Signature match

Advantages: 
-  Fast
-  Accurate for known threats
-  Low false-positive rate

  Limitations:
  -  Cannot detect unknown attacks
  -  Cannot detect zero-day threats

### Anomaly-based Analysis

Definition: Detects activity that deviates from normal behavior
Process: Normal Baseline -> Unusual Activity -> Anomaly Detected -> Alert Generated

Examples:
Activity| Detection|
-------|-----------|
Unusual login location|Anomaly
Sudden data transfer spike| Anomaly
Unexpected network connections |Anomaly
Rare process execution | Anomaly


Advantages:
-  Can identify unknown threats
-  Can detect zero-day attacks
-  Detects abnormal behaviour

Limitations
-  Higher false-positive rare
-  Requires a baseline

### Signature-Based Vs Anomaly-Baded

Feature | Signature-Based|Anomaly-Based|
--------|----------------|-------------|
Detects Known Threats|yes|yes
Detects Unknown Threats| No|Yes
Detects Zero-Day Attacks|No|Yes
Requires Signatures|Yes|No
Requires Baseline|No|Yes
False Positives|Lower|Higher

### Relationship to Suricata

Component| Suricata Usage|
---------|---------------|
NIDS|Primary function|
Signature-Based Analysis|Uses detection rules and signatures
Network Monitoring| Captures and analyzes traffic
Alerting |Generates alerts when rules match

# Suricata Rule Components

Component | Purpose|
----------|--------|
Action| Determine what happens when rule matches
Header| Define traffic to inspect|
Rule Options| Define matching conditions

## Rule Structure
1.  Action
2.  Header
3.  Rule Options

### Common Rule Actions

Action | Description|
-------|------------|
alert | Generate an alert
pass| Allow Traffic
drop | Block traffic and alert
reject | Block traffic and send reset

### Important Suricata Fields

Field | Purpose|
------|--------|
msg|alert message
sid|Signature ID
rev|Revision Number
content|Text pattern
flow|Traffic direction
http_method|HTTP method inspection

### Suricata Logs
Log File|Purpose|
--------|-------|
fast.log|Quick alert summaries
eve.json|Details structured events

### jq Commands

Command|Purpose|
-------|-------|
jq . file.json| Pretty-print JSON
jq . file.json(|)less |Read output page-by-page
jq -c '[fields]' file.json | Extract fields
jq 'select(.flow_id==X)' file.json|Filter by flow ID
