# 📘 Lesson 04 — Users, Groups & Identity Management

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 04  
**Lab:** 🟢 Hands-On / 🔵 Explore the Tool — Users & Groups  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Describe user accounts in Microsoft Entra ID
- Distinguish Member and Guest users
- Explain why organizations use groups
- Describe security groups and Microsoft 365 groups
- Explain assigned and dynamic membership at a fundamentals level
- Describe external collaboration
- Explain administrative roles
- Distinguish Microsoft Entra roles from Azure RBAC roles
- Explain least privilege in identity administration
- Recognize common user and group management areas in the Microsoft Entra admin center

---

# 👤 Users in Microsoft Entra ID

A **user identity** represents a person who needs to authenticate and access organizational resources.

Examples include:

```text
Employee

Administrator

Contractor

Consultant

Partner

Guest
```

A user object contains identity information that Microsoft Entra can use during authentication and access decisions.

Common information may include:

```text
Display Name

User Principal Name

Email

Job Title

Department

Manager

Group Membership

Assigned Roles
```

---

# 🪪 User Principal Name — UPN

A **User Principal Name**, or **UPN**, is commonly used as a user's sign-in name.

It often looks like an email address:

```text
alex@contoso.com
```

Conceptually:

```text
USER
  ↓
alex@contoso.com
  ↓
Microsoft Entra ID
  ↓
Authentication
```

A UPN and an email address may look the same, but they serve different purposes and do not have to be identical.

For SC-900, remember:

> **UPN = common sign-in identifier for a Microsoft Entra user.**

---

# 🏢 Member Users

A **Member** user is generally an identity that belongs to the organization's tenant.

Example:

```text
New Employee
     ↓
User Account Created
     ↓
User Type: Member
     ↓
Access Assigned
```

Employees are commonly represented as Member users.

---

# 🌎 Guest Users

Organizations frequently collaborate with people outside the company.

Examples:

```text
Vendor

Consultant

Partner

Contractor
```

An external collaborator can be represented in the tenant as a **Guest** user.

Conceptually:

```text
External Person
      ↓
Invitation / External Collaboration
      ↓
Guest Identity
      ↓
Authorized Resources
```

Guest access allows an organization to collaborate without treating every external person exactly like an internal employee.

---

# 🧠 Member vs Guest

| User Type | Typical Example |
|---|---|
| Member | Employee |
| Guest | External collaborator |

The exact access a user receives is determined by permissions and policies, not simply by the Member or Guest label.

---

# 👥 Why Use Groups?

Imagine an Accounting department with 20 employees.

Without groups, an administrator might need to assign access individually:

```text
Alice → Accounting Files

Bob → Accounting Files

Chris → Accounting Files

Dana → Accounting Files
```

This becomes difficult to manage.

Instead:

```text
Alice ─┐
Bob ───┤
Chris ─┼──> Accounting Group ──> Accounting Resources
Dana ──┘
```

When someone joins or leaves the department, the administrator can update group membership rather than every individual resource.

Groups can improve:

```text
Consistency

Scalability

Administration

Access Management
```

---

# 🛡️ Security Groups

A **security group** is commonly used to manage access to resources.

Conceptually:

```text
USERS
  ↓
SECURITY GROUP
  ↓
ACCESS
```

Example:

```text
Help Desk Staff
      ↓
Help-Desk-Security-Group
      ↓
Authorized Resource
```

Security groups are useful when the primary goal is controlling access.

---

# 📦 Microsoft 365 Groups

A **Microsoft 365 group** supports collaboration between users.

Microsoft 365 groups can be associated with collaborative resources across Microsoft 365.

Think:

```text
PEOPLE
  +
COLLABORATION
```

Examples can involve services such as:

```text
Microsoft Teams

SharePoint

Shared Mailbox / Conversations

Calendar
```

At the SC-900 level, remember the broad distinction:

```text
Security Group
=
Primarily access/security


Microsoft 365 Group
=
Primarily collaboration
```

---

# ➕ Assigned Membership

With **assigned membership**, an administrator explicitly chooses the members.

Example:

```text
Accounting Group

Members:
- Alice
- Bob
- Chris
```

Someone must add or remove members as needed.

---

# ⚙️ Dynamic Membership

Dynamic membership uses rules to determine group membership automatically.

Conceptually:

```text
USER ATTRIBUTES
      ↓
DYNAMIC RULE
      ↓
GROUP MEMBERSHIP
```

Example rule idea:

```text
Department = Accounting
```

Users matching the rule can automatically become members.

If a user's department changes, their membership can change based on the rule.

---

# 🌎 External Collaboration

Microsoft Entra supports collaboration with identities outside the organization.

A company might need to give a consultant access to:

