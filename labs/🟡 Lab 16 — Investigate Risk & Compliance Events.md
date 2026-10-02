# 🟡 Lab 16 --- Investigate Risk & Compliance Events

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 16 --- Insider Risk, eDiscovery & Audit\
**Lab Type:** 🟡 Scenario Lab\
**Configuration Changes:** None

------------------------------------------------------------------------

# 🎯 Lab Goal

Practice choosing between:

``` text
Insider Risk Management
eDiscovery
Audit
Communication Compliance
```

Use:

``` text
RISKY INTERNAL ACTIVITY?
→ Insider Risk Management

LEGAL / INVESTIGATIVE CONTENT?
→ eDiscovery

WHO DID WHAT?
→ Audit

RISKY COMMUNICATION?
→ Communication Compliance
```

------------------------------------------------------------------------

# 🏢 Scenario --- Contoso Manufacturing

Contoso uses Microsoft 365, Teams, Exchange Online, SharePoint,
OneDrive, and Microsoft Purview.

Several events require investigation. Your job is to choose the Purview
capability that fits each need.

------------------------------------------------------------------------

# ⚠️ Investigation Principle

Tools provide:

``` text
Signals
Activity Records
Content
Alerts
Context
```

They do not automatically prove:

``` text
Intent
Guilt
Policy Violation
Legal Liability
```

Proper human investigation remains necessary.

------------------------------------------------------------------------

# 🧩 Part 1 --- Choose the Tool

Employee downloads an unusual amount of sensitive data before leaving:

``` text
______________________________
```

Legal needs emails related to a lawsuit:

``` text
______________________________
```

IT needs to know who deleted a SharePoint file:

``` text
______________________________
```

Compliance needs to review messages that may violate policy:

``` text
______________________________
```

------------------------------------------------------------------------

# 🚦 Part 2 --- Indicators

Contoso wants to identify potential risk involving large downloads,
external sharing, sensitive-data movement, and security violations.

What is the general name for activities/signals selected for
insider-risk policies?

``` text
______________________________
```

``` text
ACTIVITY
      ↓
______________________________
      ↓
INSIDER RISK POLICY
```

------------------------------------------------------------------------

# 🚨 Part 3 --- Alert Does Not Mean Guilty

An employee triggers an insider-risk alert after downloading many files.

Should IT immediately conclude the employee is stealing data?

``` text
YES / NO
```

Why?

``` text
____________________________________
____________________________________
```

What should happen instead?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 📁 Part 4 --- Alert vs Case

``` text
ALERT
=
____________________________________
```

``` text
CASE
=
____________________________________
```

Which represents a structured investigation?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔐 Part 5 --- Privacy

Match:

Hide identifiable user details:

``` text
______________________________
```

Ensure only authorized investigators have access:

``` text
______________________________
```

Record administrative actions:

``` text
______________________________
```

Choose from:

``` text
Pseudonymization
Role-Based Access Control
Audit Logs
```

------------------------------------------------------------------------

# 👥 Part 6 --- Separation of Duties

Why separate:

``` text
Policy Configuration
Alert Review
Case Investigation
```

?

``` text
____________________________________
____________________________________
```

Which principle does this support?

``` text
______________________________
```

------------------------------------------------------------------------

# ⚖️ Part 7 --- Legal Request

Legal needs emails, Teams-related content, SharePoint documents, and
OneDrive files related to a matter.

Which capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 🧊 Part 8 --- Preserve Content

Relevant content must remain available while a case is active.

Which eDiscovery concept fits?

``` text
______________________________
```

Why?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🔍 Part 9 --- Find Evidence

Complete:

``` text
IDENTIFY
      ↓
PRESERVE
      ↓
______________________________
      ↓
REVIEW
```

------------------------------------------------------------------------

# 🧠 Part 10 --- eDiscovery or Audit?

Find lawsuit emails:

``` text
______________________________
```

