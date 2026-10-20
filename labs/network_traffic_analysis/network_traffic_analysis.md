# Network Traffic Analysis

## Objective

Analyze suspicious network activity and document evidence, impact, and recommended controls.

## Investigation Questions

- Which systems communicated?
- Which protocols and ports were used?
- Was the traffic expected or abnormal?
- What assets or services were affected?
- What evidence supports the conclusion?


## Analysis Workflow

Network alert → collect evidence → inspect source and destination → review protocol and ports → identify patterns → determine impact → recommend controls

## Potential Findings

Examples include repeated connection attempts, unexpected DNS requests, suspicious external destinations, unencrypted HTTP communications, abnormal ICMP traffic, or signs of data exfiltration.

## Recommended Controls

- Restrict unnecessary ports and services.
- Monitor DNS and outbound connections.
- Use IDS/IPS and SIEM correlation.
- Segment sensitive systems.
- Apply secure protocols and access-control rules.


## Skills Demonstrated

- Network traffic analysis
- Protocol analysis
- Incident investigation
- Security reporting 
