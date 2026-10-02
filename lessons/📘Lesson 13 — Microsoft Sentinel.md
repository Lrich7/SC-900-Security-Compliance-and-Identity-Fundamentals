# 📘 Lesson 13 --- Microsoft Sentinel

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Lesson:** 13\
**Section:** Microsoft Security Solutions\
**Lab:** 🔵 Explore the Tool --- Microsoft Sentinel\
**Difficulty:** Beginner\
**Milestone:** Completes the Microsoft Security Solutions section

------------------------------------------------------------------------

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

-   Explain Microsoft Sentinel
-   Define SIEM
-   Define SOAR
-   Explain how Sentinel collects security data
-   Describe data connectors
-   Explain analytics and threat detection
-   Describe incidents and investigation
-   Explain threat hunting at a fundamentals level
-   Describe automation rules and playbooks
-   Explain how Sentinel supports multicloud and multiplatform
    environments
-   Distinguish Microsoft Sentinel from Microsoft Defender XDR
-   Explain how Sentinel and Defender XDR can work together

------------------------------------------------------------------------

# 🛡️ What Is Microsoft Sentinel?

**Microsoft Sentinel** is Microsoft's cloud-native **Security
Information and Event Management (SIEM)** solution.

It helps security teams:

``` text
COLLECT
      ↓
DETECT
      ↓
INVESTIGATE
      ↓
RESPOND
      ↓
HUNT
```

across security data from many different systems.

Microsoft Sentinel can collect data from:

``` text
Users

Devices

Applications

Infrastructure

Microsoft Services

Third-Party Products

On-Premises Systems

Multiple Clouds
```

------------------------------------------------------------------------

# 🧠 Why Does a SIEM Exist?

A modern organization may have security data coming from:

``` text
Firewalls

Servers

Endpoints

Identity Systems

Cloud Platforms

Applications

Email Security

Network Devices
```

Without a central system:

``` text
FIREWALL LOGS → One Console

IDENTITY LOGS → Another Console

ENDPOINT LOGS → Another Console

CLOUD LOGS → Another Console
```

Security teams may struggle to see the full picture.

A SIEM helps bring that information together.

------------------------------------------------------------------------

# 📊 SIEM

**SIEM** stands for:

# Security Information and Event Management

At a fundamentals level, a SIEM:

``` text
COLLECTS SECURITY DATA

ANALYZES SECURITY DATA

DETECTS SUSPICIOUS ACTIVITY

HELPS INVESTIGATE INCIDENTS
```

Think:

``` text
MANY DATA SOURCES
      ↓
SIEM
      ↓
CENTRAL SECURITY VISIBILITY
```

------------------------------------------------------------------------

# 🤖 SOAR

**SOAR** stands for:

# Security Orchestration, Automation, and Response

SOAR helps security teams automate repeatable security tasks.

Conceptually:

``` text
SECURITY EVENT
      ↓
AUTOMATION
      ↓
RESPONSE ACTIONS
```

Examples could include:

``` text
Create a Ticket

Notify a Security Team

Gather Additional Information

Run a Response Workflow
```

The exact actions depend on the organization's configuration.

------------------------------------------------------------------------

# 🧠 SIEM vs SOAR

This distinction is important.

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
Automate
Orchestrate
Respond
```

Memory trick:

``` text
SIEM
=
SEE WHAT IS HAPPENING
```

``` text
SOAR
=
HELP DO SOMETHING ABOUT IT
```

------------------------------------------------------------------------

# 🔌 Data Connectors

Microsoft Sentinel needs security data.

**Data connectors** help bring information from different products and
services into Sentinel.

Examples can include:

``` text
Microsoft Entra ID

Microsoft Defender

Azure Services

Firewalls

Servers

AWS

Other Security Products
```

Microsoft also supports common integration methods and custom connectors
for supported scenarios.

------------------------------------------------------------------------

# 🧠 Data Connector Flow

``` text
DATA SOURCE
      ↓
DATA CONNECTOR
      ↓
MICROSOFT SENTINEL
      ↓
