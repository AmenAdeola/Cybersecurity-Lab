# Entry: 2: Suspicious File Hash Investigation

## Entry Information

Field | Information|
------|------------|
Entry Number | 2|
Incident Type | Suspicious file and potential malware|
Detection Method | IDS alert|
Investigation Tool | VirusTotal
Status | Investigated|

## Description

A SOC analyst received an alert concerning a suspicious file downloaded from a password-protected spreadsheet attached to an email.

After the employee opened the file, unauthorized executable files appeared on the workstation. An intrusion detection system detected the activity and generated an alert.

The suspicious file's SHA-256 hash was submitted to VirusTotal for further investigation.

## Timeline

Time | Event|
-----|------|
1:11 PM | Employee received the email attachment|
1:13 PM | Employee downloaded and opened the file
1:15 PM | Unauthorized executable files were created
1:20 PM | The IDS generated an alert|

# Tools Used
-  VirusTotal
-  IDS alert information
-  SHA-256 hash analysis
-  Threat intelligence sources

# The 5 W's

| The 5 W's | Information|
------------|------------|
Who caused the incident?| An employee opened a suspicious password-protected attachment. The malicious file appears to have originated from an unknown threat actor.
What happened? | A suspicious file created unauthorized executable files on the employee's workstation. VirusTotal analysis identified the file as malicious.
When did the incident occur? | The sequence of events occurred between 1:11 PM and 1:20 PM. 
Where did the incident happen? | The activity occurred on an employee workstation with the organization's environment.
Why did the incident happen? | The incident occurred after the employee downloaded and opened a suspicious email attachment. The attachment delivered a malicious  executable file.

### SHA-256

54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b

# Additional Notes
The high detection ratio and consistent malicious classifications indicate that the file should be treated as malicious.

The affected workstation should be isolated, and the identified indicators should be reviewed across the environment to determine whether other systems were affected.


