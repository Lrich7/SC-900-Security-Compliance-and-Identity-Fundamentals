# 🏗️ Project 01 — Secure an Organization's Identity Environment

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Project:** 01  
**Covers:** Lessons 01–08  
**Difficulty:** Beginner / Intermediate  
**Project Type:** Architecture & Security Design Challenge

---

# 🎯 Project Goal

You are the IT security administrator for a fictional company.

Your job is to design a Microsoft identity-security strategy using concepts from Lessons 01–08.

You will apply:

```text
Security Concepts

Zero Trust

Microsoft Entra ID

Users & Groups

MFA

Passwordless Authentication

Conditional Access

RBAC

Identity Protection

Identity Governance
```

This is not a portal configuration lab.

The goal is to demonstrate that you understand **which Microsoft identity capabilities should be used and why**.

---

# 🏢 Company Scenario — Contoso Manufacturing

Contoso Manufacturing is a growing company with:

```text
150 Employees

10 IT Administrators

20 Remote Employees

15 Contractors

3 Offices

Microsoft 365

Azure Resources

HR Application

Accounting Application

SharePoint

Microsoft Teams
```

Contoso uses Microsoft Entra ID for cloud identity.

---

# 🚨 Current Problems

An internal review discovers:

```text
1. Most users sign in with passwords only.

2. Several IT employees have permanent
   Global Administrator access.

3. Contractors remain in groups
   after projects end.

4. Employees who transfer departments
   often keep their old access.

5. Administrators can access sensitive
   resources from unmanaged devices.

6. There is no standard Conditional
   Access strategy.

7. Suspicious sign-ins are not
   consistently reviewed.

8. Access is often assigned directly
   to individual users.

9. The company wants to reduce
   dependence on passwords.

10. New employees need a more
    consistent onboarding process.
```

Your task is to improve the environment.

---

# 🧠 Project Rules

You do not need to create anything in a real Microsoft tenant.

Design the solution on paper or directly in this Markdown file.

Your answers should focus on:

```text
WHAT would you use?

WHY would you use it?

WHAT problem does it solve?
```

Avoid simply listing Microsoft product names.

Explain your reasoning.

---

# 🧩 Phase 1 — Identify the Security Principles

Review the problems above.

Choose where these Zero Trust principles apply:

```text
Verify Explicitly

Use Least Privilege

Assume Breach
```

Complete:

## Verify Explicitly

Which Contoso problems relate to verifying access requests more strongly?

```text
____________________________________

____________________________________

____________________________________
```

## Use Least Privilege

Which problems involve excessive access?

```text
____________________________________

____________________________________

____________________________________
```

## Assume Breach

What controls could limit damage if an account is compromised?

```text
____________________________________

____________________________________

____________________________________
```

---

# 👤 Phase 2 — Users and Groups

Contoso currently assigns many permissions directly to users.

Design a basic group strategy.

Departments:

```text
Accounting

Human Resources

Sales

IT
```

Create group names:

| Department | Proposed Security Group |
|---|---|
| Accounting | __________________________ |
| Human Resources | __________________________ |
| Sales | __________________________ |
| IT | __________________________ |

---

# 🧠 Group Design Question

Why is this generally easier to manage?

```text
USER
  ↓
GROUP
  ↓
RESOURCE
```

instead of:

```text
USER
  ↓
INDIVIDUAL RESOURCE PERMISSIONS
```

Answer:

```text
____________________________________

____________________________________
```

---

# 🌎 Phase 3 — Contractor Access

Contoso hires contractors for temporary projects.

Contractors need:

```text
Microsoft Teams

Project SharePoint Site

One Project Application
```

They do **not** need broad internal access.

Design the approach.

### Identity Type

```text
Member / Guest / Other
```

Answer:

```text
______________________________
```

### Access Method

Would you use:

```text
Individual Permissions

Security Groups

Access Package

Combination
```

Answer:

```text
______________________________
```

### Access Expiration

How would you prevent contractor access from lasting forever?

```text
____________________________________

____________________________________
```

---

# 🔐 Phase 4 — Authentication Strategy

Contoso currently uses passwords for most employees.

Design an improved authentication strategy for:

## Normal Employees

```text
Authentication approach:
____________________________________

Reason:
____________________________________
```

## IT Administrators

```text
Authentication approach:
____________________________________

Reason:
____________________________________
```

## Contractors

```text
Authentication approach:
____________________________________

Reason:
____________________________________
```

---

# 📱 Phase 5 — MFA

Contoso asks:

> Why can't we just require stronger passwords?

Write a short answer:

```text
____________________________________

____________________________________

____________________________________
```

Your answer should mention why passwords alone can still be compromised.

---

# 🔑 Phase 6 — Passwordless Strategy

Contoso wants to begin moving toward passwordless authentication.

Choose appropriate technologies.

Options include:

```text
Passkeys / FIDO2

Windows Hello for Business

Microsoft Authenticator

Temporary Access Pass
```

## Windows Employees

Recommended method:

```text
______________________________
```

## Privileged Administrators

Recommended strong method:

```text
______________________________
```

## New Employee Registration

Recommended temporary bootstrap method:

```text
______________________________
```

---

# 🚦 Phase 7 — Conditional Access Design

Design four high-level Conditional Access policies.

Do not worry about exact portal configuration.

Use:

```text
WHO

RESOURCE

CONDITION

CONTROL
```

---

## Policy 1 — Administrators

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONDITION:
____________________________________

CONTROL:
____________________________________
```

---

## Policy 2 — HR Application

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONDITION:
____________________________________

CONTROL:
____________________________________
```

---

## Policy 3 — Contractors

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONDITION:
____________________________________

CONTROL:
____________________________________
```

---

## Policy 4 — Risky Sign-In

```text
WHO:
____________________________________

RESOURCE:
____________________________________

CONDITION:
____________________________________

CONTROL:
____________________________________
```

---

# ⚠️ Phase 8 — Safe Conditional Access Deployment

Put these steps in a sensible order:

```text
Monitor

Design Policy

Pilot

Enable Report-Only

Expand Enforcement
```

Your order:

```text
1. __________________________

2. __________________________

3. __________________________

4. __________________________

5. __________________________
```

Why is immediately enabling a new policy for every user risky?

```text
____________________________________

____________________________________
```

---

# 👑 Phase 9 — Administrative Roles

Current situation:

```text
10 IT Administrators
      ↓
6 Have Global Administrator
```

Not all six need full tenant control.

Design a better approach.

Consider:

```text
User Administrator

Groups Administrator

Authentication Administrator

Other Task-Specific Roles

PIM
```

Write your recommendation:

```text
____________________________________

____________________________________

____________________________________
```

---

# ☁️ Phase 10 — Azure RBAC

Contoso has an Azure technician named Taylor.

Taylor needs to manage virtual machines in:

```text
Resource Group:
RG-Field-Servers
```

Taylor does not need access to every Azure resource.

Which approach is better?

```text
A.

Owner
at Subscription Scope
```

or:

```text
B.

Appropriate VM/resource-management role
at RG-Field-Servers scope
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

# 🛡️ Phase 11 — Identity Protection

Contoso wants to identify suspicious identity activity.

Which Microsoft capability should be considered?

```text
______________________________
```

What is the difference between:

```text
User Risk

and

Sign-In Risk?
```

Answer:

```text
____________________________________

____________________________________
```

---

# ⏱️ Phase 12 — Privileged Identity Management

Contoso administrators currently have permanent privileged access.

Redesign the approach using PIM.

Complete:

```text
Administrator
      ↓
______________________________
      ↓
Needs Privileged Task
      ↓
______________________________
      ↓
MFA / Approval / Justification
      ↓
Temporary Active Role
      ↓
______________________________
```

---

# 🔍 Phase 13 — Access Reviews

Contoso has 15 contractors.

Nobody remembers which contractors still need access.

Design an access review process.

### Who should be reviewed?

```text
____________________________________
```

### How often?

Choose a reasonable interval:

```text
Monthly / Quarterly / Other
```

Answer:

```text
______________________________
```

### What happens if access is no longer needed?

```text
____________________________________
```

---

# 📦 Phase 14 — Entitlement Management

Contoso repeatedly gives project contractors the same resources:

```text
Project Team

Project SharePoint Site

Project Application
```

Design an access package.

### Package Name

```text
____________________________________
```

### Resources

```text
1. _________________________________

2. _________________________________

3. _________________________________
```

### Approval Required?

```text
YES / NO
```

### Should Access Expire?

```text
YES / NO
```

Explain:

```text
____________________________________
```

---

# 🔄 Phase 15 — Joiner, Mover, Leaver

Design a basic identity lifecycle.

## Joiner

New employee starts Monday.

Identity actions:

```text
____________________________________

____________________________________
```

## Mover

Employee transfers from Accounting to HR.

Identity actions:

```text
____________________________________

____________________________________
```

## Leaver

Employee leaves the company.

Identity actions:

```text
____________________________________

____________________________________
```

---

# 🧱 Phase 16 — Build the Final Identity Architecture

Complete the architecture.

```text
                    USERS
                      │
                      ▼
              MICROSOFT ENTRA ID
                      │
          ┌───────────┼───────────┐
          │           │           │
          ▼           ▼           ▼
       GROUPS   AUTHENTICATION   GUESTS
          │           │           │
          │           ▼           │
          │      MFA / PASSWORDLESS
          │           │           │
          └───────────┼───────────┘
                      ▼
              CONDITIONAL ACCESS
                      │
                      ▼
              ACCESS DECISION
                      │
          ┌───────────┴───────────┐
          ▼                       ▼
     ENTRA ROLES               AZURE RBAC
          │                       │
          └───────────┬───────────┘
                      ▼
              LEAST PRIVILEGE
                      │
          ┌───────────┼────────────┐
          ▼           ▼            ▼
   ID PROTECTION     PIM      ACCESS REVIEWS
                      │
                      ▼
             IDENTITY GOVERNANCE
```

