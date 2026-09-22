# 📘 Lesson 03 — Microsoft Entra ID & Identity Types

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 03  
**Lab:** 🔵 Explore the Tool — Microsoft Entra ID  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Describe Microsoft Entra ID
- Explain the purpose of an identity and access management (IAM) system
- Explain tenants and directories
- Identify human and non-human identities
- Describe cloud identities
- Describe hybrid identities
- Describe external identities
- Describe device identities
- Describe workload identities
- Recognize agent identities at a fundamentals level
- Explain the relationship between Microsoft Entra ID and on-premises Active Directory Domain Services
- Recognize common areas of the Microsoft Entra admin center

---

# 👤 Identity Is the New Security Perimeter

Traditional environments often focused heavily on protecting the network perimeter.

Modern organizations have:

```text
Remote Employees

Cloud Applications

Mobile Devices

Personal Devices

Partners

Contractors

Applications

Automated Services

AI Agents
```

A user or workload may access company resources without ever being physically inside the corporate office.

Because of this, identity has become a major security control.

A modern access decision may consider:

```text
WHO is requesting access?

WHAT identity is being used?

HOW did it authenticate?

WHAT device is being used?

WHAT resource is requested?

WHAT permissions does the identity have?

IS there unusual risk?
```

---

# 🔷 What Is Microsoft Entra?

**Microsoft Entra** is Microsoft's family of identity and network access products.

One of its core services is:

# Microsoft Entra ID

Microsoft Entra ID is Microsoft's cloud-based identity and access management service.

It helps organizations manage identities and control access to resources such as:

```text
Microsoft 365

Azure

Enterprise Applications

SaaS Applications

Custom Applications

Organizational Resources
```

Microsoft Entra ID was previously named:

> **Azure Active Directory (Azure AD)**

You may still encounter the older name in documentation, older training material, scripts, or conversations.

---

# 🧠 What Does Microsoft Entra ID Do?

At a high level:

```text
IDENTITY
   ↓
AUTHENTICATION
   ↓
ACCESS DECISION
   ↓
RESOURCE
```

Microsoft Entra ID provides capabilities for areas such as:

```text
Users

Groups

Devices

Applications

Authentication

Single Sign-On

Conditional Access

Administrative Roles

Identity Protection

Identity Governance
```

We will explore many of these in later lessons.

---

# 🏢 Tenant and Directory

Two terms you will frequently see are:

```text
Tenant

Directory
```

A **Microsoft Entra tenant** is a dedicated instance of Microsoft Entra ID associated with an organization.

You can think of it as the organization's identity environment in Microsoft cloud services.

Conceptually:

```text
CONTOSO
   ↓
Microsoft Entra Tenant
   ↓
Users
Groups
Devices
Applications
Roles
Policies
```

The directory stores identity-related objects and information for the tenant.

For SC-900, understand the basic relationship rather than worrying about deep tenant architecture.

---

# 🪪 What Is an Identity?

A digital identity represents something that can interact with systems and resources.

An identity does not have to represent a person.

Examples include:

```text
Employee

Guest

Device

Application

Service

Script

Container

AI Agent
```

A useful high-level distinction is:

```text
HUMAN IDENTITIES
       +
NON-HUMAN IDENTITIES
```

---

# 👨‍💼 Human Identities

Human identities represent people.

Examples include:

```text
Employees

Frontline Workers

Administrators

Contractors

Consultants

Partners

Guests

Customers
```

A human identity may be internal to the organization or external.

---

# ☁️ Cloud Identity

A cloud identity is created and primarily managed in the cloud identity system.

Example:

```text
New Employee
     ↓
Account Created in Microsoft Entra ID
     ↓
User Signs In to Microsoft 365
```

The identity does not need to originate in an on-premises Active Directory environment.

Cloud-native organizations may manage most or all identities this way.

---

# 🔄 Hybrid Identity

Many organizations still use:

```text
On-Premises Active Directory
        +
Microsoft Entra ID
```

A **hybrid identity** connects an organization's on-premises identity environment with its cloud identity environment.

Conceptually:

```text
On-Premises AD DS
        ↓
Identity Synchronization
        ↓
Microsoft Entra ID
        ↓
Cloud Resources
```

