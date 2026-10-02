# 📘 Lesson 14 --- Microsoft Purview & Compliance

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 14\
**Section:** Microsoft Compliance Solutions\
**Lab:** 🔵 Explore the Tool --- Microsoft Purview

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Explain Microsoft Purview and its role in data security, governance,
    risk, and compliance
-   Describe the Microsoft Service Trust Portal
-   Explain Microsoft Purview Compliance Manager
-   Describe Compliance Score and improvement actions
-   Explain security versus compliance
-   Recognize Information Protection, DLP, Data Lifecycle Management,
    Records Management, eDiscovery, Audit, Insider Risk Management, and
    Communication Compliance
-   Choose the appropriate Purview capability for common SC-900
    scenarios

------------------------------------------------------------------------

# 🧭 Welcome to the Compliance Section

Lessons 09--13 focused on protecting infrastructure and detecting
threats.

The final section shifts toward:

``` text
Data
Compliance
Governance
Privacy
Risk
Investigation
```

A major Microsoft platform for these areas is:

# Microsoft Purview

------------------------------------------------------------------------

# 🧠 Security vs Compliance

Security protects systems, users, devices, applications, networks, and
data from threats and unauthorized access.

Compliance focuses on meeting:

``` text
Laws
Regulations
Industry Standards
Contractual Requirements
Internal Policies
```

A security control can also help satisfy a compliance requirement.

------------------------------------------------------------------------

# ⚠️ Shared Responsibility

Using Microsoft cloud services does not automatically make an
organization compliant.

Microsoft manages responsibilities associated with operating its cloud
services. Customers remain responsible for areas such as:

``` text
Configuration
Access
Data Classification
Retention
Policies
Organizational Processes
Applicable Requirements
```

Think:

``` text
MICROSOFT RESPONSIBILITY
+
CUSTOMER RESPONSIBILITY
=
SHARED COMPLIANCE EFFORT
```

------------------------------------------------------------------------

# 🛡️ What Is Microsoft Purview?

At the SC-900 level:

``` text
MICROSOFT PURVIEW
=
DATA SECURITY
+
DATA GOVERNANCE
+
RISK
+
COMPLIANCE
```

The Purview portal can expose different solutions depending on
licensing, permissions, tenant configuration, and Microsoft updates.

Common portal:

``` text
https://purview.microsoft.com
```

------------------------------------------------------------------------

# 🏛️ Service Trust Portal

The Microsoft Service Trust Portal provides information about
Microsoft's security, privacy, compliance, audit, and trust practices.

Common portal:

``` text
https://servicetrust.microsoft.com
```

Memory:

``` text
SERVICE TRUST PORTAL
=
Microsoft trust,
audit, and compliance
documentation
```

It is not the same as Compliance Manager.

------------------------------------------------------------------------

# 📊 Compliance Manager

Microsoft Purview Compliance Manager helps organizations assess and
manage compliance activities.

It can help organizations:

``` text
Assess Compliance Posture
Track Improvement Actions
Understand Responsibilities
Prioritize Compliance Work
Measure Progress
```

------------------------------------------------------------------------

# 📈 Compliance Score

Compliance Manager includes a Compliance Score that helps measure
progress toward completing recommended improvement actions.

``` text
COMPLIANCE REQUIREMENTS
      ↓
CONTROLS / ACTIONS
      ↓
IMPROVEMENT ACTIONS
      ↓
COMPLIANCE SCORE
```

A high score does **not** guarantee legal or regulatory compliance.

It helps:

``` text
Measure Progress
Prioritize Actions
Track Improvements
```

------------------------------------------------------------------------

# 📝 Improvement Actions

Improvement actions are activities an organization can take to improve
compliance posture.

They can involve:

``` text
Technical Controls
Policies
Procedures
Administrative Activities
```

Memory:

``` text
COMPLIANCE MANAGER
      ↓
WHAT SHOULD WE IMPROVE?
      ↓
IMPROVEMENT ACTIONS
```

------------------------------------------------------------------------

# 📋 Assessments

Compliance Manager assessments help evaluate compliance posture against
particular standards or requirements.

