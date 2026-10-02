# 🏗️ Project 02 --- Build a Microsoft Security Strategy

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Project:** 02\
**Covers:** Lessons 09--13\
**Project Type:** 🏗️ Security Architecture & Strategy Challenge\
**Difficulty:** Beginner / Intermediate\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🎯 Project Goal

In this project, you will design a Microsoft security strategy for a
fictional organization.

You will combine concepts from:

``` text
📘 Lesson 09 — Azure Infrastructure Security

📘 Lesson 10 — Microsoft Defender for Cloud

📘 Lesson 11 — Microsoft Defender XDR

📘 Lesson 12 — Microsoft Defender Security Services

📘 Lesson 13 — Microsoft Sentinel
```

The goal is not to memorize product names.

The goal is to answer:

``` text
WHAT ARE WE PROTECTING?

WHAT THREATS ARE WE WORRIED ABOUT?

WHICH MICROSOFT SECURITY
CAPABILITY FITS THE PROBLEM?

HOW DO THE TOOLS WORK TOGETHER?
```

------------------------------------------------------------------------

# 🏢 Scenario --- Contoso Manufacturing

You are an IT security specialist for:

# Contoso Manufacturing

Contoso has approximately:

``` text
150 Employees

3 Offices

20 Remote Employees

10 IT / Administrative Users

15 Contractors
```

The organization uses:

``` text
Microsoft 365

Microsoft Entra ID

Windows Laptops

Microsoft Teams

Exchange Online

SharePoint

OneDrive

Azure

Several SaaS Applications

On-Premises Windows Servers

AWS for One Business Application
```

------------------------------------------------------------------------

# 🖥️ Current Azure Environment

Contoso runs:

``` text
12 Azure Virtual Machines

3 Azure Storage Accounts

2 Azure SQL Databases

1 Public-Facing Web Application

Several Virtual Networks

Multiple Subnets

Azure Key Vault

Hybrid Connectivity
```

------------------------------------------------------------------------

# ⚠️ Current Security Problems

An internal review identifies several concerns.

``` text
1. Some Azure VMs have management ports
   exposed to the internet.

2. Administrators frequently connect
   directly to VMs using RDP.

3. Application secrets are stored
   inside configuration files.

4. Azure resources are sometimes
   created without standard security settings.

5. Security has no simple way to
   measure overall cloud security posture.

6. Employees regularly receive
   phishing emails.

7. Malicious links have reached users.

8. Security has limited visibility
   into endpoint attacks.

9. The organization has hybrid
   Active Directory identities.

10. Employees use unapproved
    cloud applications.

11. Security alerts exist across
    several different tools.

12. Analysts struggle to understand
    whether alerts are connected.

13. Firewall, server, Azure, AWS,
    identity, and Defender logs are
    spread across multiple systems.

14. Incident response contains
    many repetitive manual steps.

15. The security team has no
    centralized threat-hunting process.
```

------------------------------------------------------------------------

# 🧠 Your Role

Management asks you to design a Microsoft security strategy.

You are **not** being asked to configure the environment.

You are being asked to create the architecture and explain:

``` text
WHAT SHOULD BE USED

WHY IT SHOULD BE USED

WHAT PROBLEM IT SOLVES

HOW THE COMPONENTS CONNECT
```

------------------------------------------------------------------------

# 🧱 Phase 1 --- Defense in Depth

Before choosing products, design the security layers.

Complete:

``` text
IDENTITY
      ↓
______________________________

NETWORK
      ↓
______________________________

COMPUTE / ENDPOINT
      ↓
______________________________

APPLICATION
      ↓
______________________________

DATA / SECRETS
      ↓
______________________________

MONITORING / DETECTION
      ↓
______________________________
```

For each layer, identify at least one control or Microsoft security
capability.

------------------------------------------------------------------------

# 🌐 Phase 2 --- Secure Azure Network Traffic

Contoso has several Azure virtual machines.

Some should only accept traffic from specific systems.

Which Azure security control would you use to control inbound and
outbound traffic at the subnet or network-interface level?

