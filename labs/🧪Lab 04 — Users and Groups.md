# 🟢🔵 Lab 04 — Users & Groups

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 04 — Users, Groups & Identity Management  
**Lab Type:** 🟢 Hands-On / 🔵 Explore the Tool  
**Difficulty:** Beginner

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Locate users in Microsoft Entra ID
- Identify common user properties
- Distinguish Member and Guest users
- Locate Microsoft Entra groups
- Identify common group properties
- Explain assigned membership
- Recognize dynamic membership
- Understand how groups simplify access management
- Locate Microsoft Entra administrative roles
- Apply the principle of least privilege
- Safely create and remove test objects if authorized

---

# 🧪 Choose Your Lab Path

This lab has two paths.

## 🟢 Path A — Hands-On

Use this path if:

```text
You have authorization
        +
You can safely create test objects
        +
You understand your environment
```

You will create:

```text
1 Test User

1 Test Security Group
```

Then you will add the user to the group and remove the test objects when finished.

---

## 🔵 Path B — Explore the Tool

Use this path if:

```text
You are in a production tenant

OR

You do not have permission

OR

You do not want to make changes
```

You will inspect existing users and groups without modifying anything.

Both paths teach the SC-900 concepts.

---

# ⚠️ Production Safety

Do not create, modify, disable, or delete company accounts unless you are authorized.

Never use a real employee as the test account for this lab.

If there is any uncertainty:

> **Use Path B — Explore the Tool.**

---

# 🚀 Part 1 — Open Microsoft Entra

Open the Microsoft Entra admin center:

```text
https://entra.microsoft.com
```

Sign in with an authorized account.

Locate:

```text
Entra ID
```

---

# 👤 Part 2 — Explore Users

Navigate to:

```text
Entra ID
   ↓
Users
   ↓
All users
```

Look at the user list.

Depending on your permissions and portal layout, you may see information such as:

```text
Display Name

User Principal Name

User Type

Account Status
```

---

# 🔎 Inspect a User

If authorized, open a normal user account in read-only fashion.

Do not change anything.

Look for properties such as:

```text
Identity

Job Information

Contact Information

Groups

Roles

Authentication Information
```

### What is the user's User Type?

```text
Member / Guest
```

### What is a UPN used for?

```text
____________________________________

____________________________________
```

---

# 🌎 Part 3 — Find a Guest User

If your tenant contains Guest users, locate one.

Do not modify it.

Look for:

```text
User Type = Guest
```

Think about why the person might exist in the tenant.

Possible reasons:

```text
Vendor

Consultant

Partner

Contractor

Project Collaboration
```

### Why would an organization use a Guest identity instead of creating a normal employee account?

```text
____________________________________

____________________________________
```

If your tenant has no Guest users, simply continue.

---

# 🟢 Part 4A — Hands-On: Create a Test User

> Skip this section if you are following the read-only path.

Navigate to the user creation area.

Create a clearly identifiable test account.

Example:

```text
Display Name:
SC900 Lab User

Username:
sc900-lab-user
```

Use an approved test domain available in your tenant.

Do **not** assign:

```text
Administrative Roles

Paid Licenses

Production Access

Sensitive Groups
```

unless your organization specifically authorizes it.

Record the test user's name:

```text
____________________________________
```

---

# 🔵 Part 4B — Explore Alternative

If you cannot create users:

Choose an existing normal user and answer:

### What information is stored with the user?

```text
____________________________________

____________________________________
```

### What makes this object useful to an identity system?

```text
____________________________________

____________________________________
```

Do not record private or sensitive user information in your public GitHub notes.

---

# 👥 Part 5 — Explore Groups

Navigate to:

```text
Entra ID
   ↓
Groups
   ↓
All groups
```

Look at the groups.

Try to identify:

```text
Group Name

Group Type

Membership Type
```

---

# 🔎 Group Types

See whether your environment contains examples of:

```text
Security

Microsoft 365
```

### Which type would you normally consider when the main goal is controlling access?

```text
____________________________________
```

### Which type is associated with Microsoft 365 collaboration?

