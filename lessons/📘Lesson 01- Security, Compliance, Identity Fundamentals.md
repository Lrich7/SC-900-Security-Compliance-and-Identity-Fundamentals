# 📘 Lesson 01 — Security, Compliance & Identity Fundamentals

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 01  
**Lab:** ❌ No dedicated lab  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain the relationship between security, compliance, and identity
- Define authentication and authorization
- Explain the concept of identity as a security perimeter
- Describe identity providers
- Understand directory services
- Explain common identity types
- Understand federation
- Recognize the difference between authentication and authorization
- Identify basic security and compliance concepts
- Recognize how these concepts relate to Microsoft cloud services

---

# 🌐 The Big Picture

Modern organizations depend on users, devices, applications, networks, cloud services, and data. All of these need to be protected.

Traditionally, organizations focused heavily on protecting the physical network. Cloud computing changed this model. Today, users can access company resources from many locations and devices while the resources themselves may live in Microsoft 365, Microsoft Azure, a company datacenter, or another cloud service.

Because of this, security can no longer depend entirely on where the user is located. **Identity has become a major part of determining who should have access to what.**

---

# 🛡️ What Is Security?

Security is the practice of protecting people, devices, applications, networks, systems, services, and data from threats and unauthorized access.

Security attempts to reduce risks such as:

- Account compromise
- Malware
- Phishing
- Data theft
- Unauthorized access
- Data loss
- Ransomware
- Insider threats
- Service disruption

---

# 🔺 The CIA Triad

One of the foundational models in information security is the **CIA Triad**:

- **Confidentiality**
- **Integrity**
- **Availability**

## 🔒 Confidentiality

Confidentiality means information should only be accessible to authorized people or systems.

Examples include:

- Permissions
- Encryption
- Authentication
- Access controls
- Sensitivity labels

**Memory tip:** Confidentiality = **Who can see it?**

## 🧾 Integrity

Integrity means information should remain accurate and should not be changed improperly.

Examples include:

- Hashing
- Digital signatures
- Permissions
- Version control
- Audit logs

**Memory tip:** Integrity = **Can I trust it?**

## 🟢 Availability

Availability means systems and information should be accessible when authorized users need them.

Controls that improve availability can include:

- Backups
- Redundancy
- Failover
- Load balancing
- DDoS protection
- Disaster recovery

**Memory tip:** Availability = **Can I access it?**

---

# 👤 What Is Identity?

In computing, an identity represents something that can be authenticated and potentially granted access to resources.

Identities can represent:

- Users
- Applications
- Devices
- Services
- Workloads

## User Identity

Represents a person and may contain information such as:

- Name
- Username
- Email
- Department
- Job title
- Manager
- Group membership
- Assigned roles

## Device Identity

Devices such as laptops, desktops, phones, and tablets can have identities. Device identity can help determine whether a device should be allowed to access organizational resources.

## Application Identity

Applications may need to authenticate to other systems. Rather than using a person's account, an application can use its own identity.

## Workload Identity

A workload identity represents software workloads such as applications, services, containers, virtual machines, and automation.

---

# 🔐 Authentication

Authentication answers:

> **Who are you?**

The system attempts to verify the identity being presented.

Authentication methods can include:

- Password
- PIN
- Security key
- Passkey
- Microsoft Authenticator
- Certificate
- Biometrics

## Authentication Factors

### Something You Know

Examples:

- Password
- PIN

### Something You Have

Examples:

- Phone
- Security key
- Smart card

### Something You Are

Examples:

- Fingerprint
- Face
- Other biometrics

## Multifactor Authentication

Multifactor authentication uses factors from more than one category. For example, a password plus an authenticator application can provide MFA.

We'll examine MFA in much more detail later in the course.

---

# 🚪 Authorization

Authorization answers:

> **What are you allowed to do?**

Authentication normally occurs first. Authorization then determines what the authenticated identity can access.

```text
User
  ↓
Authentication
  ↓
Identity Verified
  ↓
Authorization
  ↓
Permissions Checked
  ↓
Access Granted / Denied
```

## 🧠 Authentication vs Authorization

Remember:

```text
AUTHENTICATION
=
WHO ARE YOU?

AUTHORIZATION
=
WHAT CAN YOU DO?
```

A badge proving that you are an employee is similar to **authentication**. Which doors that badge is permitted to open is similar to **authorization**.

---

# 🏢 What Is an Identity Provider?

An identity provider, or **IdP**, is a system that creates, maintains, and manages identity information and provides authentication services.

In Microsoft's cloud ecosystem, a major identity platform is **Microsoft Entra ID**.