ANALYSIS
```

Without data:

``` text
NO VISIBILITY
```

So data collection is one of the foundations of a SIEM.

------------------------------------------------------------------------

# 📦 Content Hub

Microsoft Sentinel provides packaged security content through the
**Content hub**.

Solutions can include items such as:

``` text
Data Connectors

Analytics Rules

Workbooks

Hunting Queries

Playbooks
```

Think:

``` text
CONTENT HUB
=
Packaged Sentinel content
for products and services
```

------------------------------------------------------------------------

# 🔎 Analytics

After data is collected, Sentinel needs to identify suspicious activity.

**Analytics rules** help detect threats in security data.

Conceptually:

``` text
SECURITY DATA
      ↓
ANALYTICS RULE
      ↓
SUSPICIOUS PATTERN?
   ↙             ↘
 NO              YES
                  ↓
               ALERT
                  ↓
              INCIDENT
```

Sentinel can use analytics to help group alerts into incidents for
investigation.

------------------------------------------------------------------------

# 🚨 Alerts and Incidents

Recall Lesson 11:

``` text
ALERT
=
Individual security detection
```

``` text
INCIDENT
=
Related alerts and evidence
grouped for investigation
```

Sentinel uses security data and analytics to help generate and
investigate incidents.

------------------------------------------------------------------------

# 🕵️ Investigation

A security analyst may need to answer:

``` text
What happened?

Which users were involved?

Which devices were involved?

Which IP addresses were involved?

How did the attack progress?

What should we do next?
```

Sentinel helps provide information and context for security
investigations.

------------------------------------------------------------------------

# 🔍 Threat Hunting

Not every attack begins with an alert.

Security teams may proactively search security data for suspicious
activity.

This is:

# Threat Hunting

Conceptually:

``` text
QUESTION
      ↓
QUERY SECURITY DATA
      ↓
LOOK FOR PATTERNS
      ↓
INVESTIGATE
```

Microsoft security hunting commonly uses:

``` text
Kusto Query Language — KQL
```

For SC-900, understand the purpose of hunting. You do not need to become
a KQL expert.

------------------------------------------------------------------------

# 📊 Workbooks

**Workbooks** provide interactive visualizations of Sentinel data.

They can help security teams understand:

``` text
Trends

Patterns

Security Events

Data Sources

Operational Information
```

Think:

``` text
SECURITY DATA
      ↓
WORKBOOK
      ↓
VISUAL DASHBOARD
```

------------------------------------------------------------------------

# 🧠 Workbook vs Analytics Rule

Do not confuse these.

``` text
WORKBOOK
=
Visualize information
```

``` text
ANALYTICS RULE
=
Detect suspicious activity
```

------------------------------------------------------------------------

# 🌐 Threat Intelligence

**Threat intelligence** provides information about known or suspected
threats.

Examples can include:

``` text
Malicious IP Addresses

Malicious Domains

Known Indicators of Compromise

Threat Actor Infrastructure
```

Sentinel can use threat intelligence to provide additional context for
detection and investigation.

------------------------------------------------------------------------

# 🧠 Threat Intelligence Example

Suppose Sentinel sees:

``` text
Internal Device
      ↓
Connection
      ↓
Known Malicious IP
```

Threat intelligence can help security teams understand that the
destination may be associated with malicious activity.

------------------------------------------------------------------------

# 🤖 Automation Rules

Sentinel provides **automation rules** to help automate incident
handling.

Conceptually:

``` text
INCIDENT CREATED
      ↓
AUTOMATION RULE
      ↓
PERFORM DEFINED ACTION
```

Examples can include:

``` text
Assign Incident

Change Status

Add Information

Run a Playbook
```

------------------------------------------------------------------------

# 📘 Playbooks

A **playbook** is a collection of automated response actions.

Microsoft Sentinel playbooks are based on:

``` text
Azure Logic Apps
```

Conceptually:

``` text
SECURITY INCIDENT
      ↓
AUTOMATION RULE
      ↓
PLAYBOOK
      ↓
AUTOMATED WORKFLOW
```

------------------------------------------------------------------------

# 🧠 Automation Rule vs Playbook

Think:

``` text
AUTOMATION RULE
=
WHEN should automation happen?
```

``` text
PLAYBOOK
=
WHAT workflow should run?
```

Example:

``` text
WHEN:
High-severity incident appears
      ↓