```text
SharePoint Site

Microsoft Teams Team

Application

Project Resources
```

A secure approach is:

```text
External Identity
      ↓
Authentication
      ↓
Authorized Access Only
      ↓
Required Resource
```

This supports the Zero Trust principle of:

> **Use least privilege access.**

---

# 👑 Administrative Roles

Normal users and administrators should not have the same permissions.

Microsoft Entra provides **roles** that grant administrative capabilities.

Examples include:

```text
Global Administrator

User Administrator

Groups Administrator

Authentication Administrator

Application Administrator
```

Each role is intended for different administrative responsibilities.

---

# 🚨 Global Administrator

The **Global Administrator** role has very broad administrative access.

Because of its power, it should not be assigned simply because someone works in IT.

Think:

```text
NEEDS LIMITED ADMIN TASKS
          ↓
ASSIGN LIMITED ROLE
```

rather than:

```text
WORKS IN IT
    ↓
GLOBAL ADMIN
```

This follows:

> **Least privilege**

---

# 🛡️ Least Privilege Example

Suppose Jordan works at the help desk and needs to perform specific user-management tasks.

A poor design might be:

```text
Jordan
   ↓
Global Administrator
```

A better design is to select the least-privileged role that supports the approved tasks.

```text
Jordan
   ↓
Appropriate Limited Role
   ↓
Required Tasks Only
```

Later in the course, you will also learn about **Privileged Identity Management (PIM)**, which can help organizations manage privileged access.

---

# 🔷 Microsoft Entra Roles vs Azure RBAC

This distinction can be confusing.

## Microsoft Entra Roles

Primarily manage identity-related resources and Microsoft Entra capabilities.

Examples:

```text
Users

Groups

Applications

Authentication

Directory Settings
```

## Azure Role-Based Access Control — Azure RBAC

Controls access to Azure resources.

Examples:

```text
Virtual Machines

Storage Accounts

Virtual Networks

Azure Resources
```

Think:

```text
ENTRA ROLE
=
Manage identity environment


AZURE RBAC
=
Manage Azure resources
```

They are separate authorization systems, although both use roles.

---

# 🧠 Role-Based Access Control

RBAC means permissions are associated with roles.

Conceptually:

```text
USER
  ↓
ROLE
  ↓
PERMISSIONS
```

Instead of assigning every permission individually, an administrator can assign an appropriate role.

This makes permissions easier to:

```text
Understand

Manage

Review

Limit
```

---

# 🔐 Groups and Access

Groups can also simplify authorization.

Example:

```text
User
  ↓
Security Group
  ↓
Application Access
```

This can be easier to manage than assigning application access separately to every user.

---

# 🔄 Identity Lifecycle

User identities change over time.

A basic identity lifecycle might look like:

```text
JOIN
 ↓
Create Identity
 ↓
Assign Appropriate Access
 ↓
CHANGE
 ↓
Update Role / Department / Groups
 ↓
LEAVE
 ↓
Remove Access
 ↓
Disable / Remove Identity
```

This is often called:

```text
Joiner

Mover

Leaver
```

Managing this lifecycle helps prevent users from keeping access they no longer need.

---

# 🏢 Real-World Example

Contoso hires Taylor as an Accounting employee.

The organization might:

```text
Create Taylor's User
        ↓
Set Department = Accounting
        ↓
Add Taylor to Accounting Group
        ↓
Assign Required Resources
        ↓
Require Appropriate Authentication
```

Six months later Taylor moves to Human Resources.

The organization should review:

```text
Old Group Membership

New Group Membership

Application Access

Administrative Roles

Resource Permissions
```

Taylor should not automatically keep unnecessary Accounting access forever.

This is part of good identity management.

---

# 👤 Manager and User Attributes

Microsoft Entra user objects can contain organizational information such as:

```text
Department

Job Title

Manager

Office

Contact Information
```

These attributes can support administration and, in some environments, automated identity processes.

Accurate identity information can make management easier.

---

# 🧠 Static vs Dynamic Example

## Assigned Group

```text
Administrator decides:
Alice belongs in Accounting
```

## Dynamic Group

```text
Rule decides:
IF Department = Accounting
THEN Add to Accounting Group
```

Dynamic membership can reduce repetitive administration, but the underlying user attributes and rules must be accurate.

---

# 🧱 Identity Management and Zero Trust

Users and groups connect directly to the Zero Trust principles from Lesson 02.

## Verify Explicitly

```text
Authenticate the identity
```

## Use Least Privilege

```text
Give only required access
```

## Assume Breach

```text
Limit how much damage
one compromised identity can cause
```

Identity management is therefore an important part of an organization's security architecture.

---

# 🎯 Exam Focus

Know these relationships:

```text
USER
=
Human identity
```

