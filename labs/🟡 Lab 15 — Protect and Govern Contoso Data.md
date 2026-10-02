# 🟡 Lab 15 --- Protect and Govern Contoso Data

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 15 --- Information Protection, DLP & Data
Lifecycle\
**Lab Type:** 🟡 Scenario Lab\
**Configuration Changes:** None

------------------------------------------------------------------------

# 🎯 Lab Goal

Practice choosing between:

``` text
Sensitive Information Types
Trainable Classifiers
Sensitivity Labels
DLP
Policy Tips
Endpoint DLP
Retention Policies
Retention Labels
Records Management
```

Use this decision process:

``` text
WHAT IS THE DATA?
      ↓
HOW SENSITIVE IS IT?
      ↓
WHAT IS THE USER DOING?
      ↓
HOW LONG SHOULD IT EXIST?
      ↓
IS IT AN OFFICIAL RECORD?
```

------------------------------------------------------------------------

# 🏢 Scenario --- Contoso Manufacturing

Contoso has:

``` text
150 Employees
Microsoft 365
Exchange Online
Teams
SharePoint
OneDrive
Windows Laptops
```

It stores:

``` text
Employee Records
Customer Information
Contracts
Financial Reports
Engineering Documents
Public Marketing Material
```

------------------------------------------------------------------------

# 🗺️ Quick Reference

``` text
IDENTIFY SENSITIVE DATA
→ Sensitive Information Type

CLASSIFY / PROTECT
→ Sensitivity Label

STOP INAPPROPRIATE SHARING
→ DLP

WARN USER
→ Policy Tip

CONTROL ENDPOINT DATA ACTIONS
→ Endpoint DLP

KEEP / DELETE BROADLY
→ Retention Policy

RETENTION BY ITEM / CONTENT
→ Retention Label

OFFICIAL RECORD
→ Records Management
```

------------------------------------------------------------------------

# 🧩 Part 1 --- Classify the Data

Assign:

``` text
Public
Internal
Confidential
Highly Confidential
```

## Public Website Brochure

``` text
______________________________
```

## Internal IT Procedure

``` text
______________________________
```

## Customer Pricing Agreement

``` text
______________________________
```

## Employee File Containing SSN and Medical Information

``` text
______________________________
```

Why should the employee file receive stronger protection?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🔎 Part 2 --- Identify Sensitive Information

An HR spreadsheet contains:

``` text
Employee Name
Address
Social Security Number
Bank Account Number
```

Which concept can help recognize SSNs and financial identifiers?

``` text
______________________________
```

------------------------------------------------------------------------

# 🤖 Part 3 --- Pattern or Classifier?

Choose:

``` text
Sensitive Information Type
Trainable Classifier
```

Recognizable credit-card-number pattern:

``` text
______________________________
```

Content category identified from learned characteristics:

``` text
______________________________
```

------------------------------------------------------------------------

# 🏷️ Part 4 --- Design Labels

  Label                 Example Use
  --------------------- --------------------------------------
  Public                \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Internal              \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Confidential          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Highly Confidential   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 🔐 Part 5 --- Protect Highly Confidential Data

Contoso wants:

``` text
Visible Classification
Encryption
Restricted Access
```

Which capability fits?

``` text
______________________________
```

Why?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 📝 Part 6 --- Content Marking

Contoso wants this at the top of confidential documents:

``` text
CONFIDENTIAL — INTERNAL USE ONLY
```

Which capability fits?

``` text
______________________________
```

Which type of marking is this?

``` text
______________________________
```

------------------------------------------------------------------------

# 📋 Part 7 --- Publish Labels

The labels exist, but users need access to them.

Complete:

``` text
CREATE LABEL
      ↓
______________________________
      ↓
USERS / GROUPS
```

------------------------------------------------------------------------

# 🚫 Part 8 --- Sensitive Email

Payroll attempts to email employee bank information to a personal
address.

Which capability fits?

``` text
______________________________
```

Possible configured responses include:

``` text
Detect
Warn
Restrict / Block
```

------------------------------------------------------------------------

# 💡 Part 9 --- User Education

Instead of immediately blocking an action, Contoso wants to display:

``` text
This file contains sensitive
customer information.
Please verify the recipient.
```

Which concept fits?

