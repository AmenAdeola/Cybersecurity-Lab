
# Core Concepts

 Concept| Definition
-------|-----------|
Threat | A potential cause of harm
Vulnerability | A weakness that can be exploited
Risk | The potential for loss, damage, disclosure, or disruption
Likelihood | Probability that a risk will occur
Severity| Impact if the risk occurs
Priority | Overall risk score based on likelihood and severity
Risk Register | Document used to track risks and their scores

 ## Basic Scoring
 ```text
 Likelihood × Severity = Priority score
```
# Relationship Between Concepts
Asset -> Threat + Vulnerability -> Risk -> Likelihood X Severity -> Priority

Examples

Threat | Vulnerability | Resulting Risk
-------|---------------|----------------|
Phishing | Lack of employee awareness| Business Email Compromise
Attacker | Poor encryption| Compromised database
Unauthorized access | Publicly accessible server| financial records leak
Criminal activity | Unlock safe |Theft
Natural disaster | Dependency on suppliers |Supply chain disruption


# Common Risks

Risk | Example
-----|-------|
Business Email Compromise | Employee tricked into sharing confidential information
Compromised User Database | Customer data poorly encrypted
Financial Records Leak | Publicly accessible database backup
Theft | Unlocked safe
Supply Chain Disruption | Natural disasters affecting deliveries

## Risk Register Fields
- Asset
- Threat
- Vulnerability
- Likelihood
- Severity
- Score
- Existing controls
- Recommended treatment
- Owner
- Status
  
## Example Scale
| Score | Likelihood | Severity |
|---:|---|---|
| 1 | Rare | Low |
| 2 | Possible or likely | Moderate |
| 3 | High or expected | High or catastrophic |

## Treatment Options
- Avoid
- Mitigate
- Transfer
- Accept
  
## Important Limitation
 A numeric score supports prioritization but does not replace business context, legal or regulatory obligations, asset criticality, or professional judgement. 
# NIST CSF Functions

Functions | Purpose|
----------|--------|
Identify | Understand assets, risks, and business environment
Protect | Implement safeguards
Detect | Identify cybersecurity events|
Respond | Take action during incidents
Recover | Restore services and operations