Determine who changed a setting:

``` text
______________________________
```

Preserve case documents:

``` text
______________________________
```

Review recorded administrator activity:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧾 Part 11 --- Deleted File

Management asks:

``` text
Who deleted it?
When?
What activity was recorded?
```

Capability:

``` text
______________________________
```

Complete:

``` text
USER / ADMIN ACTIVITY
      ↓
______________________________
      ↓
SEARCH
      ↓
INVESTIGATION
```

------------------------------------------------------------------------

# 🧠 Part 12 --- Audit or Sentinel?

Search Microsoft 365 user/admin activity:

``` text
______________________________
```

Centralize security data for SIEM/SOAR:

``` text
______________________________
```

------------------------------------------------------------------------

# 💬 Part 13 --- Communication Compliance

A regulated department wants to review potential:

``` text
Regulatory Violations
Sensitive Information Sharing
Harassing or Threatening Language
Business Conduct Violations
```

Capability:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔐 Part 14 --- Communication Privacy

Why are pseudonymization, RBAC, administrative scoping, and audit trails
important?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🏢 Part 15 --- Departing Employee

An engineer gives notice, then:

``` text
Downloads hundreds of engineering files
Copies sensitive documents
Shares files externally
Deletes several files
Sends unusual messages
```

Do not assume malicious intent.

Identify risky activity patterns:

``` text
______________________________
```

Determine who deleted files:

``` text
______________________________
```

Preserve content if legal opens a case:

``` text
______________________________
```

Review communications under an applicable policy:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 16 --- Investigation Flow

Use:

``` text
Activity Signals
Insider Risk Policy
Alert
Case
Audit
eDiscovery
```

``` text
______________________________
      ↓
______________________________
      ↓
______________________________
      ↓
______________________________
      ↓
INVESTIGATION
      ↓
______________________________
      ↓
______________________________
```

------------------------------------------------------------------------

# 🧩 Part 17 --- Match the Question

"Is internal activity creating potential risk?"

``` text
______________________________
```

"Where is content related to this legal matter?"

``` text
______________________________
```

"Who performed this action?"

``` text
______________________________
```

"Do these communications potentially violate policy?"

``` text
______________________________
```

------------------------------------------------------------------------

# 🏆 Part 18 --- Multi-Tool Investigation

## Risk Detection

``` text
Tool: ______________________________
Purpose: ___________________________
```

## Activity History

``` text
Tool: ______________________________
Purpose: ___________________________
```

## Communication Review

``` text
Tool: ______________________________
Purpose: ___________________________
```

## Legal Content

``` text
Tool: ______________________________
Purpose: ___________________________
```

------------------------------------------------------------------------

# 🗺️ Part 19 --- Complete the Purview Map

``` text
COMPLIANCE POSTURE
→ ______________________________

CLASSIFY / PROTECT
→ ______________________________

PREVENT DATA LOSS
→ ______________________________

KEEP / DELETE
→ ______________________________

OFFICIAL RECORDS
→ ______________________________

INTERNAL RISK
→ ______________________________

LEGAL CONTENT
→ ______________________________

WHO DID WHAT?
→ ______________________________

COMMUNICATION RISK
→ ______________________________
```

------------------------------------------------------------------------

# 🏁 Part 20 --- Course Product Map

``` text
IDENTITY & ACCESS
→ ______________________________

THREAT PROTECTION
→ ______________________________

SECURITY OPERATIONS
→ ______________________________

DATA SECURITY / COMPLIANCE
→ ______________________________
```

Use:

``` text
Microsoft Entra
Microsoft Defender
Microsoft Sentinel
Microsoft Purview
```

------------------------------------------------------------------------

# 🏆 Final Challenge

Detect potential employee data exfiltration:

``` text
______________________________
```

Find emails for a lawsuit:

``` text
______________________________
```

Determine which administrator changed a setting:

``` text
______________________________
```

Review messages for potential policy violations:

