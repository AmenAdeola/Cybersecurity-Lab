# Access Controls  

## Purpose

Access controls limit who or what can access systems, applications, and data.

## AAA Framework

| Concept | Purpose | Example |
|---|---|---|
| Authentication | Verify user's identity | Password, MFA, certificate |
| Authorization | Determine permitted actions | Read-only access, administrator role |
| Accounting | Record, monitoring  and review activity | Event logs, audit trails, user activity monitoring |


## Authentication Concepts

| Concept | Description |
|---|---|
| Username | Claimed identity |
| Password | Knowledge factor |
| MFA | Two or more different authentication factors |
| OAuth | Delegated authorization framework |
| SSO | One authentication session for multiple applications |
| Digital certificate | Cryptographic proof used to establish identity or trust |

## Authorization Models

- RBAC: Role-Based Access Control, access based on the person’s role.
- ABAC: access based on attributes such as department, device, time, or location.
- DAC: the resource owner determines access.
- MAC: access is controlled by centrally defined labels and policy.
Concept | Definition|
--------|-----------|
Authorization | Determines what actions a user can perform
Admin Access | Elevated privileges
Role-Based Access Control (RBAC) | Permission based on job role
Least Privilege | Minimum access necessary

## Accounting 
Concept | Definition|
--------|-----------|
Accounting | Logging and monitoring activity
Event Log | Record of events
Audit Trail | Historical record of actions
User Activity Monitoring | Tracking user behaviour

## Core Principles

- Least privilege
- Need to know
- Separation of duties
- Deny by default
- Regular access reviews
- Immediate removal of obsolete access
- Time-limited privileged access

## Example Access Review Questions

- Does the user still require the account?
- Does the role still justify the permissions?
- Are privileged accounts separate from daily accounts?
- Are inactive accounts disabled?
- Are temporary permissions expired?
- Are access changes logged and approved? 


## Authentication & Authorization 
Concept | Purpose|
--------|--------|
Username| Identification|
Password |Authentication
MFA | Authentication
OAuth | Authorization framework
SSO | Single Signe-On
Digital Certificate | Identity verification in PKI

## Hashing
Concept | Purpose|
--------|--------|
Hashing | Verify data integrity
SHA-256 |Generate a hash value
Hash Comparison | Detect modifications
Integrity | Ensure data has not changed
