# Google Threat Modeling Process

Steps | Purposes | Key Questions|
------|----------|---------|
Define the Scope | Determine the system, application, process, or environment that will be assessed| What are we assessing?
Identify Threat | Identify potential threat actors, threat sources, and threat events | what threats exits?
Characterize the Environment |Understand assets, users, technologies, architecture, data flows, and existing controls| what assets, users, systems, and controls are involved?|
Analyze threat | Evaluate how identified threats could impact assets and business operations |How could these threats affect the organization?
Mitigate Risks | Select and implement security  controls to reduce likelihood or impact | How can we reduce or prevent these threats?
Evaluate findings | Review results, assess effectiveness of mitigations, and prioritize actions | What should be addressed first?

# Example 

Step | Sneaker App Example
-----|---------------------|
Define Scope| Mobile sneaker marketplace application
Identify Threats | SQL injection, session hijacking
Characterize environment | API, PKI, SHA-256, SQL Database
Analyze threats | unauthorized access to user and payment data
Mitigate risks | MFA, Prepared statements, encryption, RBAC
Evaluate findings | Prioritize database and authentication protections

# Related Models

Model| Focus|
-----|------|
Threat Modeling | Defender perspective
Attacker Mindset | Attacker perspective
Risk assessment | Business risk perspective
PASTA | Threat modeling methodology with 7 stages
Attack three | Visual attack path mapping


# PASTA VS Google Threat Modeling

PASTA Stage | Similar Threat Modeling Activity|
------------|---------------------------------|
Define business & security objectives|Define Scope
Define Technical Scope |Characterize Environment
Decompose Application | Characterize Envrionment
Threat Analysis | Identify & Analyze Threats
Vulnerability Analysis | Analyze Threats
Attack Modeling | Analyze Attack Paths
Risk Analyis & Impact | Mitigate risks & evaluate findings