In your own words, explain how these technologies work together:

```text
____________________________________

____________________________________

____________________________________

____________________________________
```

---

# 🎯 Phase 17 — Executive Summary

Your manager does not want technical details.

Write a short 5–8 sentence explanation of your proposed identity strategy.

Include:

```text
MFA / Passwordless

Conditional Access

Least Privilege

PIM

Identity Protection

Governance
```

Your executive summary:

```text
____________________________________

____________________________________

____________________________________

____________________________________

____________________________________

____________________________________
```

---

# 🧠 Phase 18 — Technology Selection Challenge

Choose the best technology.

Options:

```text
Microsoft Entra ID

MFA

Passkey / FIDO2

Conditional Access

Microsoft Entra Role

Azure RBAC

Identity Protection

PIM

Access Reviews

Entitlement Management

Lifecycle Workflows
```

## 1. Detect suspicious sign-ins

```text
______________________________
```

## 2. Give temporary privileged access

```text
______________________________
```

## 3. Require MFA when accessing a sensitive application

```text
______________________________
```

## 4. Determine who can manage an Azure resource

```text
______________________________
```

## 5. Periodically verify contractor access

```text
______________________________
```

## 6. Provide a governed bundle of project resources

```text
______________________________
```

## 7. Provide phishing-resistant authentication

```text
______________________________
```

## 8. Automate identity tasks when an employee leaves

```text
______________________________
```

## 9. Give a help desk worker limited identity administration capabilities

```text
______________________________
```

## 10. Store and manage cloud identities

```text
______________________________
```

---

# ✅ Suggested Solution

There can be multiple reasonable designs.

A strong solution would include concepts like:

## Users and Groups

```text
Use groups to manage access
instead of excessive direct assignments.
```

## Contractors

```text
Use external/guest identities,
governed groups or access packages,
expiration, and access reviews.
```

## Authentication

```text
Require strong authentication.

Move toward passwordless and
phishing-resistant methods,
especially for administrators.
```

## Conditional Access

```text
Use policies to apply requirements
based on identity, resource,
device, and risk.
```

## Roles

```text
Replace unnecessary Global Administrator
assignments with task-specific roles.
```

## Azure RBAC

```text
Assign the appropriate role
at the narrowest practical scope.
```

## PIM

```text
Use eligible/time-limited privileged access
rather than unnecessary permanent privilege.
```

## Identity Protection

```text
Use identity risk information
to help identify suspicious activity.
```

## Governance

```text
Review access regularly,
govern temporary access,
and automate lifecycle processes.
```

---

# ✅ Technology Selection Answers

```text
1. Identity Protection

2. PIM

3. Conditional Access

4. Azure RBAC

5. Access Reviews

6. Entitlement Management

7. Passkey / FIDO2

8. Lifecycle Workflows

9. Appropriate Microsoft Entra Role

10. Microsoft Entra ID
```

---

# 🏆 Project Completion Checklist

You should be able to explain:

- [ ] Zero Trust principles
- [ ] Microsoft Entra ID
- [ ] Users and groups
- [ ] Member and guest identities
- [ ] MFA
- [ ] Passwordless authentication
- [ ] Passkeys / FIDO2
- [ ] Conditional Access
- [ ] Microsoft Entra roles
- [ ] Azure RBAC
- [ ] Least privilege
- [ ] Identity Protection
- [ ] User risk
- [ ] Sign-in risk
- [ ] PIM
- [ ] Access Reviews
- [ ] Entitlement Management
- [ ] Lifecycle Workflows

If you can explain **why** you selected each technology, you have completed Project 01.

---

# 🎓 Project Outcome

You have designed an identity environment based on:

```text
VERIFY EXPLICITLY

USE LEAST PRIVILEGE

ASSUME BREACH
```

You have also completed the first major section of the SC-900 course:

# Microsoft Entra — Identity & Access

---

# ➡️ Next

Continue to:

## 📘 Lesson 09 — Azure Infrastructure Security

The next section shifts from identity to Microsoft's broader security solutions.

You will begin exploring how Microsoft protects:

```text
Networks

Cloud Resources

Servers

Applications

Security Posture
```

---

# 📚 Project Navigation

⬅️ **[Lesson 08 — Identity Governance & Protection](../lessons/%F0%9F%93%98%20Lesson%2008%20%E2%80%94%20Identity%20Governance%20&%20Protection.md)**

🧪 **[Lab 08](../labs/Lab%2008%20—%20Explore%20Identity%20Governance%20&%20Protection.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](README.md)**

🏠 **[Return to Main README](../README.md)**
