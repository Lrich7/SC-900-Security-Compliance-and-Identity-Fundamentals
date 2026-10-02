# 🔵 Lab 09 — Explore Azure Infrastructure Security

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 09 — Azure Infrastructure Security  
**Lab Type:** 🔵 Explore the Tool  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to locate and recognize:

- Virtual Networks
- Subnets
- Network Security Groups
- Azure Firewall
- DDoS protection capabilities
- Azure Bastion
- Azure Key Vault
- Resource Locks
- Azure Policy
- Access Control (IAM)
- The relationship among Azure infrastructure security controls

---

# ⚠️ Production Safety

This is a read-only exploration lab.

Do not:

```text
Change NSG Rules

Create Firewall Rules

Expose VM Ports

Delete Resources

Add or Remove Locks

Modify Azure Policy

Change RBAC Assignments

View or Copy Production Secrets
```

unless specifically authorized.

If your organization does not provide Azure portal access, complete the conceptual exercises instead.

---

# 📋 What You Need

Ideally:

```text
Microsoft Work/School Account

Authorized Azure Portal Access

Permission to View
at Least One Azure Resource
```

Open:

```text
https://portal.azure.com
```

Some services may not exist in your tenant or subscription.

That is okay.

The goal is to learn:

```text
WHAT IT IS

WHERE IT LIVES

WHAT IT PROTECTS
```

---

# 🚀 Part 1 — Explore the Azure Portal

Open the Azure portal.

Use the search bar to locate:

```text
Virtual networks
```

Do not create one.

Observe the page and identify whether your authorized environment contains any VNets.

---

# 🌐 Part 2 — Explore a Virtual Network

If you are authorized to view an existing VNet, open it.

Look for:

```text
Address Space

Subnets

Connected Devices / Interfaces

Security-related Settings
```

Do not record real production IP ranges in a public repository.

---

# 🧩 Part 3 — Explore Subnets

Locate:

```text
Subnets
```

Conceptually, a VNet might be organized as:

```text
VNET
│
├── Web Subnet
├── Application Subnet
└── Database Subnet
```

Why might segmentation be useful?

```text
____________________________________

____________________________________
```

---

# 🛡️ Part 4 — Find Network Security Groups

Use Azure search:

```text
Network security groups
```

If an NSG is available and you have permission to view it, open it.

Look for:

```text
Inbound Security Rules

Outbound Security Rules
```

Do not change any rules.

---

# 📋 Part 5 — Read an NSG Rule

Look for fields such as:

```text
Priority

Source

Destination

Port

Protocol

Action
```

Do not copy sensitive production information.

Complete this conceptual rule:

```text
Direction:
Inbound

Protocol:
TCP

Destination Port:
443

Action:
Allow
```

What common service uses TCP 443?

```text
______________________________
```

---

# 🚪 Part 6 — NSG Scenario

A public web server needs HTTPS access but does not need database traffic directly from the internet.

Design the concept:

```text
Internet → TCP 443 → __________

Internet → Database Port → __________
```

Choose:

```text
ALLOW

DENY
```

---

# 🔥 Part 7 — Find Azure Firewall

Search for:

```text
Firewalls
```

or:

```text
Azure Firewall
```

You may not have an Azure Firewall deployed.

That is fine.

Read the service description and identify its purpose.

Complete:

```text
Azure Firewall
=
____________________________________

____________________________________
```

---

# 🧠 NSG vs Firewall

Complete:

```text
NSG
=
____________________________________
```

```text
Azure Firewall
=
____________________________________
```

Remember:

```text
NSG
=
Traffic filtering close to
subnets/network interfaces
```

```text
Azure Firewall
=
Centralized managed
network security
```

---

# 🌊 Part 8 — Find DDoS Protection

Search for:

```text
DDoS
```

You may see Azure DDoS-related capabilities or protection plans depending on your environment.

Do not configure anything.

Which CIA triad principle does DDoS protection most directly support?

```text
Confidentiality

Integrity

Availability
```

Answer:

```text
______________________________
```

---

# 🏰 Part 9 — Find Azure Bastion

Search:

```text
Bastion
```

If none is deployed, read the service overview.

Complete:

```text
Azure Bastion helps administrators
connect securely to:

______________________________
```

Why is this preferable to unnecessarily exposing RDP/SSH directly to the internet?