``` text
Technology:
____________________________________
```

Why?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔥 Phase 3 --- Centralized Network Protection

Contoso wants centralized network filtering for Azure traffic.

Which service fits?

``` text
Technology:
____________________________________
```

What is the difference between this service and an NSG?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🌊 Phase 4 --- Protect Availability

The public web application must remain available.

Management is concerned about distributed denial-of-service attacks.

Which Azure capability addresses this risk?

``` text
Technology:
____________________________________
```

Which part of the CIA triad is most directly involved?

``` text
Confidentiality / Integrity / Availability
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🖥️ Phase 5 --- Secure Administrative VM Access

Administrators currently expose:

``` text
RDP — TCP 3389
```

to the internet for management.

Design a safer approach.

``` text
Technology:
____________________________________
```

Why is this preferable to unnecessarily exposing RDP/SSH publicly?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔐 Phase 6 --- Protect Application Secrets

A developer stores:

``` text
Database Password

API Secret

Application Certificate
```

inside an application configuration file.

Which Azure service should be considered for securely storing these
types of secrets?

``` text
Technology:
____________________________________
```

What can it store?

``` text
[ ] Secrets

[ ] Keys

[ ] Certificates
```

------------------------------------------------------------------------

# 📏 Phase 7 --- Enforce Azure Standards

Contoso wants requirements such as:

``` text
Only approved Azure regions may be used.

Resources must follow
required configurations.
```

Which capability fits?

``` text
Technology:
____________________________________
```

Complete:

``` text
Azure RBAC
=
WHO can do WHAT
```

``` text
Azure Policy
=
____________________________________
```

------------------------------------------------------------------------

# 🔒 Phase 8 --- Prevent Accidental Resource Changes

A critical production resource should not be accidentally deleted.

Which Azure capability can help?

``` text
Technology:
____________________________________
```

Which lock type is most directly associated with preventing deletion?

``` text
______________________________
```

------------------------------------------------------------------------

# ☁️ Phase 9 --- Improve Cloud Security Posture

Management asks:

> How secure is our cloud environment, and what should we improve?

Which Microsoft product fits?

``` text
Product:
____________________________________
```

Which major capability focuses on improving cloud security posture?

``` text
CSPM / CWPP
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 📋 Phase 10 --- Security Recommendations

Defender for Cloud identifies:

``` text
VM management ports
exposed to the internet.
```

Is this primarily:

``` text
A. A security recommendation / posture finding

B. Proof that an attacker
   already compromised the VM
```

Answer:

``` text
______________________________
```

What should the security team do with recommendations?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 📊 Phase 11 --- Measure Cloud Posture

Management wants a high-level indicator to help track cloud security
posture and improvement.

Which Defender for Cloud concept fits?

``` text
Feature:
____________________________________
```

Does a high score guarantee the environment cannot be compromised?

``` text
YES / NO
```

Explain:

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🛡️ Phase 12 --- Protect Cloud Workloads

Contoso wants enhanced threat protection for supported cloud workloads
such as:

``` text
Servers

Storage

Databases

Containers
```

Which Defender for Cloud concept fits?

``` text
CSPM / CWPP
```

Answer:

``` text
______________________________
```

What provides workload-specific enhanced protections?

``` text
____________________________________
```

------------------------------------------------------------------------

# 📧 Phase 13 --- Protect Email

Employees receive:

``` text
Phishing Emails

Malicious Links

Malicious Attachments
```

Which Microsoft Defender product fits?

``` text
Product:
____________________________________
```

Match:

``` text
Malicious URL
→ __________________________

Malicious Attachment
→ __________________________
```

------------------------------------------------------------------------

# 💻 Phase 14 --- Protect Endpoints

Contoso wants to detect and investigate suspicious activity on company
laptops.

Which product fits?

``` text
Product:
____________________________________
```

What does EDR stand for?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🩹 Phase 15 --- Find Endpoint Vulnerabilities

Security wants to identify:

``` text
Known Vulnerabilities

Outdated Software

Risky Endpoint Configurations
```

Which Microsoft security capability fits?

