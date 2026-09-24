# Incidents Handler's Journal

## Overview 
This project contains a structured incident handler's journal documenting cybersecurity incidents investigated throughout the google Cybersecurity certificate.

Each journal entry records the incident scenario, investigative findings, tools used, indicators of compromise, response activities, and lessons learned.

Supporting technical analyses are included when an incident requires deeper examination of indicators of compromise , network activity, malicious files, or other forms of security evidence, investigation using tools such as VirusTotal, Wireshark, tcpdump etc.

# ENTRY 1: Healthcare Clinic Ransomware Incident
A healthcare clinic experienced a ransonware attack delivered through a phishing email containing a malicious attachment. Critical files and patient records were encrypted, disrupting access to important systems and normal business operations.

## Overview

A ransomware incident originating from phishing email and malicious attachment disrupted access to critical patient records and business systems.

## Skills Demonstrated
-  Incident Documentation
-  Incident Response
-  Security Event Analysis
-  Alert Investigation
-  Evidence Collection
-  Timeline Analysis
-  Security Operations
-  Network Security Monitoring
-  Cybersecurity Reporting

## Key Concepts
-  Security Event
-  Security Incident
-  Indicator Of Compromise (IOC)
-  Alert Triage
-  Incident Response Lifecycle
-  Detection and Analysis
-  Containment
-  Recovery

## Outcome

This project demonstrates the use of structured documentation to investigate, analyze, and track cybersecurity incidents from initial detection through response and remediation.


# Entry 2: Suspicious File Hash Investigation

A suspicious executable file created on an employee workstation was investigated using SHA-256 hash. Virustotal analysis confirmed that the file was malicious and identified related indicators of compromise, malware behaviours, and MITRE ATT&CK techniques.
The related phishing alert was evaluated using a phishing incident response playbook and escalated for further investigation. The analysis included vendor detection results, file hashes, related network indicators, behavioural observations, and Pyramid of Pain classification.

## Skills Demonstrated

-  Incident Documentation
-  Incident response
-  Malware Investigation
-  Threat Intelligence
-  Indicator of Compromise Analysis
-  VirusTotal Investigation
-  Pyramid of Pain
-  MITRE ATT&CK
-  Evidence Collection
-  Security Reporting

## Supporting Investigation
investigations/virustotal_ioc_analysis.md

## Outcome

This journal demonstrates the ability to document security incidents, investigate suspicious artifacts, collect indicators of compromise, and communicate findings in a structured and repeatable manner.


# Entry 3 : Final Incident Report Review
Incident Type: Customer data breach caused a web application vulnerability.

Summary

A finalized incident report was reviewed following a major data breach affecting approximately 50,000 customer records.
An attacker gained unauthorized access to customer personally identifiable information and financial information through a vulnerability in the organization's e-commerce application.
The review focused on the incident lifecycle, investigative findings, root cause, response actions, recovery activities, and recommendations.

Root Cause

The investigation identified a web application vulnerability that allowed a forced browsing attack.
The attacker modified purchase confirmation page URLs to access sequential customer transaction records without proper authorizations.

Primary Findings
-  The e-commerce application did not adequately restrict access to customer transactions.
-  The attacker used forced browsing to access transaction data
-  Web server logs revealed a large volume of sequential customer order access.
-  Personally identifiable information and financial informations were exposed
-  Approximately 50,000 customer records were affected
-  The incident demonstrated weakness in application-level authorization controls

Response Actions
-  The security team initiated an investigation
-  Web server logs were reviewed
-  The vulnerability and attack method were identified
-  Public disclosure activities were coordinated
-  Identify protection services were offered to affected customers

Recommendations
-  Perform routine vulnerability scans
-  Conduct periodic penetration testing
-  Implement stronger authorization controls
-  Use allowlisting where appropriate
-  Restrict access to approved URLs and resources
-  Confirm that authenticated users are authorized to access each requested object
-  Review web application access logs for abnormal sequential requests
-  Incorporate the findings into secure development and testing practices

Security Lessons
-   Authentication alone does not guarantee authorization
-   Applications must verify that users are authorized to access each requested resource
-   Forced browsing can expose sensitive records when predictable URLs or identifiers are used
-   Vulnerability scanning and penetration testing can help identify weaknesses before exploitation
-   Final incident reports preserve findings and support organizational improvement
-   Post-incident activity should result in updates to controls, procedures, playbooks, and development practices

Detailed Entry: entries/entry_o3_final_report_review.md


A 
