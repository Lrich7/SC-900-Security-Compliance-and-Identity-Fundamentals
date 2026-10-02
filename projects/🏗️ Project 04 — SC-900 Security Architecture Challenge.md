# 🏆 Project 04 --- SC-900 Security Architecture Challenge

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Project Type:** Final Capstone Architecture Challenge\
**Covers:** Lessons 01--16\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🏆 Capstone Goal

Design a complete Microsoft security, identity, operations, and
compliance strategy for a fictional organization.

This project combines the entire course:

``` text
SECURITY CONCEPTS
      ↓
MICROSOFT ENTRA
      ↓
AZURE SECURITY
      ↓
MICROSOFT DEFENDER
      ↓
MICROSOFT SENTINEL
      ↓
MICROSOFT PURVIEW
```

You will make architecture decisions instead of simply defining
products.

------------------------------------------------------------------------

# 🏢 Scenario --- Contoso Manufacturing

Contoso Manufacturing has:

``` text
150 Employees
3 Offices
20 Remote Employees
15 Contractors
10 IT / Administrative Users
```

Technology:

``` text
Microsoft 365
Microsoft Entra
Windows Laptops
Microsoft Teams
Exchange Online
SharePoint
OneDrive
Azure
AWS
On-Premises Windows Servers
SaaS Applications
```

Azure:

``` text
12 Virtual Machines
3 Storage Accounts
2 Azure SQL Databases
1 Public Web Application
Virtual Networks
Subnets
Key Vault
Hybrid Connectivity
```

Data:

``` text
Employee Records
Customer Data
Contracts
Financial Information
Engineering Documents
Legal Information
```

------------------------------------------------------------------------

# ⚠️ Current Security Problems

``` text
Password-only authentication exists.

Too many administrators have permanent access.

Contractor access is not reviewed consistently.

Unmanaged devices can access company resources.

VM management ports are exposed.

Secrets exist in application configuration files.

Azure standards are inconsistent.

Cloud posture is difficult to measure.

Phishing attacks reach employees.

Endpoint visibility is weak.

Hybrid identity threats are difficult to detect.

Employees use unsanctioned SaaS applications.

Security alerts are spread across tools.

Security logs exist across multiple platforms.

Incident response is repetitive and manual.

Sensitive data is inconsistently classified.

DLP controls are incomplete.

Retention is inconsistent.

Departing-user risk is not systematically reviewed.

Legal investigations are manual.
```

Your job is to design the future state.

------------------------------------------------------------------------

# 🧭 Part 1 --- Core Security Principles

## Phase 1 --- CIA Triad

Match Contoso requirements.

Keep customer information secret:

``` text
______________________________
```

Prevent unauthorized changes:

``` text
______________________________
```

Keep services available:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧱 Phase 2 --- Defense in Depth

Build the layers:

``` text
PHYSICAL
      ↓
IDENTITY
      ↓
PERIMETER
      ↓
NETWORK
      ↓
COMPUTE
      ↓
APPLICATION
      ↓
DATA
```

Why should Contoso avoid relying on one security control?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🔐 Phase 3 --- Zero Trust

Apply:

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE
ASSUME BREACH
```

Give one Contoso example for each.

Verify explicitly:

``` text
____________________________________
```

Least privilege:

``` text
____________________________________
```

Assume breach:

``` text
____________________________________
```

------------------------------------------------------------------------

# 👤 Part 2 --- Identity Architecture

## Phase 4 --- Identity Platform

Which Microsoft platform should manage cloud identity and access?

``` text
______________________________
```

------------------------------------------------------------------------

# 👥 Phase 5 --- Users and Groups

Contoso wants easier access management.

Complete:

``` text
USER
      ↓
______________________________
      ↓
RESOURCE
```

Why is group-based access usually easier to manage than many direct
assignments?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🌐 Phase 6 --- External Identities

Contractors need limited access.

Which identity concept supports collaboration with external users?

``` text
______________________________
```

What should happen when the contract ends?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🔑 Phase 7 --- Authentication

Contoso wants to reduce password-only authentication.

Recommend:

``` text
Normal Employees:
______________________________

Administrators:
______________________________

