# Threat Intelligence

## Purpose

Threat intelligence adds context to indicators, behaviours, threat actors, campaigns, tools, and vulnerabilities.

## IOC Types

- Hash values
- IP addresses
- Domains and URLs
- Filenames and paths
- Registry keys
- Processes
- Malware families
- Tactics, techniques, and procedures

## VirusTotal Workflow
```text
Hash → Detection → Details → Relations → Behavior → IOC collection → MITRE ATT&CK mapping → Pyramid of Pain
```

## Pyramid of Pain
| Indicator level | Difficulty for attacker to change |
|---|---|
| Hash | Low |
| IP address | Low |
| Domain | Moderate |
| Network or host artefact | Higher |
| Tool | High |
| TTP | Very high |

## Intelligence Validation

- Verify source reliability.
- Check timestamps and freshness.
- Correlate with internal evidence.
- Consider false positives.
- Avoid treating one indicator as proof of an incident.
- Document confidence and limitations. 
