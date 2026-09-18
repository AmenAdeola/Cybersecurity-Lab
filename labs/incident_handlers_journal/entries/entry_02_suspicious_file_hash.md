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