---

# ☁️ Microsoft Entra ID

Microsoft Entra ID is Microsoft's cloud-based identity and access management service.

You may encounter its previous name in older documentation:

```text
Azure Active Directory
Azure AD
```

The current name is:

**Microsoft Entra ID**

Microsoft Entra ID provides identity and access capabilities for users, groups, devices, applications, and cloud resources.

---

# ⚠️ Active Directory vs Microsoft Entra ID

Do not assume these are the same product.

## Active Directory Domain Services

Commonly associated with traditional on-premises environments and technologies such as:

- Domain controllers
- Windows domains
- Kerberos
- Group Policy
- Organizational Units

## Microsoft Entra ID

Cloud-based identity and access management commonly associated with:

- Microsoft 365
- Azure
- Cloud applications
- Conditional Access
- Cloud authentication

We will examine Microsoft Entra ID in much greater detail later in the course.

---

# 📖 What Is a Directory Service?

A directory service stores and organizes information about objects such as:

- Users
- Groups
- Devices
- Applications

A directory helps organizations manage identities and access.

---

# 🤝 Federation

Federation allows identities from one system or organization to be trusted by another.

Conceptually:

```text
Organization A
Identity Provider
      ↓
Authentication
      ↓
Trusted Relationship
      ↓
Application / Organization B
```

This can allow users to access resources without requiring completely separate credentials for every system.

---

# 🔑 Single Sign-On

**Single Sign-On (SSO)** allows a user to authenticate once and then access multiple authorized applications without repeatedly entering credentials.

```text
User Signs In
     ↓
Identity Provider
     ↓
 ┌───┼───┐
 ↓   ↓   ↓
App A App B App C
```

SSO can improve user experience, productivity, identity management, and security when implemented appropriately.

---

# 📋 What Is Compliance?

Compliance means meeting applicable:

- Laws
- Regulations
- Industry standards
- Organizational policies
- Contractual requirements

Requirements may relate to privacy, data retention, data protection, auditing, access control, and information handling.

---

# 🛡️ Security vs Compliance

Security and compliance overlap, but they are not identical.

**Security asks:**

> How do we protect our systems and information?

**Compliance asks:**

> What requirements must we meet?

A single control may support both security and compliance goals.

Being compliant does not automatically mean an organization is completely secure, and a strong security program still needs to understand applicable compliance obligations.

---

# 📊 Governance, Risk & Compliance

You may see the acronym **GRC**:

- **Governance**
- **Risk**
- **Compliance**

## Governance

Governance involves how an organization establishes policies, responsibilities, oversight, and decision-making.

Example:

> All administrative accounts must use MFA.

## Risk

Risk involves identifying and managing potential harm to the organization.

A simplified way to think about it is:

```text
Threat
  +
Vulnerability
  ↓
Potential Risk
```

## Compliance

Compliance focuses on meeting required standards, policies, regulations, and obligations.

---

# 🏢 Microsoft's Security, Compliance & Identity Ecosystem

Throughout this course, we'll focus heavily on several Microsoft platforms.

## 👤 Microsoft Entra

Think:

> **Identity and Access**

Examples include:

- Users
- Authentication
- MFA
- Conditional Access
- Identity Governance
- Identity Protection

## 🛡️ Microsoft Defender

Think:

> **Security and Threat Protection**

Defender products provide protection across areas such as endpoints, email, identity, cloud applications, and cloud workloads.

## 🚨 Microsoft Sentinel

Think:

> **Security Monitoring, Detection, Investigation & Response**

Two important terms you'll learn later are:

- SIEM
- SOAR

## 📋 Microsoft Purview

Think:

> **Data Security, Governance, Risk, and Compliance**

Examples include:

- Information Protection
- Data Loss Prevention
- Retention
- Audit
- eDiscovery
- Insider Risk
- Compliance management

---

# 🧠 Four Names to Start Remembering

```text
Microsoft Entra
=
IDENTITY

Microsoft Defender
=
SECURITY

Microsoft Sentinel
=
SECURITY OPERATIONS

Microsoft Purview
=
DATA SECURITY & COMPLIANCE
```

You will see these names repeatedly throughout SC-900.

---

# 🌎 Real-World Scenario

Imagine an employee named Alex attempting to access sensitive financial data from a laptop.

The organization may need to determine:

```text
WHO?
Alex
   ↓
IDENTITY
Microsoft Entra
   ↓
AUTHENTICATION
Did Alex prove their identity?
   ↓
AUTHORIZATION
Does Alex have permission?
   ↓
SECURITY
Is the account, device, or session risky?
   ↓
COMPLIANCE
Is Alex permitted to access this data?
   ↓
DATA PROTECTION
Can the information be downloaded,
shared, or copied?
```

