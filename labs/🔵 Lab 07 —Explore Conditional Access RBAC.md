# 🔵🟡 Lab 07 — Explore Conditional Access & RBAC

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 07 — Conditional Access & RBAC  
**Lab Type:** 🔵 Explore the Tool + 🟡 Scenario Lab  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Locate Conditional Access in Microsoft Entra
- Recognize the major parts of a Conditional Access policy
- Identify common Conditional Access signals
- Identify common access controls
- Recognize report-only mode
- Locate Microsoft Entra administrative roles
- Recognize Azure RBAC role assignments
- Explain role, principal, and scope
- Apply least privilege to simple scenarios
- Distinguish authentication, Conditional Access, and RBAC

---

# 🧪 Lab Philosophy

This lab combines:

# 🔵 Explore the Tool

and:

# 🟡 Scenario Practice

You will observe the administrative tools and then apply the concepts to fictional situations.

You do **not** need to create or enforce a Conditional Access policy.

---

# ⚠️ Production Safety

Conditional Access and role assignments can affect access across an organization.

For this lab:

```text
DO NOT:

Enable a policy

Disable a policy

Change assignments

Change grant controls

Assign administrative roles

Assign Azure roles

Remove role assignments
```

unless you are specifically authorized to do so in a safe test environment.

---

# 🚀 Part 1 — Open Microsoft Entra

Open:

```text
https://entra.microsoft.com
```

Sign in with an authorized account.

Locate:

```text
Entra ID
```

---

# 🚦 Part 2 — Find Conditional Access

Locate:

```text
Conditional Access
```

The exact navigation can change as Microsoft updates the portal.

If you can view policies, do not edit them.

Look for the major building blocks of a policy.

Conceptually:

```text
ASSIGNMENTS
     ↓
CONDITIONS / SIGNALS
     ↓
ACCESS CONTROLS
     ↓
POLICY STATE
```

---

# 👤 Part 3 — Identify Assignments

Within Conditional Access, look for concepts related to:

```text
Users

Groups

Target Resources
```

These answer:

```text
WHO does the policy apply to?

WHAT resource does the policy protect?
```

Complete:

```text
Users / Groups
=
____________________________________
```

```text
Target Resources
=
____________________________________
```

---

# 🔎 Part 4 — Identify Conditions and Signals

Look for conditions or signals that can influence policy evaluation.

Depending on the portal and licensing, you may encounter concepts such as:

```text
User Risk

Sign-In Risk

Device Platform

Locations

Client Apps

Device Information
```

Do not change anything.

Mark the items you can locate:

```text
[ ] User Risk

[ ] Sign-In Risk

[ ] Device Platform

[ ] Location

[ ] Client Apps

[ ] Device-related conditions

[ ] Other
```

---

# 🛡️ Part 5 — Identify Access Controls

Look for controls related to access decisions.

Examples can include:

```text
Block Access

Require MFA

Require Authentication Strength

Require Compliant Device
```

The exact options visible depend on the current Microsoft platform, licensing, and configuration.

---

# 🧠 Conditional Access Formula

Complete:

```text
IF
______________________________

THEN
______________________________
```

Example:

```text
IF
Administrator accesses
sensitive cloud resources

THEN
Require phishing-resistant authentication
```

---

# 📊 Part 6 — Find Report-Only Mode

If visible, locate the policy state options.

Look for:

```text
Report-only
```

Do not change a policy.

Why is report-only useful?

```text
____________________________________

____________________________________
```

Think:

```text
TEST BEFORE ENFORCING
```

---

# 🚨 Part 7 — Lockout Scenario

An administrator creates this policy:

```text
ALL USERS
+
ALL RESOURCES
+
BLOCK ACCESS
```

and immediately enables it without testing or exclusions.

What could happen?

```text
____________________________________

____________________________________
```

What safer steps should have been considered?

```text
____________________________________

____________________________________
```

Think about:

```text
Planning

Pilot Groups

Report-Only

Monitoring

Emergency Access
```

---

# 👑 Part 8 — Explore Microsoft Entra Roles

Locate:

```text
Roles & admins
```

Browse the role list.

Do not assign anything.

Look for roles such as:

```text
Global Administrator

User Administrator

Groups Administrator

Authentication Administrator

Application Administrator
```

---

# 🧠 Role Challenge

