# 🔵 Lab 03 — Explore Microsoft Entra ID

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 03 — Microsoft Entra ID & Identity Types  
**Lab Type:** 🔵 Explore the Tool  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Open the Microsoft Entra admin center
- Identify your Microsoft Entra tenant
- Locate users
- Locate groups
- Locate devices
- Locate applications
- Locate administrative roles
- Locate authentication methods
- Locate Conditional Access
- Recognize Identity Protection and governance areas
- Connect Microsoft Entra terminology with the actual administrative portal

---

# 🧪 Lab Philosophy

This is an:

# 🔵 Explore the Tool Lab

You are **not** being asked to configure your production environment.

The goal is:

```text
OPEN THE TOOL
      ↓
FIND THE FEATURE
      ↓
UNDERSTAND ITS PURPOSE
      ↓
CONNECT IT TO SC-900
```

If you are using a company tenant, do not change settings unless you are authorized to do so.

---

# ⚠️ Before You Begin

Microsoft Entra environments vary based on:

```text
Licensing

Administrative Role

Tenant Configuration

Microsoft Portal Updates
```

You may not see every feature described in this lab.

That is okay.

For SC-900, understanding what the feature does is more important than having access to every configuration page.

---

# 📋 What You Need

Ideally:

- A Microsoft work or school account
- Access to the Microsoft Entra admin center
- Permission to view basic tenant information

You do **not** need to be a Global Administrator to learn from this lab.

Some areas may be unavailable based on your account permissions.

---

# 🚀 Part 1 — Open Microsoft Entra

Open:

**Microsoft Entra admin center**

```text
https://entra.microsoft.com
```

Sign in using your authorized work, school, or lab account.

Do not use someone else's credentials.

---

# 👀 First Look

Before clicking anything, look at the portal.

Try to identify:

```text
Tenant / Organization

Microsoft Entra ID

Users

Groups

Devices

Applications

Roles

Protection / Governance Features
```

Microsoft periodically updates the portal, so the exact navigation layout may change.

---

# 🏢 Part 2 — Identify the Tenant

Find the area showing information about your Microsoft Entra environment.

Look for items such as:

```text
Tenant Name

Tenant ID

Primary Domain
```

You do not need to copy sensitive identifiers into this lab.

Instead, answer:

### What is a tenant?

```text
____________________________________

____________________________________
```

### What kinds of objects are stored or represented in the directory?

```text
____________________________________

____________________________________
```

Suggested examples:

```text
Users

Groups

Devices

Applications
```

---

# 👤 Part 3 — Explore Users

Navigate to the user area.

A common path is:

```text
Entra ID
   ↓
Users
   ↓
All users
```

Do **not** create, delete, disable, or modify a production user.

Look at the columns and information available.

You may see items such as:

```text
Display Name

User Principal Name

User Type

Account Status
```

---

# 🧠 Think About It

A user object represents:

```text
A HUMAN IDENTITY
```

Examples include:

```text
Employee

Administrator

Guest

Contractor
```

Write one reason Microsoft Entra needs user identities:

```text
____________________________________

____________________________________
```

---

# 👥 Part 4 — Explore Groups

Navigate to:

```text
Entra ID
   ↓
Groups
   ↓
All groups
```

Look at the groups without changing membership.

Groups can help administrators manage access for multiple identities.

Instead of:

```text
Give Alice Access

Give Bob Access

Give Chris Access

Give Dana Access
```

an organization may use:

```text
Accounting Group
       ↓
Accounting Resource
```

Users are added to the appropriate group and access can be managed more consistently.

---

# 🔎 Observe

Look for information such as:

```text
Group Name

Group Type

Membership Type
```

Do not worry if your tenant does not use every group type.

### Why might groups be easier than assigning access individually?

```text
____________________________________

____________________________________
```

---

# 💻 Part 5 — Explore Devices

Navigate to the devices area.

A common path is:

```text
Entra ID
   ↓
Devices
   ↓
All devices
```

Look for device objects.

Depending on your environment, you may see:

```text
Windows Computers

Mobile Devices

Tablets

Other Registered Devices
```

---

# 🧠 Device Identity

Remember:

```text
USER IDENTITY
=
Who is requesting access?


DEVICE IDENTITY
=
What device is being used?
```

A device identity can provide information used in access and management decisions.

Look for fields related to:

```text
Join Type

Operating System

Compliance

Ownership

Registration
```

The exact columns available may vary.

---

# 🔎 Identify the Join Type

