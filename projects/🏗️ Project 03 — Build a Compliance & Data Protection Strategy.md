# 🏗️ Project 03 --- Build a Compliance & Data Protection Strategy

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Project Type:** Compliance & Data Protection Strategy Challenge\
**Covers:** Lessons 14--16\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🎯 Project Goal

Design a Microsoft Purview strategy for a fictional organization.

You will decide how the organization should:

``` text
ASSESS COMPLIANCE
      ↓
DISCOVER / CLASSIFY DATA
      ↓
PROTECT SENSITIVE DATA
      ↓
PREVENT DATA LOSS
      ↓
RETAIN / DELETE INFORMATION
      ↓
MANAGE RECORDS
      ↓
IDENTIFY INTERNAL RISK
      ↓
SUPPORT INVESTIGATIONS
```

This project combines:

``` text
Microsoft Purview
Compliance Manager
Service Trust Portal
Information Protection
Sensitivity Labels
Sensitive Information Types
DLP
Endpoint DLP
Data Lifecycle Management
Records Management
Insider Risk Management
eDiscovery
Audit
Communication Compliance
```

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

Microsoft services include:

``` text
Microsoft 365
Exchange Online
Teams
SharePoint
OneDrive
Microsoft Entra
Microsoft Purview
Windows Laptops
```

Contoso stores:

``` text
Employee Records
Payroll Information
Customer Information
Contracts
Financial Reports
Engineering Documents
Legal Documents
Public Marketing Material
```

------------------------------------------------------------------------

# ⚠️ Current Problems

Contoso has grown quickly and does not have a consistent compliance or
data-protection strategy.

Problems include:

``` text
Sensitive data is not consistently classified.

Users can accidentally share sensitive files externally.

HR documents contain SSNs and banking information.

Engineering documents may be copied to removable storage.

Contracts do not have consistent retention rules.

Some official records are kept indefinitely.

Other important information may be deleted too early.

Management has no simple view of compliance progress.

Legal requests are handled manually.

IT has difficulty determining who performed certain actions.

Departing employees may download large amounts of company data.

Communication policy violations are handled inconsistently.
```

Your job is to design a better strategy.

------------------------------------------------------------------------

# 🧭 Phase 1 --- Identify Compliance Responsibilities

Explain why using Microsoft 365 does not automatically make Contoso
compliant.

``` text
____________________________________
____________________________________
____________________________________
```

Complete:

``` text
MICROSOFT RESPONSIBILITY
+
______________________________
=
SHARED COMPLIANCE EFFORT
```

------------------------------------------------------------------------

# 🏛️ Phase 2 --- Trust Documentation

An auditor asks Contoso for information about Microsoft's:

``` text
Security Practices
Privacy Practices
Compliance Programs
Audit Reports
```

Which resource should Contoso use?

``` text
______________________________
```

Explain why:

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 📊 Phase 3 --- Compliance Posture

Management wants to:

``` text
Measure compliance progress
Review assessments
Track recommended actions
Prioritize improvements
```

Which Purview capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 📈 Phase 4 --- Compliance Score

Explain what Compliance Score represents.

``` text
____________________________________
____________________________________
```

Does a high score automatically guarantee legal compliance?

``` text
YES / NO
```

Why?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 📝 Phase 5 --- Improvement Actions

What are improvement actions?

``` text
____________________________________
____________________________________
```

Give three example categories of work that could improve compliance
posture.

``` text
1. ______________________________

2. ______________________________

3. ______________________________
```

------------------------------------------------------------------------

# 🔎 Phase 6 --- Identify Sensitive Data

Contoso needs to recognize:

``` text
Social Security Numbers
Bank Account Numbers
Credit Card Numbers
Health Information
```

Which Purview concept fits?

``` text
______________________________
```

What does it do?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🤖 Phase 7 --- Pattern vs Learned Content

Choose:

``` text
Sensitive Information Type
Trainable Classifier
```

Recognize a credit-card-number pattern:

``` text
______________________________
```

Recognize a content category from learned characteristics:

``` text
______________________________
```

------------------------------------------------------------------------

# 🏷️ Phase 8 --- Build a Classification Scheme

Design four labels.

  Label                 Example Data
  --------------------- --------------------------------------
  Public                \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Internal              \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Confidential          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Highly Confidential   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Which capability provides these classifications?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔐 Phase 9 --- Protect Highly Confidential Information

Contoso wants highly confidential documents to support protections such
as:

``` text
Encryption
Restricted Access
Content Marking
```

Which capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 📋 Phase 10 --- Publish Labels

Complete:

``` text
CREATE LABEL
      ↓
______________________________
      ↓
USERS / GROUPS
```

Why is publishing important?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🚫 Phase 11 --- Prevent Sensitive External Sharing

A payroll employee attempts to send employee bank information to a
personal email account.

Which capability fits?

``` text
______________________________
```

Possible configured outcomes can include:

``` text
Detect
Warn
Restrict / Block
```

------------------------------------------------------------------------

