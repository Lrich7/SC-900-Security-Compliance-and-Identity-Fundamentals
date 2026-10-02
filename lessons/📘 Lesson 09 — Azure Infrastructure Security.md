# 📘 Lesson 09 — Azure Infrastructure Security

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 09  
**Section:** Microsoft Security Solutions  
**Lab:** 🔵 Explore the Tool — Azure Infrastructure Security  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain the purpose of Azure infrastructure security
- Describe Azure network security concepts
- Explain Network Security Groups (NSGs)
- Describe Azure Firewall
- Explain Azure DDoS Protection
- Describe Azure Bastion
- Explain the purpose of Azure Key Vault
- Describe Azure resource locks
- Explain how Azure Policy supports governance and security
- Recognize the relationship between infrastructure security and defense in depth
- Identify which Azure security control fits a basic scenario

---

# ☁️ Moving from Identity to Infrastructure

Lessons 03–08 focused heavily on:

```text
WHO is requesting access?
```

Now we begin looking at:

```text
WHAT are we protecting?
```

Azure infrastructure can include:

```text
Virtual Machines

Virtual Networks

Storage

Applications

Databases

Public IP Addresses

Cloud Resources
```

Security requires protecting both:

```text
IDENTITIES
+
RESOURCES
```

---

# 🧱 Defense in Depth

Recall Lesson 02:

```text
PHYSICAL SECURITY
      ↓
IDENTITY & ACCESS
      ↓
PERIMETER
      ↓
NETWORK
      ↓
COMPUTE
      ↓
APPLICATION
      ↓
DATA
```

Azure provides security capabilities across these layers.

The goal is not to rely on one security control.

Instead:

```text
CONTROL
+
CONTROL
+
CONTROL
=
DEFENSE IN DEPTH
```

---

# 🌐 Azure Virtual Networks

An **Azure Virtual Network (VNet)** provides private networking for Azure resources.

Think of a VNet as:

```text
AZURE PRIVATE NETWORK
```

Resources can communicate through network structures that administrators design and control.

---

# 🧩 Subnets

A VNet can be divided into smaller network segments called:

# Subnets

Example:

```text
VNET
│
├── Web Subnet
│
├── Application Subnet
│
└── Database Subnet
```

Segmentation helps administrators organize resources and apply security controls.

---

# 🛡️ Network Security Groups — NSGs

A **Network Security Group (NSG)** filters network traffic using security rules.

Rules can control:

```text
Inbound Traffic

Outbound Traffic
```

Conceptually:

```text
NETWORK TRAFFIC
      ↓
NSG RULES
      ↓
ALLOW / DENY
      ↓
AZURE RESOURCE
```

---

# 📋 NSG Rule Concepts

An NSG rule can consider information such as:

```text
Source

Destination

Port

Protocol

Direction

Priority

Allow / Deny
```

At the SC-900 level, focus on the purpose:

> **NSGs control network traffic to and from Azure resources or subnets.**

---

# 🚪 NSG Example

A web server needs HTTPS traffic.

Conceptually:

```text
Internet
   ↓
TCP 443
   ↓
NSG
   ↓
ALLOW
   ↓
Web Server
```

But another unnecessary port might be:

```text
Internet
   ↓
Unneeded Port
   ↓
NSG
   ↓
DENY
```

---

# 🔥 Azure Firewall

**Azure Firewall** is a managed, cloud-based network security service.

It can help control traffic between networks and resources.

Conceptually:

```text
NETWORK A
    ↓
AZURE FIREWALL
    ↓
TRAFFIC INSPECTION / RULES
    ↓
NETWORK B / INTERNET
```

Azure Firewall provides centralized network security capabilities.

---

# 🧠 NSG vs Azure Firewall

Both control network traffic, but they serve different roles.

## NSG

Think:

```text
Traffic Filtering
at Subnet / Network Interface Level
```

## Azure Firewall

Think:

```text
Centralized Managed
Network Firewall
```

Simplified:

```text
NSG
=
Local network traffic rules
```

```text
AZURE FIREWALL
=
Centralized network protection
```

They can be used together as part of defense in depth.

---

# 🌊 DDoS Attacks

A **Distributed Denial-of-Service (DDoS)** attack attempts to overwhelm a service with large amounts of traffic.

Conceptually:

```text
Thousands of Systems
       ↓
Huge Traffic Volume
       ↓
Target Service
       ↓
Service Becomes Unavailable
```

---

# 🛡️ Azure DDoS Protection

Azure provides DDoS protection capabilities to help protect Azure resources from distributed denial-of-service attacks.

At the fundamentals level:

```text
DDoS PROTECTION
=
Protect availability
against large-scale
network attacks
```

This connects to the **Availability** part of the CIA triad.

---

# 🧠 CIA Triad Connection

Recall:

```text
CONFIDENTIALITY

INTEGRITY

AVAILABILITY
```

DDoS attacks primarily threaten:

# Availability

because the attacker attempts to make a service unavailable to legitimate users.

---

# 🏰 Azure Bastion

