# 🔵 Lab 10 --- Explore Microsoft Defender for Cloud

**Course:** Microsoft SC-900 --- Security, Compliance, and Identity
Fundamentals\
**Related Lesson:** Lesson 10 --- Microsoft Defender for Cloud\
**Lab Type:** 🔵 Explore the Tool\
**Difficulty:** Beginner\
**Configuration Changes:** None required

------------------------------------------------------------------------

# 🎯 Lab Objectives

By completing this lab, you should be able to locate and recognize:

-   Microsoft Defender for Cloud
-   Cloud security overview
-   Security posture
-   Cloud Secure Score
-   Security recommendations
-   Security standards
-   Regulatory compliance
-   Workload protection
-   Security alerts
-   Asset inventory
-   Connected cloud environments
-   The difference between CSPM and CWPP

------------------------------------------------------------------------

# 🔵 Explore the Tool

``` text
FIND
  ↓
OBSERVE
  ↓
UNDERSTAND
  ↓
CONNECT TO SC-900
```

You do not need to change any Defender for Cloud settings.

------------------------------------------------------------------------

# ⚠️ Production Safety

Do not:

``` text
Enable Paid Defender Plans
Change Security Policies
Dismiss Recommendations
Exempt Resources
Change Cloud Connections
Modify Regulatory Standards
Respond to Real Security Alerts
Remediate Production Resources
```

unless specifically authorized.

Some features require particular roles, plans, licenses, or connected
environments.

------------------------------------------------------------------------

# 🌐 Part 1 --- Open Defender for Cloud

Microsoft is expanding Defender for Cloud into the unified Microsoft
Defender portal while Azure portal experiences also remain available.

Depending on your environment, explore:

``` text
https://security.microsoft.com
```

and/or:

``` text
https://portal.azure.com
```

In the Defender portal, look for:

``` text
Cloud security
```

In Azure portal, search:

``` text
Microsoft Defender for Cloud
```

Focus on the concepts rather than one exact menu path.

------------------------------------------------------------------------

# 🧭 Part 2 --- Explore the Overview

Look for high-level information such as:

``` text
Security Posture
Recommendations
Alerts / Threat Protection
Protected Assets
Cloud Environments
```

Do not record company-specific findings in a public repository.

In your own words:

``` text
What is the overview trying
to tell a security team?

____________________________________

____________________________________
```

------------------------------------------------------------------------

# 📊 Part 3 --- Find Security Posture

Locate:

``` text
Security posture
```

or the equivalent posture area.

Look for:

``` text
Cloud Secure Score / Secure Score
Recommendations
Environment Filters
Asset Information
```

------------------------------------------------------------------------

# 📈 Part 4 --- Explore Cloud Secure Score

Do not focus on your organization's actual number.

Answer:

``` text
What is the score trying to summarize?

____________________________________
```

``` text
What can help improve security posture?

____________________________________
```

Remember:

``` text
SECURE SCORE
=
SECURITY POSTURE INDICATOR
```

not:

``` text
GUARANTEE THAT NOTHING
CAN BE COMPROMISED
```

Microsoft currently has a newer risk-based Cloud Secure Score in the
Defender portal and a classic Defender for Cloud secure-score model in
Azure portal.

------------------------------------------------------------------------

# 📋 Part 5 --- Explore Recommendations

Locate:

``` text
Recommendations
```

Do not remediate or dismiss anything.

Depending on your experience, categories can include:

``` text
Misconfigurations
Vulnerabilities
Exposed Secrets
```

Look for information such as:

``` text
Description
Affected Resources
Severity / Risk
Remediation Guidance
Security Standard / Control
```

Complete:

``` text
A Defender for Cloud recommendation
helps an administrator:

____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🟡 Part 6 --- Recommendation Scenario

Defender for Cloud reports:

``` text
Management ports on a VM
are exposed to the internet.
```

Is this primarily:

``` text
A. Security Posture Finding

B. Proof that an attacker
   already compromised the VM
```

Answer:

``` text
______________________________
```

Explain:

``` text
____________________________________
```

------------------------------------------------------------------------

# 📏 Part 7 --- Explore Security Standards

Look for standards-related areas.

Try to identify:

``` text
Microsoft Cloud Security Benchmark
```

Do not change assignments.

Complete:

``` text
SECURITY STANDARD
      ↓