```text
GUEST
=
External collaborator represented in the tenant
```

```text
SECURITY GROUP
=
Primarily used to manage access
```

```text
MICROSOFT 365 GROUP
=
Collaboration
```

```text
ASSIGNED MEMBERSHIP
=
Administrator chooses members
```

```text
DYNAMIC MEMBERSHIP
=
Rules determine membership
```

```text
MICROSOFT ENTRA ROLE
=
Administrative permissions for identity/directory capabilities
```

```text
AZURE RBAC
=
Authorization for Azure resources
```

---

# 🧠 Memory Tricks

### Groups

```text
SECURITY GROUP
=
SECURE ACCESS
```

```text
M365 GROUP
=
COLLABORATE
```

### Membership

```text
ASSIGNED
=
ADMIN ADDS
```

```text
DYNAMIC
=
RULE ADDS
```

### Roles

```text
ENTRA ROLE
=
IDENTITY ADMINISTRATION
```

```text
AZURE RBAC
=
AZURE RESOURCE ACCESS
```

---

# ❓ Knowledge Check

### 1.

Which Microsoft Entra object normally represents an employee?

A. User  
B. Firewall  
C. Storage account  
D. Network

---

### 2.

Which user type commonly represents an external collaborator?

A. Member  
B. Guest  
C. Device  
D. Managed disk

---

### 3.

What is a primary purpose of a security group?

A. Video conferencing  
B. Managing access  
C. Creating virtual machines  
D. Encrypting hard drives

---

### 4.

Which group type is designed around Microsoft 365 collaboration?

A. Microsoft 365 group  
B. Network Security Group  
C. Resource group  
D. Management group

---

### 5.

With assigned membership, who or what explicitly selects group members?

A. A dynamic rule only  
B. An administrator or authorized process  
C. Azure Firewall  
D. Microsoft Sentinel

---

### 6.

What determines membership in a dynamic group?

A. Group membership rules  
B. A physical badge  
C. Network cables  
D. Encryption keys

---

### 7.

Which principle says administrators should receive only the access necessary for their tasks?

A. Data residency  
B. Least privilege  
C. Federation  
D. Availability

---

### 8.

Microsoft Entra administrative roles primarily control:

A. Identity and directory administrative capabilities  
B. Physical building access  
C. Azure datacenter cooling  
D. Internet routing

---

### 9.

Azure RBAC primarily controls access to:

A. Azure resources  
B. Microsoft Entra user passwords only  
C. Physical offices  
D. Email signatures

---

### 10.

An employee moves from Accounting to HR. What should the organization do?

A. Leave all old access forever  
B. Review and update the employee's access  
C. Give the employee Global Administrator  
D. Delete every group

---

# ✅ Knowledge Check Answers

```text
1. A — User

2. B — Guest

3. B — Managing access

4. A — Microsoft 365 group

5. B — An administrator or authorized process

6. A — Group membership rules

7. B — Least privilege

8. A — Identity and directory administrative capabilities

9. A — Azure resources

10. B — Review and update the employee's access
```

---

# 📌 Lesson Summary

You learned:

```text
USERS
=
People represented in Microsoft Entra
```

```text
GROUPS
=
Organize identities and simplify access
```

```text
GUEST USERS
=
Support external collaboration
```

```text
DYNAMIC GROUPS
=
Rule-based membership
```

```text
ADMINISTRATIVE ROLES
=
Delegate administrative capabilities
```

and:

```text
GOOD IDENTITY MANAGEMENT
=
Right Identity
+
Right Access
+
Right Time
```

---

# 🧪 Lab

This lesson benefits from a lab.

## 🟢 / 🔵 Lab 04 — Users & Groups

If you have permission in a safe test environment, you can complete the hands-on path.

If you are using a production tenant or do not have permission to create test objects, use the read-only exploration path instead.

➡️ **[Lab 04 — Users & Groups](../labs/Lab%2004%20—%20Users%20&%20Groups.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 05 — Authentication & Multifactor Authentication

Next you will learn how Microsoft Entra verifies identities using:

- Authentication methods
- Passwords
- Multifactor authentication
- Security defaults
- Authentication strength
- Password protection

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Microsoft Entra User Management](https://learn.microsoft.com/en-us/entra/fundamentals/how-to-create-delete-users)
- [Microsoft Entra Groups](https://learn.microsoft.com/en-us/entra/fundamentals/concept-learn-about-groups)
- [Microsoft Entra Built-in Roles](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference)
- [Azure RBAC Overview](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview)

---

# 📚 Course Navigation

⬅️ **Lesson 03 — Microsoft Entra ID & Identity Types**

🧪 **[Lab 04 — Users & Groups](../labs/Lab%2004%20—%20Users%20&%20Groups.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