Modern security is not one product or one firewall. It is a collection of controls working together.

---

# 🎯 Exam Focus

Make sure you understand these concepts:

| Concept | Remember |
|---|---|
| Identity | Digital representation of a user, device, application, or workload |
| Authentication | Who are you? |
| Authorization | What are you allowed to do? |
| Identity Provider | Manages identities and provides authentication |
| Federation | Trust between identity systems |
| SSO | Authenticate once and access multiple authorized resources |
| Security | Protect systems, identities, services, and data |
| Compliance | Meet applicable requirements and obligations |

---

# 🧠 Memory Tricks

## Authentication vs Authorization

```text
AuthN
=
Name
=
Who are you?

AuthZ
=
Permission
=
What can you do?
```

## Microsoft Platforms

```text
ENTRA
=
Enter / Access
=
Identity

DEFENDER
=
Defend
=
Security

SENTINEL
=
Watch
=
Security Operations

PURVIEW
=
See / Govern Data
=
Data Security & Compliance
```

---

# ❓ Knowledge Check

Try answering these before looking at the answers.

### 1. Which security principle ensures information is available only to authorized users?

A. Integrity  
B. Confidentiality  
C. Availability  
D. Federation

### 2. Which part of the CIA triad ensures information has not been improperly changed?

A. Confidentiality  
B. Authentication  
C. Integrity  
D. Availability

### 3. Authentication answers which question?

A. What are you allowed to do?  
B. Who are you?  
C. Where is the data stored?  
D. Is the organization compliant?

### 4. Authorization answers which question?

A. Who are you?  
B. What are you allowed to do?  
C. What is your password?  
D. Where are you located?

### 5. Which Microsoft service is primarily associated with identity and access management?

A. Microsoft Sentinel  
B. Microsoft Purview  
C. Microsoft Entra ID  
D. Microsoft Defender for Cloud

### 6. Which Microsoft platform is strongly associated with data security, governance, and compliance?

A. Microsoft Purview  
B. Microsoft Entra  
C. Microsoft Sentinel  
D. Azure Bastion

### 7. What does SSO stand for?

A. Secure Sign-On  
B. Single Sign-On  
C. Security Service Operation  
D. Standard Sign-On

### 8. Which authentication factor is a fingerprint?

A. Something you know  
B. Something you have  
C. Something you are  
D. Something you manage

### 9. Which term describes meeting regulatory, legal, contractual, or organizational requirements?

A. Authentication  
B. Compliance  
C. Federation  
D. Availability

### 10. What does GRC stand for?

A. Governance, Risk, and Compliance  
B. Governance, Recovery, and Control  
C. Global Risk and Cybersecurity  
D. General Regulatory Compliance

---

# ✅ Knowledge Check Answers

1. **B — Confidentiality**
2. **C — Integrity**
3. **B — Who are you?**
4. **B — What are you allowed to do?**
5. **C — Microsoft Entra ID**
6. **A — Microsoft Purview**
7. **B — Single Sign-On**
8. **C — Something you are**
9. **B — Compliance**
10. **A — Governance, Risk, and Compliance**

---

# 📌 Lesson Summary

In this lesson you learned:

```text
Security
  ↓
Protect resources

Identity
  ↓
Represent users, devices,
applications and workloads

Authentication
  ↓
Who are you?

Authorization
  ↓
What can you do?

Compliance
  ↓
Meet requirements

Microsoft Entra
  ↓
Identity & Access

Microsoft Defender
  ↓
Security

Microsoft Sentinel
  ↓
Security Operations

Microsoft Purview
  ↓
Data Security & Compliance
```

These concepts form the foundation for everything else in the course.

---

# 🧪 Lab

**❌ No dedicated lab for Lesson 01.**

This lesson is primarily conceptual. Rather than creating a lab that does not add much value, continue directly to Lesson 02.

Starting with Lesson 02, labs will be labeled as:

- 🟢 Hands-On
- 🔵 Explore the Tool
- 🟡 Scenario
- ❌ No Lab

---

# ➡️ Next Lesson

## 📘 Lesson 02 — Shared Responsibility, Defense in Depth & Zero Trust

Next you'll learn about:

- Shared responsibility
- Defense in depth
- Zero Trust
- Encryption
- Hashing
- Governance
- Risk
- Compliance

Lesson 02 will also include our first:

> 🟡 **Scenario Lab — Apply Zero Trust**

---

# 📚 Course Navigation

⬅️ **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
