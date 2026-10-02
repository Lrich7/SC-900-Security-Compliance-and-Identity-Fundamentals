# 📘 Lesson 12 --- Microsoft Defender Security Services

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 12\
**Section:** Microsoft Security Solutions\
**Lab:** 🟡 Scenario Lab --- Choose the Defender Service\
**Difficulty:** Beginner

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Identify the major Microsoft Defender security services
-   Explain Microsoft Defender for Endpoint
-   Explain Microsoft Defender for Office 365
-   Explain Microsoft Defender for Identity
-   Explain Microsoft Defender for Cloud Apps
-   Explain Microsoft Defender Vulnerability Management at a
    fundamentals level
-   Explain how the Defender services contribute signals to Microsoft
    Defender XDR
-   Choose the appropriate Defender service for common security
    scenarios
-   Distinguish Defender XDR from the individual Defender services
-   Distinguish Microsoft Defender for Cloud from the Microsoft Defender
    XDR security services

------------------------------------------------------------------------

# 🧠 Why This Lesson Matters

Microsoft uses the **Defender** name for several security products.

That can be confusing.

For SC-900, you do not need to memorize every feature inside every
Defender product.

You do need to understand:

``` text
WHAT DOES IT PROTECT?
```

and:

``` text
WHEN WOULD I USE IT?
```

------------------------------------------------------------------------

# 🗺️ Defender Security Map

``` text
                     MICROSOFT DEFENDER XDR
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
          ▼                   ▼                   ▼
      ENDPOINTS            IDENTITIES          EMAIL
          │                   │                   │
          ▼                   ▼                   ▼
 Defender for          Defender for        Defender for
   Endpoint              Identity           Office 365
          │
          │
          └───────────────────┐
                              │
                              ▼
                        CLOUD APPS
                              │
                              ▼
                       Defender for
                        Cloud Apps
```

These products focus on different security domains, while Defender XDR
helps connect security signals across them.

------------------------------------------------------------------------

# 💻 Microsoft Defender for Endpoint

**Microsoft Defender for Endpoint** is an enterprise endpoint security
platform.

Think:

``` text
LAPTOPS

DESKTOPS

SERVERS

SUPPORTED ENDPOINTS
```

Its purpose includes helping organizations:

``` text
Prevent Threats

Detect Threats

Investigate Endpoint Activity

Respond to Endpoint Attacks
```

------------------------------------------------------------------------

# 🛡️ Endpoint Detection and Response --- EDR

A major endpoint-security concept is:

# Endpoint Detection and Response

abbreviated:

``` text
EDR
```

EDR helps security teams detect and investigate suspicious behavior on
endpoints.

Conceptually:

``` text
DEVICE ACTIVITY
      ↓
SECURITY TELEMETRY
      ↓
DETECTION
      ↓
INVESTIGATION
      ↓
RESPONSE
```

------------------------------------------------------------------------

# 🧱 Attack Surface Reduction

Defender for Endpoint also includes capabilities designed to reduce the
opportunities attackers have to compromise devices.

This is often called:

``` text
Attack Surface Reduction
```

Think:

``` text
FEWER ATTACK OPPORTUNITIES
=
LOWER RISK
```

Examples can involve controlling risky behaviors or reducing exposure to
common attack techniques.

------------------------------------------------------------------------

# 🩹 Vulnerability Management

Organizations need to know whether devices have:

``` text
Vulnerable Software

Missing Security Updates

Risky Configurations

Exposed Weaknesses
```

Microsoft Defender Vulnerability Management helps organizations
identify, assess, prioritize, and remediate vulnerabilities and
misconfigurations across supported assets.

At the fundamentals level:

``` text
VULNERABILITY MANAGEMENT
=
Find weaknesses
before attackers exploit them
```

------------------------------------------------------------------------

# 📧 Microsoft Defender for Office 365

**Microsoft Defender for Office 365** helps protect email and
collaboration environments.

Think:

``` text
EMAIL

MICROSOFT TEAMS

SHAREPOINT

ONEDRIVE
```