A technician only needs approved user-management capabilities.

Which approach better follows least privilege?

```text
A. Global Administrator

B. An appropriate limited user-management role
```

Answer:

```text
______________________________
```

Why?

```text
____________________________________

____________________________________
```

---

# ☁️ Part 9 — Explore Azure RBAC

If you have authorized access to the Azure portal, open:

```text
https://portal.azure.com
```

Select an Azure resource, resource group, or subscription that you are permitted to view.

Look for:

```text
Access control (IAM)
```

Do not create or remove a role assignment.

If you do not have Azure access, complete this section conceptually.

---

# 🧩 Part 10 — RBAC Components

An Azure role assignment combines:

```text
WHO
+
WHAT ROLE
+
WHERE
```

Microsoft terminology:

```text
Security Principal
+
Role Definition
+
Scope
```

Match them:

| Question | RBAC Component |
|---|---|
| Who receives access? | __________________________ |
| What permissions are provided? | __________________________ |
| Where do they apply? | __________________________ |

---

# 📋 Part 11 — Explore Azure Roles

If visible, look for examples such as:

```text
Reader

Contributor

Owner
```

At a high level:

```text
Reader
=
View
```

```text
Contributor
=
Manage resources
but not grant Azure RBAC access
```

```text
Owner
=
Broad management
+
Can assign Azure RBAC roles
```

---

# 🎯 Part 12 — Explore Scope

Look at the resource hierarchy concept:

```text
Management Group
      ↓
Subscription
      ↓
Resource Group
      ↓
Resource
```

A role assigned at a broader scope can affect resources beneath that scope.

This is why scope matters.

---

# 🧠 Scope Scenario

Taylor needs to view one Azure virtual machine.

Which design follows least privilege better?

```text
A.
Owner at Subscription Scope
```

or:

```text
B.
Appropriate read-only role
at the narrow required scope
```

Answer:

```text
______________________________
```

Explain:

```text
____________________________________

____________________________________
```

---

# 🟡 Part 13 — Conditional Access Scenarios

For each scenario, design a simple policy idea.

Do not build these in production.

---

## Scenario 1 — Administrator Access

Administrators access sensitive Microsoft cloud administration tools.

Possible design:

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONTROL:
____________________________________
```

Think about strong or phishing-resistant authentication.

---

## Scenario 2 — HR Application

HR employees access sensitive employee information.

Contoso wants access only from appropriately managed devices.

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONTROL:
____________________________________
```

---

## Scenario 3 — Suspicious Sign-In

A supported risk signal indicates a high-risk sign-in.

```text
SIGNAL:
____________________________________

CONTROL:
____________________________________
```

---

## Scenario 4 — External Contractor

An external contractor needs access to one cloud application but should not receive broad access.

Which principles apply?

```text
____________________________________

____________________________________
```

---

# 🟡 Part 14 — RBAC Scenarios

Choose the better design.

---

## Scenario 1

Jamie needs to view Azure resources but should not modify them.

```text
Reader / Contributor / Owner
```

Answer:

```text
______________________________
```

---

## Scenario 2

A technician needs to manage one resource group but does not need control over the entire subscription.

Better scope:

```text
Subscription / Resource Group
```

Answer:

```text
______________________________
```

---

## Scenario 3

A help desk employee needs identity-management capabilities but does not need unrestricted control over the tenant.

Better approach:

```text
Global Administrator

or

Appropriate Limited Microsoft Entra Role
```

Answer:

```text
______________________________
```

---

# 🔐 Part 15 — Authentication, Conditional Access, or RBAC?

Choose:

```text
Authentication

Conditional Access

RBAC
```

## Scenario 1

Determine whether the person is really Alex.

```text
______________________________
```

## Scenario 2

Require MFA because Alex is accessing a sensitive application.

```text
______________________________
```

## Scenario 3

Determine whether Alex can modify an Azure virtual machine.

```text
______________________________
```

## Scenario 4

Require a compliant device before accessing HR data.

```text
______________________________
```

## Scenario 5

Give Morgan permission to view but not modify an Azure resource.

```text
______________________________
```

---

# 🧱 Part 16 — Build a Zero Trust Access Flow

Complete this design:

```text
USER REQUESTS ACCESS
        ↓
____________________
Verify Identity
        ↓
____________________
Evaluate Conditions
        ↓
____________________
Determine Allowed Actions
        ↓
RESOURCE
```