New Employee Bootstrap:
______________________________
```

Possible technologies:

``` text
MFA
Microsoft Authenticator
Passkeys / FIDO2
Windows Hello for Business
Temporary Access Pass
Authentication Strength
```

------------------------------------------------------------------------

# 🚪 Phase 8 --- Conditional Access

Design four policy concepts.

## Policy 1 --- Administrators

``` text
IF:
____________________________________

THEN:
____________________________________
```

## Policy 2 --- Risky Sign-In

``` text
IF:
____________________________________

THEN:
____________________________________
```

## Policy 3 --- Unmanaged Device

``` text
IF:
____________________________________

THEN:
____________________________________
```

## Policy 4 --- Sensitive Application

``` text
IF:
____________________________________

THEN:
____________________________________
```

How should policies be safely introduced?

``` text
______________________________
```

------------------------------------------------------------------------

# 👑 Phase 9 --- Administrative Access

Too many IT employees have permanent Global Administrator.

Which principle should guide the redesign?

``` text
______________________________
```

Which governance capability can provide time-limited privileged access?

``` text
______________________________
```

------------------------------------------------------------------------

# 🧑‍⚖️ Phase 10 --- RBAC

Complete:

``` text
MICROSOFT ENTRA ROLE
=
____________________________________
```

``` text
AZURE RBAC
=
____________________________________
```

Azure RBAC combines:

``` text
SECURITY PRINCIPAL
+
______________________________
+
SCOPE
```

------------------------------------------------------------------------

# 🚦 Phase 11 --- Identity Risk and Governance

Potential compromised identity:

``` text
______________________________
```

Review whether users still need access:

``` text
______________________________
```

Package resources for contractors:

``` text
______________________________
```

Automate Joiner / Mover / Leaver processes:

``` text
______________________________
```

Choose from:

``` text
Identity Protection
Access Reviews
Entitlement Management
Lifecycle Workflows
```

------------------------------------------------------------------------

# ☁️ Part 3 --- Azure Infrastructure Security

## Phase 12 --- Network Traffic

Control traffic at subnet/NIC level:

``` text
______________________________
```

Provide centralized network filtering:

``` text
______________________________
```

Protect availability from large network attacks:

``` text
______________________________
```

------------------------------------------------------------------------

# 🖥️ Phase 13 --- Secure VM Administration

Admins currently expose RDP directly to the internet.

Which Azure service provides secure VM access without requiring public
RDP/SSH exposure in the usual design?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔐 Phase 14 --- Secrets

Applications contain secrets in configuration files.

Which Azure service should store:

``` text
Secrets
Keys
Certificates
```

?

``` text
______________________________
```

------------------------------------------------------------------------

# 📋 Phase 15 --- Standards and Permissions

Require Azure resources to follow organizational standards:

``` text
______________________________
```

Control who can manage Azure resources:

``` text
______________________________
```

Prevent accidental deletion of a critical resource:

``` text
______________________________
```

------------------------------------------------------------------------

# 🛡️ Part 4 --- Defender for Cloud

## Phase 16 --- Cloud Posture

Contoso wants to find weaknesses and improve cloud posture.

Which platform fits?

``` text
______________________________
```

Which concept focuses on posture?

``` text
______________________________
```

Which measurement helps summarize posture progress?

``` text
______________________________
```

------------------------------------------------------------------------

# 🛡️ Phase 17 --- Cloud Workload Protection

Contoso also needs threat protection for supported cloud workloads.

Which concept fits?

``` text
______________________________
```

Complete:

``` text
CSPM
=
____________________________________

CWPP
=
____________________________________
```

------------------------------------------------------------------------

# 💻 Part 5 --- Microsoft Defender Security Services

## Phase 18 --- Choose the Defender Service

Endpoint attacks:

``` text
______________________________
```

Phishing and malicious email:

``` text
______________________________
```

Hybrid identity threats:

``` text
______________________________
```

Shadow IT and SaaS visibility:

``` text
______________________________
```

Endpoint vulnerabilities:

``` text
______________________________
```

------------------------------------------------------------------------

# 📧 Phase 19 --- Email Protection

Match:

``` text
Malicious URL
→ ______________________________

