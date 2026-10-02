# 🔵 Lab 11 --- Explore Microsoft Defender XDR

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 11 --- Microsoft Defender XDR\
**Lab Type:** 🔵 Explore the Tool\
**Difficulty:** Beginner\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🎯 Lab Objectives

By completing this lab, you should be able to locate and recognize:

-   The Microsoft Defender portal
-   Incidents
-   Alerts
-   Incident evidence and entities
-   Endpoints
-   Identity-related security areas
-   Email and collaboration security
-   Cloud application security
-   Automated investigation and response
-   Advanced Hunting
-   The relationship among Microsoft Defender security signals

------------------------------------------------------------------------

# 🔵 Explore the Tool

Use:

``` text
FIND
  ↓
OBSERVE
  ↓
UNDERSTAND
  ↓
CONNECT TO SC-900
```

This is a read-only exploration lab.

------------------------------------------------------------------------

# ⚠️ Production Safety

Do not:

``` text
Resolve Real Incidents

Dismiss Alerts

Isolate Devices

Delete Emails

Disable Users

Take Remediation Actions

Run Response Actions

Change Security Policies

Submit Production Indicators

Modify Automated Response Settings
```

unless specifically authorized.

Do not copy sensitive company incident information into a public GitHub
repository.

If your permissions or licensing do not expose a feature, complete the
conceptual exercise and continue.

------------------------------------------------------------------------

# 🌐 Part 1 --- Open Microsoft Defender

Open:

``` text
https://security.microsoft.com
```

Sign in with an authorized work or school account.

Observe the navigation.

The exact portal layout can change.

------------------------------------------------------------------------

# 🧭 Part 2 --- Explore the Defender Portal

Look for areas related to:

``` text
Incidents & Alerts

Assets

Endpoints

Email & Collaboration

Identities

Cloud Apps

Hunting

System / Settings
```

You may not see every area.

That is okay.

------------------------------------------------------------------------

# 🧠 First Impression

What appears to be the Defender portal's main purpose?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🚨 Part 3 --- Find Incidents

Locate:

``` text
Incidents
```

Do not change incident status or assignment.

If incidents are visible, observe only non-sensitive categories such as:

``` text
Severity

Status

Number of Alerts

Affected Assets

Creation Time
```

Do not record real incident names or user/device information.

------------------------------------------------------------------------

# 🚨 Part 4 --- Find Alerts

Locate:

``` text
Alerts
```

Observe how alerts differ from incidents.

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

------------------------------------------------------------------------

# 🧩 Part 5 --- Build an Incident

Imagine these alerts occur:

``` text
Alert 1:
Phishing email delivered

Alert 2:
Malware executed on laptop

Alert 3:
Suspicious account sign-in

Alert 4:
Unusual cloud application activity
```

Would it be useful to investigate these as:

``` text
A. Four completely unrelated events

B. One potentially connected attack story
```

Answer:

``` text
______________________________
```

Why?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔗 Part 6 --- Explore Incident Evidence

If you are authorized to safely open a non-sensitive training/demo
incident, look for concepts such as:

``` text
Alerts

Devices

Users

Mailboxes

Files

IP Addresses

URLs

Applications
```

Do not perform any response actions.

These are examples of:

``` text
Evidence

Entities

Affected Assets
```

------------------------------------------------------------------------

# 🕵️ Part 7 --- Attack Story

Put these events in a logical order:

``` text
A. Attacker accesses cloud application

B. User receives phishing email

C. Malware runs on endpoint

D. User clicks malicious link

E. Credentials are stolen

F. Suspicious sign-in occurs
```

Your order:

``` text
1. ______

2. ______

3. ______

4. ______

5. ______

6. ______
```

------------------------------------------------------------------------

# 💻 Part 8 --- Explore Endpoint Security

Look for:

``` text
Endpoints

Devices

Assets
```

depending on your portal.

Do not isolate or remediate a device.

At a high level:

``` text
Microsoft Defender for Endpoint
=
____________________________________
```

------------------------------------------------------------------------

# 👤 Part 9 --- Explore Identity Security

Look for identity-related security information available in your portal.

Depending on licensing and configuration, identity signals can help
detect suspicious identity activity.

Complete:

``` text
Microsoft Defender for Identity
=
____________________________________
```