``` text
STANDARD / REGULATION
      ↓
ASSESSMENT
      ↓
CONTROLS
      ↓
IMPROVEMENT ACTIONS
      ↓
PROGRESS
```

Applicable requirements depend on the organization's industry, location,
data, and activities.

------------------------------------------------------------------------

# 🗂️ Data Governance

Data governance helps organizations answer:

``` text
What data do we have?
Where is it?
Who owns it?
What does it mean?
Is it sensitive?
How should it be managed?
```

A useful flow is:

``` text
DISCOVER
      ↓
UNDERSTAND
      ↓
CLASSIFY
      ↓
PROTECT
      ↓
GOVERN
```

------------------------------------------------------------------------

# 🏷️ Information Protection

Microsoft Purview Information Protection helps organizations discover,
classify, and protect sensitive information.

Examples include:

``` text
Social Security Numbers
Credit Card Numbers
Health Information
Financial Data
Employee Information
Confidential Business Data
```

Sensitivity labels are an important Information Protection concept.

Lesson 15 explores these in greater detail.

------------------------------------------------------------------------

# 🚫 Data Loss Prevention --- DLP

DLP helps organizations identify and protect sensitive information from
inappropriate use or sharing.

``` text
EMPLOYEE
      ↓
Attempts to share
sensitive information
      ↓
DLP POLICY
      ↓
Detect / Warn / Restrict
depending on policy
```

Memory:

``` text
DLP
=
Help prevent inappropriate
use or sharing of
sensitive information
```

------------------------------------------------------------------------

# 🗃️ Data Lifecycle Management

Organizations need rules for how long information is kept.

``` text
CREATE
      ↓
USE
      ↓
RETAIN
      ↓
DELETE
```

Retention can be driven by business, legal, regulatory, or
internal-policy requirements.

------------------------------------------------------------------------

# 📁 Records Management

Some information must be treated as an official organizational record.

Records Management helps govern those records and their retention
requirements.

``` text
NORMAL DATA
vs
OFFICIAL RECORD
```

------------------------------------------------------------------------

# 🔎 eDiscovery

eDiscovery helps organizations identify, preserve, collect, review, and
manage electronic information for legal or investigative purposes.

``` text
LEGAL REQUEST
      ↓
FIND RELEVANT DATA
      ↓
PRESERVE
      ↓
COLLECT / REVIEW
```

Lesson 16 explores eDiscovery further.

------------------------------------------------------------------------

# 🧾 Audit

Microsoft Purview Audit helps authorized users search and investigate
recorded user and administrator activities.

Memory:

``` text
AUDIT
=
WHO DID WHAT?
```

------------------------------------------------------------------------

# ⚠️ Insider Risk Management

Potential insider risks can include:

``` text
Data Theft
Inappropriate Sharing
Departing Employee Risk
Policy Violations
Accidental Data Exposure
```

Insider Risk Management helps identify and investigate potential
malicious or inadvertent insider risks.

An alert indicates potential risk requiring review; it does not
automatically prove malicious intent.

------------------------------------------------------------------------

# 💬 Communication Compliance

Communication Compliance helps organizations detect and review potential
regulatory or business-conduct violations in supported communications.

Examples can include:

``` text
Sensitive Information Sharing
Regulated Communications
Harassing or Threatening Language
Business Conduct Violations
```

------------------------------------------------------------------------

# 🧠 Purview Capability Map

``` text
MICROSOFT TRUST DOCUMENTS
→ Service Trust Portal

COMPLIANCE POSTURE
→ Compliance Manager

CLASSIFY / PROTECT DATA
→ Information Protection

STOP INAPPROPRIATE SHARING
→ Data Loss Prevention

KEEP / DELETE DATA
→ Data Lifecycle Management

OFFICIAL RECORDS
→ Records Management

LEGAL INVESTIGATION
→ eDiscovery

WHO DID WHAT?
→ Audit

INTERNAL USER RISK
→ Insider Risk Management

COMMUNICATION POLICY RISK
→ Communication Compliance
```

------------------------------------------------------------------------

