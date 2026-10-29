# SIEM Tools

## SIEM Purpose

A Security Information and Event Management system centralizes security data, normalizes events, supports searches, correlates activity, and generates alerts.

## SIEM Workflow

```text
Collect → Normalize → Correlate → Alert → Investigate → Respond → Improve
```
## Splunk SPL

Examples
```spl
 index=main
 index=main
 fail* "login failure"
 index=main fail | chart count by host
```
## Google Security Operations
Example
```text
metadata.event_type = "USER_LOGIN"
```
- Use normalized UDM search for structured fields.
- Use raw-log search when the original event text is required.

## SIEM vs SOAR
| SIEM | SOAR |
|---|---|
| Collects and analyses logs | Orchestrates tools |
| Correlates events | Automates repetitive actions |
| Generates alerts | Executes playbooks |
| Supports investigation | Accelerates response |

## Analyst Review
- Confirm event time and source.
- Validate data quality.
- Review related events.
- Determine true or false positive.
- Document evidence and actions.
- Tune detections only after understanding the cause. 