``` text
______________________________
```

Prevent sensitive customer data from being emailed externally:

``` text
______________________________
```

Classify an HR document Highly Confidential:

``` text
______________________________
```

Keep signed contracts for the required period and govern them as
official records:

``` text
______________________________
```

------------------------------------------------------------------------

# ✅ Suggested Answers

``` text
Unusual departing-user downloads
→ Insider Risk Management

Lawsuit emails
→ eDiscovery

Who deleted a file
→ Audit

Potential message violations
→ Communication Compliance
```

``` text
Activity / signal
→ Indicator

Alert
→ Potential issue requiring review

Case
→ Structured investigation
```

An alert does not prove malicious intent. Review context and follow the
organization's investigation process.

Privacy:

``` text
Hide identity
→ Pseudonymization

Authorized access
→ Role-Based Access Control

Record admin actions
→ Audit Logs
```

Separation of duties supports:

``` text
Least Privilege
```

Legal request:

``` text
eDiscovery
```

Preservation:

``` text
Hold / Preservation
```

Evidence flow:

``` text
IDENTIFY
      ↓
PRESERVE
      ↓
SEARCH / COLLECT
      ↓
REVIEW
```

eDiscovery vs Audit:

``` text
Lawsuit emails
→ eDiscovery

Who changed a setting
→ Audit

Preserve documents
→ eDiscovery

Admin activity
→ Audit
```

Audit vs Sentinel:

``` text
Microsoft 365 activity investigation
→ Microsoft Purview Audit

SIEM / SOAR
→ Microsoft Sentinel
```

Departing employee:

``` text
Risk patterns
→ Insider Risk Management

Deleted files
→ Audit

Legal preservation
→ eDiscovery

Communication policy
→ Communication Compliance
```

Example flow:

``` text
Activity Signals
      ↓
Insider Risk Policy
      ↓
Alert
      ↓
Case
      ↓
Investigation
      ↓
Audit
      ↓
eDiscovery
```

Purview map:

``` text
Compliance posture
→ Compliance Manager

Classify / protect
→ Information Protection

Prevent data loss
→ DLP

Keep / delete
→ Data Lifecycle Management

Official records
→ Records Management

Internal risk
→ Insider Risk Management

Legal content
→ eDiscovery

Who did what
→ Audit

Communication risk
→ Communication Compliance
```

Course map:

``` text
Identity & Access
→ Microsoft Entra

Threat Protection
→ Microsoft Defender

Security Operations
→ Microsoft Sentinel

Data Security / Compliance
→ Microsoft Purview
```

Final challenge:

``` text
1. Insider Risk Management
2. eDiscovery
3. Audit
4. Communication Compliance
5. DLP
6. Sensitivity Label
7. Retention + Records Management
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

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

# ✅ Lab Completion Checklist

-   [ ] I understand Insider Risk Management.
-   [ ] I understand indicators, alerts, and cases.
-   [ ] I understand privacy considerations.
-   [ ] I understand eDiscovery and preservation.
-   [ ] I understand Microsoft Purview Audit.
-   [ ] I can distinguish Audit from Sentinel.
-   [ ] I understand Communication Compliance.
-   [ ] I can choose the correct investigation capability.

------------------------------------------------------------------------

# 🎉 Lessons Complete

You have completed:

``` text
📘 Lessons 01–16
```

Next:

## 🏗️ Project 03 --- Build a Compliance & Data Protection Strategy

Then:

## 🏆 Project 04 --- SC-900 Security Architecture Challenge

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **[Lesson 16 --- Insider Risk, eDiscovery &
Audit](../lessons/%F0%9F%93%98%20Lesson%2016%20%E2%80%94%20Insider%20Risk%2C%20eDiscovery%20%26%20Audit.md)**

🏗️ **Project 03 --- Build a Compliance & Data Protection Strategy**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏠 **[Return to Main README](../README.md)**
