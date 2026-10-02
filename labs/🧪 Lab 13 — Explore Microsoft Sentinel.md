# 🔵 Lab 13 --- Explore Microsoft Sentinel

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 13 --- Microsoft Sentinel\
**Lab Type:** 🔵 Explore the Tool\
**Difficulty:** Beginner\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🎯 Lab Objectives

By completing this lab, you should be able to locate and recognize:

-   Microsoft Sentinel
-   The Microsoft Defender portal Sentinel experience
-   Data connectors
-   Content hub
-   Analytics
-   Incidents
-   Hunting
-   Threat intelligence
-   Workbooks
-   Automation rules
-   Playbooks
-   The relationship between SIEM and SOAR

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
Connect New Data Sources

Disconnect Existing Sources

Create Analytics Rules

Disable Analytics Rules

Close Real Incidents

Modify Threat Intelligence

Run Response Actions

Create Automation Rules

Run Production Playbooks

Change Sentinel Settings
```

unless specifically authorized.

Do not copy real company incident, user, device, IP, or security
information into a public GitHub repository.

------------------------------------------------------------------------

# 🌐 Part 1 --- Open Microsoft Sentinel

For this lab, begin with the:

``` text
Microsoft Defender Portal
```

Open:

``` text
https://security.microsoft.com
```

Look for:

``` text
Microsoft Sentinel
```

in the navigation.

------------------------------------------------------------------------

# ⚠️ Portal Note

In 2026, some organizations may still use Microsoft Sentinel in the
Azure portal.

However, Microsoft has announced that after:

``` text
March 31, 2027
```

Sentinel will no longer be supported in the Azure portal.

For that reason, this lab emphasizes the Microsoft Defender portal.

If your organization still uses Azure portal Sentinel, you can perform
the equivalent read-only exploration there.

------------------------------------------------------------------------

# 🧭 Part 2 --- Explore Sentinel Navigation

Look for areas such as:

``` text
Content Management

Configuration

Threat Management

Incidents

Hunting

Advanced Hunting

Automation
```

The exact navigation can change.

Do not worry if your portal differs slightly.

------------------------------------------------------------------------

# 🧠 First Impression

What appears to be Sentinel's main purpose?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔌 Part 3 --- Explore Data Connectors

Look for:

``` text
Microsoft Sentinel
      ↓
Configuration
      ↓
Data connectors
```

Do not configure a connector.

Observe the available or installed connectors.

------------------------------------------------------------------------

# 🧠 Connector Question

Complete:

``` text
DATA SOURCE
      ↓
____________________
      ↓
MICROSOFT SENTINEL
```

What is the missing component?

``` text
______________________________
```

------------------------------------------------------------------------

# 📦 Part 4 --- Explore Content Hub

Locate:

``` text
Content hub
```

Do not install anything.

Look at the types of solutions available.

Sentinel solutions can package items such as:

``` text
Data Connectors

Analytics Rules

Workbooks

Hunting Queries

Playbooks
```

Complete:

``` text
CONTENT HUB
=
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔎 Part 5 --- Explore Analytics

Locate:

``` text
Analytics
```

or the current analytics/detection area.

Do not enable, disable, or create rules.

Observe concepts such as:

``` text
Rule Name

Status

Severity

Data Sources

MITRE ATT&CK Information
```

depending on your environment.

------------------------------------------------------------------------

# 🧠 Analytics Question

What is the main purpose of an analytics rule?

``` text
A. Detect suspicious activity

B. Create user accounts

C. Configure printers

D. Assign Microsoft 365 licenses
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🚨 Part 6 --- Explore Incidents

Locate:

``` text
Incidents
```

Do not assign, close, or modify real incidents.

Observe non-sensitive categories such as:

``` text
Severity

Status

Alerts

Affected Entities

Creation Time
```

Do not record real incident details.

------------------------------------------------------------------------

# 🧠 Alert vs Incident

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

# 🕵️ Part 7 --- Explore an Investigation

If your environment contains a safe training/demo incident, look at the
investigation experience without taking action.

Look for entities such as:

``` text
Users

Devices

IP Addresses

Azure Resources
```

If no safe incident is available, complete this conceptually.

Why is it useful to connect entities during an investigation?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🔍 Part 8 --- Explore Hunting

Locate:

``` text
Hunting
```

or:

``` text
Advanced Hunting
```

Do not worry if you cannot run queries.

Observe:

``` text
Queries

Results

Schema / Tables

Security Data
```

------------------------------------------------------------------------

# 🧠 Hunting Question

Complete:

``` text
Threat Hunting
=
____________________________________

____________________________________
```

Hint:

``` text
Proactively search
security data
```

------------------------------------------------------------------------

# 🔤 Part 9 --- KQL

Sentinel threat hunting and security-data analysis commonly use:

``` text
Kusto Query Language
```

or:

``` text
KQL
```

For SC-900:

``` text
YOU DO NOT NEED
TO MASTER KQL
```

Remember:

``` text
KQL
      ↓
