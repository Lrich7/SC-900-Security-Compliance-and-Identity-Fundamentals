# 📘 Lesson 07 — Conditional Access & RBAC

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 07  
**Lab:** 🔵 Explore the Tool + 🟡 Scenario — Conditional Access & RBAC  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain Microsoft Entra Conditional Access
- Describe common Conditional Access signals
- Describe common access decisions and controls
- Explain how Conditional Access supports Zero Trust
- Explain role-based access control (RBAC)
- Describe Microsoft Entra administrative roles
- Describe Azure RBAC at a fundamentals level
- Distinguish Microsoft Entra roles from Azure roles
- Explain least privilege
- Recognize role assignments, scopes, and permissions
- Explain why privileged access should be carefully controlled
- Locate Conditional Access and role-management areas in Microsoft portals

---

# 🚦 What Is Conditional Access?

Microsoft Entra **Conditional Access** is Microsoft's policy engine for evaluating access requests and applying access controls.

A simple way to think about it is:

```text
IF
certain conditions are true

THEN
apply an access control
```

Example:

```text
IF
User is signing in
from an unfamiliar situation

THEN
Require MFA
```

Conditional Access helps organizations make access decisions using identity and security signals rather than simply trusting a username and password.

---

# 🧠 The Basic Conditional Access Flow

```text
USER REQUESTS ACCESS
        ↓
COLLECT SIGNALS
        ↓
EVALUATE POLICY
        ↓
APPLY ACCESS CONTROLS
        ↓
ALLOW / BLOCK / REQUIRE CONTROLS
```

Conditional Access is an important part of Microsoft's Zero Trust approach.

---

# 🔎 Conditional Access Signals

Conditional Access can evaluate different types of information.

Common signals can include:

```text
User

Group

Target Resource

Device

Location

Platform

Sign-In Risk

User Risk

Authentication Context
```

Not every policy uses every signal.

---

# 👤 User and Group

A policy can target:

```text
Specific Users

Specific Groups

Directory Roles

Broad User Populations
```

Example:

```text
IT Administrators
       ↓
Require Strong Authentication
```

This lets organizations apply stronger controls to higher-risk identities.

---

# 📦 Target Resources

Conditional Access can apply when users attempt to access specific resources.

Examples can include:

```text
Microsoft 365

Azure Management

Enterprise Applications

Other Protected Resources
```

Conceptually:

```text
USER
  ↓
REQUESTS RESOURCE
  ↓
POLICY APPLIES
```

---

# 🌎 Location

Location can be one signal in an access decision.

Examples:

```text
Known Network Location

Unexpected Country/Region

Untrusted Location
```

However:

> **Location alone should not be treated as proof that a user is trustworthy.**

Zero Trust assumes that being "inside" the corporate network does not automatically make an identity safe.

---

# 💻 Device Information

Device-related information can also influence access decisions.

Examples might include:

```text
Device Platform

Device State

Compliance Status
```

A company could conceptually require:

```text
User Authenticated
       +
Device Meets Requirements
       ↓
Access Sensitive Resource
```

---

# ⚠️ Risk

Microsoft Entra can provide risk-related signals in supported environments.

Examples include:

```text
User Risk

Sign-In Risk
```

These signals can help organizations react to suspicious authentication activity.

Example:

```text
HIGH SIGN-IN RISK
       ↓
Require Additional Control
or
Block Access
```

Risk-based capabilities depend on licensing and configuration.

---

# 🛡️ Access Controls

After evaluating conditions, Conditional Access can apply controls.

Examples include:

```text
Block Access

Require MFA

Require Authentication Strength

Require Compliant Device

Require Approved Conditions
```

The exact controls available depend on Microsoft's current platform capabilities and licensing.

---

# 💪 Authentication Strength

From Lessons 05 and 06:

Authentication strength can specify which authentication methods satisfy a requirement.

Example:

```text
ADMIN ACCESS
      ↓
Conditional Access
      ↓
Require
Phishing-Resistant MFA
```

This is stronger than simply saying:

```text
Require any MFA
```

for scenarios where stronger authentication is appropriate.