``` text
Capability:
____________________________________
```

Why is vulnerability prioritization useful?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 👤 Phase 16 --- Detect Identity Threats

Contoso uses hybrid Active Directory.

Security is concerned about:

``` text
Credential Theft

Reconnaissance

Suspicious Identity Activity

Lateral Movement
```

Which product fits?

``` text
Product:
____________________________________
```

------------------------------------------------------------------------

# ☁️ Phase 17 --- Discover Shadow IT

Employees are using unapproved SaaS applications to store company data.

Which product fits?

``` text
Product:
____________________________________
```

What is this behavior called?

``` text
______________________________
```

What does CASB stand for?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🚨 Phase 18 --- Correlate the Attack

An employee receives a phishing email.

Then:

``` text
1. User clicks malicious link

2. Malware executes on laptop

3. Credentials are stolen

4. Suspicious identity activity occurs

5. Attacker accesses cloud applications
```

Different Defender services detect different stages.

Which platform helps correlate these signals into a broader incident?

``` text
Platform:
____________________________________
```

------------------------------------------------------------------------

# 🧩 Phase 19 --- Build the XDR Attack Story

Fill in:

``` text
EMAIL
      ↓
______________________________
      ↓
ENDPOINT
      ↓
______________________________
      ↓
IDENTITY
      ↓
______________________________
      ↓
CLOUD APPLICATION
      ↓
______________________________
      ↓
ALL SIGNALS
      ↓
______________________________
      ↓
INCIDENT
```

------------------------------------------------------------------------

# 🚨 Phase 20 --- Alert vs Incident

Complete:

``` text
ALERT
=
____________________________________
```

``` text
INCIDENT
=
____________________________________
```

Why is grouping related alerts useful?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔎 Phase 21 --- Threat Hunting in Defender

A security analyst wants to proactively search Microsoft Defender
security data for suspicious activity.

Which capability fits?

``` text
Capability:
____________________________________
```

Which query language is commonly used?

``` text
______________________________
```

------------------------------------------------------------------------

# 📊 Phase 22 --- Centralize Security Data

Contoso has security data from:

``` text
Microsoft Entra ID

Microsoft Defender

Azure

AWS

Windows Servers

Firewalls
```

Management wants a central SIEM.

Which Microsoft solution fits?

``` text
Solution:
____________________________________
```

What does SIEM stand for?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🔌 Phase 23 --- Connect the Data

How does Sentinel bring supported security data into the platform?

``` text
Feature:
____________________________________
```

Complete:

``` text
DATA SOURCE
      ↓
______________________________
      ↓
MICROSOFT SENTINEL
```

------------------------------------------------------------------------

# 🔎 Phase 24 --- Detect Suspicious Activity

Sentinel has received security data.

Which Sentinel capability can detect suspicious patterns in that data?

``` text
Capability:
____________________________________
```

Conceptually:

``` text
SECURITY DATA
      ↓
______________________________
      ↓
ALERT
      ↓
INCIDENT
```

------------------------------------------------------------------------

# 🕵️ Phase 25 --- Hunt Across SIEM Data

The SOC wants to proactively search centralized security data.

Which Sentinel capability fits?

``` text
Capability:
____________________________________
```

What language is commonly used to query the data?

``` text
______________________________
```

------------------------------------------------------------------------

# 📊 Phase 26 --- Visualize Security Data

Management wants visual dashboards showing security trends.

Which Sentinel capability fits?

``` text
Capability:
____________________________________
```

------------------------------------------------------------------------

# 🌐 Phase 27 --- Threat Intelligence

Sentinel sees an internal system communicating with a suspicious
external IP address.

Which type of information could provide context that the IP is
associated with known malicious activity?

``` text
Capability:
____________________________________
```

------------------------------------------------------------------------

# 🤖 Phase 28 --- Automate Incident Response

When a high-severity incident appears, Contoso wants to:

``` text
Automatically notify IT

Create a ticket

Gather incident information
```

Which Sentinel concepts fit?

``` text
Trigger / coordination:
____________________________________
```

