# 🟡 Lab 12 --- Choose the Defender Service

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 12 --- Microsoft Defender Security Services\
**Lab Type:** 🟡 Scenario Lab\
**Difficulty:** Beginner\
**Configuration Changes:** None

------------------------------------------------------------------------

# 🎯 Lab Objectives

By completing this lab, you should be able to choose between:

-   Microsoft Defender for Endpoint
-   Microsoft Defender for Office 365
-   Microsoft Defender for Identity
-   Microsoft Defender for Cloud Apps
-   Microsoft Defender XDR
-   Microsoft Defender for Cloud

You should also be able to explain:

-   Safe Links
-   Safe Attachments
-   Endpoint Detection and Response
-   Vulnerability Management
-   CASB
-   Shadow IT
-   Cross-domain incident correlation

------------------------------------------------------------------------

# 🟡 Why a Scenario Lab?

Lessons 10 and 11 gave you portal exploration.

Lesson 12 is different.

The challenge is no longer:

``` text
WHERE IS THE TOOL?
```

The challenge is:

``` text
WHICH TOOL SHOULD I USE?
```

This lab focuses on product selection.

------------------------------------------------------------------------

# 🗺️ Defender Cheat Sheet

Use this only when needed.

``` text
ENDPOINT / DEVICE
→ Defender for Endpoint

EMAIL / COLLABORATION
→ Defender for Office 365

IDENTITY THREATS
→ Defender for Identity

CLOUD APPLICATION USAGE
→ Defender for Cloud Apps

CROSS-DOMAIN ATTACK
→ Defender XDR

CLOUD INFRASTRUCTURE / POSTURE
→ Defender for Cloud
```

------------------------------------------------------------------------

# 🧩 Part 1 --- Match the Product

Choose from:

``` text
Defender for Endpoint

Defender for Office 365

Defender for Identity

Defender for Cloud Apps

Defender XDR

Defender for Cloud
```

## Scenario 1

A Windows laptop begins running suspicious processes after a user
downloads a file.

``` text
______________________________
```

## Scenario 2

Employees are receiving credential-stealing phishing emails.

``` text
______________________________
```

## Scenario 3

Security detects suspicious behavior involving Active Directory
identities.

``` text
______________________________
```

## Scenario 4

Employees are uploading company files to unapproved SaaS applications.

``` text
______________________________
```

## Scenario 5

Security wants to correlate email, endpoint, identity, and cloud-app
alerts into one investigation.

``` text
______________________________
```

## Scenario 6

The cloud team wants recommendations for improving Azure resource
security posture.

``` text
______________________________
```

------------------------------------------------------------------------

# 📧 Part 2 --- Email Security

Contoso receives an email containing:

``` text
A suspicious link

and

A suspicious attachment
```

Which Defender service should help protect the email environment?

``` text
______________________________
```

Which feature is associated with the link?

``` text
______________________________
```

Which feature is associated with the attachment?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 3 --- Safe Links

A user receives:

``` text
https://totally-not-a-phishing-site.example
```

The user clicks the link.

Which Microsoft Defender for Office 365 capability is most closely
associated with checking malicious URLs?

``` text
______________________________
```

Memory:

``` text
LINK
=
____________________
```

------------------------------------------------------------------------

# 📎 Part 4 --- Safe Attachments

An attacker emails:

``` text
Invoice.docx
```

The attachment contains malicious content.

Which capability is associated with analyzing suspicious attachments?

``` text
______________________________
```

Memory:

``` text
FILE
=
____________________
```

------------------------------------------------------------------------

# 💻 Part 5 --- Endpoint Security

A user downloads malware onto a company laptop.

Security wants to:

``` text
Detect suspicious behavior

Investigate the endpoint

Understand what happened

Respond to the attack
```

Which product fits?

``` text
______________________________
```

What does EDR stand for?

``` text
____________________________________
```

------------------------------------------------------------------------

# 🩹 Part 6 --- Vulnerability Management

Contoso has 200 endpoints.

Security wants to identify:

``` text
Outdated Software

Known Vulnerabilities

Risky Configurations
```

Which type of capability fits?

``` text
______________________________
```

Why is finding vulnerabilities before an attack useful?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 👤 Part 7 --- Identity Attack

An attacker steals an employee's credentials.

The attacker begins:

``` text
Enumerating Accounts

Looking for Privileged Users

Attempting Lateral Movement
```

Which Defender product is most closely associated with detecting
identity-based threats in supported identity environments?

``` text
______________________________
```

------------------------------------------------------------------------

# ☁️ Part 8 --- Shadow IT

An IT department approves:

``` text
Microsoft OneDrive
```

for corporate file storage.

Employees begin using several unapproved consumer cloud-storage
services.

This is an example of:

``` text
______________________________
```

Which Defender product can help provide visibility into cloud
application usage?

