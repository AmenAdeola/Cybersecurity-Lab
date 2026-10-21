# Entry 2: Suspicious File Hash and Phishing Investigation

## Date September 2026
### Entry Number 02

## Description
In this activity, I investigated a suspicious file hash associated with a phishing alert. I used VirusTotal to review detection results, file metadata, related infrastructure, behavioural information, and mapped MITRE ATT&CK techniques. I then applied phishing-response reasoning to determine whether the alert required escalation.

## Tools Used
-  VirusTotal
-  Phishing incident response playbook
-  MITRE ATT&CK
-  Pyramid of Pain
-  Incident Handler’s Journal


## The 5 W's

### Who
A user in a fictional organizational environment received a suspicious email containing or linking to a file. A cybersecurity analyst investigated the file indicator and associated activity.

### What
A suspicious SHA-256 file hash was submitted to VirusTotal. The investigation reviewed vendor detections, file details, related indicators, sandbox behaviour, and attack techniques to determine whether the file was malicious and whether the phishing alert should be escalated.

### When
The analysis was completed in September 2026. The exact completion date should be verified from the original lab screenshots or journal records.

### Where
The investigation was performed in a controlled Google Cybersecurity Certificate lab environment using VirusTotal and a phishing-response scenario.

### Why
The activity was completed to practise IOC enrichment, malware triage, phishing alert investigation, evidence-based escalation, and incident documentation.

#### Initial Indicator
SHA-256: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b 
This value should be checked against the original screenshot before publication.

## VirusTotal Investigation Workflow

Hash → Detection → Details → Relations → Behavior → IOC collection → MITRE ATT&CK mapping → Pyramid of Pain → escalation decision 

## Detection Review

The Detection tab was used to review whether security vendors classified the file as malicious or suspicious. Multiple detections increase confidence that the file requires further analysis, but the analyst should still review the remaining evidence rather than relying on a single score.

## File Details
-  Review SHA-256, SHA-1, and MD5 values.
-  Review filename, file type, size, and submission history when available.
-  Compare metadata with the alert and email attachment details.
-  Preserve hashes as investigation indicators.

 ### Relations
 
The Relations tab can connect the file to domains, URLs, IP addresses, contacted hosts, dropped files, or other artefacts. Related indicators should be documented and checked against approved threat-intelligence sources.

### Behaviour

The Behaviour tab provides sandbox observations, including processes, files, network activity, and mapped techniques. Behavioural findings help the analyst understand what the file attempted to do after execution.

## Indicators of Compromise

The following indicators were captured in the working notes. Verify each value against the original lab evidence before publication:
SHA-256: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b
SHA-1: 8f35a9e70dbec8f1904991773f394cd4f9a07f5e
MD5: 287d612e29b71c90aa54947313810a25
IP address: 104.115.151.81
Domain: a.sinkhole.yourtrap.com
Host artefact: bfsvc.exe Malware family / tool: Flagger 

## MITRE ATT&CK Mapping

-  Process Injection — T1055
-  Input Capture — T1056
-  Masquerading — T1036
-  Obfuscated Files or Information — T1027
-  Steal Web Session Cookie — T1539

These mappings must be verified against the original VirusTotal Behaviour results before publication.

## Pyramid of Pain Analysis

-  Hashes: easy for an attacker to change.
-  IP addresses: infrastructure indicators that can be replaced.
-  Domains: moderately difficult to replace.
-  Host artefacts: more disruptive to change.
-  Tools or malware families: costly to replace.
-  TTPs: most difficult because they reflect attacker behaviour.

### Assessment

The combined hash reputation, related indicators, sandbox behaviour, and mapped techniques supported classifying the file as malicious or highly suspicious. The evidence justified escalation under a phishing-response process. A file hash alone would not be sufficient; the conclusion depends on the full set of observed indicators.

### Response Actions

-  Do not open or execute the attachment.
-  Preserve the original message and associated headers.
-  Record the file hashes and related indicators.
-  Search security tools for matching indicators.
-  Identify potentially affected users and endpoints.
-  Block malicious indicators according to organizational procedures.
-  Isolate affected endpoints if execution is confirmed.
-  Reset credentials if evidence suggests credential theft.
-  Escalate to the incident-response team.
-  Document findings, decisions, and actions.

## Lessons Learned

-  VirusTotal supports IOC enrichment but does not replace analyst judgement.
-  One indicator should be correlated with metadata, relationships, behaviour, and environmental evidence.
-  MITRE ATT&CK provides a common language for observed adversary techniques.
-  The Pyramid of Pain helps prioritize indicators according to the difficulty attackers face when changing them.
-  A phishing playbook provides consistent investigation and escalation steps.

## Skills Demonstrated

-  Phishing analysis
-  Malware triage
-  VirusTotal investigation
-  IOC enrichment
-  MITRE ATT&CK mapping
-  Pyramid of Pain analysis
-  Alert escalation
-  Incident documentation