Malicious Attachment
→ ______________________________
```

Choose:

``` text
Safe Links
Safe Attachments
```

------------------------------------------------------------------------

# 🚨 Part 6 --- Microsoft Defender XDR

## Phase 20 --- Correlate the Attack

An attacker:

``` text
1. Sends phishing email.
2. User opens malicious content.
3. Endpoint is compromised.
4. Credentials are stolen.
5. Identity is abused.
6. Attacker accesses cloud apps.
```

Which platform can correlate signals across multiple Defender services
into an incident?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔍 Phase 21 --- Alert vs Incident

``` text
ALERT
=
____________________________________
```

``` text
INCIDENT
=
____________________________________
```

Why is correlation useful?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🧪 Phase 22 --- Advanced Hunting

Which Defender XDR capability allows proactive query-based
investigation?

``` text
______________________________
```

Which query language is commonly associated with it?

``` text
______________________________
```

------------------------------------------------------------------------

# 📡 Part 7 --- Microsoft Sentinel

## Phase 23 --- SIEM

Contoso wants centralized security visibility across:

``` text
Microsoft Defender
Azure
AWS
Firewalls
Servers
Identity
Other Sources
```

Which platform fits?

``` text
______________________________
```

What does SIEM mean?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🔌 Phase 24 --- Data Collection

How does Sentinel connect to many data sources?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔎 Phase 25 --- Detection and Hunting

Automatically identify suspicious patterns:

``` text
______________________________
```

Proactively search security data:

``` text
______________________________
```

Visualize security information:

``` text
______________________________
```

Choose from:

``` text
Analytics Rules
Hunting
Workbooks
```

------------------------------------------------------------------------

# ⚡ Phase 26 --- SOAR

What does SOAR represent at a high level?

``` text
____________________________________
```

Complete:

``` text
AUTOMATION RULE
=
____________________________________
```

``` text
PLAYBOOK
=
____________________________________
```

Playbooks are based on:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Phase 27 --- Defender XDR vs Sentinel

Complete:

``` text
DEFENDER XDR
=
____________________________________
____________________________________
```

``` text
SENTINEL
=
____________________________________
____________________________________
```

How can they complement one another?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🏷️ Part 8 --- Microsoft Purview

## Phase 28 --- Compliance Posture

Microsoft trust and audit documentation:

``` text
______________________________
```

Measure organizational compliance progress:

``` text
______________________________
```

Recommended compliance work:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔎 Phase 29 --- Data Classification

Recognize SSNs and credit-card numbers:

``` text
______________________________
```

Classify a document Highly Confidential:

``` text
______________________________
```

------------------------------------------------------------------------

# 🚫 Phase 30 --- Data Loss Prevention

Prevent sensitive information from being emailed externally:

``` text
______________________________
```

Warn the user at the time of action:

``` text
______________________________
```

Control supported endpoint data actions:

``` text
______________________________
```

------------------------------------------------------------------------

# 🗃️ Phase 31 --- Retention and Records

Broad retention:

``` text
______________________________
```

Item/content-based retention:

``` text
______________________________
```

Official records:

``` text
______________________________
```

------------------------------------------------------------------------

# ⚠️ Phase 32 --- Insider Risk

A departing employee downloads hundreds of confidential documents.

Which capability fits?

``` text
______________________________
```

Does an alert prove malicious intent?

``` text
YES / NO
```

------------------------------------------------------------------------

# ⚖️ Phase 33 --- Legal and Audit

Find/preserve information for a lawsuit:

``` text
______________________________
```

Determine who performed an audited activity:

``` text
______________________________
```

Potential communication policy violation:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Part 9 --- Full Product Selection

## Phase 34 --- Match the Requirement

  Requirement                    Microsoft Capability
  ------------------------------ --------------------------------------
  Cloud identity                 \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  MFA/passwordless               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Conditional access decisions   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Temporary privileged access    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Azure network traffic rules    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Central Azure firewall         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Secure VM administration       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Secrets/keys/certificates      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Azure standards                \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud posture                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Endpoint threats               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Email threats                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identity threats               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  SaaS / Shadow IT               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender signal correlation    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  SIEM/SOAR                      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Compliance posture             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Data classification            \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Data loss prevention           \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Retention                      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Insider risk                   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Legal content                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  User/admin activity            \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 🏗️ Part 10 --- Build the Final Architecture

## Phase 35 --- Identity Layer

``` text
USERS / CONTRACTORS
      ↓
