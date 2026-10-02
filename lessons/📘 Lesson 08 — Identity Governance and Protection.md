# 📘 Lesson 08 — Identity Governance & Protection

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 08  
**Lab:** 🔵🟡 Explore Identity Governance & Protection  
**Difficulty:** Beginner  
**Milestone:** Completes the Microsoft Entra section

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain Microsoft Entra ID Protection
- Describe user risk and sign-in risk
- Explain risk detections at a fundamentals level
- Describe Microsoft Entra ID Governance
- Explain Privileged Identity Management (PIM)
- Explain access reviews
- Describe entitlement management and access packages
- Describe lifecycle workflows
- Explain Terms of Use at a fundamentals level
- Connect identity governance to least privilege and Zero Trust
- Recognize when governance or protection capabilities are appropriate

---

# 🧠 Two Related Problems

Identity security has two major questions:

```text
IS THIS IDENTITY OR SIGN-IN RISKY?
```

and:

```text
SHOULD THIS IDENTITY STILL HAVE THIS ACCESS?
```

Microsoft Entra provides capabilities for both.

```text
IDENTITY PROTECTION
=
Detect and respond to identity risk
```

```text
IDENTITY GOVERNANCE
=
Manage identity access over time
```

---

# 🛡️ Microsoft Entra ID Protection

Microsoft Entra ID Protection helps organizations detect, investigate, and respond to identity-related risks.

Conceptually:

```text
SIGN-IN ACTIVITY
      ↓
RISK SIGNALS
      ↓
IDENTITY PROTECTION
      ↓
DETECT / INVESTIGATE / RESPOND
```

It helps administrators identify suspicious activity involving users and authentication.

---

# ⚠️ Risk Detection

A **risk detection** represents suspicious activity that may indicate an identity or authentication attempt has been compromised.

Examples of suspicious conditions can include signals associated with:

```text
Leaked Credentials

Unusual Sign-In Activity

Suspicious Authentication Behavior

Known Threat Intelligence
```

Microsoft's exact detections evolve over time.

For SC-900, focus on the purpose:

> **Risk detections help identify potentially compromised identities or sign-ins.**

---

# 👤 User Risk

**User risk** represents the probability that a user's identity may be compromised.

Think:

```text
IS THIS USER ACCOUNT
LIKELY COMPROMISED?
```

Example:

```text
Credentials Appear Compromised
        ↓
User Risk Increases
```

---

# 🔐 Sign-In Risk

**Sign-in risk** represents the probability that a particular authentication request was not performed by the legitimate user.

Think:

```text
IS THIS PARTICULAR SIGN-IN
LIKELY LEGITIMATE?
```

---

# 🧠 User Risk vs Sign-In Risk

```text
USER RISK
=
Risk associated with the identity
```

```text
SIGN-IN RISK
=
Risk associated with a specific sign-in
```

Example:

```text
Alex's account
may be compromised
=
USER RISK
```

```text
Alex's 2:00 AM
sign-in looks suspicious
=
SIGN-IN RISK
```

---

# 🚦 Risk and Conditional Access

Risk signals can be used with access policies in supported environments.

Conceptually:

```text
SIGN-IN REQUEST
      ↓
RISK EVALUATED
      ↓
CONDITIONAL ACCESS
      ↓
REQUIRE CONTROL
or
BLOCK
```

This connects Lesson 08 directly to Lesson 07.

---

# 🔎 Investigating Risk

Security teams may review information such as:

```text
Risky Users

Risky Sign-Ins

Risk Detections
```

The goal is to determine whether activity is legitimate or potentially malicious.

Possible organizational responses can include:

```text
Require Strong Authentication

Require Password Remediation

Block Access

Investigate Activity

Confirm User Safety
```

Exact response options depend on licensing, policy, and configuration.

---

# 🏛️ Microsoft Entra ID Governance

Identity governance focuses on ensuring:

> **The right people have the right access to the right resources at the right time.**

A useful formula:

