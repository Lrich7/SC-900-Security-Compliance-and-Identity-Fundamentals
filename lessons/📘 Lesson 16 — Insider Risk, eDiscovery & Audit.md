# 📘 Lesson 16 --- Insider Risk, eDiscovery & Audit

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 16\
**Section:** Microsoft Compliance Solutions\
**Lab:** 🟡 Scenario Lab --- Investigate Risk & Compliance Events\
**Milestone:** Final Lesson

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Explain Microsoft Purview Insider Risk Management
-   Describe insider risk policies, indicators, alerts, and cases
-   Explain privacy considerations for insider-risk investigations
-   Describe Microsoft Purview eDiscovery
-   Explain preservation, search, review, and export at a fundamentals
    level
-   Describe Microsoft Purview Audit
-   Distinguish Insider Risk Management, eDiscovery, and Audit
-   Recognize Communication Compliance at a fundamentals level
-   Choose the correct Purview capability for common investigation
    scenarios

------------------------------------------------------------------------

# 🧭 The Final SC-900 Lesson

Earlier Purview lessons focused on compliance posture and protecting
data. This lesson asks:

``` text
IS INTERNAL ACTIVITY CREATING RISK?

WHAT HAPPENED?

WHO DID IT?

WHERE IS THE RELEVANT CONTENT?

DO COMMUNICATIONS VIOLATE POLICY?
```

The main SC-900 capabilities are:

``` text
Insider Risk Management
eDiscovery
Audit
```

------------------------------------------------------------------------

# ⚠️ What Is Insider Risk?

Potential insider risk can be malicious, accidental, or negligent.

Examples:

``` text
Data Leakage
Intellectual Property Theft
Security Policy Violations
Unusual Data Exfiltration
Risky Activity by Departing Users
```

An alert does not automatically prove malicious intent. Organizations
must investigate context and follow applicable legal, privacy, HR, and
compliance requirements.

------------------------------------------------------------------------

# 🛡️ Insider Risk Management

Microsoft Purview Insider Risk Management correlates signals to identify
potential malicious or inadvertent insider risks.

``` text
USER ACTIVITY
      ↓
SIGNALS / INDICATORS
      ↓
INSIDER RISK POLICY
      ↓
ALERT
      ↓
REVIEW / TRIAGE
      ↓
CASE
      ↓
INVESTIGATION
```

------------------------------------------------------------------------

# 🚦 Indicators

Indicators are activities or signals selected for use in insider-risk
policies.

Examples can relate to:

``` text
Downloading Content
External Sharing
Sensitive Data Movement
Potential Exfiltration
Security Violations
```

Memory:

``` text
INDICATOR
=
Activity or signal used
to identify potential risk
```

------------------------------------------------------------------------

# 🚨 Alerts and Cases

``` text
ALERT
=
Potential risk
requiring review
```

An alert does not mean the user is guilty.

``` text
CASE
=
Structured investigation
of an issue
```

Cases help authorized investigators review relevant activity and
determine appropriate next steps.

------------------------------------------------------------------------

# 🔐 Privacy by Design

Insider-risk investigations involve sensitive information. Microsoft
documents privacy-oriented controls including:

``` text
Pseudonymization
Role-Based Access Controls
Administrative Opt-In / Scoping
Audit Logs
```

Pseudonymization can replace identifiable user information with a
nonpersonal identifier for certain roles.

Role separation can distinguish:

``` text
Policy Configuration
Alert Review
Case Investigation
```

This supports least privilege, separation of duties, and privacy.

------------------------------------------------------------------------

# 🧠 Insider Risk Memory Trick

``` text
INSIDER RISK
=
Is internal activity
creating potential risk?
```

------------------------------------------------------------------------

# ⚖️ Microsoft Purview eDiscovery

eDiscovery helps organizations work with electronic information for
legal and investigative needs.

Examples:

``` text
Legal Cases
Internal Investigations
Regulatory Requests
Compliance Investigations
```

At a high level:

``` text
LEGAL / INVESTIGATION NEED
      ↓
IDENTIFY DATA
      ↓
PRESERVE
      ↓
SEARCH / COLLECT
      ↓
REVIEW
      ↓
EXPORT / USE AS REQUIRED
```

------------------------------------------------------------------------

# 🧊 Preservation

Relevant information may need to be preserved while a case is active.

Conceptually:

``` text
LEGAL CASE
      ↓
RELEVANT CONTENT
      ↓
PRESERVATION / HOLD
      ↓
CONTENT REMAINS AVAILABLE
```

Exact eDiscovery workflows depend on licensing, roles, and
organizational legal processes.

------------------------------------------------------------------------

# 🔍 Search and Review

Authorized teams may need to locate relevant information across
supported Microsoft 365 content such as:

``` text
Email
Documents
SharePoint
OneDrive
Teams-Related Content
```

Memory:

``` text
eDISCOVERY
=
Find, preserve, collect,
and review information
for legal/investigative needs
```

------------------------------------------------------------------------

# 🧾 Microsoft Purview Audit

Microsoft Purview Audit helps authorized users search and investigate
recorded user and administrator activities.

Think:

``` text
WHO DID WHAT?
```

Example questions:

``` text
Who deleted the file?
When was it deleted?
Who changed the setting?
What activity was recorded?
```

Conceptually:

``` text
USER / ADMIN ACTIVITY
      ↓
AUDIT RECORD
      ↓
AUDIT SEARCH
      ↓
INVESTIGATION
```

