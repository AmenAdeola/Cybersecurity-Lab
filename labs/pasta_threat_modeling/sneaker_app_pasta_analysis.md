# PASTA Threat Modeling Analysis


## Scenario

A Sneaker marketplace company is preparing to launch a mobile application that allows buyers and sellers to trade sneakers online.

The application will:
-  Allow users to sign up and manage accounts
-  Support buyer-to-seller messaging
-  Process payments
-  Store inventory information
-  Protect customer privacy

----------------------

# Stage I - Define Business and Security Objectives

## Business Objectives
-  Provide a secure marketplace where buyers and sellers can connect.
-  Protect customer information and ensure user privacy.
-  Provide secure payment processing and prevent payment fraud.
-----------

# Stage II - Define the Technical Scope

## Technology Prioritized
The SQL database should be prioritized because it stores user accounts, inventory listings, seller information, and payment-related data. If an attacker successfully compromises the database through SQL injection or unauthorized access, sensitive customer information could be exposed. Because the database contains critical business data, it represents one of the highest-value targets in the application.

## Technologies Used
-  API
-  Public Key Infrastructure (PKI)
-  SHA-256
-  SQL Database

-------------------

# Stage III - Decompose the Application

## Data Flow Summary
'''text
User->Product Search Returned->Database->Inventory Results Returned
'''

## Assets Identified
-  Customer Data
-  User Accounts
-  Product Listings
-  Payment Information
-  Seller Information

----------------------

# Stage IV - Threat Analysis

## Threat 1

### SQL injection
An attacker could submit malicious SQL commands through application inputs to access, modify, or  delete information stored in the database

### Threat type:  External Threat

## Threat 2

### Session Hijacking
An attacker could steal or reuse session tokens and gain unauthorized access to user accounts.

### Threat type: External Threat

----------------

# Stage V - Vulnerability Analysis

## Vulnerability 1

### Lack of Prepared Statements

Failure to use parameterized queries may allow SQL injection attacks against the database

## Vulnerability 2

### Weak Authentication Controls
Weak passwords or insufficient session protection could enable account compromise and session hijacking.

------------------

# Stage VI - Attack Modeling

## Asset
User  Data

### Attack Path 1
''' text User Data->SQL Injection->Lack of Prepared Statements
'''

## Attack Path 2
... text User data->Session Hijacking->weak login credentials
'''

The attack tree demonstrates how attackers could compromises user information by exploiting weaknesses in the application and database environment.

--------------------

# Stage VII - Risk Analysis and Impact 

## Security Controls

### 1- Multi-Factor Authentication (MFA)

Reduce the likelihood of unauthorized account access.

### 2- Prepared SQL Statements

Protect the database from SQL injection attacks.

### 3- Encryption (AES / PKI)

Protect sensitive user and payment information during storage and transmission.

### 4- Least Privilege and Role-Based Access Controls (RBAC)

Limit access to sensitive data and administrative function.
-------------------

# Key Takeways

-  Database are high-value targets because they contain sensitive business and customer information.
-  SQL injection and session hijacking are common attack paths against web and mobile application
-  Threat modeling helps identify security weaknesses before deployment.
-  PASTA provides a structured process for analyzing threats, vulnerabilities, and business risk.
-  Security controls should be implemented early in the software development lifecycle.

## Skills Demonstrated

-  Threat Modeling
-  Secure Application Design
-  Threat Analysis
-  Vulnerability Analysis
-  Attack Surface Analysis
-  Security Control Selection
-  Risk Mitigation
