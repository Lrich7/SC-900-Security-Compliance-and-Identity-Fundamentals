# 📘 Lesson 11 --- Microsoft Defender XDR

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 11\
**Section:** Microsoft Security Solutions\
**Lab:** 🔵 Explore the Tool --- Microsoft Defender XDR\
**Difficulty:** Beginner

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Explain Microsoft Defender XDR
-   Explain extended detection and response (XDR)
-   Describe the Microsoft Defender portal
-   Distinguish alerts from incidents
-   Explain how Microsoft correlates security signals into an attack
    story
-   Recognize major Defender XDR security domains
-   Explain automated investigation and response at a fundamentals level
-   Describe Advanced Hunting at a fundamentals level
-   Explain how Defender XDR helps security operations teams investigate
    attacks
-   Distinguish Defender XDR from Microsoft Defender for Cloud

------------------------------------------------------------------------

# 🛡️ What Is Microsoft Defender XDR?

**Microsoft Defender XDR** is Microsoft's extended detection and
response platform.

It helps security teams detect, investigate, and respond to threats
across multiple security domains.

Think:

``` text
IDENTITIES

ENDPOINTS

EMAIL

COLLABORATION

APPLICATIONS

CLOUD APP ACTIVITY
```

Security signals from these areas can be brought together to provide a
broader view of an attack.

------------------------------------------------------------------------

# 🧠 What Does XDR Mean?

# Extended Detection and Response

Traditional security tools may investigate individual systems
separately.

Example:

``` text
EMAIL TOOL
sees phishing email
```

``` text
ENDPOINT TOOL
sees malware
```

``` text
IDENTITY TOOL
sees suspicious sign-in
```

If those systems are viewed separately, the security team may need to
manually determine whether the events are related.

XDR attempts to connect the story.

``` text
PHISHING EMAIL
      ↓
USER CLICKS LINK
      ↓
ENDPOINT COMPROMISED
      ↓
CREDENTIALS STOLEN
      ↓
SUSPICIOUS SIGN-IN
      ↓
ATTACKER ACCESSES DATA
```

Instead of five unrelated alerts, the security team can investigate the
broader attack.

------------------------------------------------------------------------

# 🌐 Microsoft Defender Portal

Microsoft security operations are brought together in the:

``` text
Microsoft Defender Portal
```

Common URL:

``` text
https://security.microsoft.com
```

The exact navigation and available features depend on licensing,
permissions, connected services, and Microsoft's current portal
experience.

For SC-900, focus on what the platform does rather than memorizing every
menu location.

------------------------------------------------------------------------

# 🧩 Major Defender XDR Security Areas

Microsoft Defender XDR can correlate signals from Microsoft security
products and services.

Important areas include:

``` text
Endpoints

Identities

Email and Collaboration

Cloud Applications
```

These are commonly associated with technologies such as:

``` text
Microsoft Defender for Endpoint

Microsoft Defender for Identity

Microsoft Defender for Office 365

Microsoft Defender for Cloud Apps
```

The unified Defender portal also brings together additional Microsoft
security experiences.

------------------------------------------------------------------------

# 💻 Microsoft Defender for Endpoint

**Microsoft Defender for Endpoint** helps protect endpoint devices.

Examples:

``` text
Windows Computers

Servers

Supported macOS Devices

Supported Linux Devices

Supported Mobile Platforms
```

Capabilities can include:

``` text
Threat Detection

Endpoint Investigation

Attack Surface Reduction

Vulnerability Management

Automated Investigation and Response
```

At the SC-900 level:

``` text
DEFENDER FOR ENDPOINT
=
Endpoint security
```

------------------------------------------------------------------------

# 👤 Microsoft Defender for Identity

**Microsoft Defender for Identity** focuses on identity-related threat
detection using identity signals, including supported on-premises and
hybrid identity environments.

It can help identify suspicious identity activity.

Examples can include:

``` text
Credential Theft

Suspicious Authentication

Identity Reconnaissance

Lateral Movement Indicators
```

At the fundamentals level:

``` text
DEFENDER FOR IDENTITY
=
Identity threat detection
```

------------------------------------------------------------------------

# 📧 Microsoft Defender for Office 365

**Microsoft Defender for Office 365** helps protect email and
collaboration environments.

Threats can include:

``` text
Phishing

Malicious Attachments

Malicious Links

Business Email Compromise
```

At the fundamentals level:

``` text
DEFENDER FOR OFFICE 365
=
Email and collaboration protection
```

------------------------------------------------------------------------

# ☁️ Microsoft Defender for Cloud Apps

**Microsoft Defender for Cloud Apps** provides visibility and security
capabilities for cloud application usage.

It can help organizations understand and protect activity involving
cloud applications.

At the fundamentals level:

``` text
DEFENDER FOR CLOUD APPS
=
Cloud application security
```

------------------------------------------------------------------------

# 🧠 Defender Product Memory Map

``` text
ENDPOINT
   ↓
Defender for Endpoint
```

``` text
IDENTITY
   ↓
Defender for Identity
```

``` text
EMAIL / COLLABORATION
   ↓
Defender for Office 365
```

``` text
CLOUD APPLICATIONS
   ↓
Defender for Cloud Apps
```

These signals can contribute to the broader Defender XDR investigation
experience.

------------------------------------------------------------------------

# 🚨 What Is an Alert?

An **alert** represents suspicious or potentially malicious activity
detected by a security capability.

Example:

``` text
Suspicious PowerShell Activity
```

or:

``` text
Malicious Email Detected
```

or:

``` text
Suspicious Identity Activity
```

Think:

``` text
ALERT
=
A SECURITY SIGNAL
THAT NEEDS ATTENTION
```

------------------------------------------------------------------------

# 🚨🚨 What Is an Incident?

An **incident** can group related alerts and evidence into a broader
security investigation.

Example:

``` text
INCIDENT
│
├── Phishing Alert
│
├── Endpoint Malware Alert
│
├── Suspicious Sign-In Alert
│
└── Cloud Application Alert
```

Think:

``` text
ALERT
=
One warning
```

``` text
INCIDENT
=
Related security story
```

------------------------------------------------------------------------

# 🧠 Alert vs Incident

This distinction is extremely useful.

``` text
ALERT
      ↓
Individual Detection
```

``` text
INCIDENT
      ↓
Collection of Related
Alerts and Evidence
```

Multiple alerts can contribute to one incident.

------------------------------------------------------------------------

# 🕵️ Attack Story

Defender XDR can correlate information to help analysts understand the
sequence of an attack.

Conceptually:

``` text
EMAIL
  ↓
USER
  ↓
DEVICE
  ↓
IDENTITY
  ↓
APPLICATION
  ↓
DATA
```

Instead of asking:

``` text
What happened on this one device?
```

XDR helps answer:

``` text
What happened across
the entire attack?
```

------------------------------------------------------------------------

# 🔗 Correlation

**Correlation** means connecting related security signals.

Example:

``` text
Alert A
Phishing Email
      +
Alert B
Malware Execution
      +
Alert C
Suspicious Sign-In
      ↓
CORRELATION
      ↓
ONE INCIDENT
```

This reduces the need for analysts to manually connect every event.

------------------------------------------------------------------------

# 🧾 Evidence and Entities

Investigations may include evidence and entities associated with an
attack.

Examples:

``` text
Users

Devices

Mailboxes

Files

IP Addresses

Applications

URLs
```

These relationships help analysts understand:

``` text
WHO was involved?

WHAT was affected?

HOW did the attack move?
```

------------------------------------------------------------------------

# 📊 Incident Queue

Security operations teams need a place to prioritize investigations.

The incident queue can help analysts review information such as:

``` text
Incident Name

Severity

Status

Affected Assets

Alerts

Investigation Details
```

The exact fields and interface can evolve.

------------------------------------------------------------------------

# ⚠️ Severity

Incidents and alerts can be assigned severity levels.

Conceptually:

``` text
LOW

MEDIUM

HIGH
```

Severity helps security teams prioritize attention, but analysts should
also consider context.

A security event affecting a critical administrator or sensitive server
may deserve different attention than the same event on a low-value test
system.

------------------------------------------------------------------------

# 🤖 Automated Investigation and Response

Microsoft Defender XDR includes automated investigation and response
capabilities.

Think:

``` text
ALERT
      ↓
AUTOMATED INVESTIGATION
      ↓
COLLECT EVIDENCE
      ↓
ANALYZE FINDINGS
      ↓
RECOMMEND / TAKE
SUPPORTED RESPONSE ACTIONS
```

The exact automated actions depend on product, configuration, licensing,
and organizational policy.

------------------------------------------------------------------------

# 🧠 Why Automation Matters

Security teams can receive large numbers of alerts.