depending on the feature and licensing.

Common threats include:

``` text
Phishing

Malicious Links

Malicious Attachments

Business Email Compromise
```

------------------------------------------------------------------------

# 🔗 Safe Links

**Safe Links** helps protect users from malicious URLs.

Conceptually:

``` text
USER CLICKS LINK
      ↓
LINK CHECKED
      ↓
SAFE?
   ↙       ↘
 YES       NO
 ↓          ↓
CONTINUE   PROTECT / WARN / BLOCK
```

The exact behavior depends on configuration and policy.

------------------------------------------------------------------------

# 📎 Safe Attachments

**Safe Attachments** helps protect users from malicious files.

Conceptually:

``` text
EMAIL ATTACHMENT
      ↓
SECURITY ANALYSIS
      ↓
MALICIOUS?
   ↙       ↘
 NO        YES
 ↓          ↓
DELIVER    PROTECT
```

For SC-900:

``` text
SAFE LINKS
=
URLs
```

``` text
SAFE ATTACHMENTS
=
Files
```

------------------------------------------------------------------------

# 🎣 Anti-Phishing Protection

Phishing attacks attempt to trick users into:

``` text
Revealing Credentials

Opening Malicious Files

Clicking Malicious Links

Sending Money

Sharing Sensitive Information
```

Defender for Office 365 provides capabilities that help organizations
protect against phishing and related email threats.

------------------------------------------------------------------------

# 👤 Microsoft Defender for Identity

**Microsoft Defender for Identity** is a cloud-based security solution
that uses identity-related signals to help detect threats involving
identities.

It is especially important in organizations with:

``` text
Active Directory Domain Services

Hybrid Identity

On-Premises Identity Infrastructure
```

------------------------------------------------------------------------

# 🕵️ Identity Threats

Examples can include attacker behavior related to:

``` text
Credential Theft

Reconnaissance

Lateral Movement

Compromised Accounts

Suspicious Authentication
```

At the fundamentals level:

``` text
DEFENDER FOR IDENTITY
=
Detect suspicious
identity activity
```

------------------------------------------------------------------------

# 🧠 Identity Security Example

An attacker compromises a user's credentials.

Then:

``` text
COMPROMISED USER
      ↓
ATTACKER ENUMERATES ENVIRONMENT
      ↓
ATTACKER TARGETS MORE ACCOUNTS
      ↓
LATERAL MOVEMENT
```

Identity-focused security signals can help security teams recognize this
behavior.

------------------------------------------------------------------------

# ☁️ Microsoft Defender for Cloud Apps

**Microsoft Defender for Cloud Apps** is a Cloud Access Security Broker
(CASB) solution and provides visibility and control over cloud
application usage.

Think:

``` text
WHO IS USING
WHICH CLOUD APPS
AND WHAT ARE THEY DOING?
```

------------------------------------------------------------------------

# ☁️ CASB

CASB stands for:

``` text
Cloud Access Security Broker
```

At a fundamentals level, a CASB helps provide:

``` text
Visibility

Control

Threat Protection

Information Protection
```

for cloud application usage.

------------------------------------------------------------------------

# 🔎 Shadow IT

Employees sometimes use cloud applications without formal IT approval.

This is commonly called:

``` text
Shadow IT
```

Example:

``` text
Employee
      ↓
Uploads Company Data
      ↓
Unapproved Cloud Storage App
```

Defender for Cloud Apps can help organizations discover and assess cloud
application usage.

------------------------------------------------------------------------

# 🧠 Cloud App Example

Contoso discovers employees are using hundreds of cloud services.

Security wants to know:

``` text
Which apps are being used?

Which apps are risky?

What data is moving?

Are accounts behaving suspiciously?
```

Defender for Cloud Apps can help provide cloud-app visibility and
security controls.

------------------------------------------------------------------------

# 🛡️ Defender XDR Brings the Signals Together

Remember Lesson 11.

Individual Defender products focus on particular security areas.