``` text
Automated workflow:
____________________________________
```

What Microsoft technology underlies Sentinel playbooks?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🧠 Phase 29 --- SIEM vs SOAR

Complete:

``` text
SIEM
=
____________________________________

____________________________________
```

``` text
SOAR
=
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔗 Phase 30 --- Sentinel + Defender XDR

Explain the difference.

## Microsoft Defender XDR

``` text
Main purpose:
____________________________________

____________________________________
```

## Microsoft Sentinel

``` text
Main purpose:
____________________________________

____________________________________
```

How can they work together?

``` text
____________________________________

____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🏗️ Phase 31 --- Build the Security Architecture

Complete this architecture.

``` text
                        CONTOSO SECURITY
                               │
         ┌─────────────────────┼─────────────────────┐
         │                     │                     │
         ▼                     ▼                     ▼
      AZURE                MICROSOFT 365          ENDPOINTS
         │                     │                     │
         ▼                     ▼                     ▼
 __________________   __________________   __________________
         │                     │                     │
         └──────────────┬──────┴──────────────┬──────┘
                        │                     │
                        ▼                     ▼
                 IDENTITY SECURITY      CLOUD APP SECURITY
                        │                     │
                        ▼                     ▼
                 __________________   __________________
                        │                     │
                        └──────────┬──────────┘
                                   ▼
                           __________________
                                   │
                                   ▼
                                INCIDENT
                                   │
                                   ▼
                           __________________
                                   │
                      ┌────────────┼────────────┐
                      ▼            ▼            ▼
                  ANALYTICS      HUNTING    AUTOMATION
                                                 │
                                                 ▼
                                         __________________
```

Use appropriate technologies from Lessons 09--13.

------------------------------------------------------------------------

# 🗺️ Phase 32 --- Build the Product Map

Complete:

  Security Need                    Microsoft Technology
  -------------------------------- ------------------------------------------------------
  Azure traffic filtering          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Central Azure network firewall   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  DDoS protection                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Secure VM administration         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Secrets / keys / certificates    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Azure configuration standards    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud security posture           \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud workload protection        \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Endpoint security                \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Email security                   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identity threat detection        \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud app security               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cross-domain XDR                 \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  SIEM / SOAR                      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Automated Sentinel workflow      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 🎯 Phase 33 --- Prioritize the Risks

Contoso can only address five items immediately.

Choose **five** from:

``` text
Public RDP Exposure

Application Secrets in Config Files

Phishing

Endpoint Visibility

Identity Threat Visibility

Shadow IT

Cloud Posture

Centralized SIEM

Incident Automation

Threat Hunting
```

Your priorities:

``` text
1. __________________________________

2. __________________________________

3. __________________________________

4. __________________________________

5. __________________________________
```

For each priority, explain why it should be addressed early.

------------------------------------------------------------------------

# 🧠 Phase 34 --- Zero Trust Connection

Connect your strategy to the three Zero Trust principles.

## Verify Explicitly

Which technologies support this principle?

``` text
____________________________________

____________________________________
```

## Use Least Privilege

Which controls support this principle?

``` text
____________________________________

____________________________________
```

## Assume Breach

Which technologies support this principle?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🧱 Phase 35 --- Defense in Depth Review

Fill in at least one security capability for each layer.

  Layer            Security Capability
  ---------------- ------------------------------------------------------
  Identity         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Endpoint         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Network          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Application      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Data / Secrets   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud Posture    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Detection        \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Response         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 📝 Phase 36 --- Executive Summary

Management does not want a list of product names.

Write a short **5--8 sentence executive summary** explaining your
strategy in plain language.

Your summary should explain:

``` text
What the major risks are

How Azure will be protected

How users/endpoints/email will be protected

How attacks will be detected

How security data will be centralized

How incidents will be investigated

How response will become more efficient
```

Write your summary:

``` text
____________________________________

____________________________________

____________________________________

____________________________________

____________________________________

____________________________________

____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🏆 Final Architecture Challenge

Create your final security flow.

Use:

``` text
Azure Infrastructure Security