```text
RIGHT IDENTITY
+
RIGHT ACCESS
+
RIGHT RESOURCE
+
RIGHT TIME
```

Identity governance helps organizations manage access throughout the identity lifecycle.

---

# 🔄 The Access Lifecycle

Access changes over time.

```text
JOINER
   ↓
Needs Access

MOVER
   ↓
Access Changes

LEAVER
   ↓
Access Removed
```

Without governance, permissions can accumulate.

Example:

```text
Accounting Employee
      ↓
Moves to HR
      ↓
Gets HR Access
      ↓
Keeps Accounting Access
      ↓
EXCESSIVE ACCESS
```

Governance helps reduce this problem.

---

# 👑 Privileged Identity Management — PIM

**Microsoft Entra Privileged Identity Management (PIM)** helps organizations manage privileged access.

Instead of:

```text
ADMIN
=
Permanent Privilege
24 Hours a Day
```

PIM can support:

```text
Eligible Access
      ↓
Activation When Needed
      ↓
Time-Limited Privilege
      ↓
Access Expires
```

---

# ⏱️ Just-in-Time Privileged Access

This is often described as:

> **Just-in-time access**

Example:

```text
Administrator Normally
Has No Active Privileged Role
        ↓
Needs Admin Access
        ↓
Activates Eligible Role
        ↓
Completes Requirements
        ↓
Uses Role Temporarily
        ↓
Role Deactivates / Expires
```

This reduces the amount of standing privileged access.

---

# 🔐 PIM Activation Controls

Depending on configuration, organizations can require controls such as:

```text
MFA

Approval

Justification

Limited Activation Duration
```

PIM helps answer:

```text
WHO needs privileged access?

WHY?

WHEN?

FOR HOW LONG?
```

---

# 🔍 Access Reviews

Access Reviews help organizations periodically verify whether users still need access.

Conceptually:

```text
USER HAS ACCESS
      ↓
TIME PASSES
      ↓
ACCESS REVIEW
      ↓
STILL NEEDED?
   ↙        ↘
 YES        NO
 ↓           ↓
KEEP       REMOVE
```

---

# 🧠 Why Access Reviews Matter

Permissions can become outdated because:

```text
Employees Change Jobs

Projects End

Contractors Leave

Managers Change

Temporary Access Becomes Permanent
```

Access reviews help reduce access that is no longer necessary.

---

# 🌎 Guest Access Review Example

Contoso invites 25 contractors to a project.

Six months later:

```text
Project Ends
      ↓
Access Review
      ↓
Which Guests Still Need Access?
      ↓
Remove Unnecessary Access
```

This is especially useful for external collaboration.

---

# 📦 Entitlement Management

**Entitlement management** helps organizations manage access to groups, applications, SharePoint sites, and other resources through governed processes.

A key concept is:

# Access Packages

An access package can bundle resources a user needs.

Example:

```text
NEW MARKETING CONTRACTOR
        ↓
Requests:
"Marketing Contractor Package"
        ↓
Package Provides Approved Access
        ↓
Access Can Expire
```

---

# 📦 Access Package Example

Instead of separately granting:

```text
Marketing Team

Marketing SharePoint

Marketing Application

Project Group
```

an organization can create a governed package:

```text
Marketing Contractor
Access Package
      ↓
Required Resources
```

This can simplify access requests and lifecycle management.

---

# 📝 Approval and Expiration

Access packages can support governance concepts such as:

```text
Request

Approval

Assignment

Expiration

Review
```

This is useful when access should not remain forever.

---

# 🔄 Lifecycle Workflows

**Lifecycle Workflows** help automate identity lifecycle tasks around events such as employees joining, moving, or leaving.

Conceptually:

```text
EMPLOYEE EVENT
      ↓
WORKFLOW
      ↓
AUTOMATED TASKS
```

Examples might include processes related to:

```text
Onboarding

Role Changes

Offboarding
```

The exact available tasks and integrations can change over time.

---

# 🧠 Lifecycle Workflow Example

A company knows Taylor's final employment date.

