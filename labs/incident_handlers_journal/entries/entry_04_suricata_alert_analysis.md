# Incident Handler's Journal

## Entry 4: Suricata Alert Analysis

### Date: September 2026

### Description

In this activity, I used Suricata an open-source network intrusion detection system (NIDS), to examine a custom detection rule and analyze alerts generated from a packet capture file.

The objective was to understand how Suricata signatures detect specific network activity and how security analysts can use Suricata logs to investigate alerts.

---------------------

## Tools Used

-  Suricata
-  Linux command line
-  Packet capture file (PCAP)
-  Custom Suricata rules
-  'fast.log'
-  'eve.json'
-  'jq'

----------------


# The 5 W's

| The 5 W's | Information|
------------|------------|
Who| The activity involved network traffic between an internal system and an external web server. The traffic was analyzed by a security analyst using Suricata detection rules|
What| Suricata analyzed an existing packet capture file and generated alerts when the network traffic matched a custom HTTP detection rule. The rule was designed to detect HTTP 'GET' requests travelling from the internal network to the external network.|
When| The detection occured when Suricata processed the packet capture file. The timestamps associated with the events were recorded in the Suricata log files|
Where| The activity was performed in a Linux lab environment. The alerts were stored in the following Suricata log files: /var/log/suricata/fast.log; /var/log/suricata/eve.json|
Why| The activity was completed to understand how intrusion detection systems use signatures to detect suspicious or noteworthy network activity. IT also demonstrated how analysts can use structured logs and flow identifiers to investigate related network events.