---

# 📱 Device Compliance Example

Imagine Contoso has sensitive HR data.

A policy design might conceptually say:

```text
IF
User accesses HR application

THEN
Require MFA
AND
Require compliant device
```

This combines:

```text
Identity Security
+
Device Security
```

---

# 🚫 Block Access Example

An organization may decide that certain access conditions are unacceptable.

Example:

```text
IF
Access request violates
a critical policy condition

THEN
Block Access
```

Conditional Access can therefore do more than simply request MFA.

---

# 🧱 Conditional Access and Zero Trust

Conditional Access strongly supports:

# Verify Explicitly

Instead of:

```text
Correct Password
      ↓
TRUST USER
```

a modern decision can consider:

```text
Identity

Authentication

Device

Application

Location

Risk

Policy
```

Then:

```text
VERIFY
   ↓
EVALUATE
   ↓
DECIDE
```

---

# ⚠️ Conditional Access Safety

Conditional Access policies can affect large numbers of users.

A poorly designed policy can potentially prevent legitimate users or administrators from accessing resources.

Production changes should be:

```text
Planned

Tested

Piloted

Monitored
```

Microsoft also provides capabilities such as **Report-only mode** that can help evaluate policies before enforcement.

Organizations should also plan for emergency access accounts when designing resilient Conditional Access deployments.

---

# 📊 Report-Only Mode

Report-only mode allows administrators to evaluate how a Conditional Access policy would behave without enforcing it.

Conceptually:

```text
CREATE POLICY
      ↓
REPORT-ONLY
      ↓
OBSERVE RESULTS
      ↓
ADJUST
      ↓
ENFORCE WHEN READY
```

This supports safer deployment.

---

# 🔐 What Is RBAC?

**Role-Based Access Control (RBAC)** assigns permissions through roles.

Instead of assigning individual permissions one by one:

```text
USER
 ↓
PERMISSION A
PERMISSION B
PERMISSION C
```

you can use:

```text
USER
 ↓
ROLE
 ↓
SET OF PERMISSIONS
```

This makes access easier to manage and review.

---

# 👑 Microsoft Entra Roles

Microsoft Entra roles control administrative capabilities in Microsoft Entra and related identity services.

Examples include:

```text
Global Administrator

User Administrator

Groups Administrator

Authentication Administrator

Application Administrator
```

Different roles provide different permissions.

---

# 🚨 Global Administrator

Global Administrator is a highly privileged Microsoft Entra role.

It should not be the default role for everyone in IT.

A better principle is:

```text
JOB REQUIREMENT
      ↓
MINIMUM NECESSARY ROLE
```

This supports:

> **Least privilege**

---

# ☁️ Azure RBAC

Azure also uses role-based access control.

**Azure RBAC** controls access to Azure resources.

Examples include:

```text
Virtual Machines

Storage Accounts

Virtual Networks

Subscriptions

Resource Groups
```

Common Azure roles include concepts such as:

```text
Owner

Contributor

Reader
```

and many service-specific roles.

---

# 🧠 Entra Roles vs Azure RBAC

This distinction is important.

## Microsoft Entra Role

```text
Identity / Directory Administration
```

Example:

```text
User Administrator
```

## Azure RBAC Role

```text
Azure Resource Authorization
```

Example:

```text
Virtual Machine Contributor
```

Memory trick:

```text
ENTRA ROLE
=
WHO CAN ADMINISTER IDENTITY?
```

```text
AZURE RBAC
=
WHO CAN DO WHAT
TO AZURE RESOURCES?
```

---

# 🎯 RBAC Components

At a high level, an Azure role assignment connects:

```text
SECURITY PRINCIPAL
        +
ROLE DEFINITION
        +
SCOPE
```

---

# 👤 Security Principal

The identity receiving access.

Examples:

```text
User

Group

Service Principal

Managed Identity
```

---

# 📋 Role Definition

The role describes allowed actions.

Examples:

```text
Reader

Contributor

Owner
```

At a fundamentals level:

```text
Reader
=
View resources
```

```text
Contributor
=
Manage resources,
but not grant Azure RBAC access
```