This can allow the same organizational identity to be used across on-premises and cloud resources.

---

# 🏠 Active Directory vs Microsoft Entra ID

These are related identity technologies, but they are not the same thing.

## Active Directory Domain Services — AD DS

Traditionally used for on-premises environments.

Common capabilities include:

```text
Domain Join

Kerberos

LDAP

Group Policy

On-Premises Authentication

Computer Management
```

## Microsoft Entra ID

Designed for modern cloud identity and access management.

Common capabilities include:

```text
Cloud Authentication

Microsoft 365 Access

SaaS Application Access

Modern Authentication

Conditional Access

Cloud Application SSO

Identity Governance
```

Do not think:

```text
Microsoft Entra ID
=
AD DS hosted in Azure
```

That is not an accurate model.

They are different technologies that can work together.

---

# 🌎 External Identities

Organizations often need to collaborate with people who are not employees.

Examples:

```text
Vendor

Consultant

Business Partner

Contractor

Guest
```

Microsoft Entra External ID supports scenarios involving external users.

Example:

```text
Contoso Employee
        ↓
Invites Partner
        ↓
Partner Authenticates
        ↓
Partner Receives Authorized Access
        ↓
Shared Resource
```

The organization can provide access without treating every external collaborator exactly like an internal employee.

---

# 💻 Device Identities

People are not the only things represented in Microsoft Entra ID.

Devices can also have identities.

Examples:

```text
Windows Laptop

Desktop

Mobile Phone

Tablet

IoT Device
```

A device identity gives Microsoft Entra information about a device that can be used in access and management decisions.

Common device identity states include:

```text
Microsoft Entra Registered

Microsoft Entra Joined

Microsoft Entra Hybrid Joined
```

---

# 📱 Microsoft Entra Registered

Registration is commonly associated with scenarios such as:

```text
Personal Devices

BYOD

Mobile Devices
```

The device is known to Microsoft Entra, but it is not necessarily fully organization-owned or joined in the same way as a corporate Windows device.

---

# 💼 Microsoft Entra Joined

Microsoft Entra join is commonly used for organization-owned modern Windows devices.

Conceptually:

```text
Company Laptop
      ↓
Joined to Microsoft Entra ID
      ↓
User Signs In with Organizational Identity
```

---

# 🔄 Microsoft Entra Hybrid Joined

A hybrid joined device is connected to:

```text
On-Premises Active Directory
        +
Microsoft Entra ID
```

This is commonly encountered in organizations transitioning from traditional on-premises management toward cloud-based identity and device management.

---

# ⚙️ Workload Identities

Applications and services also need identities.

A **workload identity** represents a software workload that needs to authenticate and access resources.

Examples include:

```text
Application

Service

Script

Container

Automation

CI/CD Process
```

In Microsoft Entra, workload identities include concepts such as:

```text
Applications

Service Principals

Managed Identities
```

---

# 🤖 Why Workload Identities Matter

Imagine an automated application needs to retrieve a secret from Azure Key Vault.

You do not want to create a normal employee account and give its password to the application.

Instead:

```text
Application
     ↓
Workload Identity
     ↓
Authentication
     ↓
Authorized Resource
```

The application receives its own identity and appropriate permissions.

This supports:

> **Least privilege**

from Lesson 02.

---

# 🧑‍💻 Service Principals

A service principal is an identity used by an application or service in a tenant.

At a fundamentals level, think:

```text
APPLICATION
     ↓
Needs to access something
     ↓
SERVICE PRINCIPAL
     ↓
Receives permissions
```

You do not need to master application registration architecture for SC-900.

Know why non-human identities exist and why they must be secured.

---

# 🪪 Managed Identities

Managed identities can provide identities for supported Azure resources.

A major benefit is reducing the need for developers or administrators to manually manage credentials for the workload.

Conceptually:

```text
Azure Resource
      ↓
Managed Identity
      ↓
Authenticate to Another Resource
      ↓
Authorized Access
```

---

# 🤖 Agent Identities

Current SC-900 objectives also include **agent ID** within Microsoft Entra identity types.

AI agents can act on behalf of users or organizations and may need to:

```text
Authenticate

Access Applications

Access Data

Perform Tasks

Use Permissions
```

Microsoft Entra can provide identity capabilities for AI agents.

At the SC-900 level, remember:

> An AI agent may need its own identity so its access can be identified, authenticated, governed, and controlled.

This continues the same principle used for people, devices, and workloads:

```text
EVERY IDENTITY
      ↓
SHOULD BE KNOWN
      ↓
AUTHENTICATED
      ↓
AUTHORIZED
      ↓
GOVERNED
```

---

# 🧠 Identity Types at a Glance

| Identity Type | Represents | Example |
|---|---|---|
| Human | Person | Employee |
| External | Person outside organization | Vendor |
| Device | Physical/virtual device | Laptop |
| Workload | Software workload | Application |
| Managed Identity | Azure resource identity | Azure VM accessing Key Vault |
| Agent | AI agent | AI agent accessing an application |

---

# 🔐 Identity and Zero Trust

Microsoft Entra plays an important role in implementing Zero Trust.

Remember the three principles:

```text
VERIFY EXPLICITLY

USE LEAST PRIVILEGE

ASSUME BREACH
```

Identity information can help answer questions such as:

```text
Who is the user?

How did they authenticate?

What device are they using?

What application are they accessing?

What permissions do they have?

Is the identity risky?
```

Microsoft Entra capabilities can then help enforce access decisions.

---

# 🖥️ Microsoft Entra Admin Center

Administrators commonly manage Microsoft Entra through the:

> **Microsoft Entra admin center**

The portal provides access to areas such as:

```text
Users

Groups

Devices

Applications

Roles & Admins

Authentication Methods

Conditional Access

Identity Protection

Identity Governance
```

Your Lab 03 will explore this portal without making production changes.

---

# 🗺️ A Simple Microsoft Entra Map

```text
                    MICROSOFT ENTRA ID
                           │
       ┌───────────────────┼───────────────────┐
       │                   │                   │
     PEOPLE              DEVICES          APPLICATIONS
       │                   │                   │
       ↓                   ↓                   ↓
     Users              Laptops            Workloads
     Guests             Phones             Services
     Partners           Tablets            Automation
       │                   │                   │
       └───────────────────┼───────────────────┘
                           ↓
                   AUTHENTICATION
                           ↓
                    ACCESS CONTROL
                           ↓
                       RESOURCES
```

---

# 🌎 Real-World Example

Suppose Contoso hires Alex.

Alex receives:

```text
Employee Identity
       ↓
Microsoft Entra User Account
       ↓
Assigned to Groups
       ↓
Authenticates
       ↓
Accesses Microsoft 365
```

Alex uses a company laptop:

```text
Laptop
   ↓
Device Identity
```

Contoso works with an outside accounting firm:

```text
Accountant
    ↓
External Identity
```

A cloud application automatically retrieves information:

```text
Application
    ↓
Workload Identity
```

An AI agent performs an approved automated task:

```text
AI Agent
    ↓
Agent Identity
```

Microsoft Entra helps the organization manage access for these different identities.

---

# 🎯 Exam Focus

Be able to recognize:

```text
Microsoft Entra ID
=
Cloud identity and access management
```

```text
Hybrid Identity
=
On-premises identity + cloud identity
```

```text
External Identity
=
Identity for outside users/customers/partners scenarios
```

```text
Device Identity
=
Identity representing a device
```

```text
Workload Identity
=
Identity for software such as an app, service, script, or container
```

```text
Agent Identity
=
Identity for an AI agent
```

Also remember:

```text
Microsoft Entra ID ≠ Active Directory Domain Services
```

They can work together, but they are different technologies.

---

# 🧠 Memory Tricks

### Entra

```text
ENTRA
≈
ENTER
```

Think:

> Who can **enter** and access the resource?

### Hybrid

```text
HYBRID
=
ON-PREM + CLOUD
```

### Workload Identity

```text
WORKLOAD
=
SOFTWARE NEEDS AN IDENTITY TOO
```

### Device Identity

```text
DEVICE
=
THE MACHINE HAS AN IDENTITY
```

---

# ❓ Knowledge Check

### 1.

What is Microsoft Entra ID primarily used for?