Defender for Cloud

Defender for Endpoint

Defender for Office 365

Defender for Identity

Defender for Cloud Apps

Defender XDR

Microsoft Sentinel

Automation Rules

Playbooks
```

Build:

``` text
PREVENT
      ↓
PROTECT
      ↓
DETECT
      ↓
CORRELATE
      ↓
INVESTIGATE
      ↓
AUTOMATE
      ↓
RESPOND
```

For each stage, identify the Microsoft technologies that contribute.

------------------------------------------------------------------------

# ✅ Suggested Solution

There is more than one reasonable architecture. The following is a
sample.

------------------------------------------------------------------------

# 🧱 Azure Infrastructure

``` text
Network Security Groups
=
Subnet / NIC traffic filtering

Azure Firewall
=
Centralized network filtering

Azure DDoS Protection
=
Availability protection

Azure Bastion
=
Secure VM administrative access

Azure Key Vault
=
Secrets, keys, certificates

Azure Policy
=
Resource configuration standards

Resource Locks
=
Protection against accidental changes
```

------------------------------------------------------------------------

# ☁️ Cloud Security

``` text
Microsoft Defender for Cloud
=
Cloud security posture
and workload protection

CSPM
=
Assess and improve posture

Cloud Secure Score
=
Track posture

Security Recommendations
=
Guide remediation

CWPP / Defender Plans
=
Protect supported workloads
```

------------------------------------------------------------------------

# 🛡️ Defender Security Services

``` text
Defender for Endpoint
=
Endpoint security / EDR

Defender for Office 365
=
Email and collaboration security

Safe Links
=
URL protection

Safe Attachments
=
Attachment protection

Defender for Identity
=
Identity threat detection

Defender for Cloud Apps
=
Cloud application visibility,
CASB, and Shadow IT
```

------------------------------------------------------------------------

# 🔗 XDR

``` text
EMAIL
      ↓
Defender for Office 365

ENDPOINT
      ↓
Defender for Endpoint

IDENTITY
      ↓
Defender for Identity

CLOUD APP
      ↓
Defender for Cloud Apps

ALL SIGNALS
      ↓
Microsoft Defender XDR
      ↓
Correlated Incident
      ↓
Investigation / Response
```

------------------------------------------------------------------------

# 📊 Sentinel

``` text
DATA SOURCES
      ↓
DATA CONNECTORS
      ↓
MICROSOFT SENTINEL
      ↓
ANALYTICS
      ↓
INCIDENT
      ↓
INVESTIGATION / HUNTING
      ↓
AUTOMATION RULE
      ↓
PLAYBOOK
      ↓
RESPONSE
```

------------------------------------------------------------------------

# 🧠 SIEM / SOAR

``` text
SIEM
=
Collect
Analyze
Detect
Investigate
```

``` text
SOAR
=
Orchestrate
Automate
Respond
```

------------------------------------------------------------------------

# 🗺️ Sample Product Map

  Security Need                    Microsoft Technology
  -------------------------------- ---------------------------
  Azure traffic filtering          Network Security Group
  Central Azure network firewall   Azure Firewall
  DDoS protection                  Azure DDoS Protection
  Secure VM administration         Azure Bastion
  Secrets / keys / certificates    Azure Key Vault
  Azure configuration standards    Azure Policy
  Cloud security posture           Defender for Cloud / CSPM
  Cloud workload protection        Defender for Cloud / CWPP
  Endpoint security                Defender for Endpoint
  Email security                   Defender for Office 365
  Identity threat detection        Defender for Identity
  Cloud app security               Defender for Cloud Apps
  Cross-domain XDR                 Microsoft Defender XDR
  SIEM / SOAR                      Microsoft Sentinel
  Automated Sentinel workflow      Playbook

------------------------------------------------------------------------

# 🧠 Sample Zero Trust Mapping

## Verify Explicitly

``` text
Microsoft Entra authentication

MFA

Conditional Access

Identity security signals
```

## Use Least Privilege

``` text
Azure RBAC

Microsoft Entra Roles