Defines expected
________________________
```

``` text
RECOMMENDATION
      ↓
Suggests
________________________
```

------------------------------------------------------------------------

# 📜 Part 8 --- Explore Regulatory Compliance

Locate:

``` text
Regulatory compliance
```

if available.

Does viewing a compliance dashboard automatically prove that an
organization is fully legally compliant?

``` text
YES / NO
```

Explain:

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🛡️ Part 9 --- Find Workload Protection

Locate the workload-protection area available in your portal.

Look for workload areas such as:

``` text
Servers
Containers
Storage
Databases
APIs
```

Do not enable a paid plan.

------------------------------------------------------------------------

# 🧠 Part 10 --- CSPM or CWPP?

## Scenario 1 --- Find an insecure cloud configuration.

``` text
CSPM / CWPP
```

## Scenario 2 --- Protect a server workload from threats.

``` text
CSPM / CWPP
```

## Scenario 3 --- Provide security recommendations.

``` text
CSPM / CWPP
```

## Scenario 4 --- Detect malicious activity against a protected workload.

``` text
CSPM / CWPP
```

------------------------------------------------------------------------

# 🚨 Part 11 --- Explore Security Alerts

Locate security alerts or the threat-detection area.

Do not respond to or modify real alerts.

Complete:

``` text
RECOMMENDATION
=
____________________________________
```

``` text
ALERT
=
____________________________________
```

Memory trick:

``` text
RECOMMENDATION → IMPROVE
ALERT → INVESTIGATE
```

------------------------------------------------------------------------

# 📦 Part 12 --- Explore Asset Inventory

Locate:

``` text
Inventory
Assets
Cloud assets
```

depending on the portal.

Why is asset inventory important?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🌎 Part 13 --- Explore Environment Coverage

Look for connected environments, cloud scopes, or environment settings.

Defender for Cloud can support connected:

``` text
Azure
AWS
GCP
Hybrid / On-Premises Resources
```

Do not add or remove connections.

Why is centralized multicloud visibility useful?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🛤️ Part 14 --- Find Attack Paths

If your plan and portal provide:

``` text
Attack paths
```

open the area in read-only mode.

If unavailable, complete this conceptually.

``` text
Weakness
      ↓
Connection
      ↓
Another Weakness
      ↓
Important Asset
```

Why can a chain of smaller weaknesses matter?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🎯 Part 15 --- Prioritize the Work

Imagine Defender for Cloud identifies:

``` text
A:
Low-risk issue on an isolated test resource

B:
Critical weakness on an internet-exposed
production resource

C:
Minor issue on an unused resource
```

Which would you investigate first?

``` text
A / B / C
```

Why?

``` text
____________________________________

____________________________________
```

------------------------------------------------------------------------

# 🧱 Part 16 --- Connect to Lesson 09

Choose:

``` text
NSG
Azure Bastion
Azure Key Vault
Defender for Cloud
```

## Control network traffic to a VM

``` text
______________________________
```

## Securely connect to a VM without unnecessarily exposing RDP/SSH

``` text
______________________________
```

## Protect application secrets

``` text
______________________________
```

## Continuously assess the cloud environment and recommend improvements

``` text
______________________________
```

------------------------------------------------------------------------

# 🏗️ Part 17 --- Build the Defender for Cloud Flow

Choices:

``` text
Cloud Resources
Continuous Assessment
Recommendations
Remediation
Improved Security Posture
```

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
```

------------------------------------------------------------------------

# 🛡️ Part 18 --- Posture vs Protection

Complete:

``` text
CSPM
      ↓
Find ______________________
      ↓
Generate __________________
      ↓
Improve ___________________
```

and:

``` text
CWPP
      ↓
Protect ___________________
      ↓
Detect ____________________
      ↓
Generate __________________
```

------------------------------------------------------------------------

# 🏢 Part 19 --- Contoso Challenge

Contoso has Azure VMs, AWS workloads, on-premises servers, storage,
databases, and containers.

## What cloud configurations should we improve?

``` text
Capability:
______________________________
```

## What issues should we fix?

``` text
Feature:
______________________________
```

## How can we summarize our posture?