``` text
______________________________
```

------------------------------------------------------------------------

# 💻 Part 10 --- USB Scenario

A user attempts to copy sensitive engineering documents to removable USB
storage.

Which capability is most closely associated with supported endpoint data
controls?

``` text
______________________________
```

------------------------------------------------------------------------

# 📋 Part 11 --- Label or DLP?

Choose:

``` text
Sensitivity Label
DLP
```

Mark a file Highly Confidential:

``` text
______________________________
```

Encrypt a classified document:

``` text
______________________________
```

Stop sensitive external sharing:

``` text
______________________________
```

Warn a user about sensitive sharing:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Part 12 --- One File, Two Controls

A file is labeled:

``` text
Highly Confidential
```

Then the user attempts to email it externally.

Classification/protection:

``` text
______________________________
```

Evaluate the sharing action:

``` text
______________________________
```

------------------------------------------------------------------------

# 🗃️ Part 13 --- Contract Retention

Legal requires contracts to be kept for seven years.

Which general concept fits?

``` text
______________________________
```

What question does retention answer?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🏢 Part 14 --- Broad Retention

Contoso wants broad retention across a supported location.

Choose:

``` text
Retention Policy
Retention Label
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🏷️ Part 15 --- Item-Based Retention

Documents identified as:

``` text
Signed Contract
```

should receive a seven-year retention period.

Choose:

``` text
Retention Policy
Retention Label
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 📁 Part 16 --- Official Records

Signed contracts must become official evidence of business activity.

Which capability fits?

``` text
______________________________
```

Why might records need stronger governance?

``` text
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🧠 Part 17 --- Lifecycle or Records?

Choose:

``` text
Data Lifecycle Management
Records Management
```

Routine Teams retention:

``` text
______________________________
```

Signed legal contract as an official record:

``` text
______________________________
```

Delete obsolete content after an approved period:

``` text
______________________________
```

Govern official corporate records:

``` text
______________________________
```

------------------------------------------------------------------------

# 🏢 Part 18 --- HR Strategy

HR stores employee, payroll, tax, and medical records.

Identify sensitive patterns:

``` text
______________________________
```

Classify highly sensitive files:

``` text
______________________________
```

Prevent improper external sharing:

``` text
______________________________
```

Manage how long information is kept:

``` text
______________________________
```

------------------------------------------------------------------------

# 💰 Part 19 --- Finance Scenario

Before public release, a quarterly financial report is highly sensitive.

Classification:

``` text
______________________________
```

Classification/protection capability:

``` text
______________________________
```

Prevent improper sharing:

``` text
______________________________
```

Retention consideration:

``` text
____________________________________
```

------------------------------------------------------------------------

# 📢 Part 20 --- Public Data

A product brochure is intended for public distribution.

Should it be labeled Highly Confidential?

``` text
YES / NO
```

Better classification:

``` text
______________________________
```

------------------------------------------------------------------------

# ⚠️ Part 21 --- Overclassification

What could happen if every document is marked Highly Confidential?

``` text
____________________________________
____________________________________
____________________________________
```

------------------------------------------------------------------------

# ⚠️ Part 22 --- Over-Retention

What problems can result from keeping all data forever?

``` text
____________________________________
____________________________________
____________________________________
```

Consider:

``` text
Privacy
Legal Risk
Storage
Data Management
```

------------------------------------------------------------------------

# ⚠️ Part 23 --- Under-Retention

What problems can result from deleting important information too early?

``` text
____________________________________
____________________________________
____________________________________
```

------------------------------------------------------------------------

# 🗺️ Part 24 --- Choose the Capability

Detect an SSN:

``` text
______________________________
```

Recognize a learned content category:

``` text
______________________________
```

Mark a file Confidential:

``` text
______________________________
```

Block sensitive external sharing:

``` text
______________________________
```

Warn a user:

``` text
______________________________
```

Restrict supported USB copying:

``` text
______________________________
```

Apply broad location retention:

``` text
______________________________
```

Apply retention to a specific document category:

``` text
______________________________
```

Manage an official corporate record:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 25 --- Build the Flow

Fill in:

``` text
DISCOVER
      ↓
______________________________
      ↓
CLASSIFY / PROTECT
      ↓
______________________________
      ↓
PREVENT LOSS
      ↓