Without automation:

``` text
ANALYST
  ↓
MANUALLY INVESTIGATES
EVERYTHING
```

With automation:

``` text
AUTOMATION
      ↓
HANDLES / INVESTIGATES
SUPPORTED TASKS
      ↓
ANALYST FOCUSES
ON HIGHER-VALUE WORK
```

Automation supports analysts; it does not eliminate the need for human
judgment.

------------------------------------------------------------------------

# 🔎 Advanced Hunting

**Advanced Hunting** provides a query-based threat-hunting capability in
Microsoft Defender.

Security analysts can search security data to investigate suspicious
activity.

Conceptually:

``` text
SECURITY DATA
      ↓
QUERY
      ↓
RESULTS
      ↓
INVESTIGATION
```

Advanced Hunting commonly uses:

``` text
Kusto Query Language — KQL
```

SC-900 does not require you to become a KQL expert.

Know the purpose:

> **Advanced Hunting allows security teams to proactively search
> security data for threats and suspicious activity.**

------------------------------------------------------------------------

# 🔍 Hunting vs Alerts

Alerts are generated when detection logic identifies suspicious
activity.

Threat hunting can be more proactive.

``` text
ALERT
=
System tells analyst:
"Look at this."
```

``` text
HUNTING
=
Analyst asks:
"Can I find evidence of this?"
```

------------------------------------------------------------------------

# 🏢 Example Attack

Contoso employee Alex receives a phishing email.

``` text
1. Malicious Email Arrives
         ↓
2. Alex Clicks Link
         ↓
3. Malware Runs on Laptop
         ↓
4. Credentials Are Stolen
         ↓
5. Attacker Signs In
         ↓
6. Attacker Accesses Cloud App
```

Different security products may see different parts.

``` text
Defender for Office 365
        ↓
Email
```

``` text
Defender for Endpoint
        ↓
Device
```

``` text
Identity Security Signals
        ↓
Account Activity
```

``` text
Defender for Cloud Apps
        ↓
Cloud Application Activity
```

Defender XDR helps connect these signals into a broader investigation.

------------------------------------------------------------------------

# 🧱 XDR and Defense in Depth

Defender XDR does not replace preventive controls.

Organizations still need:

``` text
MFA

Conditional Access

Passwordless Authentication

Endpoint Hardening

Email Protection

Network Security

Least Privilege
```

XDR adds:

``` text
DETECTION

CORRELATION

INVESTIGATION

RESPONSE
```

Defense in depth includes both:

``` text
PREVENT
+
DETECT
+
RESPOND
```

------------------------------------------------------------------------

# ☁️ Defender XDR vs Defender for Cloud

Do not confuse these.

## Microsoft Defender for Cloud

Lesson 10:

``` text
Cloud Security Posture
+
Cloud Workload Protection
```

Think:

``` text
HOW SECURE
ARE MY CLOUD RESOURCES?
```

## Microsoft Defender XDR

Lesson 11:

``` text
Cross-Domain Threat
Detection and Response
```

Think:

``` text
WHAT ATTACK IS HAPPENING
ACROSS MY ENVIRONMENT?
```

They can complement one another.

------------------------------------------------------------------------

# 🧠 Quick Comparison

  Product                   Main Focus
  ------------------------- -----------------------------------------------------
  Defender for Cloud        Cloud posture and workload protection
  Defender XDR              Cross-domain detection, investigation, and response
  Defender for Endpoint     Endpoint security
  Defender for Identity     Identity threat detection
  Defender for Office 365   Email and collaboration security
  Defender for Cloud Apps   Cloud application security

------------------------------------------------------------------------

# 🛡️ Security Operations --- SOC

A **Security Operations Center (SOC)** is a team or function responsible
for monitoring, detecting, investigating, and responding to security
threats.

Defender XDR provides tools that can support SOC workflows.

``` text
DETECT
   ↓
TRIAGE
   ↓
INVESTIGATE
   ↓
RESPOND
   ↓
IMPROVE
```

------------------------------------------------------------------------

# 🎯 Exam Focus

Know these relationships:

``` text
DEFENDER XDR
=
Extended Detection
and Response
```

``` text
ALERT
=
Individual security detection
```

``` text
INCIDENT
=
Related alerts and evidence
grouped into an investigation
```

``` text
DEFENDER FOR ENDPOINT
=
Endpoint security
```

``` text
DEFENDER FOR IDENTITY
=
Identity threat detection
```

