# Attack Surface and Attack Vectors

## Definitions

# Attack surface & attack vectors

Concept | Definition | Example |
--------|------------|---------|
Attack surface | All possible points where an attacker can interact with a target | Workstation, network, UB ports
Attack vector | Method used to gain unauthorized access |Phishing, malware, USB baiting
Threat Actor |Person or group carrying out on attack | Hacker, insider, competitor
Payload| Malicious software or code delivered through an attack vector
Social Engineering |Manipulation people into revealing information | Phishing email
USB Baiting | Leaving infected USB devices where targets may find them | Parking lot USB attack


## Attack Surface Categories
- Network: open ports, exposed services, remote access
- Application: login forms, APIs, file uploads, input fields
- Human: phishing, social engineering, credential reuse
-  Physical: USB devices, unattended equipment, tailgating
-  Cloud: public storage, excessive permissions, exposed keys

  
# USB Security

Risk |Example| 
-----|-------|
Malware Infection | Malicious code executes when USB is connected
Data Theft | Sensitive files copied from the device
Credential theft | Malware captures usernames and passwords
Social Engineering | Personal information used for phishing
Unauthorized Access | Attackers gain access to organizational systems


# Controls Against USB Attacks

Control Type | Example|
-------------|--------|
Technical | Endpoint protection, antivirus, device control
Operational |Security awareness trianing
Administrative |USB usage policies
Preventive |Disable unauthorized USB devices
Detective | Monitor endpoint activity
Corrective | Incident response procedures

# Applying an attacker Mindset

Step | Description|
-----|------------|
Identify a target| Determine what asset to attack
Determine access | Understand how the target can be reached
Evaluate attack vectors | Identify exploitable weaknesses
Find tools and methods | Determine how the attack would be executed

# Vulnerability Management Process

Step | Description|
-----|------------|
Discover | Identify vulnerabilities
Analyze | Validate findings
Assess Risk | Evaluate likelihood and impact
Remediate | Apply fixes and controls
Monitor | Reassess continuously


# Common Vulnerabilities and Exposures (CVE®) list criteria
-  Supporting evidence
-  Recognized as a security risk
-  Independent of other issues
-  Associated with a single codebase/source code origin

 ## Common Attack Vectors
-  Phishing attachment or link
- Stolen or weak credentials
-  Malware
-  Unpatched software
-  Misconfiguration
-  SQL injection
-  Malicious USB device
-  Insider misuse

## Reduction Strategies
-  Remove unnecessary services.
- Patch systems.
- Enforce MFA.
- Validate input.
- Apply least privilege.
- Segment networks.
- Monitor important activity.
- Train users.
- Restrict removable media.

## Security Chain
```text
 Threat actor → Attack vector → Exploited vulnerability → Compromised asset → Business impact → Security control
```
