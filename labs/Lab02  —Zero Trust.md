# 🟡 Lab 02 — Apply Zero Trust

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 02 — Shared Responsibility, Defense in Depth & Zero Trust  
**Lab Type:** 🟡 Scenario  
**Difficulty:** Beginner  
**Configuration Changes:** None

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Apply the three Zero Trust principles to a realistic scenario
- Identify examples of least privilege
- Identify where explicit verification should occur
- Explain how defense in depth reduces risk
- Recognize customer responsibilities in a cloud environment
- Identify where encryption and hashing may help
- Think about security as multiple controls working together

---

# 🏢 Scenario — Contoso Manufacturing

You are helping review security for a fictional company called:

# Contoso Manufacturing

Contoso has:

```text
150 Employees

Microsoft 365

Microsoft Entra ID

Company Laptops

Remote Employees

Office Wi-Fi

Microsoft Teams

SharePoint Online

OneDrive

Several Administrators
```

Employees work from:

```text
Main Office

Home

Hotels

Customer Locations

Mobile Devices
```

Management wants employees to work from anywhere while keeping company information secure.

---

# 🚨 Current Environment

During your review, you discover the following.

### Issue 1 — Password-Only Sign-In

Employees currently sign in using only:

```text
Username
+
Password
```

No additional authentication is required.

---

### Issue 2 — Administrators Have Too Much Access

Several IT employees have permanent high-level administrative access even though they only occasionally need it.

---

### Issue 3 — Office Location Is Automatically Trusted

Contoso assumes that anyone connected from inside the office network is trustworthy.

Some security checks are reduced for office users.

---

### Issue 4 — Personal Devices

Employees sometimes access Microsoft 365 from personal devices.

Contoso does not currently evaluate the device before allowing access to sensitive information.

---

### Issue 5 — Sensitive Documents

HR stores employee information in SharePoint Online.

The files contain:

```text
Names

Addresses

Payroll Information

Benefits Information

Personal Information
```

---

### Issue 6 — Limited Monitoring

Contoso has limited security monitoring and assumes that blocking attackers at the perimeter is enough.

---

# 🧠 Part 1 — Identify the Zero Trust Principles

Microsoft's three guiding Zero Trust principles are:

```text
Verify Explicitly

Use Least Privilege Access

Assume Breach
```

Match each issue with the principle that MOST directly applies.

---

## Question 1

Employees authenticate using only passwords.

Which Zero Trust principle suggests evaluating stronger authentication and additional signals?

```text
Answer:
____________________________________
```

Why?

```text
____________________________________

____________________________________
```

---

## Question 2

IT administrators have permanent privileges they rarely need.

Which Zero Trust principle applies most directly?

```text
Answer:
____________________________________
```

What could Contoso change?

```text
____________________________________

____________________________________
```

---

## Question 3

Contoso automatically trusts users because they are inside the office.

Which Zero Trust principle is being violated?

```text
Answer:
____________________________________
```

Why is location alone insufficient?

```text
____________________________________

____________________________________
```

---

## Question 4

Contoso assumes its perimeter will prevent every attacker from entering the environment.

Which Zero Trust principle should change this thinking?

```text
Answer:
____________________________________
```

What should Contoso plan for?

```text
____________________________________

____________________________________
```

---

# 🛡️ Part 2 — Build Defense in Depth

Contoso wants to protect its HR information.

Instead of relying on one control, create multiple layers.

Fill in an example control for each area.

| Layer | Example Control |
|---|---|
| Identity | ______________________________ |
| Device | ______________________________ |
| Network | ______________________________ |
| Application | ______________________________ |
| Data | ______________________________ |
| Monitoring | ______________________________ |

---

# 🧠 Think About It

Suppose an attacker steals an employee password.

If Contoso uses:

```text
MFA
+
Conditional Access
+
Device Controls
+
Least Privilege
+
Data Protection
+
Monitoring
```

does the stolen password automatically give the attacker access to everything?

```text
YES / NO
```

Why?

```text
____________________________________

____________________________________
```

This is the basic purpose of:

> **Defense in depth.**

---

# 🤝 Part 3 — Shared Responsibility

Contoso uses Microsoft 365.

Determine whether the following is primarily a **Microsoft**, **Contoso**, or **Shared** responsibility at a high level.

> Exact responsibilities can vary by service and configuration. Focus on the general shared-responsibility concept.

---

## Physical Datacenter Security

```text
Microsoft / Contoso / Shared

Answer:
______________________________
```

---

## Employee Account Management

```text
Microsoft / Contoso / Shared

Answer:
______________________________
```

---

## Deciding Which Employees Can Access HR Files

```text
Microsoft / Contoso / Shared

Answer:
______________________________
```

---

## Maintaining the Underlying Microsoft 365 Cloud Infrastructure

```text
Microsoft / Contoso / Shared

Answer:
______________________________
```

---

## Protecting Organizational Data

```text
Microsoft / Contoso / Shared

Answer:
______________________________
```

---

# 🔐 Part 4 — Encryption or Hashing?

Choose the concept that best fits each scenario.

---

## Scenario A

Contoso wants sensitive stored information to be unreadable without the appropriate cryptographic key.

```text
Encryption / Hashing

Answer:
______________________________
```

---

## Scenario B

Contoso wants to determine whether a downloaded file has changed.

```text
Encryption / Hashing

Answer:
______________________________
```

---

## Scenario C

Contoso wants to protect information while it travels between a browser and a web service.

