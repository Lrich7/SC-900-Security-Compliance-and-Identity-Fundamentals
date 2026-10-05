# 📝 SC-900 Cheat Sheet

A condensed review of the most important concepts from **Microsoft
SC-900 --- Security, Compliance, and Identity Fundamentals**.

Use this for quick review before practice exams or the certification
exam.

------------------------------------------------------------------------

# 🧠 Four-Platform Memory Map

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

# 🔐 Core Security Concepts

## CIA Triad

``` text
CONFIDENTIALITY
→ Prevent unauthorized access

INTEGRITY
→ Prevent unauthorized modification

AVAILABILITY
→ Keep systems and data accessible
```

## Zero Trust

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE
ASSUME BREACH
```

## Defense in Depth

Use multiple security layers so one failed control does not expose the
entire environment.

``` text
Physical
Identity
Perimeter
Network
Compute
Application
Data
```

## Shared Responsibility

``` text
ON-PREMISES
→ Customer manages almost everything

IAAS
→ Provider manages physical infrastructure
→ Customer manages more of the OS/apps/data

PAAS
→ Provider manages more of the platform
→ Customer focuses more on apps/data/access

SAAS
→ Provider manages most infrastructure/application stack
→ Customer still manages identities, access, data, and configuration
```

------------------------------------------------------------------------

# 👤 Identity Fundamentals

``` text
AUTHENTICATION
→ Who are you?

AUTHORIZATION
→ What are you allowed to do?
```

Authentication factors:

``` text
Something you KNOW
Something you HAVE
Something you ARE
```

MFA requires **two or more different factor types**.

Two passwords are not MFA.

------------------------------------------------------------------------

# 👤 Microsoft Entra

``` text
MICROSOFT ENTRA
→ Identity & Access
```

Microsoft Entra ID was previously called **Azure Active Directory (Azure
AD)**.

Important features:

``` text
Users
Groups
Devices
Applications
Authentication
MFA
Passwordless
Conditional Access
Roles
Identity Protection
Identity Governance
PIM
Access Reviews
Entitlement Management
```

## Identity Types

``` text
Human Identity
Device Identity
Workload Identity
External Identity
Agent Identity
```

## Device Identity

``` text
Entra Registered
Entra Joined
Entra Hybrid Joined
```

## Conditional Access

Think:

``` text
IF
→ User / Device / Location / Risk / App

THEN
→ Allow / Block / Require MFA /
   Require compliant device /
   Require authentication strength
```

## Roles

``` text
MICROSOFT ENTRA ROLE
→ Directory / identity administration

AZURE RBAC
→ Azure resource authorization
```

## Identity Protection

``` text
USER RISK
→ Probability identity is compromised

SIGN-IN RISK
→ Probability a specific sign-in is suspicious
```

## Identity Governance

``` text
PIM
→ Just-in-time privileged access

ACCESS REVIEWS
→ Review whether access is still needed

ENTITLEMENT MANAGEMENT
→ Access packages and access lifecycle

LIFECYCLE WORKFLOWS
→ Joiner / Mover / Leaver automation
```

------------------------------------------------------------------------

# 🔑 Passwordless Authentication

``` text
Passkeys / FIDO2
Windows Hello for Business
Microsoft Authenticator
Temporary Access Pass
```

TAP is especially useful for onboarding or recovery.

Passkeys/FIDO2 and Windows Hello can provide strong phishing-resistant
authentication.

------------------------------------------------------------------------

# ☁️ Azure Infrastructure Security

``` text
NSG
→ Network traffic rules

AZURE FIREWALL
→ Centralized network protection

DDoS PROTECTION
→ Availability against DDoS attacks

AZURE BASTION
→ Secure VM access without exposing RDP/SSH publicly

KEY VAULT
→ Secrets, keys, certificates

RESOURCE LOCK
→ Prevent accidental deletion/change

AZURE POLICY
→ Enforce/evaluate resource standards

AZURE RBAC
→ Control Azure resource permissions
```

------------------------------------------------------------------------

# 🛡️ Microsoft Defender

## Defender for Cloud

``` text
CSPM
→ Cloud Security Posture Management

CWPP
→ Cloud Workload Protection
```

``` text
SECURE SCORE / RECOMMENDATIONS
→ Improve security posture

ALERT
→ Potential security threat
```

## Defender Services

``` text
DEFENDER FOR ENDPOINT
→ Endpoint/device threats

DEFENDER FOR OFFICE 365
→ Email and collaboration threats

DEFENDER FOR IDENTITY
→ Identity threats involving on-premises AD signals

DEFENDER FOR CLOUD APPS
→ SaaS / cloud app visibility and control

DEFENDER VULNERABILITY MANAGEMENT
→ Vulnerability assessment/prioritization

DEFENDER XDR
→ Correlates security signals across services
```

## Defender XDR

``` text
ALERT
→ Individual suspicious activity

INCIDENT
→ Related alerts grouped into an attack story
```

------------------------------------------------------------------------

# 📡 Microsoft Sentinel

``` text
MICROSOFT SENTINEL
→ SIEM + SOAR
```

``` text
SIEM
→ Collect, analyze, detect, investigate

SOAR
→ Automate and orchestrate response
```

Important features:

``` text
Data Connectors
Analytics Rules
Incidents
Hunting
KQL
Workbooks
Automation Rules
Playbooks
Threat Intelligence
```

------------------------------------------------------------------------

# 🏷️ Microsoft Purview

``` text
SERVICE TRUST PORTAL
→ Microsoft trust/compliance documentation

COMPLIANCE MANAGER
→ Compliance posture and assessments

COMPLIANCE SCORE
→ Measure improvement progress

INFORMATION PROTECTION
→ Discover, classify, protect data

SENSITIVITY LABEL
→ Classify/protect content

DLP
→ Prevent inappropriate sharing/use

POLICY TIP
→ Warn/educate user

ENDPOINT DLP
→ Protect sensitive data actions on endpoints

DATA LIFECYCLE MANAGEMENT
→ Retention/deletion

RETENTION POLICY
→ Broad location-based retention

RETENTION LABEL
→ Item/content-level retention

RECORDS MANAGEMENT
→ Govern official records

INSIDER RISK MANAGEMENT
→ Identify potential internal risk

eDISCOVERY
→ Legal/investigative content

AUDIT
→ Who did what?

COMMUNICATION COMPLIANCE
→ Communication policy/regulatory risk
```

------------------------------------------------------------------------

# 🎯 Quick Product Selection

  Requirement                       Technology
  --------------------------------- --------------------------------
  Identity and access               Microsoft Entra
  Conditional access decisions      Conditional Access
  Temporary privileged access       PIM
  Review access periodically        Access Reviews
  Azure permissions                 Azure RBAC
  Cloud security posture            Defender for Cloud
  Endpoint threat protection        Defender for Endpoint
  Email threat protection           Defender for Office 365
  Identity threat detection         Defender for Identity
  Cloud app visibility              Defender for Cloud Apps
  Cross-domain attack correlation   Defender XDR
  SIEM/SOAR                         Microsoft Sentinel
  Data classification/protection    Purview Information Protection
  Prevent sensitive data loss       Purview DLP
  Retention/deletion                Data Lifecycle Management
  Official records                  Records Management
  Internal risk                     Insider Risk Management
  Legal content search              eDiscovery
  Activity history                  Audit

------------------------------------------------------------------------

# 🧠 Final Memory Trick

``` text
ENTRA
→ WHO?

DEFENDER
→ WHAT THREAT?

SENTINEL
→ WHAT IS HAPPENING?

PURVIEW
→ WHAT DATA?
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