```text
____________________________________
```

---

# 🟢 Part 6A — Hands-On: Create a Test Security Group

> Skip this section if you are following the read-only path.

Create a test group.

Suggested name:

```text
SC900-Lab-Security-Group
```

Choose:

```text
Group Type:
Security
```

Use:

```text
Membership Type:
Assigned
```

Do not assign production permissions to this group.

---

# ➕ Part 7A — Add the Test User

If you created both test objects:

```text
SC900 Lab User
        ↓
SC900-Lab-Security-Group
```

Add the test user as a member of the test group.

Then verify that the membership appears.

---

# 🧠 What Just Happened?

Instead of assigning access directly to:

```text
SC900 Lab User
```

an organization could assign access to:

```text
SC900-Lab-Security-Group
```

Then group membership can determine who receives that access.

Conceptually:

```text
USER
  ↓
GROUP
  ↓
RESOURCE
```

This can simplify administration.

---

# 🔵 Part 6B — Read-Only Alternative

If you are not creating anything, select an existing non-sensitive group.

Inspect:

```text
Group Type

Membership Type

Members
```

Do not add or remove anyone.

Answer:

### Is the membership assigned or dynamic?

```text
____________________________________
```

### What might this group be used for?

```text
____________________________________

____________________________________
```

---

# ⚙️ Part 8 — Look for Dynamic Groups

Look through your groups to see whether any use:

```text
Dynamic User

or

Dynamic Device
```

Do not create or edit a dynamic membership rule in a production tenant for this fundamentals lab.

If you can inspect an existing authorized example, look at the concept behind the rule.

A rule might conceptually say:

```text
IF
Department = Accounting

THEN
Add User to Accounting Group
```

---

# 🧠 Assigned vs Dynamic

Complete:

```text
ASSIGNED MEMBERSHIP
=
____________________________________
```

```text
DYNAMIC MEMBERSHIP
=
____________________________________
```

Suggested answer:

```text
Assigned
=
Members are explicitly added


Dynamic
=
Membership is determined by rules
```

---

# 👑 Part 9 — Explore Administrative Roles

Navigate to the area containing:

```text
Roles & admins
```

Do not assign or remove roles.

Look for examples such as:

```text
Global Administrator

User Administrator

Groups Administrator

Authentication Administrator
```

---

# 🚨 Think Before Assigning Global Admin

Scenario:

A technician needs to perform approved user-management tasks.

Which design is better?

```text
A.
Technician
    ↓
Global Administrator
```

or:

```text
B.
Technician
    ↓
Appropriate Limited Role
```

Answer:

```text
______________________________
```

Which Zero Trust principle does this support?

```text
______________________________
```

---

# 🔷 Part 10 — Entra Role or Azure RBAC?

Choose the best answer.

## Scenario 1

An administrator needs permission to manage Microsoft Entra users.

```text
Microsoft Entra Role / Azure RBAC

Answer:
______________________________
```

## Scenario 2

An administrator needs permission to manage an Azure virtual machine.

```text
Microsoft Entra Role / Azure RBAC

Answer:
______________________________
```

## Scenario 3

An administrator needs to manage authentication settings for users.

```text
Microsoft Entra Role / Azure RBAC

Answer:
______________________________
```

---

# 🔄 Part 11 — Identity Lifecycle Scenario

A user named Alex moves from:

```text
Accounting
    ↓
Human Resources
```

Alex currently belongs to:

```text
Accounting-Users

Accounting-Reports

Company-All-Employees
```

What should IT review?

Check all that apply:

```text
[ ] Existing group membership

[ ] Access to Accounting resources

[ ] Access needed for HR

[ ] Administrative roles

[ ] Whether old access is still necessary
```

Correct answer:

> **All of them should be reviewed as appropriate.**

---

# 🧠 Why?

A common security problem is:

```text
User Changes Jobs
      ↓
Gets New Access
      ↓
Keeps All Old Access
      ↓
Excessive Permissions
```

Good identity management aims for:

```text
RIGHT USER
+
RIGHT ACCESS
+
RIGHT TIME
```

---

