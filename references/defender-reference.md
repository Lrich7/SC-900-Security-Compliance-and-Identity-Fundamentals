# 🛡️ Microsoft Defender Reference

A quick-reference guide to the Microsoft Defender services covered by
SC-900.

------------------------------------------------------------------------

# 🧠 Main Purpose

``` text
MICROSOFT DEFENDER
=
SECURITY & THREAT PROTECTION
```

The name **Microsoft Defender** represents a family of security products
rather than one single tool.

------------------------------------------------------------------------

# ☁️ Microsoft Defender for Cloud

Protects cloud infrastructure and workloads.

Two major concepts:

``` text
CSPM
→ Cloud Security Posture Management

CWPP
→ Cloud Workload Protection Platform
```

## CSPM

Focuses on:

``` text
Security Posture
Recommendations
Standards
Secure Score
Misconfigurations
Attack Paths
```

## CWPP

Focuses on protecting cloud workloads such as:

``` text
Servers
Containers
Databases
Storage
Other Cloud Resources
```

## Remember

``` text
RECOMMENDATION
→ Improve posture

ALERT
→ Potential threat
```

Defender for Cloud can support Azure, hybrid, and multicloud
environments.

------------------------------------------------------------------------

# 💻 Defender for Endpoint

Protects endpoint devices.

Think:

``` text
LAPTOPS
DESKTOPS
SERVERS
ENDPOINT THREATS
```

Capabilities can include:

``` text
Endpoint Detection and Response
Threat Detection
Investigation
Response
Vulnerability Information
```

Memory:

``` text
DEVICE ATTACK?
→ Defender for Endpoint
```

------------------------------------------------------------------------

# 📧 Defender for Office 365

Protects email and collaboration workloads.

Think:

``` text
Phishing
Malicious Links
Malicious Attachments
Email Threats
Teams/Collaboration Threats
```

Important features:

``` text
Safe Links
Safe Attachments
```

Memory:

``` text
PHISHING EMAIL?
→ Defender for Office 365
```

------------------------------------------------------------------------

# 👤 Defender for Identity

Uses identity-related signals, especially from on-premises Active
Directory environments, to detect identity threats.

Think:

``` text
Credential Theft
Suspicious Authentication
Identity Reconnaissance
Lateral Movement
Compromised Accounts
```

Memory:

``` text
IDENTITY ATTACK?
→ Defender for Identity
```

Do not confuse it with **Microsoft Entra ID**.

``` text
ENTRA
→ Identity & access platform

DEFENDER FOR IDENTITY
→ Identity threat detection
```

------------------------------------------------------------------------

# ☁️ Defender for Cloud Apps

Provides visibility and control for cloud applications and SaaS usage.

Think:

``` text
Cloud Apps
SaaS
Shadow IT
App Discovery
Cloud App Risk
```

Memory:

``` text
UNSANCTIONED CLOUD APP?
→ Defender for Cloud Apps
```

------------------------------------------------------------------------

# 🩺 Defender Vulnerability Management

Helps identify, assess, and prioritize vulnerabilities.

Think:

``` text
WHAT IS VULNERABLE?
WHAT SHOULD WE FIX FIRST?
```

------------------------------------------------------------------------

# 🧩 Microsoft Defender XDR

Correlates signals across multiple security domains.

Sources can include:

``` text
Endpoints
Identities
Email
Applications
Cloud Apps
```

## Alert vs Incident

``` text
ALERT
→ Individual suspicious activity

INCIDENT
→ Related alerts correlated into an attack story
```

Important concepts:

``` text
Incidents
Alerts
Evidence
Entities
Automated Investigation and Response
Advanced Hunting
KQL
```

------------------------------------------------------------------------

# 🔎 Advanced Hunting

Used to proactively search security data.

Common query language:

``` text
KQL
→ Kusto Query Language
```

At SC-900 level, know its purpose rather than memorizing complex
queries.

------------------------------------------------------------------------

# 🆚 Defender for Cloud vs Defender for Cloud Apps

``` text
DEFENDER FOR CLOUD
→ Cloud infrastructure/workloads/security posture

DEFENDER FOR CLOUD APPS
→ SaaS/cloud application visibility and control
```

------------------------------------------------------------------------

# 🆚 Defender XDR vs Sentinel

``` text
DEFENDER XDR
→ Correlates Microsoft Defender security signals
  into incidents and attack stories

MICROSOFT SENTINEL
→ SIEM/SOAR across broader security data
```

They can work together.

------------------------------------------------------------------------

# 🧠 Which Defender?

``` text
CLOUD POSTURE / WORKLOADS
→ Defender for Cloud

ENDPOINT
→ Defender for Endpoint

EMAIL / PHISHING
→ Defender for Office 365

IDENTITY THREAT
→ Defender for Identity

SAAS / SHADOW IT
→ Defender for Cloud Apps

VULNERABILITIES
→ Defender Vulnerability Management

CROSS-DOMAIN ATTACK
→ Defender XDR
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