# 🏢 Contoso Example

``` text
Track compliance progress
→ Compliance Manager

Find Microsoft audit/trust documents
→ Service Trust Portal

Protect sensitive HR data
→ Information Protection

Stop sensitive external sharing
→ DLP

Retain information appropriately
→ Data Lifecycle Management

Manage official records
→ Records Management

Find data for a legal case
→ eDiscovery

Investigate user/admin activity
→ Audit

Investigate potential internal risk
→ Insider Risk Management
```

------------------------------------------------------------------------

# 🧠 Microsoft Security Ecosystem

``` text
MICROSOFT ENTRA
=
Identity & Access

MICROSOFT DEFENDER
=
Threat Protection

MICROSOFT SENTINEL
=
Security Operations

MICROSOFT PURVIEW
=
Data Security,
Governance,
Risk,
and Compliance
```

------------------------------------------------------------------------

# 🎯 Exam Focus

``` text
SERVICE TRUST PORTAL
→ Microsoft trust/compliance documentation

COMPLIANCE MANAGER
→ Assess and improve compliance posture

COMPLIANCE SCORE
→ Measure progress

IMPROVEMENT ACTION
→ Recommended compliance work

INFORMATION PROTECTION
→ Discover, classify, protect data

DLP
→ Protect against inappropriate data use/sharing

eDISCOVERY
→ Legal/investigative content

AUDIT
→ User/admin activity

INSIDER RISK
→ Potential internal risk
```

------------------------------------------------------------------------

# ❓ Knowledge Check

1.  What is Microsoft Purview associated with?\
    **A. Data security, governance, risk, and compliance**

2.  Where can organizations find Microsoft trust and compliance
    documentation?\
    **A. Service Trust Portal**

3.  What does Compliance Manager help organizations do?\
    **A. Assess and improve compliance posture**

4.  What does Compliance Score represent?\
    **A. Progress toward recommended compliance actions**

5.  Does Compliance Score guarantee legal compliance?\
    **A. No**

6.  Which capability helps prevent inappropriate sharing of sensitive
    data?\
    **A. Data Loss Prevention**

7.  Which capability helps legal teams locate relevant electronic
    information?\
    **A. eDiscovery**

8.  Which capability helps investigate user/admin activity?\
    **A. Audit**

9.  Which capability focuses on potential internal user risk?\
    **A. Insider Risk Management**

10. Does using Microsoft cloud services automatically make an
    organization compliant?\
    **A. No**

------------------------------------------------------------------------

# 📌 Lesson Summary

``` text
TRUST DOCUMENTS
→ Service Trust Portal

COMPLIANCE PROGRESS
→ Compliance Manager

SENSITIVE DATA
→ Information Protection

STOP DATA LOSS
→ DLP

KEEP / DELETE
→ Data Lifecycle Management

OFFICIAL RECORD
→ Records Management

LEGAL SEARCH
→ eDiscovery

ACTIVITY HISTORY
→ Audit

INTERNAL RISK
→ Insider Risk Management
```

------------------------------------------------------------------------

# 🧪 Lab

## 🔵 Lab 14 --- Explore Microsoft Purview

➡️ **[Lab 14 --- Explore Microsoft
Purview](../labs/%F0%9F%94%B5%20Lab%2014%20%E2%80%94%20Explore%20Microsoft%20Purview.md)**

------------------------------------------------------------------------

# ➡️ Next Lesson

## 📘 Lesson 15 --- Information Protection, DLP & Data Lifecycle

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Purview](https://learn.microsoft.com/en-us/purview/)
-   [Microsoft Purview Portal](https://purview.microsoft.com/)
-   [Compliance
    Manager](https://learn.microsoft.com/en-us/purview/compliance-manager)
-   [Service Trust Portal](https://servicetrust.microsoft.com/)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Project 02 --- Build a Microsoft Security Strategy**

🧪 **[Lab
14](../labs/%F0%9F%94%B5%20Lab%2014%20%E2%80%94%20Explore%20Microsoft%20Purview.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏠 **[Return to Main README](../README.md)**