# 🏗️ Part 12 — Design a Group Strategy

Contoso has these departments:

```text
Accounting

Human Resources

Sales

IT
```

Create a simple group naming plan.

Example:

```text
SG-Accounting

SG-HR

SG-Sales

SG-IT
```

Now design your own:

| Department | Security Group |
|---|---|
| Accounting | __________________________ |
| Human Resources | __________________________ |
| Sales | __________________________ |
| IT | __________________________ |

---

# 🎯 Part 13 — Scenario Challenge

Contoso hires Morgan.

Morgan:

```text
Works in HR

Needs HR documents

Needs normal Microsoft 365 collaboration

Does NOT administer Microsoft Entra
```

Which objects or access approaches make sense?

Consider:

```text
User Account

HR Security Group

Microsoft 365 Group

Global Administrator

Guest Account
```

Write your choices:

```text
____________________________________

____________________________________
```

Explain why Global Administrator should or should not be assigned:

```text
____________________________________

____________________________________
```

---

# 🧹 Part 14 — Hands-On Cleanup

> Complete this section only if you created test objects.

Before deleting anything, verify that you are working with the objects created specifically for this lab.

You should have:

```text
SC900 Lab User

SC900-Lab-Security-Group
```

Do **not** delete similarly named production objects unless you created them specifically for this exercise and are authorized to remove them.

Remove the test user from the test group if necessary.

Then remove the lab objects according to your organization's procedures.

Confirm:

```text
[ ] Test user removed

[ ] Test group removed

[ ] No production object changed
```

---

# ✅ Suggested Answers

## Group Types

```text
Security Group
=
Primarily access/security


Microsoft 365 Group
=
Collaboration
```

## Administrative Role Scenario

```text
B — Appropriate Limited Role
```

Zero Trust principle:

```text
Use Least Privilege Access
```

## Entra Role or Azure RBAC

```text
Scenario 1
=
Microsoft Entra Role


Scenario 2
=
Azure RBAC


Scenario 3
=
Microsoft Entra Role
```

## Morgan Scenario

Reasonable choices include:

```text
Member User Account

HR Security Group

Appropriate Microsoft 365 collaboration group
```

Morgan should not receive Global Administrator merely because Morgan needs normal business access.

---

# 🎓 What You Should Have Learned

You should now understand how:

```text
USERS
     ↓
Represent people


GROUPS
     ↓
Organize identities


SECURITY GROUPS
     ↓
Simplify access


M365 GROUPS
     ↓
Support collaboration


ROLES
     ↓
Delegate administrative permissions
```

You should also understand why:

```text
EVERY USER
DOES NOT
NEED ADMIN ACCESS
```

and why access should change when a person's responsibilities change.

---

# ✅ Lab Completion Checklist

Before marking this lab complete, make sure you can answer:

- [ ] What does a Microsoft Entra user represent?
- [ ] What is a UPN?
- [ ] What is the difference between Member and Guest?
- [ ] Why are groups useful?
- [ ] What is a security group?
- [ ] What is a Microsoft 365 group?
- [ ] What is assigned membership?
- [ ] What is dynamic membership?
- [ ] What is an administrative role?
- [ ] Why should Global Administrator be limited?
- [ ] What is the difference between a Microsoft Entra role and Azure RBAC?
- [ ] Why should access be reviewed when a user changes jobs?

If you can answer these, Lab 04 is complete.

---

# ➡️ Next

Continue to:

## 📘 Lesson 05 — Authentication & Multifactor Authentication

You will learn how Microsoft Entra verifies identities and why MFA is one of the most important controls for protecting user accounts.

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Microsoft Entra Groups](https://learn.microsoft.com/en-us/entra/fundamentals/concept-learn-about-groups)
- [Microsoft Entra Built-in Roles](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference)
- [Azure RBAC Overview](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview)

---

# 📚 Course Navigation

⬅️ **[Lesson 04 — Users, Groups & Identity Management](../lessons/%F0%9F%93%98%20Lesson%2004%20%E2%80%94%20Users,%20Groups%20&%20Identity%20Management.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
