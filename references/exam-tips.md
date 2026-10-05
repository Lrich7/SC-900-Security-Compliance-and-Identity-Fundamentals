# 🎯 SC-900 Exam Tips

Practical tips for recognizing SC-900 concepts and answering
fundamentals-level questions.

This page is designed to help you **recognize what a question is
testing**, not memorize answer letters.

------------------------------------------------------------------------

# 🧠 Tip 1 --- Identify the Product Family First

Before looking at individual features, ask:

``` text
IS THIS ABOUT...

IDENTITY?
→ Entra

THREATS?
→ Defender

SECURITY OPERATIONS?
→ Sentinel

DATA / COMPLIANCE?
→ Purview
```

This can eliminate several wrong answers quickly.

------------------------------------------------------------------------

# 👤 Tip 2 --- Authentication vs Authorization

``` text
AUTHENTICATION
→ Who are you?

AUTHORIZATION
→ What can you do?
```

If the question is about proving identity, think **authentication**.

If it is about permissions after sign-in, think **authorization**.

------------------------------------------------------------------------

# 🔐 Tip 3 --- Remember the Zero Trust Trio

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE
ASSUME BREACH
```

Common clues:

``` text
Evaluate signals
→ Verify Explicitly

Only necessary permissions
→ Least Privilege

Monitor as though compromise is possible
→ Assume Breach
```

------------------------------------------------------------------------

# 🔑 Tip 4 --- Two Passwords Are Not MFA

MFA requires different factor categories.

``` text
KNOW
HAVE
ARE
```

Two things you know are still the same factor type.

------------------------------------------------------------------------

# 🚦 Tip 5 --- Conditional Access Is IF → THEN

``` text
IF
Risk / Device / Location / User / App

THEN
Require MFA / Block /
Require compliant device /
Require stronger authentication
```

If the question describes access conditions, think **Conditional
Access**.

------------------------------------------------------------------------

# 👑 Tip 6 --- Entra Role vs Azure RBAC

``` text
MANAGE USERS / DIRECTORY?
→ Microsoft Entra Role

MANAGE AZURE RESOURCE ACCESS?
→ Azure RBAC
```

------------------------------------------------------------------------

# ⏱️ Tip 7 --- Temporary Admin = PIM

``` text
JUST-IN-TIME
PRIVILEGED ACCESS
→ PIM
```

If someone should become an administrator only when needed, PIM is a
strong clue.

------------------------------------------------------------------------

# 🔍 Tip 8 --- Review Existing Access = Access Reviews

``` text
DO THEY STILL NEED ACCESS?
→ Access Reviews
```

------------------------------------------------------------------------

# ⚠️ Tip 9 --- User Risk vs Sign-In Risk

``` text
USER RISK
→ Is the identity compromised?

SIGN-IN RISK
→ Is this login attempt suspicious?
```

------------------------------------------------------------------------

# ☁️ Tip 10 --- Know the Azure Security Tools

``` text
TRAFFIC RULES
→ NSG

CENTRAL NETWORK FIREWALL
→ Azure Firewall

DDoS ATTACK
→ DDoS Protection

SECURE VM CONNECTION
→ Azure Bastion

SECRETS / KEYS / CERTIFICATES
→ Key Vault

RESOURCE STANDARDS
→ Azure Policy

RESOURCE PERMISSIONS
→ Azure RBAC

ACCIDENTAL DELETE
→ Resource Lock
```

------------------------------------------------------------------------

# 🛡️ Tip 11 --- Know Which Defender

``` text
CLOUD POSTURE
→ Defender for Cloud

ENDPOINT
→ Defender for Endpoint

EMAIL / PHISHING
→ Defender for Office 365

IDENTITY ATTACK
→ Defender for Identity

SAAS / SHADOW IT
→ Defender for Cloud Apps

VULNERABILITIES
→ Defender Vulnerability Management

CORRELATED ATTACK STORY
→ Defender XDR
```

------------------------------------------------------------------------

# 📡 Tip 12 --- Sentinel = SIEM + SOAR

``` text
SIEM
→ Collect / Analyze / Detect / Investigate

SOAR
→ Automate / Orchestrate / Respond
```

Common Sentinel clues:

``` text
Data Connectors
Analytics Rules
Hunting
Workbooks
Playbooks
Automation
```

------------------------------------------------------------------------

# 🏷️ Tip 13 --- Know the Purview Keywords

``` text
COMPLIANCE POSTURE
→ Compliance Manager

CLASSIFY / PROTECT
→ Information Protection

PREVENT SHARING
→ DLP

KEEP / DELETE
→ Data Lifecycle Management

OFFICIAL RECORD
→ Records Management

INTERNAL RISK
→ Insider Risk Management

LEGAL SEARCH
→ eDiscovery

WHO DID WHAT?
→ Audit

RISKY COMMUNICATION
→ Communication Compliance
```

------------------------------------------------------------------------

# 🆚 Tip 14 --- Sensitivity Label vs DLP

``` text
SENSITIVITY LABEL
→ What is this data and how should it be protected?

DLP
→ What actions should be prevented or controlled?
```

A document can use both.

------------------------------------------------------------------------

# 🗓️ Tip 15 --- Retention Policy vs Retention Label

``` text
BROAD LOCATION/WORKLOAD
→ Retention Policy

SPECIFIC ITEM/CONTENT
→ Retention Label
```

------------------------------------------------------------------------

# 🚨 Tip 16 --- Alert vs Incident

``` text
ALERT
→ Individual suspicious event/activity

INCIDENT
→ Related alerts grouped into an attack story
```

------------------------------------------------------------------------

# 📊 Tip 17 --- Score Does Not Equal Guarantee

``` text
COMPLIANCE SCORE
≠
LEGAL GUARANTEE

SECURE SCORE
≠
PERFECT SECURITY
```

Scores help prioritize improvements.

------------------------------------------------------------------------

# 🧩 Tip 18 --- Read the Requirement, Not the Product Name

Microsoft exam questions may include several real Microsoft products.

Ask:

``` text
WHAT IS THE REQUIREMENT?
```

Then select the technology whose **primary purpose** matches it.

------------------------------------------------------------------------

# 🚫 Tip 19 --- Watch for Absolute Language

Be cautious with statements such as:

``` text
ALWAYS
NEVER
GUARANTEES
ELIMINATES ALL RISK
```

Security tools usually **reduce, detect, manage, or help protect against
risk** rather than guaranteeing perfect security.

------------------------------------------------------------------------

# 📝 Tip 20 --- Fundamentals Means Purpose Over Configuration

SC-900 is a fundamentals exam.

Prioritize knowing:

``` text
WHAT IS IT?

WHAT DOES IT DO?

WHEN WOULD I USE IT?

HOW IS IT DIFFERENT?
```

You generally do not need deep configuration knowledge.

------------------------------------------------------------------------

# 🎯 Final Rapid Review

``` text
ENTRA
→ Identity

DEFENDER
→ Threat Protection

SENTINEL
→ SIEM / SOAR

PURVIEW
→ Data / Compliance

ZERO TRUST
→ Verify / Least Privilege / Assume Breach

CONDITIONAL ACCESS
→ IF / THEN

PIM
→ Temporary Privilege

DLP
→ Prevent Data Loss

eDISCOVERY
→ Legal Search

AUDIT
→ Who Did What?
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