______________________________
      ↓
MFA / PASSWORDLESS
      ↓
______________________________
      ↓
APPLICATIONS / RESOURCES
```

------------------------------------------------------------------------

# ☁️ Phase 36 --- Azure Layer

``` text
INTERNET
      ↓
______________________________
      ↓
______________________________
      ↓
NSG
      ↓
APPLICATION / VM
      ↓
______________________________
```

Add:

``` text
Secure Admin Access
→ ______________________________

Standards
→ ______________________________

Permissions
→ ______________________________

Accidental Deletion Protection
→ ______________________________
```

------------------------------------------------------------------------

# 🛡️ Phase 37 --- Defender Layer

``` text
EMAIL
→ ______________________________

ENDPOINT
→ ______________________________

IDENTITY
→ ______________________________

CLOUD APPS
→ ______________________________

CLOUD INFRASTRUCTURE
→ ______________________________

        ↓
______________________________
        ↓
CORRELATED INCIDENT
```

------------------------------------------------------------------------

# 📡 Phase 38 --- Security Operations Layer

``` text
DEFENDER
AZURE
AWS
FIREWALLS
SERVERS
IDENTITY
      ↓
______________________________
      ↓
ANALYTICS
      ↓
INCIDENT
      ↓
INVESTIGATION
      ↓
AUTOMATION
      ↓
PLAYBOOK
```

------------------------------------------------------------------------

# 🏷️ Phase 39 --- Data & Compliance Layer

``` text
DATA
      ↓
DISCOVER / CLASSIFY
      ↓
______________________________
      ↓
PROTECT
      ↓
______________________________
      ↓
PREVENT LOSS
      ↓
______________________________
      ↓
RETAIN / DELETE
      ↓
______________________________
      ↓
INVESTIGATE
      ↓
______________________________
```

------------------------------------------------------------------------

# 🔐 Part 11 --- Zero Trust Review

## Phase 40 --- Verify Explicitly

Identify three technologies from your architecture that help verify
explicitly.

``` text
1. ______________________________
2. ______________________________
3. ______________________________
```

------------------------------------------------------------------------

# 👑 Phase 41 --- Least Privilege

Identify three technologies/processes that support least privilege.

``` text
1. ______________________________
2. ______________________________
3. ______________________________
```

------------------------------------------------------------------------

# 🚨 Phase 42 --- Assume Breach

Identify three technologies/processes that support detection,
investigation, or response after a control fails.

``` text
1. ______________________________
2. ______________________________
3. ______________________________
```

------------------------------------------------------------------------

# 🧱 Part 12 --- Defense in Depth Review

## Phase 43 --- Place the Controls

``` text
IDENTITY
→ ______________________________

NETWORK
→ ______________________________

COMPUTE / ENDPOINT
→ ______________________________

APPLICATION / EMAIL
→ ______________________________

SECURITY OPERATIONS
→ ______________________________

DATA
→ ______________________________
```

------------------------------------------------------------------------

# 🚨 Part 13 --- Final Attack Scenario

## Phase 44 --- The Attack

An attacker:

``` text
1. Sends a phishing email.
2. Employee clicks a malicious link.
3. Endpoint becomes compromised.
4. Credentials are stolen.
5. Attacker attempts risky sign-in.
6. Attacker accesses cloud applications.
7. Sensitive customer files are downloaded.
8. Attacker attempts to email data externally.
9. Security teams investigate.
```

For each step, identify one or more relevant Microsoft controls.

### Step 1 --- Phishing Email

``` text
______________________________
```

### Step 2 --- Malicious Link

``` text
______________________________
```

### Step 3 --- Endpoint Compromise

``` text
______________________________
```

### Step 4 --- Credential Theft

``` text
______________________________
```

### Step 5 --- Risky Sign-In

``` text
______________________________
```

### Step 6 --- Cloud Application Access

``` text
______________________________
```

### Step 7 --- Sensitive Data Download

``` text
______________________________
```

### Step 8 --- External Data Sharing

``` text
______________________________
```

### Step 9 --- Investigation

``` text
______________________________
```

------------------------------------------------------------------------

# 🏆 Phase 45 --- Executive Architecture

Complete the final map:

``` text
                    CONTOSO SECURITY ARCHITECTURE

                           USERS
                             │
                             ▼
                    ┌────────────────┐
                    │ MICROSOFT      │
                    │ ______________ │
                    └───────┬────────┘
                            │
               MFA / PASSWORDLESS / CA
                            │
                            ▼
             ┌──────────────────────────┐
             │ APPLICATIONS & RESOURCES │
             └────────────┬─────────────┘
                          │
          ┌───────────────┼────────────────┐
          ▼               ▼                ▼
      ENDPOINTS          AZURE           M365
          │               │                │
          └───────────────┼────────────────┘
                          ▼
                    MICROSOFT DEFENDER
                          │
                          ▼
                    __________________
                          │
                          ▼
                    SECURITY OPERATIONS

