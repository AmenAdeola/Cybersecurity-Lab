# Entry 3 : Final Review

## Description

A review was conducted on a finalized incident report documenting a major data breach affecting approximately 50,000 customer records. The purpose of the review was to understand the incident lifecycle, identify the root cause, evaluate the response actions, and review recommendations for preventing future incidents.

## Incident Summary
An attacker gained unauthorized access to customer personally identifiable information (PII) and financial information through a vulnerability in the organization's e-commerce application.
Approximately 50,000 customer records were affected.

## Root Cause

The investigation identified a web application vulnerability that allowed a forced browsing attack.
The attacker modified purchase confirmation page URLs to access customer transaction data and exfiltrate sensitive information.

## Investigation Findings

-  Vulnerability located in the e-commerce application
-  Forced browsing attack used
-  Web server logs revealed large volumes of sequential customer order access
-  Customer data was exposed and exfiltrated

## Response Actions

-  Security team initiated and investigation
-  Web server logs were reviewed
-  Public disclosure was coordinated
-  Free identity protection services were offered to affected customers.

## Recommendations

- Perform routine vulnerability scans.
- Conduct penetration testing
- Implement allowlisting controls
- Restrict access to approved URLs
- Ensure authenticated users are properly authorized

## Lessons Learned

Regular vulnerability assessments, penetration testing, and access controls are critical for preventing data breaches caused by application-level vulnerabilities