# 💡 Phase 12 --- Educate the User

Contoso wants users to receive a warning when they attempt risky
handling of sensitive information.

Which DLP concept fits?

``` text
______________________________
```

Example message:

``` text
This content contains sensitive
employee information.
Verify the recipient before sharing.
```

------------------------------------------------------------------------

# 💻 Phase 13 --- Protect Endpoint Data

An engineer attempts to copy sensitive engineering files to removable
USB storage.

Which capability is associated with supported endpoint data controls?

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Phase 14 --- Sensitivity Label vs DLP

Complete:

``` text
WHAT IS THE DATA?
HOW SHOULD IT BE PROTECTED?
→ ______________________________
```

``` text
WHAT IS THE USER
TRYING TO DO WITH IT?
→ ______________________________
```

------------------------------------------------------------------------

# 🗃️ Phase 15 --- Data Lifecycle

Contoso needs consistent rules for:

``` text
CREATE
      ↓
USE
      ↓
RETAIN
      ↓
DELETE
```

Which Purview area fits?

``` text
______________________________
```

------------------------------------------------------------------------

# ⏳ Phase 16 --- Retention Strategy

Contoso wants general retention across a supported location.

Choose:

``` text
Retention Policy
Retention Label
```

Answer:

``` text
______________________________
```

Contoso wants signed contracts to receive a specific seven-year
retention period.

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 📁 Phase 17 --- Records Management

Signed legal contracts must be treated as official evidence of business
activity.

Which capability fits?

``` text
______________________________
```

Explain why an official record may require stronger governance.

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# ⚠️ Phase 18 --- Over-Retention and Under-Retention

List two risks of keeping everything forever.

``` text
1. ______________________________

2. ______________________________
```

List two risks of deleting important information too early.

``` text
1. ______________________________

2. ______________________________
```

------------------------------------------------------------------------

# 🚦 Phase 19 --- Insider Risk

A departing engineer downloads hundreds of confidential files.

Which capability helps identify potential risky internal activity?

``` text
______________________________
```

Does an alert prove malicious intent?

``` text
YES / NO
```

Explain:

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🔐 Phase 20 --- Insider Risk Privacy

Match:

``` text
Hide identifiable information
→ ______________________________

Restrict investigator access
→ ______________________________

Record administrative activity
→ ______________________________
```

Choose from:

``` text
Pseudonymization
Role-Based Access Control
Audit Logs
```

------------------------------------------------------------------------

# 🚨 Phase 21 --- Alert vs Case

Complete:

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

# ⚖️ Phase 22 --- Legal Investigation

Contoso receives a legal request involving:

``` text
Email
Teams-Related Content
SharePoint
OneDrive
```

Which capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 🧊 Phase 23 --- Preserve Information

Legal says relevant information must remain available during the
investigation.

Which concept fits?

``` text
______________________________
```

Why?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🧾 Phase 24 --- Audit Activity

A critical SharePoint document disappears.

Management asks:

``` text
Who deleted it?
When?
What activity was recorded?
```

Which capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 💬 Phase 25 --- Communication Compliance

A regulated department needs to review potential:

``` text
Sensitive Information Sharing
Regulatory Violations
Harassing or Threatening Language
Business Conduct Violations
```

Which capability fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 🗺️ Phase 26 --- Build the Purview Architecture

Complete:

``` text
TRUST DOCUMENTS
      ↓
______________________________

COMPLIANCE POSTURE
      ↓
______________________________

DISCOVER SENSITIVE DATA
      ↓
______________________________

CLASSIFY / PROTECT
      ↓
______________________________

PREVENT LOSS
      ↓
______________________________

KEEP / DELETE
      ↓
______________________________

OFFICIAL RECORDS
      ↓
______________________________

INTERNAL RISK
      ↓
______________________________

LEGAL CONTENT
      ↓
______________________________

WHO DID WHAT?
      ↓
______________________________

COMMUNICATION RISK
      ↓
______________________________
```

------------------------------------------------------------------------

# 🏢 Phase 27 --- Department Strategy

## Human Resources

Data:

``` text
SSNs
Banking Information
Medical Information
Employee Records
```

Classification:

``` text
______________________________
```

Protection:

``` text
______________________________
```

Data-loss control:

``` text
______________________________
```

Retention consideration:

``` text
______________________________
```

------------------------------------------------------------------------

## Finance

Data:

``` text
Financial Reports
Banking Information
Customer Payment Information
```

Classification:

``` text
______________________________
```

Protection:

``` text
______________________________
```

Data-loss control:

``` text
______________________________
```

------------------------------------------------------------------------

## Legal

Data:

``` text
Contracts
Legal Correspondence
Case Documents
```

Retention:

``` text
______________________________
```

Official records:

``` text
______________________________
```

