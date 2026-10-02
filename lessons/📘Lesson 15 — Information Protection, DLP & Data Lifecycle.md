# 📘 Lesson 15 --- Information Protection, DLP & Data Lifecycle

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 15\
**Section:** Microsoft Compliance Solutions\
**Lab:** 🟡 Scenario Lab --- Protect and Govern Contoso Data

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Explain data classification in Microsoft Purview
-   Describe sensitive information types and trainable classifiers
-   Explain sensitivity labels and label policies
-   Describe Data Loss Prevention (DLP), policy tips, and Endpoint DLP
-   Explain Data Lifecycle Management
-   Distinguish retention policies from retention labels
-   Explain Records Management
-   Choose the appropriate Purview capability for common data-protection
    scenarios

------------------------------------------------------------------------

# 🧠 The Big Question

Organizations create enormous amounts of data:

``` text
Emails
Documents
Teams Messages
SharePoint Files
OneDrive Files
Customer Records
Employee Records
Contracts
Financial Reports
```

The challenge is:

``` text
WHAT DATA DO WE HAVE?
IS IT SENSITIVE?
CAN IT BE SHARED?
HOW SHOULD IT BE PROTECTED?
HOW LONG SHOULD WE KEEP IT?
IS IT AN OFFICIAL RECORD?
```

------------------------------------------------------------------------

# 🗺️ Data Protection Flow

``` text
DISCOVER
   ↓
CLASSIFY
   ↓
PROTECT
   ↓
PREVENT LOSS
   ↓
RETAIN / DELETE
   ↓
MANAGE RECORDS
```

------------------------------------------------------------------------

# 🏷️ Data Classification

Data classification helps identify and categorize information.

Example classifications:

``` text
Public
Internal
Confidential
Highly Confidential
```

Classification can influence access, sharing, encryption, and retention
decisions.

------------------------------------------------------------------------

# 🔎 Sensitive Information Types

Microsoft Purview **Sensitive Information Types** help identify
recognizable categories of sensitive data.

Examples include:

``` text
Credit Card Numbers
Social Security Numbers
Bank Account Information
Passport Numbers
Health Information
Government Identifiers
```

They can use patterns, keywords, checksums, supporting evidence, and
confidence levels.

Memory:

``` text
SENSITIVE INFORMATION TYPE
=
Recognize a category
of sensitive data
```

------------------------------------------------------------------------

# 🤖 Trainable Classifiers

Some content cannot be recognized by a simple number pattern.

**Trainable classifiers** use machine-learning-based classification to
identify categories of content from learned characteristics.

``` text
SENSITIVE INFORMATION TYPE
=
Pattern-based recognition

TRAINABLE CLASSIFIER
=
Learned content recognition
```

------------------------------------------------------------------------

# 🏷️ Sensitivity Labels

Sensitivity labels help classify and protect organizational information.

Examples:

``` text
Public
General
Confidential
Highly Confidential
```

Depending on configuration and workload, labels can support protections
such as:

``` text
Encryption
Access Restrictions
Headers
Footers
Watermarks
Sharing Controls
```

Memory:

``` text
SENSITIVITY LABEL
=
What is this data,
and how should it
be protected?
```

------------------------------------------------------------------------

# 👤 Manual and Automatic Labeling

Depending on licensing and configuration, labels can be:

``` text
Manually Applied
Recommended
Automatically Applied
Applied by Default
```

Classification can therefore be user-driven or automated.

------------------------------------------------------------------------

# 📋 Label Policies

Creating a label does not necessarily make it available to users.

Label policies publish/configure labels for users and groups.

``` text
CREATE LABEL
      ↓
PUBLISH THROUGH POLICY
      ↓
USERS / GROUPS
```

------------------------------------------------------------------------

# 🚫 Data Loss Prevention --- DLP

DLP helps identify, monitor, and protect sensitive information from
inappropriate use or sharing.

Example:

``` text
SENSITIVE DATA
      ↓
USER ATTEMPTS TO SHARE
      ↓
DLP POLICY
      ↓
ALLOW / WARN / RESTRICT
depending on policy
```

Supported locations can include Microsoft 365 workloads such as
Exchange, SharePoint, OneDrive, Teams, and supported endpoints.

------------------------------------------------------------------------

# 💡 Policy Tips

A DLP **policy tip** can warn or educate a user while they are handling
sensitive information.

Example:

``` text
⚠ This document contains
sensitive financial information.
```

This can help users make better decisions at the moment of action.

------------------------------------------------------------------------

# 💻 Endpoint DLP

Endpoint DLP extends data-protection controls to supported endpoint
activities.

Examples can include:

``` text
Copy to USB
Print
Copy to Clipboard
Upload to Cloud Services
Transfer Through Applications
```

Exact controls depend on configuration, licensing, and supported
platforms.

------------------------------------------------------------------------

# 🧠 Sensitivity Label vs DLP

``` text
SENSITIVITY LABEL
=
What is this data?
How should it be protected?
```

``` text
DLP
=
What is the user
trying to do with it?
```

Example:

``` text
Document labeled Highly Confidential
=
Sensitivity Label

User tries to send it externally
and policy evaluates the action
=
DLP
```

------------------------------------------------------------------------

# 🗃️ Data Lifecycle Management

Organizations need deliberate rules for how long information exists.

``` text
CREATE
   ↓
USE
   ↓
STORE
   ↓
RETAIN
   ↓
DELETE
```

