# NIST Cybersecurity Framework Analysis

## Identify

Attack Type:
ICMP Food attack

Affected Systems:
-  Internal network infrastructure
-  Network Services
-  User access to internal resources

Vulnerability: 
Improper Firewall configuration

Potential Risk:
Network service diruption and denial of service

--------

## Protect 

-  Implement stronger firewall rules.
-  Configure ICMP rate limiting.
-  Perform regular firewall audits.
-  Verify source IP adresses.
-  Maintain secure baseline configurations.
These controls reduce the attack surface and make future attacks more difficult to execute.

-------

## Detect

-  Deploy IDS/IPS monitoring.
-  Implement SIEM monitoring and alerting.
-  Analyze firewall logs and network traffic patterns.
-  Create alerts for unusual ICMP traffic volumes.
-  Continuous monitoring helps identify attacks more quickly

--------

## Respond

-  Block malicious ICMP traffic
-  Escalate incidents to network and security teams.
-  collect and preserve logs.
-  Perform root cause analysis.
-  Maintain and update incident response playbooks.
-  Document lessons learned.

----------

## Recover 

-  Restore critical network services.
-  Validate firewall configurations
-  Verify network stability.
-  Review the effectivenness of implemented controls
-  conduct a post-incident review and update security procedures.
-  Implement additional monitoring where necessary