______________________________
      ↓
KEEP / DELETE
      ↓
______________________________
      ↓
OFFICIAL RECORD
      ↓
______________________________
```

------------------------------------------------------------------------

# 🏆 Final Challenge --- The Contoso Contract

A contract contains:

``` text
Customer Information
Pricing
Banking Details
Confidential Terms
```

It must:

``` text
1. Be recognized as containing sensitive financial data.
2. Be classified Confidential.
3. Be protected from inappropriate external sharing.
4. Be retained seven years.
5. Become an official record after signing.
```

Requirement 1:

``` text
______________________________
```

Requirement 2:

``` text
______________________________
```

Requirement 3:

``` text
______________________________
```

Requirement 4:

``` text
______________________________
```

Requirement 5:

``` text
______________________________
```

------------------------------------------------------------------------

# 📝 Final Design Exercise

  Data Type           Classification   Protection     DLP            Retention / Record
  ------------------- ---------------- -------------- -------------- --------------------
  Public Brochure     \_\_\_\_\_\_     \_\_\_\_\_\_   \_\_\_\_\_\_   \_\_\_\_\_\_
  HR Employee File    \_\_\_\_\_\_     \_\_\_\_\_\_   \_\_\_\_\_\_   \_\_\_\_\_\_
  Customer Contract   \_\_\_\_\_\_     \_\_\_\_\_\_   \_\_\_\_\_\_   \_\_\_\_\_\_
  Financial Report    \_\_\_\_\_\_     \_\_\_\_\_\_   \_\_\_\_\_\_   \_\_\_\_\_\_
  Internal IT Guide   \_\_\_\_\_\_     \_\_\_\_\_\_   \_\_\_\_\_\_   \_\_\_\_\_\_

There is not always one perfect answer. Explain **why** each control
fits.

------------------------------------------------------------------------

# ✅ Suggested Answers

``` text
Public Brochure
→ Public

Internal IT Procedure
→ Internal

Customer Pricing Agreement
→ Confidential

Employee SSN / Medical File
→ Highly Confidential
```

``` text
SSN / financial identifier
→ Sensitive Information Type

Learned content category
→ Trainable Classifier

Classify / protect
→ Sensitivity Label

Publish labels
→ Label Policy

Sensitive external sharing
→ DLP

User warning
→ Policy Tip

USB / endpoint activity
→ Endpoint DLP

Broad retention
→ Retention Policy

Item/content retention
→ Retention Label

Official record
→ Records Management
```

Label vs DLP:

``` text
Mark Highly Confidential
→ Sensitivity Label

Encrypt classified document
→ Sensitivity Label

Stop external sharing
→ DLP

Warn user
→ DLP / Policy Tip
```

Lifecycle vs Records:

``` text
Routine Teams retention
→ Data Lifecycle Management

Signed legal contract
→ Records Management

Delete obsolete information
→ Data Lifecycle Management

Official corporate record
→ Records Management
```

Final contract:

``` text
1. Sensitive Information Type
2. Sensitivity Label
3. DLP
4. Retention Label / appropriate retention configuration
5. Records Management
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

``` text
WHAT IS IT?
→ Classification

HOW SENSITIVE IS IT?
→ Sensitivity Label

WHAT IS THE USER DOING?
→ DLP

HOW LONG DO WE KEEP IT?
→ Retention

IS IT AN OFFICIAL RECORD?
→ Records Management
```

------------------------------------------------------------------------

# ✅ Lab Completion Checklist

-   [ ] I understand sensitive information types.
-   [ ] I understand trainable classifiers.
-   [ ] I understand sensitivity labels and label policies.
-   [ ] I understand DLP and policy tips.
-   [ ] I understand Endpoint DLP.
-   [ ] I can distinguish retention policies from retention labels.
-   [ ] I understand Records Management.
-   [ ] I can design a simple data-protection strategy.

------------------------------------------------------------------------

# ➡️ Next

## 📘 Lesson 16 --- Insider Risk, eDiscovery & Audit

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **[Lesson 15 --- Information Protection, DLP & Data
Lifecycle](../lessons/%F0%9F%93%98%20Lesson%2015%20%E2%80%94%20Information%20Protection%2C%20DLP%20%26%20Data%20Lifecycle.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