QUERY DATA
      ↓
INVESTIGATE
```

------------------------------------------------------------------------

# 📊 Part 10 --- Explore Workbooks

If available in your Sentinel experience, locate:

``` text
Workbooks
```

Do not create or modify one.

A workbook is primarily used to:

``` text
A. Visualize security data

B. Reset passwords

C. Create virtual machines

D. Assign licenses
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🌐 Part 11 --- Explore Threat Intelligence

Look for:

``` text
Threat intelligence
```

Do not add, edit, or remove indicators.

Threat intelligence can include information such as:

``` text
Malicious IP Addresses

Malicious Domains

Indicators of Compromise
```

Why might this information help an investigation?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🤖 Part 12 --- Explore Automation

Locate:

``` text
Microsoft Sentinel
      ↓
Configuration
      ↓
Automation
```

Do not create or modify rules.

Look for concepts such as:

``` text
Automation Rules

Playbooks
```

------------------------------------------------------------------------

# 🧠 Automation Rule vs Playbook

Complete:

``` text
AUTOMATION RULE
=
____________________________________
```

``` text
PLAYBOOK
=
____________________________________
```

Memory:

``` text
AUTOMATION RULE
=
WHEN
```

``` text
PLAYBOOK
=
WHAT WORKFLOW
```

------------------------------------------------------------------------

# 📘 Part 13 --- Playbooks

Sentinel playbooks are based on:

``` text
A. Azure Logic Apps

B. Microsoft Word

C. Azure Bastion

D. Windows Hello
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🧩 Part 14 --- SIEM or SOAR?

Choose:

``` text
SIEM

SOAR
```

## Collect security logs

``` text
______________________________
```

## Analyze security events

``` text
______________________________
```

## Detect suspicious activity

``` text
______________________________
```

## Automatically run a response workflow

``` text
______________________________
```

## Orchestrate repetitive response actions

``` text
______________________________
```

## Investigate centralized security data

``` text
______________________________
```

------------------------------------------------------------------------

# 🏢 Part 15 --- Contoso Data Sources

Contoso uses:

``` text
Microsoft Entra ID

Microsoft Defender

Azure

AWS

Windows Servers

Firewalls
```

Draw the flow:

``` text
ENTRA ───────────────┐
                     │
DEFENDER ────────────┤
                     │
AZURE ───────────────┤
                     │
AWS ─────────────────┼──→ __________________
                     │
SERVERS ─────────────┤
                     │
FIREWALLS ───────────┘
```

What belongs in the blank?

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 16 --- Build the Sentinel Flow

Use:

``` text
Data Sources

Data Connectors

Microsoft Sentinel

Analytics

Incident

Investigation

Automation / Playbook

Response
```

Fill in:

``` text
____________________
        ↓
____________________
        ↓
____________________
        ↓
____________________
        ↓
____________________
        ↓
____________________
        ↓
____________________
        ↓
____________________
```

------------------------------------------------------------------------

# 🛡️ Part 17 --- Sentinel or Defender XDR?

Choose:

``` text
Microsoft Sentinel

Microsoft Defender XDR
```

## Collect security data from many Microsoft and third-party sources

``` text
______________________________
```

## Correlate Microsoft endpoint, identity, email, and cloud-app security signals

``` text
______________________________
```

## Provide SIEM capabilities

``` text
______________________________
```

## Provide extended detection and response across Defender security domains

``` text
______________________________
```

## Provide SOAR automation with Sentinel automation rules and playbooks

``` text
______________________________
```

------------------------------------------------------------------------

# 🔗 Part 18 --- Better Together

Fill in:

``` text
DEFENDER XDR
      ↓
Cross-Domain
Microsoft Security Signals
      ↓
________________________
      ↓
Broad SIEM Data
+
Third-Party Sources
      ↓
Detection
Investigation
Automation
Response
```

Answer:

``` text
______________________________
```

------------------------------------------------------------------------

# 🎯 Part 19 --- Choose the Sentinel Feature

Choose from:

``` text
Data Connector

Analytics Rule

Workbook

Hunting

Threat Intelligence

Automation Rule

Playbook
```

## Bring firewall data into Sentinel

``` text
______________________________
```

## Detect a suspicious pattern

``` text
______________________________
```

## Visualize security trends

``` text
______________________________
```

## Proactively search security data

``` text
______________________________
```

## Add context about known malicious infrastructure

``` text
______________________________
```

## Decide when automated incident handling occurs

``` text
______________________________
```

## Run an automated response workflow

``` text
______________________________
```

------------------------------------------------------------------------

# 🏆 Final Challenge

Contoso wants to build a basic SOC workflow.

Requirements:

``` text
1. Collect logs from cloud and on-premises systems

2. Detect suspicious activity

3. Group security findings for investigation