``` text
DEFENDER FOR OFFICE 365
=
Email / collaboration security
```

``` text
DEFENDER FOR CLOUD APPS
=
Cloud application security
```

``` text
ADVANCED HUNTING
=
Proactive query-based
threat investigation
```

------------------------------------------------------------------------

# 🧠 Memory Map

``` text
DEVICE
  ↓
Defender for Endpoint

IDENTITY
  ↓
Defender for Identity

EMAIL
  ↓
Defender for Office 365

CLOUD APP
  ↓
Defender for Cloud Apps

ALL SIGNALS
  ↓
Defender XDR
  ↓
Incident
  ↓
Investigation
  ↓
Response
```

------------------------------------------------------------------------

# ❓ Knowledge Check

### 1. What does XDR stand for?

A. Extended Detection and Response\
B. External Data Recovery\
C. Extended Device Registration\
D. Extra Directory Roles

### 2. What is the primary purpose of Defender XDR?

A. Correlate security signals to detect, investigate, and respond to
attacks\
B. Create Azure subscriptions\
C. Replace Microsoft Entra ID\
D. Manage printers

### 3. What is an alert?

A. An individual security detection or warning\
B. A group of subscriptions\
C. A user license\
D. A backup schedule

### 4. What is an incident?

A. A broader investigation that can contain related alerts and evidence\
B. A password reset\
C. An Azure resource group\
D. A compliance label

### 5. Which product focuses on endpoint security?

A. Defender for Endpoint\
B. Defender for Office 365\
C. Defender for Cloud Apps\
D. Microsoft Purview

### 6. Which product focuses on email and collaboration protection?

A. Defender for Office 365\
B. Defender for Endpoint\
C. Azure Bastion\
D. Azure Policy

### 7. What is correlation?

A. Connecting related security signals into a broader attack story\
B. Creating passwords\
C. Assigning licenses\
D. Encrypting every file manually

### 8. What is Advanced Hunting used for?

A. Query-based investigation and proactive threat hunting\
B. Creating SharePoint sites\
C. Managing billing\
D. Replacing Conditional Access

### 9. What can automated investigation and response help do?

A. Investigate supported security findings and assist with response\
B. Guarantee attacks never occur\
C. Replace all security analysts\
D. Create employee accounts

### 10. Which statement is correct?

A. Defender for Cloud focuses on cloud posture/workloads, while Defender
XDR focuses on cross-domain detection and response\
B. They are exactly the same product\
C. Defender XDR is only a firewall\
D. Defender for Cloud only protects email

------------------------------------------------------------------------

# ✅ Knowledge Check Answers

``` text
1. A
2. A
3. A
4. A
5. A
6. A
7. A
8. A
9. A
10. A
```

------------------------------------------------------------------------

# 📌 Lesson Summary

``` text
MICROSOFT DEFENDER XDR
=
Cross-domain detection
+
Correlation
+
Investigation
+
Response
```

``` text
ALERT
=
Individual warning
```

``` text
INCIDENT
=
Related security story
```

``` text
ADVANCED HUNTING
=
Proactive investigation
```

Defender XDR helps security teams understand attacks across identities,
endpoints, email, collaboration tools, and cloud applications.

------------------------------------------------------------------------

# 🧪 Lab

## 🔵 Lab 11 --- Explore Microsoft Defender XDR

➡️ **[Lab 11 --- Explore Microsoft Defender
XDR](../labs/%F0%9F%94%B5%20Lab%2011%20%E2%80%94%20Explore%20Microsoft%20Defender%20XDR.md)**

------------------------------------------------------------------------

# ➡️ Next Lesson

## 📘 Lesson 12 --- Microsoft Defender Security Services

Next you will compare Microsoft's Defender services and learn which
security product fits different scenarios.

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Defender XDR
    Overview](https://learn.microsoft.com/en-us/defender-xdr/microsoft-365-defender)
-   [Incidents and
    Alerts](https://learn.microsoft.com/en-us/defender-xdr/incidents-overview)
-   [Advanced
    Hunting](https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-overview)
-   [Automated Investigation and
    Response](https://learn.microsoft.com/en-us/defender-xdr/m365d-autoir)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Lesson 10 --- Microsoft Defender for Cloud**

🧪 **[Lab
11](../labs/%F0%9F%94%B5%20Lab%2011%20%E2%80%94%20Explore%20Microsoft%20Defender%20XDR.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
