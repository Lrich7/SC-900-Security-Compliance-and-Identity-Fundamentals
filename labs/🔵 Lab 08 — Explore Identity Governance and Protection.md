# 🔵🟡 Lab 08 — Explore Identity Governance & Protection

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 08 — Identity Governance & Protection  
**Lab Type:** 🔵 Explore the Tool + 🟡 Scenario  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Locate Microsoft Entra ID Protection
- Recognize risky users, risky sign-ins, and risk detections
- Locate Microsoft Entra ID Governance
- Locate Privileged Identity Management
- Locate access reviews
- Locate entitlement management
- Recognize access packages
- Locate lifecycle workflows
- Match governance tools to business scenarios
- Explain how governance supports Zero Trust

---

# ⚠️ Production Safety

This is a read-only lab.

Do not:

```text
Dismiss Risk

Confirm Compromise

Change Risk Policies

Activate Privileged Roles

Create Access Reviews

Create Access Packages

Modify Lifecycle Workflows

Change User Access
```

unless specifically authorized in a safe environment.

Some features require specific Microsoft Entra licensing or administrative permissions.

If a page is unavailable, complete the conceptual exercise and continue.

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

# 🛡️ Part 2 — Find Identity Protection

Locate:

```text
Identity Protection
```

Look for areas related to:

```text
Risky Users

Risky Sign-Ins

Risk Detections
```

Do not take action on any real alert or user as part of this lab.

---

# 🧠 Part 3 — User Risk or Sign-In Risk?

Classify each.

## Scenario 1

Microsoft security signals suggest Alex's identity may have been compromised.

```text
User Risk / Sign-In Risk
```

Answer:

```text
______________________________
```

## Scenario 2

A specific authentication attempt appears suspicious.

```text
User Risk / Sign-In Risk
```

Answer:

```text
______________________________
```

---

# 🔎 Part 4 — Risk Investigation

If your permissions allow, inspect the types of information available on a risk page.

Do not record real names, IP addresses, locations, or other company information in public notes.

Instead, identify categories of information you can see.

```text
[ ] Risk Level

[ ] Risk State

[ ] Sign-In Information

[ ] Detection Information

[ ] Date / Time

[ ] Other
```

---

# 🚦 Part 5 — Risk Response Scenario

Contoso detects a suspicious sign-in for an employee.

Which responses might make sense depending on policy and investigation?

```text
[ ] Investigate the sign-in

[ ] Require stronger authentication

[ ] Block access when appropriate

[ ] Ignore every risk alert automatically
```

Explain:

```text
____________________________________

____________________________________
```

---

# 🏛️ Part 6 — Find Identity Governance

Locate:

```text
Identity Governance
```

Look for capabilities such as:

```text
Privileged Identity Management

Access Reviews

Entitlement Management

Lifecycle Workflows
```

Available features depend on licensing and permissions.

---

# 👑 Part 7 — Explore PIM

Locate:

```text
Privileged Identity Management
```

Do not activate or change any role.

Look for concepts such as:

```text
Eligible Roles

Active Roles

Assignments

Activation
```

---

# ⏱️ PIM Scenario

Jordan occasionally needs privileged administrative access.

Compare:

```text
OPTION A

Jordan has permanent
Global Administrator access
24/7
```

with:

```text
OPTION B

Jordan is eligible for
an appropriate privileged role

Jordan activates it
only when needed
```

Which better supports least privilege?

```text
______________________________
```

Why?

```text
____________________________________

____________________________________
```

---

# 🔐 Part 8 — PIM Controls

Which controls could make privileged activation safer?

```text
[ ] MFA

[ ] Approval

[ ] Justification

[ ] Limited Duration

[ ] Permanent unrestricted access for everyone
```

---

# 🔍 Part 9 — Explore Access Reviews

Locate:

```text
Access Reviews
```

Do not create one.

Think about what an access review asks:

```text
DOES THIS IDENTITY
STILL NEED THIS ACCESS?
```

---

# 🌎 Contractor Scenario

Contoso gave 20 contractors access to a project.

The project ends.

What should happen?

```text
____________________________________

____________________________________
```

Which governance feature fits best?

```text
______________________________
```

---

# 📦 Part 10 — Explore Entitlement Management

Locate:

```text
Entitlement Management
```

Look for:

```text
Access Packages

Catalogs

Requests

Assignments
```

Do not create anything.

---

# 📦 Access Package Scenario

A new contractor needs:

```text
Project Team Membership

Project SharePoint Access

Project Application Access
```

Instead of granting each item separately, what could an organization use?

```text
______________________________
```

What could happen when the assignment expires?

```text
____________________________________
```

---

# 🔄 Part 11 — Explore Lifecycle Workflows

Locate:

```text
Lifecycle Workflows
```

Do not create or run a workflow.

Think about:

```text
JOINER

MOVER

LEAVER
```

---

# 🧠 Lifecycle Scenario

Taylor leaves Contoso on Friday.

Which type of identity process applies?

```text
Joiner / Mover / Leaver
```

Answer:

```text
______________________________
```

Why can automation help?

```text
____________________________________

____________________________________
```