Administrators sometimes need remote access to Azure virtual machines.

Traditionally, administrators might expose:

```text
RDP — TCP 3389

SSH — TCP 22
```

directly to the internet.

That can increase attack surface.

---

# 🔐 Azure Bastion

**Azure Bastion** provides secure remote connectivity to Azure virtual machines through the Azure platform.

Conceptually:

```text
ADMINISTRATOR
      ↓
AZURE PORTAL / BASTION
      ↓
SECURE CONNECTION
      ↓
VIRTUAL MACHINE
```

A major benefit is reducing the need to expose VM management ports directly to the public internet.

---

# 🧠 Bastion Memory Trick

```text
BASTION
=
Secure way into the VM
without directly exposing
RDP/SSH to the internet
```

---

# 🔑 Azure Key Vault

Applications need sensitive information such as:

```text
Secrets

Encryption Keys

Certificates
```

Storing these directly inside source code or configuration files can create security risks.

---

# 🗝️ Azure Key Vault

**Azure Key Vault** helps securely store and manage sensitive information.

Conceptually:

```text
APPLICATION
      ↓
AUTHORIZED REQUEST
      ↓
AZURE KEY VAULT
      ↓
SECRET / KEY / CERTIFICATE
```

---

# 🚫 Poor Secret Management

Avoid designs such as:

```text
Application Source Code

DatabasePassword = "Password123!"
```

If the code is exposed:

```text
CODE LEAK
   ↓
PASSWORD LEAK
```

Centralized secret management helps reduce this risk.

---

# 🧠 Key Vault Memory Trick

```text
KEY VAULT
=
Keys
Secrets
Certificates
```

---

# 🔒 Resource Locks

Azure resources can sometimes be accidentally:

```text
Deleted

Modified
```

Azure **resource locks** help protect resources from accidental administrative changes.

Common concepts include:

```text
CanNotDelete

ReadOnly
```

---

# 🚫 Delete Lock

Conceptually:

```text
IMPORTANT RESOURCE
      ↓
DELETE LOCK
      ↓
ACCIDENTAL DELETE ATTEMPT
      ↓
BLOCKED
```

A resource lock is not a replacement for proper access control.

It is an additional administrative safeguard.

---

# 📜 Azure Policy

**Azure Policy** helps organizations enforce or assess standards across Azure resources.

Examples:

```text
Require Certain Configurations

Restrict Certain Resource Types

Audit Noncompliant Resources

Enforce Organizational Standards
```

Conceptually:

```text
ORGANIZATION STANDARD
      ↓
AZURE POLICY
      ↓
AZURE RESOURCES
      ↓
COMPLIANT / NONCOMPLIANT
```

---

# 🧠 Azure Policy vs RBAC

This is an important distinction.

## Azure RBAC

```text
WHO can do WHAT?
```

## Azure Policy

```text
WHAT configurations
are allowed or required?
```

Example:

```text
RBAC
=
Taylor can create resources
```

but:

```text
POLICY
=
Resources must follow
company requirements
```

Both can work together.

---

# 🏷️ Policy Example

Contoso requires resources to be deployed only in approved Azure regions.

Conceptually:

```text
USER CREATES RESOURCE
      ↓
AZURE POLICY
      ↓
APPROVED REGION?
   ↙       ↘
 YES       NO
 ↓          ↓
ALLOW     DENY / FLAG
```

The exact effect depends on policy configuration.

---

# 🏗️ Azure Resource Manager

Azure resources are managed through **Azure Resource Manager (ARM)**.

ARM provides the management layer used to:

```text
Create

Update

Delete

Organize

Control Access to
```

Azure resources.

Technologies such as:

```text
Azure RBAC

Azure Policy

Resource Locks

Tags
```

work with Azure resource management.

---

# 🧱 Infrastructure Security Example

Contoso hosts a web application in Azure.

A layered design could include:

```text
INTERNET
   ↓
DDoS Protection
   ↓
Azure Firewall
   ↓
Network Security Group
   ↓
Web Server
   ↓
Application
   ↓
Key Vault
   ↓
Protected Secrets
```

Administrators could connect using:

```text
Azure Bastion
```

while:

```text
Azure Policy
```

helps enforce standards and:

```text
Resource Locks
```

help prevent accidental administrative changes.

This is defense in depth.

---

# 🔐 Identity Still Matters

Infrastructure security does not replace identity security.

A secure Azure environment combines:

```text
MICROSOFT ENTRA
      +
RBAC
      +
NETWORK SECURITY
      +
RESOURCE SECURITY
      +
MONITORING
```

Example:

```text
Administrator
      ↓
Strong Authentication
      ↓
Conditional Access
      ↓
Azure RBAC
      ↓
Azure Resource
      ↓
Network / Resource Controls
```

---

# 🧠 Shared Responsibility Connection

Remember the shared responsibility model.

Microsoft secures the underlying cloud infrastructure, but customers remain responsible for many aspects of:

```text
Identity

Data

Access

Configuration

Applications

Resource Security
```

The exact division depends on whether the service is:

```text
IaaS

PaaS

SaaS
```