``` text
______________________________
```

------------------------------------------------------------------------

# ☁️ Part 9 --- CASB

What does CASB stand for?

``` text
____________________________________
```

Which product is associated with CASB capabilities?

``` text
______________________________
```

At a high level, what does a CASB help provide?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🚨 Part 10 --- One Attack, Many Products

Contoso experiences:

``` text
1. Phishing email delivered

2. User clicks malicious link

3. Malware runs on endpoint

4. Credentials are stolen

5. Suspicious identity activity occurs

6. Attacker accesses cloud applications
```

Match each area.

  Attack Stage                  Security Service
  ----------------------------- --------------------------------------
  Phishing email                \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Malicious endpoint activity   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identity activity             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud application activity    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Which platform helps correlate the attack into a broader incident?

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Part 11 --- Individual Product or XDR?

Choose:

``` text
Individual Defender Service

Defender XDR
```

## Detect malicious activity on an endpoint

``` text
______________________________
```

## Connect endpoint, email, and identity alerts

``` text
______________________________
```

## Protect against phishing email

``` text
______________________________
```

## Build a cross-domain incident

``` text
______________________________
```

------------------------------------------------------------------------

# ☁️ Part 12 --- The Two "Cloud" Products

Choose:

``` text
Defender for Cloud

Defender for Cloud Apps
```

## Scenario 1

Find insecure Azure configurations.

``` text
______________________________
```

## Scenario 2

Discover unapproved SaaS application usage.

``` text
______________________________
```

## Scenario 3

Improve cloud infrastructure security posture.

``` text
______________________________
```

## Scenario 4

Monitor risky cloud application behavior.

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Part 13 --- Explain the Difference

Complete:

``` text
Defender for Cloud
=
____________________________________

____________________________________
```

``` text
Defender for Cloud Apps
=
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🏢 Part 14 --- Contoso Security Team

Contoso has:

``` text
150 Employees

Windows Laptops

Microsoft 365

Hybrid Active Directory

Azure Resources

Several SaaS Applications
```

Choose the most appropriate Defender service for each team.

## Endpoint Team

Needs device threat detection.

``` text
______________________________
```

## Messaging Team

Needs phishing and malicious attachment protection.

``` text
______________________________
```

## Identity Team

Needs identity-threat visibility.

``` text
______________________________
```

## Cloud-App Team

Needs SaaS visibility and Shadow IT discovery.

``` text
______________________________
```

## SOC

Needs correlated cross-domain incidents.

``` text
______________________________
```

## Azure Security Team

Needs cloud security posture recommendations.

``` text
______________________________
```

------------------------------------------------------------------------

# 🎯 Part 15 --- Rapid-Fire Challenge

Write the product or feature.

## Malicious URL

``` text
______________________________
```

## Malicious email attachment

``` text
______________________________
```

## Endpoint malware

``` text
______________________________
```

## Identity reconnaissance

``` text
______________________________
```

## Shadow IT

``` text
______________________________
```

## Cross-domain incident

``` text
______________________________
```

## Azure security recommendations

``` text
______________________________
```

## Endpoint vulnerabilities

``` text
______________________________
```

------------------------------------------------------------------------

# 🧠 Part 16 --- Build the Defender Map From Memory

Fill in:

``` text
DEVICE
      ↓
______________________________

EMAIL
      ↓
______________________________

IDENTITY
      ↓
______________________________

CLOUD APPLICATION
      ↓
______________________________

ALL SECURITY SIGNALS
      ↓
______________________________

CLOUD INFRASTRUCTURE
      ↓
______________________________
```

------------------------------------------------------------------------

# 🏗️ Part 17 --- Design a Security Stack

Contoso wants a Microsoft security stack that covers:

``` text
Endpoints

Email

Identities

Cloud Applications

Cross-Domain Investigation

Azure Cloud Posture
```

Fill in:

  Security Need                Microsoft Solution
  ---------------------------- ------------------------------------------------------
  Endpoints                    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Email                        \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identities                   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud Applications           \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cross-Domain Investigation   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Azure/Cloud Posture          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# 🔎 Part 18 --- Explain Your Choices

Pick any **three** rows from the previous table.

For each, explain why the selected service fits.

## Choice 1

``` text
Service:
____________________________________

Reason:
____________________________________

____________________________________
```

## Choice 2

``` text
Service:
____________________________________

Reason:
____________________________________

____________________________________
```

## Choice 3

``` text
Service:
____________________________________

Reason:
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🏆 Final Challenge

A security analyst receives this report:

> An employee received a phishing email containing a malicious link.
> After clicking it, suspicious software executed on the employee's
> laptop. Shortly afterward, unusual identity activity appeared,
> followed by suspicious access to a cloud application.

Answer:

## Which service helps protect the email?

``` text
______________________________
```