------------------------------------------------------------------------

# ⚠️ Audit vs Microsoft Sentinel

``` text
PURVIEW AUDIT
=
Search and investigate
Microsoft activity records
```

``` text
MICROSOFT SENTINEL
=
SIEM + SOAR
for broader security operations
```

Both can support investigations, but they solve different problems.

------------------------------------------------------------------------

# 💬 Communication Compliance

Microsoft Purview Communication Compliance helps organizations detect
and review potential regulatory or business-conduct violations in
supported communications.

Examples can include:

``` text
Sensitive Information Sharing
Harassing or Threatening Language
Regulated Communications
Business Conduct Violations
```

It includes privacy-oriented capabilities such as pseudonymization,
role-based access, administrative scoping, and audit trails.

Memory:

``` text
COMMUNICATION COMPLIANCE
=
Are communications
potentially violating
policy or regulation?
```

------------------------------------------------------------------------

# 🧩 Which Tool?

``` text
Departing employee copies sensitive files
→ Insider Risk Management

Legal needs emails for a lawsuit
→ eDiscovery

Security asks who deleted a file
→ Audit

Potential policy violation in messages
→ Communication Compliance
```

------------------------------------------------------------------------

# 🔗 Working Together

A single investigation can use several capabilities.

``` text
DEPARTING EMPLOYEE
      ↓
Unusual Activity
      ↓
INSIDER RISK MANAGEMENT
      ↓
Alert / Case
      ↓
AUDIT
Review activity records
      ↓
eDISCOVERY
Preserve / find relevant content
if legal investigation requires it
```

The tools provide evidence and context. They do not replace appropriate
human, legal, HR, or management judgment.

------------------------------------------------------------------------

# 🗺️ Complete Purview Map

``` text
COMPLIANCE POSTURE
→ Compliance Manager

CLASSIFY / PROTECT
→ Information Protection

PREVENT DATA LOSS
→ DLP

KEEP / DELETE
→ Data Lifecycle Management

OFFICIAL RECORDS
→ Records Management

INTERNAL RISK
→ Insider Risk Management

LEGAL / INVESTIGATIVE CONTENT
→ eDiscovery

WHO DID WHAT?
→ Audit

COMMUNICATION POLICY RISK
→ Communication Compliance
```

------------------------------------------------------------------------

# 🎯 Exam Focus

``` text
INSIDER RISK MANAGEMENT
→ Potential internal risk

INDICATOR
→ Activity/signal used by policy

ALERT
→ Potential issue requiring review

CASE
→ Structured investigation

eDISCOVERY
→ Find/preserve/review electronic information

AUDIT
→ Search user/admin activity

COMMUNICATION COMPLIANCE
→ Potential communication policy violations
```

------------------------------------------------------------------------

# ❓ Knowledge Check

1.  Which capability identifies potential malicious or inadvertent
    internal risk?\
    **A. Insider Risk Management**

2.  What is an insider-risk indicator?\
    **A. An activity or signal used to identify potential risk**

3.  Does an alert automatically prove malicious intent?\
    **A. No**

4.  What is an Insider Risk case?\
    **A. A structured investigation**

5.  Which capability fits finding and preserving information for a legal
    case?\
    **A. eDiscovery**

6.  What can preservation/hold concepts help do?\
    **A. Preserve relevant content**

7.  Which capability helps answer "Who performed this activity?"\
    **A. Audit**

8.  Which capability addresses potential policy violations in
    communications?\
    **A. Communication Compliance**

9.  Which privacy feature can hide identifiable user information from
    certain roles?\
    **A. Pseudonymization**

10. Can Insider Risk, eDiscovery, and Audit complement one another?\
    **A. Yes**

------------------------------------------------------------------------

# 📌 Lesson Summary

``` text
RISKY INTERNAL ACTIVITY?
→ Insider Risk Management

LEGAL CONTENT?
→ eDiscovery

WHO DID WHAT?
→ Audit

RISKY COMMUNICATION?
→ Communication Compliance
```

------------------------------------------------------------------------

# 🧪 Lab

## 🟡 Lab 16 --- Investigate Risk & Compliance Events

➡️ **[Lab 16 --- Investigate Risk & Compliance
Events](../labs/%F0%9F%9F%A1%20Lab%2016%20%E2%80%94%20Investigate%20Risk%20%26%20Compliance%20Events.md)**

------------------------------------------------------------------------

# 🏗️ Next

## Project 03 --- Build a Compliance & Data Protection Strategy

Then:

## 🏆 Project 04 --- SC-900 Security Architecture Challenge

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Purview Insider Risk
    Management](https://learn.microsoft.com/en-us/purview/insider-risk-management)
-   [Microsoft Purview
    eDiscovery](https://learn.microsoft.com/en-us/purview/ediscovery)
-   [Microsoft Purview
    Audit](https://learn.microsoft.com/en-us/purview/audit-solutions-overview)
-   [Communication
    Compliance](https://learn.microsoft.com/en-us/purview/communication-compliance)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Lesson 15 --- Information Protection, DLP & Data Lifecycle**

🧪 **[Lab
16](../labs/%F0%9F%9F%A1%20Lab%2016%20%E2%80%94%20Investigate%20Risk%20%26%20Compliance%20Events.md)**

🏗️ **Project 03 --- Build a Compliance & Data Protection Strategy**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏠 **[Return to Main README](../README.md)**