If your environment contains devices, see whether you can find examples of:

```text
Microsoft Entra Registered

Microsoft Entra Joined

Microsoft Entra Hybrid Joined
```

Do not worry if all three are not present.

### Which type might commonly appear for a personal/BYOD device?

```text
____________________________________
```

### Which type might commonly appear for a cloud-managed corporate Windows device?

```text
____________________________________
```

---

# 📦 Part 6 — Explore Applications

Locate the applications area.

Look for areas such as:

```text
Enterprise Applications

App Registrations
```

Do not create or modify an application.

At a fundamentals level:

```text
Enterprise Application
        ↓
Application used within the tenant
```

and applications can have identities and permissions.

This connects to:

```text
WORKLOAD IDENTITIES
```

from Lesson 03.

---

# ⚙️ Workload Identity Review

Imagine an automated service needs access to a cloud resource.

Instead of using:

```text
employee@example.com
+
Employee Password
```

the application can use an appropriate workload identity.

Why is that better?

```text
____________________________________

____________________________________
```

Think about:

```text
Accountability

Least Privilege

Credential Management

Automation
```

---

# 🛡️ Part 7 — Explore Roles & Admins

Find:

```text
Roles & admins
```

Browse the available Microsoft Entra roles.

Do **not** assign yourself or anyone else a role.

You may recognize roles such as:

```text
Global Administrator

User Administrator

Groups Administrator

Authentication Administrator
```

---

# 🧠 Least Privilege Connection

From Lesson 02:

> Give identities only the access necessary to perform their work.

Suppose someone only needs to manage users.

Which approach better follows least privilege?

```text
A. Global Administrator

B. A more limited user-management role
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

# 🔐 Part 8 — Find Authentication Methods

Locate the authentication area.

Depending on the current portal layout, look for:

```text
Authentication methods
```

You may encounter methods or policies related to:

```text
Microsoft Authenticator

Passkeys / FIDO2

Temporary Access Pass

SMS

Voice

Windows Hello for Business
```

Do not change authentication policies.

We will study authentication in more detail in:

> **Lesson 05 — Authentication & Multifactor Authentication**

and passwordless methods in Lesson 06.

---

# 🚦 Part 9 — Find Conditional Access

Locate:

```text
Conditional Access
```

Do not create or modify a production policy.

For now, remember:

```text
SIGNALS
   ↓
POLICY
   ↓
ACCESS DECISION
```

Conditional Access helps organizations apply access policies based on signals and conditions.

Examples might involve:

```text
User

Group

Device

Location

Risk

Application
```

We will explore this properly in Lesson 07.

---

# 🛡️ Part 10 — Find Identity Protection

Look for:

```text
Identity Protection
```

Depending on licensing and permissions, you may see areas related to:

```text
Risky Users

Risky Sign-ins

Risk Detections
```

Do not worry if these features are unavailable in your tenant.

At a high level:

```text
IDENTITY PROTECTION
=
Detect and respond to identity-related risk
```

---

# 🏛️ Part 11 — Find Identity Governance

Look for identity governance features.

You may encounter:

```text
Privileged Identity Management

Access Reviews

Entitlement Management

Lifecycle Workflows
```

Some capabilities require additional licensing.

At a high level:

```text
IDENTITY GOVERNANCE
=
Make sure the right identities
have the right access
for the right reasons
and for the appropriate time
```

We will return to these features in Lesson 08.

---

# 🌎 Part 12 — Find External Identities

Look for an area related to:

```text
External Identities
```

Depending on your portal and permissions, you may see options related to external collaboration.

Think about:

```text
Partners

Guests

Contractors

Customers
```

### Why might an organization need external identities?

```text
____________________________________

____________________________________
```

---

# 🤖 Part 13 — Look for Workload or Agent Identity Areas

Microsoft Entra continues to expand support for non-human identities.

Depending on your tenant, licensing, and current portal experience, you may see references to:

```text
Workload Identities

Managed Identities

Enterprise Applications

Service Principals

Agents / Agent Identities
```

Do not worry if you cannot access or locate every item.

The SC-900 concept is more important:

```text
PEOPLE need identities

DEVICES need identities

SOFTWARE may need identities