## Which feature relates to the malicious URL?

``` text
______________________________
```

## Which service investigates the laptop?

``` text
______________________________
```

## Which service focuses on the identity activity?

``` text
______________________________
```

## Which service focuses on cloud-app activity?

``` text
______________________________
```

## Which platform correlates the entire attack?

``` text
______________________________
```

------------------------------------------------------------------------

# ✅ Suggested Answers

## Part 1

``` text
1. Defender for Endpoint

2. Defender for Office 365

3. Defender for Identity

4. Defender for Cloud Apps

5. Defender XDR

6. Defender for Cloud
```

## Email Security

``` text
Service
=
Defender for Office 365

Link
=
Safe Links

Attachment
=
Safe Attachments
```

## Endpoint

``` text
Defender for Endpoint

EDR
=
Endpoint Detection and Response
```

## Vulnerability Management

``` text
Microsoft Defender Vulnerability Management
```

Finding vulnerabilities early gives administrators an opportunity to
reduce risk before weaknesses are exploited.

## Identity

``` text
Defender for Identity
```

## Shadow IT

``` text
Shadow IT

Defender for Cloud Apps
```

## CASB

``` text
Cloud Access Security Broker

Defender for Cloud Apps
```

CASB capabilities help provide visibility, control, threat protection,
and information protection for cloud application usage.

## Attack Stages

``` text
Phishing
=
Defender for Office 365

Endpoint
=
Defender for Endpoint

Identity
=
Defender for Identity

Cloud App
=
Defender for Cloud Apps

Correlation
=
Defender XDR
```

## Individual vs XDR

``` text
1. Individual Defender Service

2. Defender XDR

3. Individual Defender Service

4. Defender XDR
```

## Two Cloud Products

``` text
1. Defender for Cloud

2. Defender for Cloud Apps

3. Defender for Cloud

4. Defender for Cloud Apps
```

## Contoso Teams

``` text
Endpoint
=
Defender for Endpoint

Messaging
=
Defender for Office 365

Identity
=
Defender for Identity

Cloud Apps
=
Defender for Cloud Apps

SOC
=
Defender XDR

Azure Security
=
Defender for Cloud
```

## Rapid Fire

``` text
Malicious URL
=
Safe Links

Malicious Attachment
=
Safe Attachments

Endpoint Malware
=
Defender for Endpoint

Identity Reconnaissance
=
Defender for Identity

Shadow IT
=
Defender for Cloud Apps

Cross-Domain Incident
=
Defender XDR

Azure Recommendations
=
Defender for Cloud

Endpoint Vulnerabilities
=
Defender Vulnerability Management
```

## Defender Map

``` text
DEVICE
→ Defender for Endpoint

EMAIL
→ Defender for Office 365

IDENTITY
→ Defender for Identity

CLOUD APPLICATION
→ Defender for Cloud Apps

ALL SECURITY SIGNALS
→ Defender XDR

CLOUD INFRASTRUCTURE
→ Defender for Cloud
```

## Final Challenge

``` text
Email
=
Defender for Office 365

URL
=
Safe Links

Laptop
=
Defender for Endpoint

Identity
=
Defender for Identity

Cloud App
=
Defender for Cloud Apps

Entire Attack
=
Defender XDR
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

The key skill from this lab is:

``` text
SEE THE SECURITY PROBLEM
      ↓
IDENTIFY THE DOMAIN
      ↓
CHOOSE THE DEFENDER SERVICE
```

Remember:

``` text
DEVICE → Endpoint

EMAIL → Office 365

IDENTITY → Identity

SAAS → Cloud Apps

EVERYTHING TOGETHER → XDR

CLOUD RESOURCES → Defender for Cloud
```

------------------------------------------------------------------------

# ✅ Lab Completion Checklist

-   [ ] I can choose Defender for Endpoint.
-   [ ] I can choose Defender for Office 365.
-   [ ] I understand Safe Links.
-   [ ] I understand Safe Attachments.
-   [ ] I can choose Defender for Identity.
-   [ ] I can choose Defender for Cloud Apps.
-   [ ] I understand CASB.
-   [ ] I understand Shadow IT.
-   [ ] I can choose Defender XDR.
-   [ ] I can distinguish Defender for Cloud from Defender for Cloud
    Apps.
-   [ ] I can explain why each Defender service exists.

------------------------------------------------------------------------

# ➡️ Next

## 📘 Lesson 13 --- Microsoft Sentinel

Next you will learn about:

``` text
SIEM

SOAR

Data Connectors

Analytics

Incidents

Automation

Security Operations
```

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

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

⬅️ **[Lesson 12 --- Microsoft Defender Security
Services](../lessons/%F0%9F%93%98%20Lesson%2012%20%E2%80%94%20Microsoft%20Defender%20Security%20Services.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
