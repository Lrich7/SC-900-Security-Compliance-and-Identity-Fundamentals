# 📖 SC-900 Glossary

A quick alphabetical reference for important **Security, Compliance,
Identity, Azure, Defender, Sentinel, and Purview** terminology.

------------------------------------------------------------------------

## A

### Access Review

Microsoft Entra Identity Governance capability used to periodically
review whether users still require access.

### Agent Identity

A digital identity associated with an AI agent or agent-based workload.

### Alert

A notification that suspicious or potentially malicious activity has
been detected.

### Authentication

The process of proving identity.

``` text
Authentication
→ Who are you?
```

### Authentication Strength

A Microsoft Entra control used to specify which authentication methods
or combinations satisfy an access requirement.

### Authorization

The process of determining what an authenticated identity is allowed to
access or do.

``` text
Authorization
→ What can you do?
```

### Azure Bastion

Azure service that provides secure connectivity to virtual machines
without requiring public RDP or SSH exposure.

### Azure Firewall

Managed Azure network-security service used to centrally control network
traffic.

### Azure Policy

Azure governance service used to evaluate and enforce organizational
standards on Azure resources.

### Azure RBAC

Role-Based Access Control used to control access to Azure resources.

------------------------------------------------------------------------

## C

### CIA Triad

Security model consisting of:

``` text
Confidentiality
Integrity
Availability
```

### Cloud Security Posture Management --- CSPM

Continuous assessment and improvement of cloud security posture.

### Cloud Workload Protection Platform --- CWPP

Security capabilities focused on protecting cloud workloads.

### Communication Compliance

Microsoft Purview capability for identifying communications that may
violate organizational or regulatory policies.

### Compliance

The process of meeting applicable laws, regulations, standards, and
organizational requirements.

### Compliance Manager

Microsoft Purview solution used to assess and improve compliance
posture.

### Compliance Score

Measurement within Compliance Manager that helps track progress on
recommended improvement actions.

### Conditional Access

Microsoft Entra policy engine that uses signals and controls to make
access decisions.

------------------------------------------------------------------------

## D

### Data at Rest

Data stored on disks, databases, storage systems, or other media.

### Data in Transit

Data moving between systems or across networks.

### Data in Use

Data actively being processed.

### Data Loss Prevention --- DLP

Controls designed to identify sensitive information and prevent
inappropriate use or sharing.

### Data Lifecycle Management

Microsoft Purview capabilities for controlling how long information is
retained and when it is deleted.

### Defense in Depth

Security strategy that uses multiple layers of controls.

### Defender for Cloud

Microsoft cloud security solution providing cloud security posture
management and workload protection.

### Defender for Cloud Apps

Microsoft Defender service focused on cloud/SaaS application visibility
and control.

### Defender for Endpoint

Microsoft Defender service focused on endpoint security.

### Defender for Identity

Microsoft Defender service focused on identity-related threat detection
using identity signals, including on-premises Active Directory signals.

### Defender for Office 365

Microsoft Defender service focused on email and collaboration threats.

### Defender Vulnerability Management

Microsoft Defender capability used to identify, assess, and prioritize
vulnerabilities.

### Defender XDR

Extended detection and response platform that correlates security
signals across multiple security domains.

### DDoS

Distributed Denial of Service attack intended to overwhelm a service and
reduce availability.

### Dynamic Group

Microsoft Entra group whose membership is automatically determined using
configured rules.

------------------------------------------------------------------------

## E

### eDiscovery

Microsoft Purview capabilities used to identify, preserve, collect,
review, and export content for legal or investigative purposes.

### Encryption

Process of transforming information so it is unreadable without the
appropriate key.

### Endpoint DLP

Microsoft Purview DLP capabilities that help control sensitive-data
actions on supported endpoint devices.

### Entitlement Management

Microsoft Entra Identity Governance capability used to manage access
packages and access lifecycles.

### External Identity

Identity belonging to someone outside the organization, such as a
partner, guest, or contractor.

------------------------------------------------------------------------

## F

### Federation

Trust relationship that allows authentication across different identity
systems or organizations.

### FIDO2

Open authentication standard used for strong passwordless and
phishing-resistant authentication.

------------------------------------------------------------------------

## G

### Governance, Risk, and Compliance --- GRC

Framework combining organizational governance, risk management, and
compliance activities.

### Guest User

External identity invited into an organization's Microsoft Entra tenant
for collaboration.

------------------------------------------------------------------------

## H

### Hashing

One-way process that produces a fixed representation of data, commonly
used to support integrity verification and secure credential handling.

### Hybrid Identity

Identity environment that connects on-premises identity systems with
cloud identity services.

------------------------------------------------------------------------

## I

### Identity

Digital representation of a user, device, application, service,
workload, or agent.

### Identity Governance

Processes and Microsoft Entra capabilities used to ensure the right
identities have the right access for the right amount of time.

### Identity Provider --- IdP

System that authenticates identities and provides identity information
to applications or services.

### Identity Protection

Microsoft Entra capability used to detect and respond to
identity-related risk.

### Incident

Collection of related security alerts grouped into a broader attack
story or investigation.

### Information Protection

Microsoft Purview capabilities used to discover, classify, label, and
protect information.

### Insider Risk Management

Microsoft Purview solution used to identify and investigate potential
internal risk while incorporating privacy controls.