AI AGENTS may need identities
```

---

# 🗺️ Part 14 — Build Your Entra Map

Complete this table from what you observed.

| Portal Area | What Does It Manage? |
|---|---|
| Users | __________________________ |
| Groups | __________________________ |
| Devices | __________________________ |
| Enterprise Applications | __________________________ |
| Roles & Admins | __________________________ |
| Authentication Methods | __________________________ |
| Conditional Access | __________________________ |
| Identity Protection | __________________________ |
| Identity Governance | __________________________ |

---

# 🧠 Part 15 — Match the Identity

Match each scenario with the best identity type.

Choices:

```text
Human Identity

External Identity

Device Identity

Workload Identity

Agent Identity
```

### Scenario 1

Maria is an employee in the Accounting department.

```text
Answer:
______________________________
```

### Scenario 2

A vendor is invited to collaborate on a project.

```text
Answer:
______________________________
```

### Scenario 3

A company-owned Windows laptop is registered in the organization's identity environment.

```text
Answer:
______________________________
```

### Scenario 4

An automated application needs access to Azure resources.

```text
Answer:
______________________________
```

### Scenario 5

An AI agent needs permission to access an organizational application.

```text
Answer:
______________________________
```

---

# 🔄 Part 16 — Cloud or Hybrid?

### Scenario A

A company creates employee accounts directly in Microsoft Entra ID and has no on-premises Active Directory.

```text
Cloud / Hybrid

Answer:
______________________________
```

### Scenario B

A company maintains users in on-premises Active Directory and synchronizes identities to Microsoft Entra ID.

```text
Cloud / Hybrid

Answer:
______________________________
```

---

# 🎯 Final Challenge

A new employee receives:

```text
Microsoft Entra User
       +
Company Laptop
       +
Microsoft 365 Access
```

Identify the identities involved.

### Employee

```text
______________________________
```

### Laptop

```text
______________________________
```

### Automated application used by the employee's department

```text
______________________________
```

Now imagine the employee signs in.

Microsoft Entra may eventually help evaluate:

```text
WHO?
        ↓
User Identity

WHAT DEVICE?
        ↓
Device Identity

HOW AUTHENTICATED?
        ↓
Authentication

WHAT ACCESS?
        ↓
Authorization / Access Policy
```

This is the foundation for the next several lessons.

---

# ✅ Suggested Answers

## Device Questions

Personal/BYOD devices commonly use:

```text
Microsoft Entra Registered
```

Cloud-managed organization-owned Windows devices commonly use:

```text
Microsoft Entra Joined
```

---

## Least Privilege

```text
B — A more limited user-management role
```

Giving only the permissions required reduces unnecessary administrative access.

---

## Match the Identity

```text
1. Human Identity

2. External Identity

3. Device Identity

4. Workload Identity

5. Agent Identity
```

---

## Cloud or Hybrid

```text
Scenario A
=
Cloud


Scenario B
=
Hybrid
```

---

## Final Challenge

```text
Employee
=
Human Identity


Laptop
=
Device Identity


Automated Application
=
Workload Identity
```

---

# 🎓 What You Should Have Learned

You should now be able to recognize:

```text
Microsoft Entra ID
=
Cloud identity and access management
```

and identify:

```text
Human Identities

External Identities

Device Identities

Workload Identities

Agent Identities

Hybrid Identities
```

You should also know where to begin looking for major identity and access features inside the Microsoft Entra admin center.

---

# ✅ Lab Completion Checklist

Before marking the lab complete, make sure you can answer:

- [ ] What is Microsoft Entra ID?
- [ ] What is a tenant?
- [ ] Where are users located?
- [ ] Where are groups located?
- [ ] Where are devices located?
- [ ] What is a device identity?
- [ ] What is a workload identity?
- [ ] What is an external identity?
- [ ] What is an agent identity?
- [ ] What does hybrid identity mean?
- [ ] Where are administrative roles located?
- [ ] Where would you look for Conditional Access?
- [ ] Why should you avoid making unnecessary changes while exploring a production tenant?

If you can answer these, Lab 03 is complete.

---

# ➡️ Next

Continue to:

## 📘 Lesson 04 — Users, Groups & Identity Management

You will take a deeper look at how organizations manage users and groups and use them to control access.

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [What is Microsoft Entra?](https://learn.microsoft.com/en-us/entra/fundamentals/what-is-entra)
- [Workload Identities](https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-overview)
- [Device Identities](https://learn.microsoft.com/en-us/entra/identity/devices/overview)

---

# 📚 Course Navigation

⬅️ **[Lesson 03 — Microsoft Entra ID & Identity Types](../lessons/%F0%9F%93%98%20Lesson%2003%20%E2%80%94%20Microsoft%20Entra%20ID%20&%20Identity%20Types.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
