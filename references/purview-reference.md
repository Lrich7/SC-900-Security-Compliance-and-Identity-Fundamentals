# 🏷️ Microsoft Purview Reference

A quick-reference guide to Microsoft Purview concepts covered by SC-900.

------------------------------------------------------------------------

# 🧠 Main Purpose

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

------------------------------------------------------------------------

# 📋 Compliance Manager

Helps organizations understand and improve their compliance posture.

Important concepts:

``` text
Assessments
Improvement Actions
Compliance Score
```

## Compliance Score

Helps measure progress toward recommended compliance actions.

Important:

``` text
HIGH COMPLIANCE SCORE
≠
LEGAL GUARANTEE OF COMPLIANCE
```

------------------------------------------------------------------------

# 📑 Service Trust Portal

Provides Microsoft trust, security, privacy, and compliance
documentation.

Think:

``` text
NEED MICROSOFT AUDIT/
COMPLIANCE DOCUMENTATION?
→ Service Trust Portal
```

------------------------------------------------------------------------

# 🏷️ Information Protection

Helps discover, classify, and protect sensitive information.

------------------------------------------------------------------------

# 🔎 Sensitive Information Types

Identify sensitive information using patterns and other detection logic.

Examples can include:

``` text
Credit Card Numbers
Government IDs
Financial Information
Personal Information
```

------------------------------------------------------------------------

# 🧠 Trainable Classifiers

Use machine-learning-based classification to recognize categories of
content based on examples.

Think:

``` text
PATTERN-BASED DATA
→ Sensitive Information Type

LEARNED CONTENT CATEGORY
→ Trainable Classifier
```

------------------------------------------------------------------------

# 🏷️ Sensitivity Labels

Classify and protect content.

Labels may support protections such as:

``` text
Encryption
Access Restrictions
Content Markings
Classification
```

Example classification:

``` text
Public
Internal
Confidential
Highly Confidential
```

------------------------------------------------------------------------

# 🚫 Data Loss Prevention --- DLP

Helps prevent sensitive information from being shared or used
inappropriately.

Think:

``` text
SENSITIVE DATA
+
RISKY ACTION
=
DLP RESPONSE
```

Possible actions can include:

``` text
Warn
Block
Restrict
Audit
```

------------------------------------------------------------------------

# 💡 Policy Tips

Provide warnings or guidance to users when a DLP rule is triggered.

``` text
POLICY TIP
→ Educate/warn user
```

------------------------------------------------------------------------

# 💻 Endpoint DLP

Extends DLP controls to supported endpoint activities.

Example concerns:

``` text
USB
Clipboard
Printing
Browser Upload
Local File Actions
```

------------------------------------------------------------------------

# 🆚 Sensitivity Label vs DLP

``` text
SENSITIVITY LABEL
→ Classify/protect the content

DLP
→ Control what users can do with sensitive content
```

The same file can use both.

------------------------------------------------------------------------

# 🗓️ Data Lifecycle Management

Controls how long data should be retained and when it should be deleted.

------------------------------------------------------------------------

# 📌 Retention Policy

Generally applies retention broadly to locations or workloads.

Think:

``` text
BROAD RETENTION
→ Retention Policy
```

------------------------------------------------------------------------

# 🏷️ Retention Label

Applies retention at the item/content level.

Think:

``` text
SPECIFIC CONTENT
→ Retention Label
```

------------------------------------------------------------------------

# 🗃️ Records Management

Provides additional controls for content that must be managed as an
official record.

``` text
OFFICIAL RECORD?
→ Records Management
```

------------------------------------------------------------------------

# ⚠️ Insider Risk Management

Helps identify and investigate potential internal risk.

Insider risk can be:

``` text
Malicious
Accidental
Negligent
```

Important:

``` text
INSIDER RISK ALERT
≠
PROOF OF MALICIOUS INTENT
```

Concepts:

``` text
Indicators
Policies
Alerts
Cases
Investigations
```

------------------------------------------------------------------------

# ⚖️ eDiscovery

Used for legal and investigative content.

Simplified flow:

``` text
IDENTIFY
    ↓
PRESERVE
    ↓
SEARCH / COLLECT
    ↓
REVIEW
    ↓
EXPORT / USE
```

Memory:

``` text
LEGAL CONTENT?
→ eDiscovery
```

------------------------------------------------------------------------

# 🧾 Audit

Provides activity history.

Memory:

``` text
WHO DID WHAT?
→ Audit
```

Audit can help investigate user and administrator activity.

------------------------------------------------------------------------

# 💬 Communication Compliance

Helps identify communication that may violate organizational or
regulatory policies.

Memory:

``` text
RISKY COMMUNICATION?
→ Communication Compliance
```

------------------------------------------------------------------------

# 🧠 Purview Decision Map

``` text
TRUST DOCUMENTS
→ Service Trust Portal

COMPLIANCE PROGRESS
→ Compliance Manager

CLASSIFY / PROTECT
→ Information Protection

PREVENT DATA LOSS
→ DLP

KEEP / DELETE
→ Data Lifecycle Management

OFFICIAL RECORD
→ Records Management

INTERNAL RISK
→ Insider Risk Management

LEGAL CONTENT
→ eDiscovery

WHO DID WHAT?
→ Audit

COMMUNICATION RISK
→ Communication Compliance
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