```text
Encryption / Hashing

Answer:
______________________________
```

---

# 🌍 Part 5 — GRC

Consider these requirements.

---

## Scenario A

Contoso creates a company rule requiring MFA for administrative accounts.

Is this primarily an example of:

```text
Governance
Risk
Compliance
```

Answer:

```text
______________________________
```

---

## Scenario B

Contoso identifies phishing as a threat that could lead to employee account compromise.

Is this primarily an example of:

```text
Governance
Risk
Compliance
```

Answer:

```text
______________________________
```

---

## Scenario C

Contoso must follow a legal requirement governing how certain customer information is handled.

Is this primarily an example of:

```text
Governance
Risk
Compliance
```

Answer:

```text
______________________________
```

---

# 🏗️ Part 6 — Design a Better Access Decision

Originally, Contoso used:

```text
Inside Office?
      ↓
YES
      ↓
TRUST
```

Replace that with a Zero Trust-style decision.

Complete the flow:

```text
User requests access
        ↓
________________________
        ↓
________________________
        ↓
________________________
        ↓
________________________
        ↓
ALLOW / BLOCK / REQUIRE MORE VERIFICATION
```

Possible signals to consider:

```text
Identity

Authentication

Device

Location

Risk

Application

Requested Resource
```

There is not one required order.

The important idea is:

> **Access is evaluated using relevant signals and policy rather than automatically trusted because of network location.**

---

# 🎯 Part 7 — Final Security Recommendation

Management asks:

> "What are the three most important Zero Trust changes you would make first?"

Write three recommendations.

### Recommendation 1

```text
____________________________________

____________________________________
```

### Recommendation 2

```text
____________________________________

____________________________________
```

### Recommendation 3

```text
____________________________________

____________________________________
```

For each recommendation, try to connect it to:

```text
Verify Explicitly

Least Privilege

Assume Breach
```

---

# ✅ Suggested Answers

Try the lab yourself before reviewing this section.

---

## Part 1

### Question 1

**Verify explicitly**

Contoso should evaluate more than a username and password. Authentication strength, MFA, device information, risk, and other signals can contribute to an access decision.

### Question 2

**Use least privilege access**

Administrators should receive only the permissions necessary for their work, ideally only when those privileges are needed.

### Question 3

**Verify explicitly**

Being physically inside an office does not prove that the user, account, or device is safe.

### Question 4

**Assume breach**

Contoso should plan for the possibility that an attacker gets past one security control and use monitoring, segmentation, least privilege, and other controls to limit damage.

---

# 🛡️ Part 2 — Example

Possible answers include:

| Layer | Example |
|---|---|
| Identity | MFA |
| Device | Require an approved/compliant device |
| Network | Segmentation/firewall controls |
| Application | Application access controls |
| Data | Encryption/sensitivity controls |
| Monitoring | Security logging and threat detection |

Many answers can be valid.

The key is to use **multiple independent layers**.

---

# 🤝 Part 3

### Physical Datacenter Security

```text
Microsoft
```

For Microsoft 365, Microsoft operates and secures the underlying cloud datacenter infrastructure.

### Employee Account Management

```text
Contoso
```

The organization is responsible for managing its users and appropriate access.

### HR File Permissions

```text
Contoso
```

Contoso decides which identities should have access to its organizational data.

### Underlying Microsoft 365 Infrastructure

```text
Microsoft
```

### Protecting Organizational Data

```text
Shared
```

Microsoft provides security capabilities and protects the cloud service infrastructure, while Contoso must appropriately classify, configure, govern, and control access to its data.

---

# 🔐 Part 4

### Scenario A

```text
Encryption
```

### Scenario B

```text
Hashing
```

### Scenario C

```text
Encryption
```

---

# 🏛️ Part 5

### Scenario A

```text
Governance
```

### Scenario B

```text
Risk
```

### Scenario C

```text
Compliance
```

---

# 🏗️ Part 6 — Example

One possible design:

```text
User requests access
        ↓
Verify Identity
        ↓
Evaluate Authentication
        ↓
Evaluate Device & Risk
        ↓
Evaluate Requested Resource
        ↓
Apply Access Policy
        ↓
ALLOW / BLOCK / REQUIRE MORE VERIFICATION
```

---

# 🎓 What You Should Have Learned

After this lab, you should be able to explain:

```text
ZERO TRUST
=
Never automatically trust
based only on location
```

and remember:

```text
Verify Explicitly

Use Least Privilege Access

Assume Breach
```

You should also understand:

```text
Defense in Depth
=
Multiple security layers
```

and:

```text
Cloud Security
=
Shared Responsibility
```

---

# 🧪 Lab Type

This was a:

## 🟡 Scenario Lab

No Microsoft tenant, Azure subscription, or configuration changes were required.

The goal was to learn how to **think about security decisions** before we begin exploring Microsoft security tools.

---

# ➡️ Next

Continue to:

## 📘 Lesson 03 — Microsoft Entra ID & Identity Types

Lesson 03 introduces Microsoft's cloud identity platform.

Its lab will be:

> 🔵 **Explore the Tool — Microsoft Entra admin center**

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Describe security and compliance concepts](https://learn.microsoft.com/en-us/training/modules/describe-security-concepts-methodologies/)

---

# 📚 Course Navigation

⬅️ **[Lesson 02](../lessons/%F0%9F%93%98%20Lesson%2002%20%E2%80%94%20Shared%20Responsibility,%20Defense%20in%20Depth%20&%20Zero%20Trust.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