DATA
 │
 ▼
____________________
 │
 ├── Classification
 ├── DLP
 ├── Retention
 ├── Records
 ├── Insider Risk
 ├── eDiscovery
 └── Audit
```

------------------------------------------------------------------------

# 📝 Phase 46 --- Executive Summary

Write a six-to-ten sentence recommendation for Contoso leadership.

Address:

``` text
Identity
Zero Trust
Azure Security
Threat Protection
Security Operations
Data Protection
Compliance
Investigation
```

``` text
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
```

------------------------------------------------------------------------

# ⚡ Phase 47 --- Rapid-Fire Product Challenge

``` text
Identity?
→ __________________

Cloud posture?
→ __________________

Endpoint?
→ __________________

Email?
→ __________________

Identity threats?
→ __________________

Cloud apps?
→ __________________

XDR?
→ __________________

SIEM/SOAR?
→ __________________

Compliance?
→ __________________

Sensitive-data protection?
→ __________________
```

------------------------------------------------------------------------

# 🧠 Phase 48 --- Four-Platform Memory Map

Complete:

``` text
MICROSOFT ENTRA
=
____________________________________

MICROSOFT DEFENDER
=
____________________________________

MICROSOFT SENTINEL
=
____________________________________

MICROSOFT PURVIEW
=
____________________________________
```

------------------------------------------------------------------------

# ✅ Suggested Architecture

## Identity

``` text
Microsoft Entra
      ↓
Users / Groups / External Identities
      ↓
MFA / Passwordless
      ↓
Conditional Access
      ↓
Applications / Resources
```

Governance:

``` text
PIM
Access Reviews
Entitlement Management
Lifecycle Workflows
Identity Protection
```

------------------------------------------------------------------------

## Azure

``` text
INTERNET
      ↓
DDoS Protection
      ↓
Azure Firewall
      ↓
NSG
      ↓
WORKLOAD
      ↓
Key Vault
```

Additional controls:

``` text
Azure Bastion
→ Secure VM administration

Azure Policy
→ Standards

Azure RBAC
→ Permissions

Resource Locks
→ Accidental-change protection
```

------------------------------------------------------------------------

## Cloud Posture

``` text
Microsoft Defender for Cloud

CSPM
→ Find weaknesses / improve posture

Cloud Secure Score
→ Measure posture

CWPP
→ Protect workloads
```

------------------------------------------------------------------------

## Defender

``` text
EMAIL
→ Defender for Office 365

ENDPOINT
→ Defender for Endpoint

IDENTITY
→ Defender for Identity

CLOUD APPS
→ Defender for Cloud Apps

VULNERABILITIES
→ Defender Vulnerability Management

        ↓
Microsoft Defender XDR
        ↓
Correlated Incident
```

------------------------------------------------------------------------

## Sentinel

``` text
DATA SOURCES
      ↓
DATA CONNECTORS
      ↓
MICROSOFT SENTINEL
      ↓
ANALYTICS RULES
      ↓
INCIDENT
      ↓
INVESTIGATION / HUNTING
      ↓
AUTOMATION RULE
      ↓
PLAYBOOK
```

``` text
SIEM
→ Visibility / detection / investigation

SOAR
→ Orchestration / automation / response
```

------------------------------------------------------------------------

## Purview

``` text
Service Trust Portal
→ Microsoft trust documentation

Compliance Manager
→ Compliance posture