Keeping everything forever can increase privacy, legal, storage, and
management risk. Deleting information too early can violate legal,
regulatory, or business requirements.

------------------------------------------------------------------------

# ⏳ Retention Policies

Retention policies can apply retention settings broadly across supported
locations.

Think:

``` text
RETENTION POLICY
=
Broad retention
across locations
```

------------------------------------------------------------------------

# 🏷️ Retention Labels

Retention labels can apply retention settings to individual items or
categories of content.

Example:

``` text
Signed Contract
      ↓
Retention Label
      ↓
Keep 7 Years
```

Think:

``` text
RETENTION LABEL
=
Item / content-based
retention
```

------------------------------------------------------------------------

# 📁 Records Management

Some information must be treated as an official business record.

Microsoft Purview Records Management helps govern records and their
retention requirements.

Examples:

``` text
Signed Contracts
Official Financial Records
Regulatory Documents
Corporate Policies
Legal Records
```

Memory:

``` text
RECORD
=
Official evidence
of business activity
```

------------------------------------------------------------------------

# 🧠 Lifecycle vs Records

``` text
DATA LIFECYCLE MANAGEMENT
=
How long should
information exist?
```

``` text
RECORDS MANAGEMENT
=
Which information must
be governed as an
official record?
```

------------------------------------------------------------------------

# 🏢 Contoso Examples

``` text
Detect SSNs in HR files
→ Sensitive Information Type

Mark HR files Highly Confidential
→ Sensitivity Label

Prevent financial data from
being emailed externally
→ DLP

Keep contracts seven years
→ Retention

Treat signed contracts as
official records
→ Records Management
```

------------------------------------------------------------------------

# 🗺️ Decision Map

``` text
IDENTIFY SENSITIVE DATA?
→ Sensitive Information Type

CLASSIFY / PROTECT?
→ Sensitivity Label

STOP INAPPROPRIATE SHARING?
→ DLP

KEEP / DELETE FOR A PERIOD?
→ Retention

MANAGE OFFICIAL RECORDS?
→ Records Management
```

------------------------------------------------------------------------

# 🔗 One Document, Multiple Controls

``` text
EMPLOYEE CONTRACT
      ↓
Sensitive Information Detected
      ↓
Sensitivity Label
      ↓
DLP Prevents Improper Sharing
      ↓
Retention Label
      ↓
Record Declaration
if required
```

Each control solves a different problem.

------------------------------------------------------------------------

# 🎯 Exam Focus

``` text
SENSITIVE INFORMATION TYPE
→ Identify sensitive patterns

TRAINABLE CLASSIFIER
→ Recognize learned content categories

SENSITIVITY LABEL
→ Classify and protect

DLP
→ Prevent inappropriate use/sharing

POLICY TIP
→ Warn or educate users

ENDPOINT DLP
→ Protect endpoint data actions

RETENTION POLICY
→ Broad location-based retention

RETENTION LABEL
→ Item/content-based retention

RECORDS MANAGEMENT
→ Govern official records
```

------------------------------------------------------------------------

# ❓ Knowledge Check

1.  What identifies categories such as Social Security numbers?\
    **A. Sensitive Information Type**

2.  What primarily classifies and protects information?\
    **A. Sensitivity Label**

3.  What helps prevent inappropriate sharing of sensitive data?\
    **A. DLP**

4.  What can warn users while they handle sensitive information?\
    **A. Policy Tip**

5.  What can control supported endpoint data activities?\
    **A. Endpoint DLP**

6.  What is retention concerned with?\
    **A. How long information is kept or when it is deleted**

7.  What is the broad difference between retention policies and labels?\
    **A. Policies apply broadly; labels can apply to specific
    items/content**

8.  What governs official organizational records?\
    **A. Records Management**

9.  What best classifies a document as Highly Confidential?\
    **A. Sensitivity Label**

10. What best fits stopping sensitive customer data from being emailed
    externally?\
    **A. DLP**

------------------------------------------------------------------------

# 📌 Lesson Summary

``` text
FIND IT
→ Sensitive Information Types

LABEL IT
→ Sensitivity Labels

STOP IT LEAVING
→ DLP

KEEP IT
→ Retention

MAKE IT OFFICIAL
→ Records Management
```

------------------------------------------------------------------------

# 🧪 Lab

## 🟡 Lab 15 --- Protect and Govern Contoso Data

➡️ **[Lab 15 --- Protect and Govern Contoso
Data](../labs/%F0%9F%9F%A1%20Lab%2015%20%E2%80%94%20Protect%20and%20Govern%20Contoso%20Data.md)**

------------------------------------------------------------------------

# ➡️ Next Lesson

## 📘 Lesson 16 --- Insider Risk, eDiscovery & Audit

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Purview Information
    Protection](https://learn.microsoft.com/en-us/purview/information-protection)
-   [Sensitivity
    Labels](https://learn.microsoft.com/en-us/purview/sensitivity-labels)
-   [Data Loss
    Prevention](https://learn.microsoft.com/en-us/purview/dlp-learn-about-dlp)
-   [Data Lifecycle
    Management](https://learn.microsoft.com/en-us/purview/data-lifecycle-management)
-   [Records
    Management](https://learn.microsoft.com/en-us/purview/records-management)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Lesson 14 --- Microsoft Purview & Compliance**

🧪 **[Lab
15](../labs/%F0%9F%9F%A1%20Lab%2015%20%E2%80%94%20Protect%20and%20Govern%20Contoso%20Data.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
