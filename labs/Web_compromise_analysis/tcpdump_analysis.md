# TCPDump and Protocol Analysis

## DNS Activity

### Request
Client systems queried:

'''text
yummyrecipesforme.com

### Response 
DNS resolved: 203.0.113.22

DNS also resolved; greatrecipesforme.com
which was later identified as a malicious website

HTTP Activity
Observed Requests: HTTP GET/ for yummyrecipesforme.com and greatrecipesforme.com

### Findings
The traffic analysis confirmed communication with both the legitimate and the malicious website.
The investigation determined that malicious JavaScript embedded in the legitimate website redirected users to the malicious domain after downloading a file. 

### Protocols Involved

Protocol | Role |
---------|------|
DNS | Resolved domain names into IP addresses
HTTP | Delivered webpage content
JavaScript | Redirected users to a malicious website