``` text
Defender for Office 365
      ↓
Phishing Email
```

``` text
Defender for Endpoint
      ↓
Malware on Laptop
```

``` text
Defender for Identity
      ↓
Suspicious Identity Activity
```

``` text
Defender for Cloud Apps
      ↓
Suspicious Cloud App Activity
```

Then:

``` text
SECURITY SIGNALS
      ↓
MICROSOFT DEFENDER XDR
      ↓
CORRELATION
      ↓
INCIDENT
      ↓
INVESTIGATION
```

------------------------------------------------------------------------

# 🧠 Individual Service vs XDR

Think:

``` text
INDIVIDUAL DEFENDER SERVICE
=
Protect / monitor
a security domain
```

``` text
DEFENDER XDR
=
Connect security signals
across domains
```

------------------------------------------------------------------------

# ☁️ What About Microsoft Defender for Cloud?

Do not confuse:

``` text
Microsoft Defender for Cloud
```

with:

``` text
Microsoft Defender for Cloud Apps
```

They are different products.

------------------------------------------------------------------------

# ☁️ Defender for Cloud

From Lesson 10:

``` text
Cloud Security Posture Management

Cloud Workload Protection

Security Recommendations

Cloud Secure Score
```

Think:

``` text
CLOUD INFRASTRUCTURE
AND WORKLOAD SECURITY
```

------------------------------------------------------------------------

# ☁️ Defender for Cloud Apps

Think:

``` text
CLOUD APPLICATION
USAGE AND SECURITY
```

Example:

``` text
Microsoft 365

Salesforce

Dropbox

Other SaaS Apps
```

depending on connections and supported capabilities.

------------------------------------------------------------------------

# 🧠 Cloud vs Cloud Apps

``` text
DEFENDER FOR CLOUD
=
Cloud infrastructure
and workload security
```

``` text
DEFENDER FOR CLOUD APPS
=
Cloud application usage
and security
```

This distinction is worth memorizing.

------------------------------------------------------------------------

# 🏢 Contoso Example

Contoso has several security problems.

## Problem 1

Employees receive phishing emails.

Use:

``` text
Defender for Office 365
```

## Problem 2

A laptop begins running suspicious malware.

Use:

``` text
Defender for Endpoint
```

## Problem 3

Suspicious identity activity occurs in the hybrid identity environment.

Use:

``` text
Defender for Identity
```

## Problem 4

Employees use unapproved cloud storage services.

Use:

``` text
Defender for Cloud Apps
```

## Problem 5

The security team wants one correlated investigation across those
events.

Use:

``` text
Microsoft Defender XDR
```

------------------------------------------------------------------------

# 🗺️ Product Selection Map

``` text
DEVICE PROBLEM?
      ↓
Defender for Endpoint
```

``` text
EMAIL PROBLEM?
      ↓
Defender for Office 365
```

``` text
IDENTITY THREAT?
      ↓
Defender for Identity
```

``` text
CLOUD APP USAGE?
      ↓
Defender for Cloud Apps
```

``` text
CROSS-DOMAIN ATTACK?
      ↓
Defender XDR
```

``` text
CLOUD INFRASTRUCTURE POSTURE?
      ↓
Defender for Cloud
```

------------------------------------------------------------------------

# 🎯 Exam Focus

Know these relationships:

``` text
DEFENDER FOR ENDPOINT
=
Endpoint security
```

``` text
DEFENDER FOR OFFICE 365
=
Email and collaboration security
```

``` text
SAFE LINKS
=
URL protection
```

``` text
SAFE ATTACHMENTS
=
File / attachment protection
```

``` text
DEFENDER FOR IDENTITY
=
Identity threat detection
```

``` text
DEFENDER FOR CLOUD APPS
=
Cloud app visibility and security
```

``` text
CASB
=
Cloud Access Security Broker
```

``` text
DEFENDER XDR
=
Cross-domain detection,
correlation, investigation,
and response
```

------------------------------------------------------------------------