```text
Owner
=
Broad resource management
+
Can assign Azure RBAC roles
```

---

# 🎯 Scope

Scope determines **where** the role applies.

Azure scopes can include:

```text
Management Group

Subscription

Resource Group

Resource
```

Conceptually:

```text
Broad
Management Group
      ↓
Subscription
      ↓
Resource Group
      ↓
Individual Resource
Narrow
```

---

# 🧠 Why Scope Matters

Suppose Alex only needs to manage one virtual machine.

This:

```text
Alex
 ↓
Broad Subscription-Level Owner
```

may provide far more access than necessary.

A better design could be:

```text
Alex
 ↓
Appropriate Role
 ↓
Specific Required Scope
```

This supports least privilege.

---

# 🛡️ Least Privilege

Least privilege means:

> Give an identity only the access necessary to perform its required tasks.

Think:

```text
RIGHT IDENTITY
+
RIGHT ROLE
+
RIGHT SCOPE
+
RIGHT TIME
```

This concept appears throughout Microsoft security.

---

# ⏱️ Permanent vs Just-in-Time Access

Some administrative access may not need to be permanent.

Microsoft Entra Privileged Identity Management (PIM), covered more in Lesson 08, can help organizations manage privileged access using concepts such as:

```text
Eligible Access

Time-Limited Activation

Approval

MFA

Access Reviews
```

Instead of:

```text
ADMIN
=
Permanent Privilege Forever
```

organizations can move toward:

```text
ADMIN
=
Privilege When Needed
```

---

# 🏢 Real-World Scenario

Contoso has an IT technician named Morgan.

Morgan needs to:

```text
Reset certain user information

Review identity settings

Manage a small set of Azure resources
```

A poor design:

```text
Morgan
 ↓
Global Administrator
+
Azure Subscription Owner
```

A better design:

```text
Morgan
 ↓
Appropriate Entra Role
+
Appropriate Azure Role
+
Limited Scope
```

The exact roles depend on the required tasks.

The principle is:

> Do not grant broad access when narrower access will do the job.

---

# 🔗 Conditional Access + RBAC

Conditional Access and RBAC solve different problems.

## RBAC

Determines:

```text
WHAT ARE YOU AUTHORIZED TO DO?
```

## Conditional Access

Determines:

```text
UNDER WHAT CONDITIONS
CAN YOU ACCESS IT?
```

Together:

```text
USER
 ↓
HAS APPROPRIATE ROLE
 ↓
REQUESTS ACCESS
 ↓
CONDITIONAL ACCESS EVALUATES REQUEST
 ↓
ACCESS GRANTED UNDER REQUIRED CONDITIONS
```

---

# 🧠 Authentication + Conditional Access + RBAC

These concepts fit together:

```text
AUTHENTICATION
=
Who are you?
```

```text
CONDITIONAL ACCESS
=
Under what conditions
can you access?
```

```text
RBAC
=
What are you allowed to do?
```

This is a very useful SC-900 mental model.

---

# 🎯 Exam Focus

Know these relationships:

```text
CONDITIONAL ACCESS
=
Policy-based access decisions
using signals and controls
```

```text
SIGNALS
=
User, device, location,
resource, risk, and more
```

```text
RBAC
=
Permissions through roles
```

```text
MICROSOFT ENTRA ROLES
=
Identity/directory administration
```

```text
AZURE RBAC
=
Azure resource authorization
```

```text
SCOPE
=
Where a role assignment applies
```

```text
LEAST PRIVILEGE
=
Minimum necessary access
```

---

# 🧠 Memory Tricks

### Conditional Access

```text
IF THIS
THEN THAT
```

### RBAC

```text
ROLE
=
BUNDLE OF PERMISSIONS
```

### Scope

```text
SCOPE
=
WHERE THE ROLE WORKS
```

### Least Privilege

```text
ONLY WHAT YOU NEED
```

---

# ❓ Knowledge Check

### 1.

What does Conditional Access primarily do?

A. Repairs hardware  
B. Evaluates access policies using signals and controls  
C. Creates network cables  
D. Replaces all authentication