RUN:
Playbook
      ↓
Create ticket
Notify security team
Gather information
```

------------------------------------------------------------------------

# 🏢 SOC

A **Security Operations Center (SOC)** monitors and responds to security
threats.

A common workflow is:

``` text
COLLECT
      ↓
DETECT
      ↓
TRIAGE
      ↓
INVESTIGATE
      ↓
RESPOND
      ↓
HUNT
      ↓
IMPROVE
```

Sentinel provides capabilities across much of this workflow.

------------------------------------------------------------------------

# 🌎 Multicloud and Multiplatform

Sentinel is designed to collect security data across different
environments.

That can include:

``` text
Microsoft Cloud

Other Cloud Platforms

On-Premises Infrastructure

Third-Party Security Products

Network Devices

Applications
```

This is important because real organizations rarely use only one product
or platform.

------------------------------------------------------------------------

# 🧱 Sentinel + Defender XDR

Microsoft Sentinel and Defender XDR can work together.

## Defender XDR

Think:

``` text
Microsoft Security Signals
      ↓
Cross-Domain Detection
      ↓
Incident
      ↓
Investigation / Response
```

## Sentinel

Think:

``` text
Broad Security Data
from Many Sources
      ↓
SIEM Analytics
      ↓
Detection
      ↓
Investigation
      ↓
SOAR
```

------------------------------------------------------------------------

# 🔗 Unified Security Operations

Microsoft Sentinel is available in the **Microsoft Defender portal**,
providing a more unified experience with Defender XDR.

This can combine:

``` text
SIEM
+
XDR
```

into a more centralized security operations experience.

For SC-900, understand the relationship rather than memorizing every
portal menu.

------------------------------------------------------------------------

# ⚠️ Current Portal Direction

Microsoft Sentinel is currently available in both the Microsoft Defender
portal and the Azure portal.

Microsoft has announced that after:

``` text
March 31, 2027
```

Microsoft Sentinel will no longer be supported in the Azure portal and
will be available through the Microsoft Defender portal.

Because this course is being built in 2026, the lab emphasizes the
**Microsoft Defender portal** while acknowledging that some
organizations may still use the Azure portal during the transition.

------------------------------------------------------------------------

# 🏢 Real-World Example

Contoso uses:

``` text
Microsoft 365

Microsoft Entra ID

Windows Endpoints

Azure

AWS

Firewalls

On-Premises Servers
```

Security wants centralized visibility.

Conceptually:

``` text
ENTRA ──────────────┐
                    │
DEFENDER ───────────┤
                    │
AZURE ──────────────┤
                    │
AWS ────────────────┼──→ MICROSOFT SENTINEL
                    │           ↓
FIREWALLS ──────────┤       ANALYTICS
                    │           ↓
SERVERS ────────────┘       INCIDENTS
                                ↓
                           INVESTIGATION
                                ↓
                            AUTOMATION
                                ↓
                             RESPONSE
```

------------------------------------------------------------------------

# 🎯 Exam Focus

Know these relationships:

``` text
MICROSOFT SENTINEL
=
Cloud-native SIEM
```

``` text
SIEM
=
Security Information
and Event Management
```

``` text
SOAR
=
Security Orchestration,
Automation, and Response
```

``` text
DATA CONNECTOR
=
Bring security data
into Sentinel
```

``` text
ANALYTICS RULE
=
Detect suspicious activity
```

``` text
WORKBOOK
=
Visualize data
```

``` text
HUNTING
=
Proactively search
for threats
```

``` text
AUTOMATION RULE
=
Trigger / coordinate automation
```

``` text
PLAYBOOK
=
Automated response workflow
```

------------------------------------------------------------------------

# 🧠 Memory Map

``` text
DATA
  ↓
CONNECTOR
  ↓
SENTINEL
  ↓
ANALYTICS
  ↓
ALERT / INCIDENT
  ↓
INVESTIGATE
  ↓
AUTOMATION
  ↓
PLAYBOOK
  ↓
