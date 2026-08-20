# Cybersecurity Incident report 

## Incident Summary

Several users reported unusual behavior while visiting yummyrecipesforme.com.

Users were prompted to download an executable file. After executing the file, users were redirected to malicious website called greatrecipesforme.com

The website owner also reported losing access to administrative account.

## Attack Type
Brute force attack

## Impact

-  Administration account compromised
-  website source code modified
-  Malware distribution to visitors
-  redirection to malicious website
-  Potential compromise of customer systems

## Root Cause

The attacker successfully guessed the administration account password through a brute force attack using known default credentials.

## Investigation findings 

The attacker: 
1-  Gained access to the administrative account
2- Modified website source code
3- Added malicious JavaScript
4- Distributed malware
5- Redirected users to malicious website
6- Changed the administrator password>

## System Affected

-  Website administrative accounts
-  web server
-  Website source code
-  End-user systems

## security recommendations

-  Implementation multifactor authentication (MFA)
-  Remove default credentials
-  Enforce strong password policies
-  Enable logging and monitoring
-  Perform regular source code reviews
-  conduct periods security audits
-   