Investigation:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧩 Phase 28 --- Product Selection

  Requirement                          Purview Capability
  ------------------------------------ --------------------------------------
  Microsoft audit reports              \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Measure compliance progress          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Detect SSNs                          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Mark a document Confidential         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Stop sensitive external sharing      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Warn users about risky sharing       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Control supported endpoint copying   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Keep information for a period        \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Govern official records              \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identify risky internal activity     \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Find content for a lawsuit           \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Determine who performed an action    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Review risky communications          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 🏆 Phase 29 --- Final Contoso Data Strategy

Design a complete strategy for this document:

``` text
SIGNED CUSTOMER CONTRACT

Contains:
Customer Information
Pricing
Banking Details
Confidential Terms
```

Requirement 1 --- Recognize sensitive financial information:

``` text
______________________________
```

Requirement 2 --- Classify the document:

``` text
______________________________
```

Requirement 3 --- Protect the document:

``` text
______________________________
```

Requirement 4 --- Prevent improper external sharing:

``` text
______________________________
```

Requirement 5 --- Keep it seven years:

``` text
______________________________
```

Requirement 6 --- Treat it as an official record:

``` text
______________________________
```

Requirement 7 --- Find it later for a legal case:

``` text
______________________________
```

Requirement 8 --- Determine who accessed or changed supported audited
activity:

``` text
______________________________
```

------------------------------------------------------------------------

# 📝 Phase 30 --- Executive Summary

Write a short recommendation for Contoso leadership.

Include:

``` text
Compliance posture
Data classification
Data protection
DLP
Retention
Records
Insider risk
Investigation
```

``` text
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
____________________________________
```

------------------------------------------------------------------------

# ✅ Suggested Solution

## Compliance

``` text
Trust documentation
→ Service Trust Portal

Compliance posture
→ Compliance Manager

Progress measurement
→ Compliance Score

Recommended work
→ Improvement Actions
```

## Classification and Protection

``` text
Recognize patterns
→ Sensitive Information Types

Recognize learned categories
→ Trainable Classifiers

Classify / protect
→ Sensitivity Labels

Publish labels
→ Label Policies
```

## Data Loss

``` text
Sensitive sharing
→ DLP

User warning
→ Policy Tip

Supported endpoint activity
→ Endpoint DLP
```

## Lifecycle

``` text
Broad retention
→ Retention Policy

Item/content retention
→ Retention Label

Official records
→ Records Management
```

## Investigation

``` text
Internal risk
→ Insider Risk Management

Potential issue
→ Alert

Structured investigation
→ Case

Legal content
→ eDiscovery

Preservation
→ Hold / preservation

Who did what
→ Audit

Communication risk
→ Communication Compliance
```

## Purview Architecture

``` text
SERVICE TRUST PORTAL
      ↓
Microsoft trust documentation

COMPLIANCE MANAGER
      ↓
Compliance posture

INFORMATION PROTECTION
      ↓
Discover / classify / protect

DLP
      ↓
Prevent inappropriate use/sharing

DATA LIFECYCLE
      ↓
Retention / deletion

RECORDS MANAGEMENT
      ↓
Official records

INSIDER RISK
      ↓
Potential internal risk

eDISCOVERY
      ↓
Legal / investigative content

AUDIT
      ↓
Activity history

COMMUNICATION COMPLIANCE
      ↓
Communication policy risk
```

## Final Contract

``` text
1. Sensitive Information Type
2. Confidential / appropriate Sensitivity Label
3. Sensitivity Label protections
4. DLP
5. Retention Label / appropriate retention configuration
6. Records Management
7. eDiscovery
8. Audit
```

------------------------------------------------------------------------

# 🎓 Project Outcomes

After completing Project 03, you should be able to explain:

``` text
HOW PURVIEW ASSESSES COMPLIANCE

HOW DATA IS CLASSIFIED

HOW SENSITIVE DATA IS PROTECTED

HOW DLP REDUCES DATA LOSS

HOW RETENTION GOVERNS DATA LIFECYCLE

HOW RECORDS ARE MANAGED

HOW INSIDER RISK IS INVESTIGATED

HOW eDISCOVERY SUPPORTS LEGAL WORK

HOW AUDIT SUPPORTS INVESTIGATIONS
```

------------------------------------------------------------------------

# ✅ Completion Checklist

-   [ ] I can explain Compliance Manager.
-   [ ] I understand Service Trust Portal.
-   [ ] I can distinguish sensitive information types and classifiers.
-   [ ] I understand sensitivity labels.
-   [ ] I understand DLP and Endpoint DLP.
-   [ ] I understand retention policies and labels.
-   [ ] I understand Records Management.
-   [ ] I understand Insider Risk Management.
-   [ ] I understand eDiscovery.
-   [ ] I understand Audit.
-   [ ] I understand Communication Compliance.
-   [ ] I can design a basic Purview strategy.

------------------------------------------------------------------------

# ➡️ Next

## 🏆 Project 04 --- SC-900 Security Architecture Challenge

This final capstone combines Lessons 01--16.

------------------------------------------------------------------------

# 📚 Course Navigation

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](README.md)**

🏠 **[Return to Main README](../README.md)**