---

### 2.

Which could be a Conditional Access signal?

A. User identity  
B. Device information  
C. Location  
D. All of the above

---

### 3.

Which is an example of a Conditional Access control?

A. Require MFA  
B. Replace a laptop battery  
C. Add RAM  
D. Print a document

---

### 4.

What is RBAC?

A. Role-Based Access Control  
B. Remote Backup Access Computer  
C. Risk-Based Azure Cloud  
D. Resource Backup Administration Center

---

### 5.

Which system primarily controls administrative permissions for Microsoft Entra identities?

A. Microsoft Entra roles  
B. Azure Firewall  
C. Microsoft Sentinel  
D. Azure Storage

---

### 6.

Which system primarily controls authorization to Azure resources?

A. Azure RBAC  
B. Microsoft Authenticator  
C. Microsoft Purview  
D. Defender for Office 365

---

### 7.

What does scope determine in an Azure role assignment?

A. Where the permissions apply  
B. The user's password  
C. The user's email address  
D. The physical datacenter temperature

---

### 8.

Which approach best follows least privilege?

A. Give every IT employee Global Administrator  
B. Give the minimum role and scope needed  
C. Give every user Owner  
D. Disable all roles

---

### 9.

What does Conditional Access report-only mode help administrators do?

A. Evaluate policy impact before enforcement  
B. Delete every policy  
C. Disable authentication  
D. Create physical reports only

---

### 10.

Which statement best describes the relationship among authentication, Conditional Access, and RBAC?

A. They are identical  
B. Authentication verifies identity, Conditional Access evaluates access conditions, and RBAC defines authorized actions  
C. RBAC authenticates passwords  
D. Conditional Access replaces all roles

---

# ✅ Knowledge Check Answers

```text
1. B — Evaluates access policies using signals and controls

2. D — All of the above

3. A — Require MFA

4. A — Role-Based Access Control

5. A — Microsoft Entra roles

6. A — Azure RBAC

7. A — Where the permissions apply

8. B — Give the minimum role and scope needed

9. A — Evaluate policy impact before enforcement

10. B — Authentication verifies identity,
Conditional Access evaluates conditions,
and RBAC defines authorized actions
```

---

# 📌 Lesson Summary

You learned:

```text
CONDITIONAL ACCESS
=
IF conditions
THEN controls
```

```text
RBAC
=
Permissions through roles
```

```text
ENTRA ROLES
=
Identity administration
```

```text
AZURE RBAC
=
Azure resource authorization
```

```text
LEAST PRIVILEGE
=
Minimum role
+
Minimum scope
+
Only when needed
```

Together, these controls help organizations make better access decisions and reduce excessive permissions.

---

# 🧪 Lab

This lesson benefits strongly from a lab.

## 🔵🟡 Lab 07 — Explore Conditional Access & RBAC

The lab combines:

- 🔵 Read-only portal exploration
- 🟡 Access-control scenarios

You will locate Conditional Access and role-management areas without changing production policies.

➡️ **[Lab 07 — Explore Conditional Access & RBAC](../labs/Lab%2007%20—%20Explore%20Conditional%20Access%20&%20RBAC.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 08 — Identity Governance & Protection

Next you will learn about:

- Identity Protection
- Risky users and sign-ins
- Privileged Identity Management
- Access Reviews
- Entitlement Management
- Lifecycle Workflows

After Lesson 08, you will reach the first major project checkpoint:

> 🏗️ **Project 01 — Secure an Organization's Identity Environment**

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Conditional Access Overview](https://learn.microsoft.com/en-us/entra/identity/conditional-access/overview)
- [Microsoft Entra Built-in Roles](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference)
- [Azure RBAC Overview](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview)
- [Azure RBAC Scope](https://learn.microsoft.com/en-us/azure/role-based-access-control/scope-overview)

---

# 📚 Course Navigation

⬅️ **Lesson 06 — Passwordless Authentication**

🧪 **[Lab 07 — Explore Conditional Access & RBAC](../labs/Lab%2007%20—%20Explore%20Conditional%20Access%20&%20RBAC.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