# 🧠 Memory Tricks

``` text
ENDPOINT
=
Device
```

``` text
OFFICE 365
=
Email
```

``` text
IDENTITY
=
Accounts
```

``` text
CLOUD APPS
=
SaaS Usage
```

``` text
XDR
=
Connect the Attack
```

``` text
DEFENDER FOR CLOUD
=
Cloud Resources
```

------------------------------------------------------------------------

# ❓ Knowledge Check

### 1. Which service focuses on endpoint security?

A. Defender for Endpoint\
B. Defender for Office 365\
C. Defender for Cloud Apps\
D. Microsoft Purview

### 2. Which service helps protect email and collaboration?

A. Defender for Office 365\
B. Defender for Endpoint\
C. Azure Bastion\
D. Defender for Cloud

### 3. What does Safe Links primarily protect against?

A. Malicious URLs\
B. Vulnerable operating systems\
C. Physical theft\
D. Azure subscription changes

### 4. What does Safe Attachments primarily analyze?

A. Files and attachments\
B. Password length\
C. Network cables\
D. Azure regions

### 5. Which service focuses on identity-related threats?

A. Defender for Identity\
B. Defender for Endpoint\
C. Defender for Cloud Apps\
D. Azure Firewall

### 6. Which service provides cloud-app visibility and CASB capabilities?

A. Defender for Cloud Apps\
B. Defender for Cloud\
C. Defender for Endpoint\
D. Azure Policy

### 7. What is Shadow IT?

A. Use of applications or services outside normal IT approval or
visibility\
B. A dark-mode portal setting\
C. A backup technology\
D. An Azure region

### 8. What does Defender XDR primarily add?

A. Cross-domain correlation, investigation, and response\
B. Printer management\
C. Azure billing\
D. File storage

### 9. Which product is primarily associated with cloud infrastructure posture and workload protection?

A. Defender for Cloud\
B. Defender for Cloud Apps\
C. Defender for Office 365\
D. Defender for Identity

### 10. Which product would best fit a phishing-email scenario?

A. Defender for Office 365\
B. Defender for Endpoint\
C. Defender for Cloud Apps\
D. Azure Key Vault

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
DEVICE
→ Defender for Endpoint
```

``` text
EMAIL
→ Defender for Office 365
```

``` text
IDENTITY
→ Defender for Identity
```

``` text
CLOUD APPLICATION
→ Defender for Cloud Apps
```

``` text
CROSS-DOMAIN ATTACK
→ Defender XDR
```

``` text
CLOUD INFRASTRUCTURE
→ Defender for Cloud
```

The key to this lesson is choosing the correct Microsoft security
service for the problem being solved.

------------------------------------------------------------------------

# 🧪 Lab

## 🟡 Lab 12 --- Choose the Defender Service

➡️ **[Lab 12 --- Choose the Defender
Service](../labs/%F0%9F%9F%A1%20Lab%2012%20%E2%80%94%20Choose%20the%20Defender%20Service.md)**

------------------------------------------------------------------------

# ➡️ Next Lesson

## 📘 Lesson 13 --- Microsoft Sentinel

Next you will learn how Microsoft Sentinel provides SIEM and SOAR
capabilities for security operations.

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Defender
    XDR](https://learn.microsoft.com/en-us/defender-xdr/microsoft-365-defender)
-   [Microsoft Defender for
    Endpoint](https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint)
-   [Microsoft Defender for Office
    365](https://learn.microsoft.com/en-us/defender-office-365/mdo-about)
-   [Microsoft Defender for
    Identity](https://learn.microsoft.com/en-us/defender-for-identity/what-is)
-   [Microsoft Defender for Cloud
    Apps](https://learn.microsoft.com/en-us/defender-cloud-apps/what-is-defender-for-cloud-apps)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Lesson 11 --- Microsoft Defender XDR**

🧪 **[Lab
12](../labs/%F0%9F%9F%A1%20Lab%2012%20%E2%80%94%20Choose%20the%20Defender%20Service.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