---

# 🎯 Exam Focus

Know these relationships:

```text
NSG
=
Allow / deny network traffic
```

```text
AZURE FIREWALL
=
Centralized managed network firewall
```

```text
DDoS PROTECTION
=
Protect availability
from distributed attacks
```

```text
AZURE BASTION
=
Secure VM remote access
without directly exposing
RDP/SSH
```

```text
KEY VAULT
=
Secrets, keys, certificates
```

```text
RESOURCE LOCK
=
Help prevent accidental
deletion or modification
```

```text
AZURE POLICY
=
Assess / enforce
resource standards
```

```text
AZURE RBAC
=
Who can do what
to Azure resources
```

---

# 🧠 Memory Map

```text
NETWORK TRAFFIC
      ↓
NSG / FIREWALL

ATTACK FLOOD
      ↓
DDoS PROTECTION

REMOTE VM ACCESS
      ↓
BASTION

SECRET / KEY
      ↓
KEY VAULT

ACCIDENTAL DELETE
      ↓
RESOURCE LOCK

RESOURCE STANDARD
      ↓
AZURE POLICY

USER PERMISSION
      ↓
AZURE RBAC
```

---

# ❓ Knowledge Check

### 1.

What does an NSG primarily control?

A. Network traffic  
B. Password resets  
C. Email retention  
D. User licenses

---

### 2.

What is Azure Firewall?

A. A managed network security service  
B. A password manager  
C. An identity directory  
D. A compliance report

---

### 3.

Which security concern is most directly associated with DDoS attacks?

A. Availability  
B. User job titles  
C. Licensing  
D. Password length

---

### 4.

What does Azure Bastion help provide?

A. Secure remote access to Azure VMs  
B. Email encryption  
C. User provisioning  
D. Data classification

---

### 5.

What should commonly be stored in Azure Key Vault?

A. Secrets, keys, and certificates  
B. Public marketing images only  
C. Printer drivers  
D. Employee schedules

---

### 6.

What can a resource lock help prevent?

A. Accidental deletion or modification  
B. Phishing emails  
C. Password reuse  
D. DDoS attacks

---

### 7.

What is the main purpose of Azure Policy?

A. Assess and enforce resource standards  
B. Authenticate users  
C. Replace all firewalls  
D. Manage email

---

### 8.

Which statement is correct?

A. Azure RBAC determines who can perform actions on Azure resources  
B. Azure Policy authenticates passwords  
C. Key Vault is a network firewall  
D. Bastion performs access reviews

---

### 9.

Which service can reduce the need to expose RDP or SSH directly to the internet?

A. Azure Bastion  
B. Azure Policy  
C. Microsoft Purview  
D. Access Reviews

---

### 10.

Using NSGs, Azure Firewall, Key Vault, identity controls, and monitoring together demonstrates what principle?

A. Defense in depth  
B. Password reuse  
C. Single-layer security  
D. Anonymous access

---

# ✅ Knowledge Check Answers

```text
1. A — Network traffic

2. A — A managed network security service

3. A — Availability

4. A — Secure remote access to Azure VMs

5. A — Secrets, keys, and certificates

6. A — Accidental deletion or modification

7. A — Assess and enforce resource standards

8. A — Azure RBAC determines who can perform actions on Azure resources

9. A — Azure Bastion

10. A — Defense in depth
```

---

# 📌 Lesson Summary

You learned:

```text
AZURE INFRASTRUCTURE SECURITY
=
Protect networks
+
Protect resources
+
Protect administrative access
+
Protect secrets
+
Enforce standards
```

Key technologies include:

```text
NSGs

Azure Firewall

DDoS Protection

Azure Bastion

Azure Key Vault

Resource Locks

Azure Policy
```

These controls work together with identity and monitoring as part of defense in depth.

---

# 🧪 Lab

Complete:

## 🔵 Lab 09 — Explore Azure Infrastructure Security

The lab is read-only and focuses on locating these controls in Azure.

➡️ **[Lab 09 — Explore Azure Infrastructure Security](../labs/Lab%2009%20—%20Explore%20Azure%20Infrastructure%20Security.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 10 — Microsoft Defender for Cloud

Next you will learn how Microsoft Defender for Cloud helps organizations understand and improve cloud security posture and protect workloads.

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Azure Network Security Groups](https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)
- [Azure Firewall](https://learn.microsoft.com/en-us/azure/firewall/overview)
- [Azure DDoS Protection](https://learn.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview)
- [Azure Bastion](https://learn.microsoft.com/en-us/azure/bastion/bastion-overview)
- [Azure Key Vault](https://learn.microsoft.com/en-us/azure/key-vault/general/overview)
- [Azure Resource Locks](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/lock-resources)
- [Azure Policy](https://learn.microsoft.com/en-us/azure/governance/policy/overview)

---

# 📚 Course Navigation

⬅️ **Project 01 — Secure an Organization's Identity Environment**

🧪 **[Lab 09](../labs/Lab%2009%20—%20Explore%20Azure%20Infrastructure%20Security.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
