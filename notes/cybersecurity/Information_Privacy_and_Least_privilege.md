# Information Privacy and Least Privilege

## Information Privacy
Information privacy concerns the appropriate collection, use, storage, sharing, retention, and disposal of personal and sensitive information.

## Personally Identifiable Information
Examples may include:
- Full name
- Address
- Email address
- Employee or customer identifier
- Financial information
- Authentication information
- Health or other protected records

## Least Privilege
Least privilege means granting only the minimum access required to complete an authorized task.

## Risks of Excessive Access
- Accidental disclosure
- Unauthorized modification
- Insider misuse
- Larger impact if an account is compromised
- Difficulty attributing actions
- Regulatory or contractual exposure

Concept | Definition|
--------|-----------|
Information Privacy | Protection of sensitive information from unauthorized access or dislcosure
Least Privilege | Grant only the minimum access required to perform a task
Access Control | Restrict access to authorized users
Data Leak | Unauthorized exposure of information
Role-based access control (RBAC) | Access granted according to job responsabilities
Temporary Access | Access granted for a limited time
Access Review Periodic validation of user permissions

NIST SP 800-53 AC-6

Element | Description|
--------|------------|
Control | Least Privilege
Objective | Limit user access to the minimum necessary
Enhancement | Restrict access based on roles
Enhancement | Automatically revoke temporary access
Enhancement | Maintain activity logs
Enhancement | Audit privileges regularly


## Recommended Controls
- Role-based access control
- MFA
- Access approval workflows
- Periodic access reviews
- Automatic expiry of temporary access
- Logging and audit trails
- Data encryption
- Data minimization
- Secure disposal

## Data Leak Response
1. Identify the exposed information.
2. Preserve evidence.
3. Identify affected users and systems.
4. Restrict or revoke inappropriate access.
5. Notify the appropriate security or privacy contact.
6. Determine whether additional reporting is required.
7. Document corrective actions and lessons learned. 