Information Protection
→ Classification / protection

DLP
→ Prevent inappropriate data use/sharing

Data Lifecycle Management
→ Retention / deletion

Records Management
→ Official records

Insider Risk Management
→ Potential internal risk

eDiscovery
→ Legal / investigative content

Audit
→ User/admin activity

Communication Compliance
→ Communication policy risk
```

------------------------------------------------------------------------

# 🚨 Suggested Attack Response

``` text
Phishing Email
→ Defender for Office 365

Malicious URL
→ Safe Links

Endpoint Compromise
→ Defender for Endpoint

Credential / Identity Threat
→ Defender for Identity

Risky Sign-In
→ Identity Protection + Conditional Access

Cloud App Activity
→ Defender for Cloud Apps

Sensitive Data
→ Purview Information Protection

External Sharing
→ DLP

Correlation
→ Defender XDR

Broader Investigation
→ Microsoft Sentinel

User/Admin Activity
→ Purview Audit

Legal Investigation
→ eDiscovery
```

------------------------------------------------------------------------

# 🧠 Final Course Memory Map

``` text
WHO CAN ACCESS?
→ Microsoft Entra

WHAT IS ATTACKING US?
→ Microsoft Defender

WHAT IS HAPPENING ACROSS THE ENVIRONMENT?
→ Microsoft Sentinel

WHAT DATA DO WE HAVE AND HOW MUST WE GOVERN IT?
→ Microsoft Purview
```

------------------------------------------------------------------------

# 🎓 Capstone Outcomes

After completing this project, you should be able to:

``` text
Apply Zero Trust

Design Identity Controls

Choose Authentication Methods

Use Conditional Access Concepts

Apply RBAC and Governance

Select Azure Security Controls

Explain Defender for Cloud

Choose Defender Security Services

Explain Defender XDR

Explain Microsoft Sentinel

Explain SIEM and SOAR

Design Data Protection

Explain Compliance Manager

Choose Purview Controls

Support Security and Legal Investigations
```

------------------------------------------------------------------------

# ✅ Final Completion Checklist

## Security Concepts

-   [ ] CIA Triad
-   [ ] Shared Responsibility
-   [ ] Defense in Depth
-   [ ] Zero Trust

## Microsoft Entra

-   [ ] Users / Groups
-   [ ] MFA
-   [ ] Passwordless
-   [ ] Conditional Access
-   [ ] RBAC
-   [ ] Identity Protection
-   [ ] Identity Governance

## Azure Security

-   [ ] NSG
-   [ ] Azure Firewall
-   [ ] DDoS Protection
-   [ ] Azure Bastion
-   [ ] Key Vault
-   [ ] Azure Policy
-   [ ] Resource Locks

## Microsoft Defender

-   [ ] Defender for Cloud
-   [ ] Defender for Endpoint
-   [ ] Defender for Office 365
-   [ ] Defender for Identity
-   [ ] Defender for Cloud Apps
-   [ ] Defender XDR

## Microsoft Sentinel

-   [ ] SIEM
-   [ ] SOAR
-   [ ] Data Connectors
-   [ ] Analytics
-   [ ] Hunting
-   [ ] Automation
-   [ ] Playbooks

## Microsoft Purview

-   [ ] Compliance Manager
-   [ ] Information Protection
-   [ ] DLP
-   [ ] Retention
-   [ ] Records Management
-   [ ] Insider Risk
-   [ ] eDiscovery
-   [ ] Audit
-   [ ] Communication Compliance

------------------------------------------------------------------------

# 🎉 Course Projects Complete

You have completed:

``` text
🏗️ Project 01
Secure an Organization's Identity Environment

🏗️ Project 02
Build a Microsoft Security Strategy

🏗️ Project 03
Build a Compliance & Data Protection Strategy

🏆 Project 04
SC-900 Security Architecture Challenge
```

Next:

# 📝 Practice Exams

Recommended sequence:

``` text
Practice Exam 1
→ Lessons 01–08

Practice Exam 2
→ Lessons 09–16

Final Exam
→ Lessons 01–16
```

------------------------------------------------------------------------

# 📚 Course Navigation

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](README.md)**

🏠 **[Return to Main README](../README.md)**