RESPONSE
```

------------------------------------------------------------------------

# ❓ Knowledge Check

### 1. What type of security solution is Microsoft Sentinel?

A. SIEM\
B. Password manager\
C. Endpoint operating system\
D. Email client

### 2. What does SIEM stand for?

A. Security Information and Event Management\
B. Secure Identity Endpoint Management\
C. System Internet Event Monitoring\
D. Security Infrastructure Email Management

### 3. What does SOAR stand for?

A. Security Orchestration, Automation, and Response\
B. Security Operations and Resource Allocation\
C. Secure Office Application Reporting\
D. System Operations Automatic Recovery

### 4. What is the purpose of a data connector?

A. Bring data from a source into Sentinel\
B. Reset user passwords\
C. Create virtual machines\
D. Assign Microsoft 365 licenses

### 5. What do analytics rules help do?

A. Detect suspicious activity\
B. Create email signatures\
C. Configure printers\
D. Purchase Azure subscriptions

### 6. What is a workbook primarily used for?

A. Visualizing security data\
B. Resetting passwords\
C. Creating users\
D. Blocking all network traffic

### 7. What is threat hunting?

A. Proactively searching security data for suspicious activity\
B. Creating backups\
C. Buying threat intelligence\
D. Assigning RBAC roles

### 8. What is a Sentinel playbook?

A. An automated response workflow\
B. A password policy\
C. A network subnet\
D. A compliance label

### 9. What technology underlies Sentinel playbooks?

A. Azure Logic Apps\
B. Microsoft Word\
C. Windows Hello\
D. Azure Bastion

### 10. Which statement is correct?

A. Sentinel provides SIEM/SOAR capabilities, while Defender XDR focuses
on extended detection and response\
B. Sentinel is only an email filter\
C. Sentinel replaces Microsoft Entra ID\
D. Sentinel is only an endpoint antivirus product

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
MICROSOFT SENTINEL
=
SIEM
+
SOAR
```

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
Automate
Orchestrate
Respond
```

Sentinel helps security teams collect security data from many sources,
detect threats, investigate incidents, hunt for suspicious activity, and
automate response.

------------------------------------------------------------------------

# 🧪 Lab

## 🔵 Lab 13 --- Explore Microsoft Sentinel

➡️ **[Lab 13 --- Explore Microsoft
Sentinel](../labs/%F0%9F%94%B5%20Lab%2013%20%E2%80%94%20Explore%20Microsoft%20Sentinel.md)**

------------------------------------------------------------------------

# 🏗️ Project Checkpoint

You have now completed:

``` text
Lesson 09 — Azure Infrastructure Security

Lesson 10 — Microsoft Defender for Cloud

Lesson 11 — Microsoft Defender XDR

Lesson 12 — Microsoft Defender Security Services

Lesson 13 — Microsoft Sentinel
```

Next complete:

## 🏗️ Project 02 --- Build a Microsoft Security Strategy

This project combines the Microsoft security concepts from Lessons
09--13.

------------------------------------------------------------------------

# ➡️ After Project 02

Continue to:

## 📘 Lesson 14 --- Microsoft Purview & Compliance

This begins the Microsoft Compliance Solutions section.

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [SC-900 Study
    Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
-   [Microsoft Sentinel
    Overview](https://learn.microsoft.com/en-us/azure/sentinel/overview)
-   [Microsoft Sentinel Data
    Connectors](https://learn.microsoft.com/en-us/azure/sentinel/connect-data-sources)
-   [Microsoft Sentinel
    Automation](https://learn.microsoft.com/en-us/azure/sentinel/automation/automation)
-   [Microsoft Sentinel in the Defender
    Portal](https://learn.microsoft.com/en-us/azure/sentinel/microsoft-sentinel-defender-portal)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **Lesson 12 --- Microsoft Defender Security Services**

🧪 **[Lab
13](../labs/%F0%9F%94%B5%20Lab%2013%20%E2%80%94%20Explore%20Microsoft%20Sentinel.md)**

🏗️ **Project 02 --- Build a Microsoft Security Strategy**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

🏠 **[Return to Main README](../README.md)**