```text
____________________________________

____________________________________
```

---

# 🔑 Part 10 — Explore Azure Key Vault

Search:

```text
Key vaults
```

If you can view an existing Key Vault, open only the general resource overview.

Do **not** open or copy production secret values.

Identify the three major things associated with Key Vault:

```text
1. __________________________

2. __________________________

3. __________________________
```

Hint:

```text
Secrets

Keys

Certificates
```

---

# 🚫 Part 11 — Secret Management Scenario

A developer writes:

```text
database_password = "Contoso123!"
```

directly in application source code.

What is wrong with this design?

```text
____________________________________

____________________________________
```

What Azure service could help?

```text
______________________________
```

---

# 🔒 Part 12 — Find Resource Locks

If you have permission to view an Azure resource, look for:

```text
Locks
```

Do not create or remove one.

Common lock concepts include:

```text
Delete / CanNotDelete

ReadOnly
```

---

# 🧠 Lock Scenario

Contoso has a critical production resource.

Administrators want to reduce accidental deletion.

Which control fits best?

```text
Azure Firewall

Resource Lock

MFA

Access Review
```

Answer:

```text
______________________________
```

---

# 📜 Part 13 — Explore Azure Policy

Search:

```text
Policy
```

Open Azure Policy if available.

Look for concepts such as:

```text
Definitions

Assignments

Compliance
```

Do not create or modify a policy.

---

# 🧠 Policy Scenario

Contoso requires Azure resources to follow approved organizational standards.

Which technology fits?

```text
______________________________
```

Complete:

```text
Azure Policy
=
____________________________________

____________________________________
```

---

# 👤 Part 14 — Find Access Control (IAM)

Open an Azure resource you are authorized to view.

Look for:

```text
Access control (IAM)
```

Do not change role assignments.

Recall:

```text
Azure RBAC
=
WHO can do WHAT
at WHAT scope
```

---

# 🧠 RBAC vs Policy

Match:

## Scenario 1

Taylor can view a virtual machine.

```text
Azure RBAC / Azure Policy
```

Answer:

```text
______________________________
```

## Scenario 2

All new resources must follow an approved configuration standard.

```text
Azure RBAC / Azure Policy
```

Answer:

```text
______________________________
```

---

# 🧱 Part 15 — Defense-in-Depth Challenge

Contoso hosts a web application.

Choose the best technology for each problem.

Options:

```text
NSG

Azure Firewall

DDoS Protection

Azure Bastion

Azure Key Vault

Resource Lock

Azure Policy

Azure RBAC
```

## Problem 1

Control inbound and outbound subnet/resource traffic.

```text
______________________________
```

## Problem 2

Provide centralized managed network filtering.

```text
______________________________
```

## Problem 3

Protect service availability from large distributed attacks.

```text
______________________________
```

## Problem 4

Provide secure administrative connectivity to VMs.

```text
______________________________
```

## Problem 5

Protect application secrets and encryption keys.

```text
______________________________
```

## Problem 6

Help prevent accidental deletion.

```text
______________________________
```

## Problem 7

Enforce or assess resource configuration standards.

```text
______________________________
```

## Problem 8

Control which identity can manage an Azure resource.

```text
______________________________
```

---

# 🏗️ Part 16 — Build the Architecture

Fill in the security controls.

```text
                    INTERNET
                       │
                       ▼
              __________________
              Protect Availability
                       │
                       ▼
              __________________
              Central Network
                 Protection
                       │
                       ▼
              __________________
               Traffic Rules
                       │
                       ▼
                  WEB SERVER
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
      __________________   __________________
       Secure Admin       Protect Secrets
          Access
```

Choices:

```text
DDoS Protection

Azure Firewall

NSG

Azure Bastion

Azure Key Vault
```

---

# 🔐 Part 17 — Add Identity

Infrastructure security should also include identity controls.

Complete:

```text
ADMINISTRATOR
      ↓
Strong Authentication
      ↓
Conditional Access
      ↓
____________________
Controls Azure Permissions
      ↓
AZURE RESOURCE
```

Answer:

```text
______________________________
```

---

# 🧠 Part 18 — Shared Responsibility

Microsoft operates the cloud infrastructure.

Does that mean customers no longer need to configure:

```text
Identity

Permissions

Network Rules

Data Protection

Application Security
```

