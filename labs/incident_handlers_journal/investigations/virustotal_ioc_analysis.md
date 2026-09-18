# VirusTotal  IOC Analysis

## Objective

Investigate a suspicious file using VirusTotal and classify the identified indicators of compromise using the Pyramid of Pain

## Initial SHA-256 Hash

54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b


## Malicious File Determination

The file was identified as malicious based on the following evidence:
-  51 out of 70 security vendors flagged the file as malicious
-  The VirusTotal community score was -294
-  Multiple vendors classified the file as a Trojan, backdoor, or malware variant.
-  Malware family labels included Flagpro, Fragtor, and Bifit.
-  Behavioural analysis identified suspicious execution techniques.
  
## File Details 

Attribute | Value|
----------|------|
File Name | bfsvc.exe
Fiel Type | win32 EXE
File Size | 430 KB
Digital Signature | Not signed
Malware Family | Flagpro/ Fragtor
MD5 | 287d612e29b71c90aa54947313810a25
SHA-1 | 8f35a9e70dbec8f1904991773f394cd4f9a07f5e

## Indicators Of Compromise

IOC Type | Indicator|
---------|----------|
SHA-256 Hash | 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b
MD% Hash | 287d612e29b71c90aa54947313810a25
SHA-1 | 8f35a9e70dbec8f1904991773f394cd4f9a07f5e
IP Address | 104.115.151.81
Domain Name | a.sinkhole.yourtrap.com
Malware Family /Tool | Flagpro
TTP | Process Injection, T1055



## MITRE ATTACK Techniques Observed

Technique |Technique ID|
----------|------------|
Process Injection | T1055
Input Capture | T1056
Masquerading | T1036
Obfuscated files or Information | T1027
Steal Web Session Cookie | T1539

## Pyramid of Pain Classification 

Pyramid Level | Indicator | Attack Difficulty|
--------------|-----------|------------------|
Hash Values | SHA-256, SHA-1, and MD5 hashes | Easy
IP Addresses | 104.115.151.81| Easy
Domain Names | a.sinkhole.yourtrap.com| Moderate
Network / Host Artifacts | bfsvc.exe | Difficult
Tools| Flagpro malware family| Hard
TTPs| Process Injection T1055 | Very Hard

## Analysis 

Hash values are useful for identifying the exact malicious file, but an attacker can change a file hash by modifying the file. 
IP addresses and domains provide network indicators, but attackers may replace their infrastructure. 
Host artifacts and tools are more difficult to change because doing so may require modifications to the malware's operation.
Tactics, techniques, and procedures are the most valuable defensive indicators because changing attack behaviour requires the greatest effort from the attacker.

## Recommended Response Actions

-  Isolate the affected workstation.
-  Preserve the suspicious file and relevant logs
-  Search the environment for the identified hashes
-  Review DNS and network logs for the identified domain and IP address
-  Block confirmed malicious indicators when appropriate
-  Review email security logs to identify the original message
-  Reset Potentially affected user credentials
-  Perform endpoint scanning
-  Document and escalate the incident according to the incident response plan

## Key Takeaways

-  VirusTotal combines information from multiple security vendors and intelligence sources.
-  File hashes can be used as initial indicators of compromise
-  The relations section helps reveal connected domains and IP addresses
-  The Behavior section helps identify host artifacts and MITRE ATT&ACK techniques
-  The Pyramid of Pain helps analysts prioritize indicators based on how difficult they are for attackers to change