------------------------------------------------------------------------

# 📧 Part 10 --- Explore Email & Collaboration

Look for:

``` text
Email & collaboration
```

or related areas.

Do not delete or remediate messages.

Which threats might this area help address?

``` text
[ ] Phishing

[ ] Malicious Links

[ ] Malicious Attachments

[ ] Business Email Compromise
```

At a high level:

``` text
Microsoft Defender for Office 365
=
____________________________________
```

------------------------------------------------------------------------

# ☁️ Part 11 --- Explore Cloud Application Security

Look for cloud-app-related security capabilities if available.

At a high level:

``` text
Microsoft Defender for Cloud Apps
=
____________________________________
```

Think:

``` text
Cloud application visibility
and security
```

------------------------------------------------------------------------

# 🧠 Part 12 --- Match the Defender Service

Choose:

``` text
Defender for Endpoint

Defender for Identity

Defender for Office 365

Defender for Cloud Apps
```

## Protect and investigate a laptop

``` text
______________________________
```

## Detect identity-related threats

``` text
______________________________
```

## Protect users from phishing email

``` text
______________________________
```

## Monitor and protect cloud application activity

``` text
______________________________
```

------------------------------------------------------------------------

# 🤖 Part 13 --- Explore Automated Investigation

Look for:

``` text
Investigations

Action center

Automated investigation
```

depending on your portal and licensing.

Do not approve or reject real actions.

Complete:

``` text
Automated Investigation
and Response helps:

____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🧠 Automation Scenario

A security platform can automatically collect evidence and investigate
supported suspicious activity.

What is the primary benefit?

``` text
A. Reduce repetitive investigation work

B. Eliminate the need for all security staff

C. Guarantee no attack succeeds

D. Disable every account automatically
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🔎 Part 14 --- Explore Advanced Hunting

Locate:

``` text
Advanced Hunting
```

Do not worry if you do not have permission to run queries.

Observe the interface.

You may see:

``` text
Query Area

Schema / Tables

Results

Query History
```

------------------------------------------------------------------------

# 🧠 What Is Advanced Hunting?

Complete:

``` text
Advanced Hunting
=
____________________________________

____________________________________
```

Hint:

``` text
Query-based proactive
security investigation
```

------------------------------------------------------------------------

# 🔤 Part 15 --- KQL

Advanced Hunting commonly uses:

``` text
Kusto Query Language
```

abbreviated:

``` text
KQL
```

For SC-900, you do not need to become a KQL expert.

Remember:

``` text
KQL
      ↓
Query Security Data
      ↓
Find Suspicious Activity
```

------------------------------------------------------------------------

# 🕵️ Part 16 --- Alert or Hunting?

## Scenario 1

Microsoft detects malware and tells the analyst to investigate.

``` text
Alert / Hunting
```

Answer:

``` text
______________________________
```

## Scenario 2

An analyst proactively searches for devices that contacted a suspicious
domain.

``` text
Alert / Hunting
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🏢 Part 17 --- Contoso Attack

Contoso experiences:

``` text
1. Phishing email

2. Malicious attachment

3. Endpoint compromise

4. Credential theft

5. Suspicious sign-in

6. Cloud application access
```

Match the areas:

  Event                        Defender Area
  ---------------------------- ------------------------------------------------------
  Phishing email               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Endpoint compromise          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Identity activity            \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud application activity   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

What platform helps connect the overall attack?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 18 --- Build the XDR Flow

Fill in:

``` text
EMAIL
      ↓
____________________
      ↓
ENDPOINT
      ↓
____________________
      ↓
IDENTITY
      ↓
____________________
      ↓
CLOUD APP
      ↓
____________________
      ↓
DEFENDER XDR
      ↓
____________________
      ↓
INVESTIGATION
      ↓
RESPONSE
```

Use appropriate Defender services and:

``` text
Incident
```

------------------------------------------------------------------------

# 🚨 Part 19 --- Incident vs Alert Challenge

Choose:

``` text
Alert

Incident
```

## A malicious attachment is detected.

``` text
______________________________
```

## Several related security detections are grouped into one attack investigation.

``` text
______________________________
```

## Suspicious endpoint behavior is detected.

``` text
______________________________
```

## Phishing, endpoint malware, and identity compromise are correlated.

``` text
______________________________
```

------------------------------------------------------------------------

# ☁️ Part 20 --- Defender XDR or Defender for Cloud?

Choose:

``` text
Microsoft Defender XDR