A. Cloud identity and access management  
B. Network cabling  
C. Physical server repair  
D. Database backup only

---

### 2.

What was Microsoft Entra ID previously called?

A. Microsoft Defender ID  
B. Azure Active Directory  
C. Azure Sentinel  
D. Microsoft Purview ID

---

### 3.

Which identity type represents an application, service, script, or container?

A. Human identity  
B. Device identity  
C. Workload identity  
D. Guest network

---

### 4.

Which identity type could represent a company laptop?

A. Device identity  
B. Workload identity  
C. External identity  
D. Compliance identity

---

### 5.

What is a hybrid identity?

A. An identity used only on mobile devices  
B. An identity spanning on-premises and cloud identity environments  
C. An anonymous account  
D. An identity used only by applications

---

### 6.

A consulting partner needs access to a shared company resource. Which concept is most relevant?

A. External identity  
B. Managed disk  
C. Network Security Group  
D. Azure Firewall

---

### 7.

Which statement is correct?

A. Microsoft Entra ID and AD DS are identical  
B. Microsoft Entra ID is simply AD DS hosted in Azure  
C. Microsoft Entra ID and AD DS are different technologies that can work together  
D. AD DS is a Microsoft Purview service

---

### 8.

Why might an Azure application use a managed identity?

A. To give the application an identity without manually managing normal user credentials  
B. To create a physical server  
C. To replace all employees  
D. To encrypt a network cable

---

### 9.

Which Microsoft Entra concept can identify and control an AI agent?

A. Agent identity  
B. Network identity  
C. Data residency  
D. Hash identity

---

### 10.

Which portal is commonly used to manage Microsoft Entra?

A. Microsoft Entra admin center  
B. Windows Calculator  
C. Azure Storage Explorer only  
D. Microsoft Paint

---

# ✅ Knowledge Check Answers

```text
1. A — Cloud identity and access management

2. B — Azure Active Directory

3. C — Workload identity

4. A — Device identity

5. B — An identity spanning on-premises and cloud identity environments

6. A — External identity

7. C — Microsoft Entra ID and AD DS are different technologies that can work together

8. A — Give the application an identity without manually managing normal user credentials

9. A — Agent identity

10. A — Microsoft Entra admin center
```

---

# 📌 Lesson Summary

You learned:

```text
MICROSOFT ENTRA ID
=
Cloud identity and access management


HUMAN IDENTITY
=
Person


EXTERNAL IDENTITY
=
Outside user/customer/partner scenario


DEVICE IDENTITY
=
Laptop, phone, tablet, or other device


WORKLOAD IDENTITY
=
Application, service, script, or container


AGENT IDENTITY
=
AI agent


HYBRID IDENTITY
=
On-Premises + Cloud
```

Identity is not limited to employees.

Modern organizations must secure:

```text
People

Devices

Applications

Services

Automation

AI Agents
```

---

# 🧪 Lab

This lesson benefits from a lab.

## 🔵 Lab 03 — Explore Microsoft Entra ID

The goal is **not** to change production settings.

You will explore the Microsoft Entra admin center and locate:

- Tenant information
- Users
- Groups
- Devices
- Applications
- Roles
- Authentication methods
- Conditional Access
- Identity Protection
- Identity Governance

➡️ **[Lab 03 — Explore Microsoft Entra ID](../labs/Lab%2003%20—%20Explore%20Microsoft%20Entra%20ID.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 04 — Users, Groups & Identity Management

Next, you will take a closer look at how Microsoft Entra manages people and access using:

- Users
- Groups
- Membership
- External users
- Administrative roles
- Identity management

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Microsoft Entra Fundamentals](https://learn.microsoft.com/en-us/entra/fundamentals/what-is-entra)
- [Identity and Access Management Fundamentals](https://learn.microsoft.com/en-us/entra/fundamentals/identity-fundamental-concepts)
- [Workload Identities](https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-overview)

---

# 📚 Course Navigation

⬅️ **Lesson 02 — Shared Responsibility, Defense in Depth & Zero Trust**

🧪 **[Lab 03 — Explore Microsoft Entra ID](../labs/Lab%2003%20—%20Explore%20Microsoft%20Entra%20ID.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