4. Let analysts proactively search security data

5. Automatically notify the IT team
   when a high-severity incident appears
```

Choose the Sentinel capability for each.

## Requirement 1

``` text
______________________________
```

## Requirement 2

``` text
______________________________
```

## Requirement 3

``` text
______________________________
```

## Requirement 4

``` text
______________________________
```

## Requirement 5

``` text
______________________________
```

------------------------------------------------------------------------

# 🗺️ Part 20 --- Build Your Sentinel Map

  Capability            Main Purpose
  --------------------- ------------------------------------------------------
  Microsoft Sentinel    \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  SIEM                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  SOAR                  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Data Connectors       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Analytics Rules       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Incidents             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Hunting               \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Workbooks             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Threat Intelligence   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Automation Rules      \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Playbooks             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# ✅ Suggested Answers

## Data Connector

``` text
DATA SOURCE
      ↓
DATA CONNECTOR
      ↓
MICROSOFT SENTINEL
```

## Content Hub

``` text
Packaged Sentinel security
content and solutions
```

## Analytics

``` text
A — Detect suspicious activity
```

## Alert vs Incident

``` text
Alert
=
Individual security detection

Incident
=
Related alerts and evidence
grouped for investigation
```

## Hunting

``` text
Proactively search
security data for threats
or suspicious activity
```

## Workbook

``` text
A — Visualize security data
```

## Automation

``` text
Automation Rule
=
Determines when / how
automation is triggered

Playbook
=
Automated response workflow
```

## Playbook Technology

``` text
A — Azure Logic Apps
```

## SIEM vs SOAR

``` text
Collect logs
=
SIEM

Analyze events
=
SIEM

Detect suspicious activity
=
SIEM

Automated response workflow
=
SOAR

Orchestrate response
=
SOAR

Investigate centralized data
=
SIEM
```

## Contoso Data

``` text
Microsoft Sentinel
```

## Sentinel Flow

``` text
Data Sources
      ↓
Data Connectors
      ↓
Microsoft Sentinel
      ↓
Analytics
      ↓
Incident
      ↓
Investigation
      ↓
Automation / Playbook
      ↓
Response
```

## Sentinel vs XDR

``` text
Many Microsoft / third-party sources
=
Microsoft Sentinel

Defender-domain correlation
=
Microsoft Defender XDR

SIEM
=
Microsoft Sentinel

Extended Detection and Response
=
Microsoft Defender XDR

Sentinel SOAR
=
Microsoft Sentinel
```

## Better Together

``` text
Microsoft Sentinel
```

## Choose the Feature

``` text
Firewall Data
=
Data Connector

Suspicious Pattern
=
Analytics Rule

Visual Trends
=
Workbook

Proactive Search
=
Hunting

Known Malicious Infrastructure
=
Threat Intelligence

When Automation Happens
=
Automation Rule

Automated Workflow
=
Playbook
```

## Final Challenge

``` text
1. Data Connectors

2. Analytics Rules

3. Incidents

4. Hunting

5. Automation Rule + Playbook
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

``` text
MICROSOFT SENTINEL
=
SIEM + SOAR
```

``` text
DATA CONNECTOR
=
Bring in data
```

``` text
ANALYTICS
=
Detect
```

``` text
INCIDENT
=
Investigate
```

``` text
HUNTING
=
Search proactively
```

``` text
AUTOMATION RULE
=
When
```

``` text
PLAYBOOK
=
Automated workflow
```

------------------------------------------------------------------------

# ✅ Lab Completion Checklist

-   [ ] I can explain SIEM.
-   [ ] I can explain SOAR.
-   [ ] I can locate Microsoft Sentinel.
-   [ ] I understand data connectors.
-   [ ] I understand the Content hub.
-   [ ] I understand analytics rules.
-   [ ] I can explain incidents.
-   [ ] I understand threat hunting.
-   [ ] I understand workbooks.
-   [ ] I understand threat intelligence.
-   [ ] I can distinguish automation rules from playbooks.
-   [ ] I can distinguish Sentinel from Defender XDR.
-   [ ] I understand how Sentinel and Defender XDR can work together.

------------------------------------------------------------------------

# 🏗️ Next

You have completed the Microsoft Security Solutions lessons.

Continue to:

## 🏗️ Project 02 --- Build a Microsoft Security Strategy

This project will combine:

``` text
Azure Infrastructure Security

Defender for Cloud

Defender XDR

Defender Security Services

Microsoft Sentinel
```

After Project 02:

## 📘 Lesson 14 --- Microsoft Purview & Compliance

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

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

⬅️ **[Lesson 13 --- Microsoft
Sentinel](../lessons/%F0%9F%93%98%20Lesson%2013%20%E2%80%94%20Microsoft%20Sentinel.md)**

🏗️ **Project 02 --- Build a Microsoft Security Strategy**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏠 **[Return to Main README](../README.md)**