Choices:

```text
Authentication

Conditional Access

RBAC
```

---

# 🏢 Part 17 — Contoso Challenge

Contoso has:

```text
150 Employees

10 IT Administrators

20 Remote Employees

5 Contractors

Sensitive HR Data

Azure Resources
```

Design five high-level controls.

Example categories:

```text
Authentication

Conditional Access

Administrative Roles

Azure RBAC

External Access
```

Your design:

```text
1. ____________________________________

2. ____________________________________

3. ____________________________________

4. ____________________________________

5. ____________________________________
```

Try to apply:

```text
Verify Explicitly

Use Least Privilege

Assume Breach
```

---

# 🗺️ Part 18 — Build Your Access Control Map

Complete:

| Technology | Main Question |
|---|---|
| Authentication | __________________________ |
| Conditional Access | __________________________ |
| Microsoft Entra Roles | __________________________ |
| Azure RBAC | __________________________ |
| Scope | __________________________ |
| PIM | __________________________ |

---

# ✅ Suggested Answers

## Report-Only

```text
Report-only lets administrators
evaluate how a policy would behave
before enforcing it.
```

---

## Lockout Scenario

The policy could block legitimate users and administrators from accessing resources.

Safer planning can include:

```text
Pilot Users

Report-Only Mode

Monitoring

Careful Scope

Emergency Access Planning
```

---

## Entra Role Challenge

```text
B — Appropriate limited role
```

Reason:

```text
Least Privilege
```

---

## RBAC Components

```text
Who?
=
Security Principal

What permissions?
=
Role Definition

Where?
=
Scope
```

---

## Scope Scenario

```text
B — Appropriate read-only role
at the narrow required scope
```

---

## RBAC Scenarios

```text
Scenario 1
=
Reader

Scenario 2
=
Resource Group

Scenario 3
=
Appropriate Limited Microsoft Entra Role
```

---

## Authentication / Conditional Access / RBAC

```text
Scenario 1
=
Authentication

Scenario 2
=
Conditional Access

Scenario 3
=
RBAC

Scenario 4
=
Conditional Access

Scenario 5
=
RBAC
```

---

## Zero Trust Access Flow

```text
USER REQUESTS ACCESS
        ↓
AUTHENTICATION
Verify Identity
        ↓
CONDITIONAL ACCESS
Evaluate Conditions
        ↓
RBAC
Determine Allowed Actions
        ↓
RESOURCE
```

---

# 🎓 What You Should Have Learned

You should now understand:

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

and:

```text
LEAST PRIVILEGE
=
Minimum permissions
+
Appropriate scope
+
Only as needed
```

---

# ✅ Lab Completion Checklist

Before marking this lab complete, make sure you can answer:

- [ ] What is Conditional Access?
- [ ] What are Conditional Access signals?
- [ ] What are access controls?
- [ ] What is report-only mode?
- [ ] Why can a poorly designed Conditional Access policy be dangerous?
- [ ] What is RBAC?
- [ ] What is a Microsoft Entra role?
- [ ] What is Azure RBAC?
- [ ] What is a security principal?
- [ ] What is a role definition?
- [ ] What is scope?
- [ ] What is least privilege?
- [ ] How are authentication, Conditional Access, and RBAC different?

If you can answer these, Lab 07 is complete.

---

# ➡️ Next

Continue to:

## 📘 Lesson 08 — Identity Governance & Protection

Lesson 08 completes the Microsoft Entra section of the course.

After Lesson 08 and Lab 08, complete:

## 🏗️ Project 01 — Secure an Organization's Identity Environment

This will combine the concepts from Lessons 01–08 into a larger identity-security scenario.

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [Conditional Access Overview](https://learn.microsoft.com/en-us/entra/identity/conditional-access/overview)
- [Microsoft Entra Built-in Roles](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference)
- [Azure RBAC Overview](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview)
- [Azure RBAC Scope](https://learn.microsoft.com/en-us/azure/role-based-access-control/scope-overview)

---

# 📚 Course Navigation

⬅️ **[Lesson 07 — Conditional Access & RBAC](../lessons/%F0%9F%93%98%20Lesson%2007%20%E2%80%94%20Conditional%20Access%20&%20RBAC.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
