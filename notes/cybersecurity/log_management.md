# Log_management 

## Logs 

Concept | Definition|
--------|------------|
Log| Record of on event that occurred on a system, application, or network
Log Entry | Individual record within a log
Log Source | System or device generating logs
Log Aggregation |Collecting logs from multiple sources
Log Retention | Keeping logs for future analysis
Log Analysis | Reviewing logs to identify events and incidents

### Why Logs Matter

Purpose | Example|
--------|--------|
Detect Incidents | Unauthorized login
Investigate Alerts| Malware execution
Support Forensics | Timeline reconstruction
Identify IOCs|Malicious IP addresses
Audit Activity|User actions

## Common Log Components

Component | Description|
----------|------------|
Timestamp | Date and time of event|
Hostname| Device generating the log
Source IP | Origin of activity
Destination IP| Target of activity
Username| User involved
Severity | Event importance
Message | Description of activity

## Common Log File Formats

Format | Deescription | Example Use|
-------|--------------|------------|
JSON | Structured key-value format| SIEM platforms, APIs
Syslog| Standard logging format used by linux and et network devices| Routers, firewalls, Linux servers
XML| Markup-based structured format|Windows logs, application logs
CSV| Comma-separated values|Exported reports and datasets
CEF (Common Event Format)| Vendor-neutral standardized security log format|SIEM ingestion and security tools|