---

# 🧩 Part 12 — Match the Tool

Choose:

```text
Identity Protection

PIM

Access Reviews

Entitlement Management

Lifecycle Workflows
```

## Scenario 1

Detect a suspicious authentication attempt.

```text
______________________________
```

## Scenario 2

Give an administrator temporary privileged access.

```text
______________________________
```

## Scenario 3

Verify every quarter that contractors still need access.

```text
______________________________
```

## Scenario 4

Provide a governed package of resources to a project member.

```text
______________________________
```

## Scenario 5

Automate tasks when an employee leaves.

```text
______________________________
```

---

# 🛡️ Part 13 — Zero Trust Mapping

Match each feature to the Zero Trust principle it most strongly supports.

Choices:

```text
Verify Explicitly

Use Least Privilege

Assume Breach
```

| Feature | Principle |
|---|---|
| Identity risk signals | __________________ |
| PIM | __________________ |
| Access Reviews | __________________ |
| Removing stale access | __________________ |

Some controls support more than one principle.

---

# 🏢 Part 14 — Contoso Governance Challenge

Contoso has:

```text
150 Employees

10 Administrators

20 Contractors

Frequent Department Transfers

Microsoft 365

Azure Resources
```

Problems:

```text
Admins have permanent privileged roles

Old contractors still appear in groups

Employees keep access after changing departments

No regular access reviews

Suspicious sign-ins are difficult to prioritize
```

Choose a Microsoft Entra capability for each problem.

| Problem | Capability |
|---|---|
| Permanent privileged roles | __________________ |
| Old contractor access | __________________ |
| Department changes | __________________ |
| No periodic verification | __________________ |
| Suspicious identity activity | __________________ |

---

# 🗺️ Part 15 — Build Your Governance Map

Complete:

```text
Identity Protection
=
____________________________________
```

```text
PIM
=
____________________________________
```

```text
Access Reviews
=
____________________________________
```

```text
Entitlement Management
=
____________________________________
```

```text
Lifecycle Workflows
=
____________________________________
```

---

# ✅ Suggested Answers

## User Risk vs Sign-In Risk

```text
Scenario 1
=
User Risk

Scenario 2
=
Sign-In Risk
```

## PIM Scenario

```text
Option B
```

Temporary, controlled privileged access better supports least privilege than unnecessary permanent privilege.

## PIM Controls

```text
MFA

Approval

Justification

Limited Duration
```

## Contractor Scenario

Review the contractors' access and remove access that is no longer needed.

Best-fit capability:

```text
Access Reviews
```

## Access Package

```text
Entitlement Management / Access Package
```

Access can be governed and can expire according to the configured process.

## Lifecycle

```text
Leaver
```

Automation can make offboarding more consistent and reduce forgotten access.

## Match the Tool

```text
1. Identity Protection

2. PIM

3. Access Reviews

4. Entitlement Management

5. Lifecycle Workflows
```

## Contoso Challenge

```text
Permanent privileged roles
=
PIM

Old contractor access
=
Access Reviews

Department changes
=
Lifecycle Workflows / governed lifecycle processes

No periodic verification
=
Access Reviews

Suspicious identity activity
=
Identity Protection
```

---

# 🎓 What You Should Have Learned

You should now understand:

```text
PROTECTION
=
Is this identity activity risky?
```

and:

```text
GOVERNANCE
=
Should this identity have
this access now?
```

Together:

```text
IDENTITY SECURITY
=
VERIFY
+
LIMIT
+
REVIEW
+
REMOVE
```

---

# ✅ Lab Completion Checklist

- [ ] I can explain user risk.
- [ ] I can explain sign-in risk.
- [ ] I know what Identity Protection does.
- [ ] I know what PIM does.
- [ ] I know what an access review does.
- [ ] I know what an access package is.
- [ ] I know what entitlement management does.
- [ ] I know what lifecycle workflows do.
- [ ] I can connect governance to least privilege.
- [ ] I can choose the appropriate governance capability for a basic scenario.

---

# 🏗️ Next — Project 01

You have completed the Microsoft Entra lessons.

Now complete:

## 🏗️ Project 01 — Secure an Organization's Identity Environment

➡️ **[Open Project 01](../projects/Project%2001%20—%20Secure%20an%20Organization's%20Identity%20Environment.md)**

The project combines concepts from Lessons 01–08.

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [Microsoft Entra ID Protection](https://learn.microsoft.com/en-us/entra/id-protection/overview-identity-protection)
- [Microsoft Entra ID Governance](https://learn.microsoft.com/en-us/entra/id-governance/identity-governance-overview)
- [Privileged Identity Management](https://learn.microsoft.com/en-us/entra/id-governance/privileged-identity-management/pim-configure)
- [Access Reviews](https://learn.microsoft.com/en-us/entra/id-governance/access-reviews-overview)
- [Entitlement Management](https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-overview)

---

# 📚 Course Navigation

⬅️ **[Lesson 08 — Identity Governance & Protection](../lessons/%F0%9F%93%98%20Lesson%2008%20%E2%80%94%20Identity%20Governance%20&%20Protection.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