Answer:

```text
YES / NO
```

Explain:

```text
____________________________________

____________________________________
```

---

# 🗺️ Part 19 — Build Your Azure Security Map

Complete:

| Technology | Main Purpose |
|---|---|
| NSG | __________________________ |
| Azure Firewall | __________________________ |
| DDoS Protection | __________________________ |
| Azure Bastion | __________________________ |
| Azure Key Vault | __________________________ |
| Resource Lock | __________________________ |
| Azure Policy | __________________________ |
| Azure RBAC | __________________________ |

---

# ✅ Suggested Answers

## Segmentation

Segmentation can help organize workloads and apply different network controls to different parts of an environment.

## NSG Rule

```text
TCP 443
=
HTTPS
```

## Web Server Scenario

```text
Internet → TCP 443 → ALLOW

Internet → Database Port → DENY
```

assuming direct database access from the internet is not required.

## DDoS

```text
Availability
```

## Bastion

```text
Azure Virtual Machines
```

It can reduce the need to expose RDP/SSH management ports directly to the public internet.

## Key Vault

```text
Secrets

Keys

Certificates
```

## Secret Scenario

Hard-coded credentials can be exposed if source code or configuration is leaked.

Use:

```text
Azure Key Vault
```

## Resource Lock

```text
Resource Lock
```

## RBAC vs Policy

```text
Scenario 1
=
Azure RBAC

Scenario 2
=
Azure Policy
```

## Defense-in-Depth Challenge

```text
1. NSG

2. Azure Firewall

3. DDoS Protection

4. Azure Bastion

5. Azure Key Vault

6. Resource Lock

7. Azure Policy

8. Azure RBAC
```

## Architecture

```text
                    INTERNET
                       │
                       ▼
                DDoS Protection
                       │
                       ▼
                 Azure Firewall
                       │
                       ▼
                      NSG
                       │
                       ▼
                  WEB SERVER
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
        Azure Bastion       Azure Key Vault
```

## Identity

```text
Azure RBAC
```

## Shared Responsibility

```text
NO
```

Customers still have responsibilities for identities, permissions, data, configurations, and workloads depending on the cloud service model.

---

# 🎓 What You Should Have Learned

You should now understand:

```text
NSG
=
Traffic rules
```

```text
FIREWALL
=
Centralized network protection
```

```text
DDoS
=
Availability protection
```

```text
BASTION
=
Secure VM administration
```

```text
KEY VAULT
=
Secrets / keys / certificates
```

```text
LOCK
=
Administrative safeguard
```

```text
POLICY
=
Resource standards
```

```text
RBAC
=
Resource permissions
```

Together, these technologies create layers of Azure infrastructure security.

---

# ✅ Lab Completion Checklist

- [ ] I can explain a VNet and subnet.
- [ ] I know what an NSG does.
- [ ] I know what Azure Firewall does.
- [ ] I know what DDoS Protection protects.
- [ ] I know what Azure Bastion does.
- [ ] I know what belongs in Key Vault.
- [ ] I know what resource locks do.
- [ ] I can distinguish Azure Policy from Azure RBAC.
- [ ] I understand defense in depth.
- [ ] I understand that cloud security is still a shared responsibility.

---

# ➡️ Next

Continue to:

## 📘 Lesson 10 — Microsoft Defender for Cloud

Next you will explore how Microsoft helps organizations:

```text
Assess Security Posture

Find Recommendations

Improve Cloud Security

Protect Workloads
```

---

# 🔗 Official Microsoft Resources

- [Azure Portal](https://portal.azure.com/)
- [Network Security Groups](https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)
- [Azure Firewall](https://learn.microsoft.com/en-us/azure/firewall/overview)
- [Azure DDoS Protection](https://learn.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview)
- [Azure Bastion](https://learn.microsoft.com/en-us/azure/bastion/bastion-overview)
- [Azure Key Vault](https://learn.microsoft.com/en-us/azure/key-vault/general/overview)
- [Azure Policy](https://learn.microsoft.com/en-us/azure/governance/policy/overview)

---

# 📚 Course Navigation

⬅️ **[Lesson 09 — Azure Infrastructure Security](../lessons/%F0%9F%93%98%20Lesson%2009%20%E2%80%94%20Azure%20Infrastructure%20Security.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