### Integrity

CIA-triad principle concerned with keeping information accurate and
protected from unauthorized modification.

------------------------------------------------------------------------

## J

### Joiner-Mover-Leaver --- JML

Identity lifecycle model covering users joining an organization,
changing roles, and leaving.

### Just-in-Time Access

Access granted only when needed and typically for a limited duration.

------------------------------------------------------------------------

## K

### Key Vault

Azure service used to securely store and manage secrets, encryption
keys, and certificates.

### KQL

Kusto Query Language, used by Microsoft security services such as
Sentinel and Advanced Hunting to query data.

------------------------------------------------------------------------

## L

### Least Privilege

Security principle of granting only the minimum permissions required to
perform a task.

### Lifecycle Workflows

Microsoft Entra Identity Governance feature used to automate joiner,
mover, and leaver identity tasks.

------------------------------------------------------------------------

## M

### Managed Identity

Azure identity that allows supported resources to authenticate to
services without developers manually managing credentials.

### Microsoft Entra

Microsoft identity and network access product family.

### Microsoft Entra ID

Microsoft cloud identity and access management service formerly known as
Azure Active Directory.

### Microsoft Sentinel

Microsoft cloud-native SIEM and SOAR security-operations solution.

### Microsoft Purview

Microsoft family of data security, governance, risk, and compliance
solutions.

### Multifactor Authentication --- MFA

Authentication requiring two or more different authentication factor
categories.

------------------------------------------------------------------------

## N

### Network Security Group --- NSG

Azure control containing inbound and outbound network traffic rules.

### Number Matching

Microsoft Authenticator feature requiring users to match a number during
certain authentication prompts, helping reduce accidental approvals.

------------------------------------------------------------------------

## P

### Passkey

Passwordless authentication credential based on public-key cryptography.

### Passwordless Authentication

Authentication that does not require the user to enter a traditional
password.

### Phishing

Attack that attempts to trick users into revealing credentials or taking
unsafe actions.

### Phishing-Resistant Authentication

Authentication designed to resist credential phishing, such as
appropriately implemented FIDO2/passkey methods.

### Playbook

Automated workflow used with Microsoft Sentinel, commonly based on Azure
Logic Apps.

### Policy Tip

User-facing DLP notification that can warn or educate a user about
sensitive-data actions.

### Privileged Identity Management --- PIM

Microsoft Entra capability for managing, monitoring, and providing
time-limited privileged access.

------------------------------------------------------------------------

## R

### RBAC

Role-Based Access Control. Permissions are assigned through roles rather
than individually defining every permission.

### Records Management

Microsoft Purview capabilities used to govern content that must be
managed as an official record.

### Resource Lock

Azure feature used to help prevent accidental deletion or modification
of resources.

### Retention Label

Microsoft Purview label used to apply retention behavior to specific
content/items.

### Retention Policy

Microsoft Purview policy used to apply retention behavior broadly to
supported locations or workloads.

### Risk Detection

Signal or event used by Microsoft Entra Identity Protection to identify
potentially risky activity.

------------------------------------------------------------------------

## S

### Secure Score

A measurement used by Microsoft security products to help organizations
understand and improve security posture.

### Security Defaults

Microsoft Entra baseline identity-security configuration intended to
provide common protections with minimal customization.

### Sensitive Information Type

Microsoft Purview classifier that detects sensitive information using
patterns and related detection logic.

### Sensitivity Label

Microsoft Purview label used to classify and potentially protect
content.

### Service Principal

Identity representation used by an application or service within a
Microsoft Entra tenant.

### Service Trust Portal

Microsoft portal providing security, privacy, compliance, and audit
documentation.

### Shared Responsibility Model

Cloud-security model describing which responsibilities belong to the
cloud provider and which remain with the customer.

### SIEM

Security Information and Event Management. Collects and analyzes
security information for detection and investigation.

### Sign-In Risk

Probability that a specific authentication request may not be
legitimate.

### Single Sign-On --- SSO

Allows a user to authenticate once and access multiple authorized
applications without repeatedly signing in.

### SOAR

Security Orchestration, Automation, and Response. Automates and
coordinates security-response activities.

------------------------------------------------------------------------

## T

### Temporary Access Pass --- TAP

Time-limited authentication method that can help users register or
recover strong/passwordless authentication methods.

### Threat Intelligence

Information about known or emerging threats, attackers, indicators, and
attack techniques.

### Trainable Classifier

Microsoft Purview classifier that uses machine learning to identify
categories of content based on examples.

------------------------------------------------------------------------

## U

### User Principal Name --- UPN

Sign-in name commonly used to identify a user in Microsoft Entra.

### User Risk

Probability that a user's identity may be compromised.

------------------------------------------------------------------------

## W

### Windows Hello for Business

Passwordless authentication technology using strong device-bound
credentials with PIN or biometric gestures.

### Workload Identity

Identity used by software workloads such as applications, services,
scripts, or automation.

------------------------------------------------------------------------

## Z

### Zero Trust

Security model based on three core principles:

``` text
Verify Explicitly
Use Least Privilege
Assume Breach
```

------------------------------------------------------------------------

# 🧠 Core Product Map

``` text
ENTRA
→ Identity & Access

DEFENDER
→ Threat Protection

SENTINEL
→ Security Operations

PURVIEW
→ Data Security & Compliance
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