Microsoft Defender for Cloud
```

## Improve Azure/cloud security posture

``` text
______________________________
```

## Correlate phishing, endpoint, and identity alerts

``` text
______________________________
```

## Review cloud security recommendations

``` text
______________________________
```

## Investigate a cross-domain attack incident

``` text
______________________________
```

------------------------------------------------------------------------

# 🗺️ Part 21 --- Build Your Defender XDR Map

  Capability                Main Purpose
  ------------------------- ------------------------------------------------------
  Defender XDR              \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Alert                     \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Incident                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender for Endpoint     \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender for Identity     \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender for Office 365   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender for Cloud Apps   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Automated Investigation   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Advanced Hunting          \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# ✅ Suggested Answers

## Alert vs Incident

``` text
Alert
=
Individual security detection

Incident
=
Related alerts and evidence
grouped into an investigation
```

## Incident Scenario

``` text
B
```

The events may represent stages of one attack and should be investigated
in context.

## Attack Story

``` text
1. B — Phishing email

2. D — User clicks link

3. C — Malware runs

4. E — Credentials stolen

5. F — Suspicious sign-in

6. A — Cloud application access
```

## Defender Services

``` text
Endpoint
=
Endpoint security

Identity
=
Identity threat detection

Office 365
=
Email and collaboration security

Cloud Apps
=
Cloud application security
```

## Match the Service

``` text
Laptop
=
Defender for Endpoint

Identity threats
=
Defender for Identity

Phishing
=
Defender for Office 365

Cloud application activity
=
Defender for Cloud Apps
```

## Automation

``` text
A — Reduce repetitive investigation work
```

## Advanced Hunting

``` text
Query-based proactive
security investigation
```

## Alert vs Hunting

``` text
1. Alert

2. Hunting
```

## Contoso Attack

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

Overall correlation
=
Microsoft Defender XDR
```

## XDR Flow

``` text
EMAIL
      ↓
Defender for Office 365
      ↓
ENDPOINT
      ↓
Defender for Endpoint
      ↓
IDENTITY
      ↓
Defender for Identity
      ↓
CLOUD APP
      ↓
Defender for Cloud Apps
      ↓
DEFENDER XDR
      ↓
Incident
      ↓
INVESTIGATION
      ↓
RESPONSE
```

## Incident vs Alert

``` text
1. Alert

2. Incident

3. Alert

4. Incident
```

## XDR vs Defender for Cloud

``` text
Cloud posture
=
Defender for Cloud

Cross-domain correlation
=
Defender XDR

Cloud recommendations
=
Defender for Cloud

Cross-domain incident
=
Defender XDR
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

``` text
DEFENDER XDR
=
Connect security signals
across domains
```

``` text
ALERT
=
One security warning
```

``` text
INCIDENT
=
Related attack story
```

``` text
AUTOMATION
=
Help investigate and respond
```

``` text
ADVANCED HUNTING
=
Proactively query security data
```

------------------------------------------------------------------------

# ✅ Lab Completion Checklist

-   [ ] I can locate the Microsoft Defender portal.
-   [ ] I can distinguish alerts from incidents.
-   [ ] I understand attack correlation.
-   [ ] I know what Defender for Endpoint protects.
-   [ ] I know what Defender for Identity focuses on.
-   [ ] I know what Defender for Office 365 protects.
-   [ ] I know what Defender for Cloud Apps focuses on.
-   [ ] I understand automated investigation and response.
-   [ ] I understand the purpose of Advanced Hunting.
-   [ ] I can distinguish Defender XDR from Defender for Cloud.

------------------------------------------------------------------------

# ➡️ Next

## 📘 Lesson 12 --- Microsoft Defender Security Services

Next you will compare the major Microsoft Defender services and practice
choosing the correct service for different security scenarios.

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [Microsoft Defender Portal](https://security.microsoft.com/)
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

⬅️ **[Lesson 11 --- Microsoft Defender
XDR](../lessons/%F0%9F%93%98%20Lesson%2011%20%E2%80%94%20Microsoft%20Defender%20XDR.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