PIM

Scoped permissions
```

## Assume Breach

``` text
Defender XDR

Defender for Endpoint

Defender for Identity

Defender for Cloud

Microsoft Sentinel

Threat Hunting
```

------------------------------------------------------------------------

# 🏆 Sample Final Architecture

``` text
                         USERS
                           │
                           ▼
                  MICROSOFT 365 / EMAIL
                           │
                           ▼
                 Defender for Office 365
                           │
                           │
      ┌────────────────────┼─────────────────────┐
      │                    │                     │
      ▼                    ▼                     ▼
 ENDPOINTS             IDENTITIES            CLOUD APPS
      │                    │                     │
      ▼                    ▼                     ▼
 Defender for        Defender for         Defender for
   Endpoint             Identity            Cloud Apps
      │                    │                     │
      └────────────────────┼─────────────────────┘
                           ▼
                   MICROSOFT DEFENDER XDR
                           │
                           ▼
                    CORRELATED INCIDENT
                           │
                           │
       AZURE / AWS / FIREWALL / SERVER LOGS
                           │
                           ▼
                   MICROSOFT SENTINEL
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
          ANALYTICS      HUNTING     AUTOMATION
                                        │
                                        ▼
                                    PLAYBOOK
                                        │
                                        ▼
                                     RESPONSE
```

Azure resources are additionally protected by:

``` text
NSGs

Azure Firewall

DDoS Protection

Azure Bastion

Azure Key Vault

Azure Policy

Resource Locks

Defender for Cloud
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

You should now be able to look at a security problem and select the
appropriate layer or Microsoft capability.

``` text
AZURE NETWORK
→ NSG / Azure Firewall

AZURE POSTURE
→ Defender for Cloud

DEVICE
→ Defender for Endpoint

EMAIL
→ Defender for Office 365

IDENTITY THREAT
→ Defender for Identity

CLOUD APP
→ Defender for Cloud Apps

CROSS-DOMAIN ATTACK
→ Defender XDR

CENTRAL SECURITY DATA
→ Microsoft Sentinel

AUTOMATED RESPONSE
→ Automation Rules + Playbooks
```

More importantly, you should understand that these technologies are not
isolated.

They form layers of a broader security architecture.

------------------------------------------------------------------------

# ✅ Project Completion Checklist

-   [ ] I can explain defense in depth.
-   [ ] I can select Azure infrastructure security controls.
-   [ ] I can explain Defender for Cloud.
-   [ ] I can distinguish CSPM from CWPP.
-   [ ] I can select Defender for Endpoint.
-   [ ] I can select Defender for Office 365.
-   [ ] I can select Defender for Identity.
-   [ ] I can select Defender for Cloud Apps.
-   [ ] I understand Defender XDR correlation.
-   [ ] I can explain alerts vs incidents.
-   [ ] I can explain Microsoft Sentinel.
-   [ ] I can explain SIEM.
-   [ ] I can explain SOAR.
-   [ ] I understand data connectors.
-   [ ] I understand analytics rules.
-   [ ] I understand threat hunting.
-   [ ] I can distinguish automation rules from playbooks.
-   [ ] I can explain how Sentinel and Defender XDR work together.
-   [ ] I can explain the security strategy to management.

------------------------------------------------------------------------

# 🎉 Project Complete

You have completed:

# 🏗️ Project 02 --- Build a Microsoft Security Strategy

You have now finished the course's:

# 🛡️ Microsoft Security Solutions

section.

------------------------------------------------------------------------

# ➡️ Next

Continue to:

## 📘 Lesson 14 --- Microsoft Purview & Compliance

The next section shifts from protecting identities, devices, workloads,
and infrastructure to protecting and governing organizational data.

You will begin exploring:

``` text
Microsoft Purview

Compliance

Data Governance

Information Protection

Data Loss Prevention

Risk Management
```

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **📘 Lesson 13 --- Microsoft Sentinel**

📘 **Lesson 14 --- Microsoft Purview & Compliance**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](README.md)**

🏠 **[Return to Main README](../README.md)**