``` text
Feature:
______________________________
```

## How can we protect workloads from threats?

``` text
Capability:
______________________________
```

------------------------------------------------------------------------

# 🗺️ Part 20 --- Build Your Defender for Cloud Map

  Capability                 Main Purpose
  -------------------------- ------------------------------------------------------
  Defender for Cloud         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  CSPM                       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Security Recommendations   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Cloud Secure Score         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Security Standards         \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  CWPP                       \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Defender Plans             \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Security Alerts            \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
  Asset Inventory            \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

------------------------------------------------------------------------

# ✅ Suggested Answers

## Recommendation Scenario

``` text
A — Security Posture Finding
```

The exposed port is a security weakness. The finding alone does not
prove compromise.

## Security Standard

``` text
Expected security controls
or configurations
```

Recommendation:

``` text
Guidance for improving
an identified issue
```

## Compliance

``` text
NO
```

Technical assessment is only part of organizational compliance.

## CSPM vs CWPP

``` text
1. CSPM
2. CWPP
3. CSPM
4. CWPP
```

## Recommendation vs Alert

``` text
Recommendation
=
Guidance for improving security posture

Alert
=
Potential threat activity
that should be investigated
```

## Priority

``` text
B
```

Context, exposure, criticality, and potential impact make it the
strongest priority.

## Lesson 09 Mapping

``` text
1. NSG
2. Azure Bastion
3. Azure Key Vault
4. Defender for Cloud
```

## Defender for Cloud Flow

``` text
Cloud Resources
      ↓
Continuous Assessment
      ↓
Recommendations
      ↓
Remediation
      ↓
Improved Security Posture
```

## Posture vs Protection

``` text
CSPM
      ↓
Find weaknesses
      ↓
Generate recommendations
      ↓
Improve security posture
```

``` text
CWPP
      ↓
Protect workloads
      ↓
Detect threats
      ↓
Generate alerts
```

## Contoso Challenge

``` text
1. CSPM
2. Security Recommendations
3. Cloud Secure Score
4. CWPP / Defender Plans
```

------------------------------------------------------------------------

# 🎓 What You Should Have Learned

``` text
DEFENDER FOR CLOUD
=
Cloud security management
```

``` text
CSPM = Posture
RECOMMENDATIONS = Improve
CLOUD SECURE SCORE = Measure / track posture
CWPP = Protect workloads
ALERTS = Investigate threats
```

------------------------------------------------------------------------

# ✅ Lab Completion Checklist

-   [ ] I can locate Defender for Cloud.
-   [ ] I can explain CSPM.
-   [ ] I can locate security recommendations.
-   [ ] I understand Cloud Secure Score.
-   [ ] I understand security standards.
-   [ ] I can explain CWPP.
-   [ ] I understand Defender plans at a high level.
-   [ ] I can distinguish a recommendation from an alert.
-   [ ] I understand asset inventory.
-   [ ] I understand Defender for Cloud's multicloud purpose.
-   [ ] I understand why risk prioritization matters.

------------------------------------------------------------------------

# ➡️ Next

## 📘 Lesson 11 --- Microsoft Defender XDR

Next you will explore how Microsoft combines signals across identities,
endpoints, email, applications, and other security domains to help
security teams detect and respond to attacks.

------------------------------------------------------------------------

# 🔗 Official Microsoft Resources

-   [Microsoft Defender for Cloud
    Overview](https://learn.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction)
-   [Security
    Recommendations](https://learn.microsoft.com/en-us/azure/defender-for-cloud/security-recommendations)
-   [Cloud Secure
    Score](https://learn.microsoft.com/en-us/azure/defender-for-cloud/secure-score-access-and-track)
-   [Cloud Security Posture
    Management](https://learn.microsoft.com/en-us/azure/defender-for-cloud/concept-cloud-security-posture-management)

------------------------------------------------------------------------

# 📚 Course Navigation

⬅️ **[Lesson 10 --- Microsoft Defender for
Cloud](../lessons/%F0%9F%93%98%20Lesson%2010%20%E2%80%94%20Microsoft%20Defender%20for%20Cloud.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

🏗️ **[Projects](../projects/README.md)**

🏠 **[Return to Main README](../README.md)**