A lifecycle process could help coordinate identity-related offboarding actions.

Conceptually:

```text
LEAVER EVENT
      ↓
LIFECYCLE WORKFLOW
      ↓
IDENTITY TASKS
      ↓
ACCESS REDUCED / REMOVED
```

Automation helps make identity processes more consistent.

---

# 📜 Terms of Use

Microsoft Entra Terms of Use can present organizational terms that users may need to accept before accessing resources.

Example:

```text
External Contractor
      ↓
Attempts Access
      ↓
Terms of Use
      ↓
Accepts Required Terms
      ↓
Continues According to Policy
```

This can support governance and compliance requirements.

---

# 🧩 Governance Tool Map

| Need | Microsoft Entra Capability |
|---|---|
| Detect risky identities | ID Protection |
| Detect risky sign-ins | ID Protection |
| Temporary privileged role | PIM |
| Periodically verify access | Access Reviews |
| Package governed access | Entitlement Management |
| Automate joiner/mover/leaver tasks | Lifecycle Workflows |
| Require acknowledgement of terms | Terms of Use |

---

# 🛡️ Identity Governance and Zero Trust

Governance strongly supports:

## Use Least Privilege

```text
ONLY NECESSARY ACCESS
```

and:

## Assume Breach

```text
LIMIT STANDING PRIVILEGE
+
REVIEW ACCESS
+
REMOVE UNUSED ACCESS
```

Identity Protection also supports:

## Verify Explicitly

by using risk information to help make access decisions.

---

# 🏢 Real-World Example

Contoso has:

```text
150 Employees

10 IT Administrators

20 Contractors

Microsoft 365

Azure Resources
```

A mature identity approach might use:

```text
MFA / Passwordless
      ↓
Conditional Access
      ↓
Risk Detection
      ↓
Least-Privilege Roles
      ↓
PIM for Privileged Access
      ↓
Access Reviews
      ↓
Lifecycle Processes
```

These are not isolated tools.

They work together as an identity security strategy.

---

# 🧠 Lessons 03–08 Identity Map

```text
MICROSOFT ENTRA ID
        │
        ├── Users & Groups
        │
        ├── Authentication
        │
        ├── MFA
        │
        ├── Passwordless
        │
        ├── Conditional Access
        │
        ├── Roles / RBAC
        │
        ├── Identity Protection
        │
        └── Identity Governance
```

This completes the major Microsoft Entra section of the course.

---

# 🎯 Exam Focus

Know these relationships:

```text
IDENTITY PROTECTION
=
Detect identity risk
```

```text
USER RISK
=
Is the identity compromised?
```

```text
SIGN-IN RISK
=
Is this sign-in suspicious?
```

```text
PIM
=
Manage privileged access
```

```text
ACCESS REVIEW
=
Does this person still need access?
```

```text
ENTITLEMENT MANAGEMENT
=
Govern access requests and packages
```

```text
LIFECYCLE WORKFLOWS
=
Automate identity lifecycle tasks
```

---

# 🧠 Memory Tricks

### PIM

```text
PRIVILEGE
IN
MOMENTS
```

Remember:

```text
Admin access when needed,
not necessarily forever
```

### Access Reviews

```text
STILL NEED IT?
```

### Entitlement Management

```text
PACKAGE THE ACCESS
```

### Identity Protection

```text
WHO / SIGN-IN LOOKS RISKY?
```

---

# ❓ Knowledge Check

### 1.

What does Microsoft Entra ID Protection help detect?

A. Identity-related risk  
B. Printer toner levels  
C. Network cable faults  
D. Laptop battery health

---

### 2.

What does user risk represent?

A. The likelihood that an identity may be compromised  
B. The cost of a Microsoft license  
C. The number of groups a user owns  
D. Internet speed

---

### 3.

What does sign-in risk represent?

A. The probability that a particular sign-in may not be legitimate  
B. The user's job title  
C. The number of Azure subscriptions  
D. A SharePoint storage quota

---

### 4.

What is a primary purpose of PIM?

