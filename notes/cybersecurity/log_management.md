# Log_management 

## Logs 
Logs provide evidence of activity across systems, applications, identities, endpoints, and networks.
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

## Common Fields

- Timestamp
- Hostname
- Username
- Source and destination IP
- Port and protocol
- Event type
- Severity
- Action
- Message 

## Common Log Sources

- Authentication systems
- Operating systems
- Applications
- Firewalls
- IDS/IPS
- DNS
- Proxy and web servers
- Cloud services
- Endpoint protection

## Common Log File Formats

Format | Description | Typical Use|
-------|--------------|------------|
JSON | Structured key-value format| SIEM platforms, APIs
Syslog| Standard logging format used by linux and et network devices| Routers, firewalls, Linux servers
XML| Markup-based structured format|Windows logs, application logs
CSV| Comma-separated values|Exported reports and datasets
CEF (Common Event Format)| Vendor-neutral standardized security log format|SIEM ingestion and security tools|

## Log Lifecycle

```text
Generate → Collect → Parse → Normalize → Store → Search → Correlate → Retain → Dispose
```

 ## Good Practices
 
 - Synchronize system time.
 - Protect log integrity.
 - Restrict access.
 - Centralize important logs.
 - Define retention periods.
 - Monitor ingestion failures.
 - Test searches and alerts.
 - Avoid logging sensitive data unnecessarily. 
