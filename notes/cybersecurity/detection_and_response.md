# Detection and Response

## Definitions

Concept| Definition|
-------|-----------|
Event| Any observable occurrence on a system or network
Security Event | An event related to security operations
Security Incident | An event that compromises confidentiality, integrity, or availabiltiy
Alert| Notification generated when suspicious activity is detected
Indicator of Compromise| Observable evidence of malicious activity
Detection| Process of identifying suspicious or malicious activity
Incident Response | Process of managing and mitigating security incidents

## Event Vs Incident

Event|Incdient|
-----|--------|
Login|Unauthorized login
File access| Unauthorized file access
Network connection | Data exfiltration
Email received | Phishing attack

## Incident Response Lifecycle (NIST)

Phase | Purpose|
------|--------|
Preparation| Prepare people, tools, and procedures
Detection and Analysis | Identify and validate incidents
Containment | Limit the impact and spread
Eradication| Remove the threat
Recovery | Restore systems and operations
Lessons Learned | Improve future response efforts

### incident response workflow
Event->Alert->Investigation->Incident->Containment->Eradication->Recovery->Lessons Learned


## Incident Response Teams

Role | Responsability|
-----|---------------|
Security Analyst | Investigate alerts and incidents
Incident Manager | Coordinates response activities
Technical Lead| Provides technical remediation guidance
System Administrator | Performs containment and recovery activities
Legal Team | Ensures legal and regulatory compliance
Communications Team | Handles internal and external communications
Management | Makes business decisions


## Incident Response Plan

component | Purpose|
----------|--------|
Preparation | Establish procedures before incidents occur
Roles and Responsibilities | Define responsibilities
Communication plan| Establish communication channels
Escalation Procedures | Define escalation paths
Recovery Procedures| Restore systems abd services
Documentation Process| Record investigative findings

## Documentation 

why documentation matters

Benefit | Description|
--------|------------|
Preserves Evidence| Maintains investigative records
Supports Investigations | Tracks activities and findings
Supports Lessons Learned | Improves future response
Creates Audit Trail| Demonstrates accountability

## Detection Tools

Tool| Purpose|
----|--------|
IDS| Detect suspicious activity
IPS | Detect and block malicious activity
Antivirus | Detect malware
EDR| Endpoint Detection and Response
SIEM| Security Information and Event Management
SOAR| Security Orchestration, Automation and Response

### IDS Vs IPS

IDS | IPS
----|----|
Detects threats| Detect and blocks threats
Passive | Active
Generates alerts| Takes protective actions

## SIEM
Purpose: collect, normalize, correlate and analyze security events.

Steps in SIEM Process

Step| Purpose| Output|
----|--------|-------|
Collect and Aggregate Data| Gather logs from multiple sources|Centralized data
Normalize Data | Standardize formats | Consistent records
Analyze and Correlate Events | Identify suspicious patterns | Correlated events
Generate Alerts | Detect threats | Alert
Investigate Alerts|Validate findings|Incident determination
Response and Remediate | Contain and mitigate | Response actions
Report and Improve| Document findings |Lessons learned

### SIEM Workflows
logs->collection->normalization->correlation->alert->investigation->response->reporting

## Common SIEM Data Sources

Source| Example|
------|--------|
Endpoints | Workstations laptops
Servers|Windows and Linux servers
Firewalls| Network security devices
Applications|Business applications
Active Directory | Authentication logs
Cloud Services| AWS, Azure, Microsoft 365
IDS/IPS| Security alerts
EDR | Endpoint telemetry

## SOAR
Purpose: Automate incident response activities and coordinate actions across multiple tools.

SOAR Functions

Function | Purpose|
---------|--------|
Orchestration| Connect security tools
Automation|Reduce manual tasks
Response |Execute predefined actions
Investigation Support|Streamline workflows


### SIEM Vs SOAR

SIEM| SOAR|
----|-----|
Collects and analyzes logs | Automate response actions
Detects threats | Responds to threats
Generates alerts | Executes playbooks
Provides visibility | Reduces manual effort

## Investigative tools

Tool Type | Purpose
----------|--------|
Detection Tools| Generate alerts
Investigative tools | Analyze alerts and evidence
Response tools | Mitigate incidents


# Key takeaways

-  Security events become incidents when they threaten confidentiality, integrity or availability
-  Detection and response are core SOC functions
-  Documentation is critical throughout incident response
-  IDS detects; IPS detects and blocks.
-  SIEM improves visibility and detection
-  SOAR improves automation and response
-  Incident response phases can overlap
-  The incident Handler's Journal provides a structured way to record investigations