A. Manage privileged access  
B. Create email signatures  
C. Manage printers  
D. Store backups

---

### 5.

What is an access review designed to answer?

A. Does this user still need this access?  
B. What color should the portal be?  
C. Which laptop model is fastest?  
D. How many emails were sent?

---

### 6.

What can entitlement management use to bundle governed access?

A. Access packages  
B. Network packets  
C. Storage disks  
D. Email aliases

---

### 7.

Which capability helps automate identity lifecycle tasks?

A. Lifecycle Workflows  
B. Azure Firewall  
C. Microsoft Defender Antivirus  
D. Azure DNS

---

### 8.

Which concept best supports reducing permanent privileged access?

A. Just-in-time access with PIM  
B. Giving everyone Global Administrator  
C. Never reviewing roles  
D. Shared administrator passwords

---

### 9.

Which Zero Trust principle is strongly supported by access reviews and PIM?

A. Use least privilege  
B. Trust internal networks automatically  
C. Disable monitoring  
D. Share accounts

---

### 10.

A contractor's project has ended. Which capability could help verify whether the contractor still needs access?

A. Access Review  
B. Azure Storage  
C. Microsoft Paint  
D. Windows Update

---

# ✅ Knowledge Check Answers

```text
1. A — Identity-related risk

2. A — The likelihood that an identity may be compromised

3. A — The probability that a particular sign-in may not be legitimate

4. A — Manage privileged access

5. A — Does this user still need this access?

6. A — Access packages

7. A — Lifecycle Workflows

8. A — Just-in-time access with PIM

9. A — Use least privilege

10. A — Access Review
```

---

# 📌 Lesson Summary

You learned:

```text
IDENTITY PROTECTION
=
Detect and respond to identity risk
```

```text
PIM
=
Control privileged access
```

```text
ACCESS REVIEWS
=
Regularly verify access
```

```text
ENTITLEMENT MANAGEMENT
=
Govern access packages and requests
```

```text
LIFECYCLE WORKFLOWS
=
Automate identity lifecycle tasks
```

Together, these capabilities help organizations maintain appropriate access over time.

---

# 🧪 Lab

Complete:

## 🔵🟡 Lab 08 — Explore Identity Governance & Protection

➡️ **[Lab 08 — Explore Identity Governance & Protection](../labs/Lab%2008%20—%20Explore%20Identity%20Governance%20&%20Protection.md)**

---

# 🏗️ Project Checkpoint

You have now completed Lessons 01–08.

Before moving into Microsoft Security Solutions, complete:

## 🏗️ Project 01 — Secure an Organization's Identity Environment

The project combines:

```text
Zero Trust

Users & Groups

Authentication

MFA

Passwordless

Conditional Access

RBAC

Identity Protection

Identity Governance
```

➡️ **[Project 01 — Secure an Organization's Identity Environment](../projects/Project%2001%20—%20Secure%20an%20Organization's%20Identity%20Environment.md)**

---

# ➡️ Next Lesson

After Project 01:

## 📘 Lesson 09 — Azure Infrastructure Security

This begins the Microsoft Security Solutions section.

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Microsoft Entra ID Protection](https://learn.microsoft.com/en-us/entra/id-protection/overview-identity-protection)
- [Microsoft Entra ID Governance](https://learn.microsoft.com/en-us/entra/id-governance/identity-governance-overview)
- [Privileged Identity Management](https://learn.microsoft.com/en-us/entra/id-governance/privileged-identity-management/pim-configure)
- [Access Reviews](https://learn.microsoft.com/en-us/entra/id-governance/access-reviews-overview)
- [Entitlement Management](https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-overview)

---

# 📚 Course Navigation

⬅️ **Lesson 07 — Conditional Access & RBAC**

🧪 **[Lab 08](../labs/Lab%2008%20—%20Explore%20Identity%20Governance%20&%20Protection.md)**

🏗️ **[Project 01](../projects/Project%2001%20—%20Secure%20an%20Organization's%20Identity%20Environment.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
