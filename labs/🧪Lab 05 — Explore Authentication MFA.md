# 🔵 Lab 05 — Explore Authentication & MFA

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 05 — Authentication & Multifactor Authentication  
**Lab Type:** 🔵 Explore the Tool  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Locate authentication settings in Microsoft Entra
- Identify available authentication methods
- Locate the authentication methods policy
- Recognize Microsoft Authenticator settings
- Recognize passkey/FIDO2 settings
- Locate Security Defaults
- Locate password protection settings
- Locate Conditional Access
- Understand where sign-in and authentication information can be reviewed
- Connect authentication features to Zero Trust

---

# 🧪 Lab Philosophy

This is a:

# 🔵 Explore the Tool Lab

The goal is:

```text
FIND THE FEATURE
      ↓
UNDERSTAND ITS PURPOSE
      ↓
CONNECT IT TO SC-900
```

You do not need to change anything.

---

# ⚠️ Production Safety

Authentication settings can affect every user in an organization.

Changing:

```text
MFA

Authentication Methods

Security Defaults

Conditional Access

Password Protection
```

can have major consequences.

For this lab:

> **Observe only unless you are specifically authorized to make changes in a test environment.**

---

# 📋 What You Need

Ideally:

- A Microsoft work or school account
- Access to the Microsoft Entra admin center
- Permission to view some identity settings

Some pages may require administrative roles or additional licensing.

If a feature is unavailable:

```text
READ THE DESCRIPTION
      ↓
UNDERSTAND THE PURPOSE
      ↓
CONTINUE
```

You can still complete the learning objective.

---

# 🚀 Part 1 — Open Microsoft Entra

Open:

```text
https://entra.microsoft.com
```

Sign in with an authorized account.

Locate:

```text
Entra ID
```

---

# 🔐 Part 2 — Find Authentication Methods

Look for:

```text
Authentication methods
```

The exact navigation can change as Microsoft updates the portal.

Once there, look for available authentication methods.

You may see methods such as:

```text
Passkey (FIDO2)

Microsoft Authenticator

SMS

Voice Call

Temporary Access Pass

Certificate-Based Authentication
```

Your tenant may not have every method enabled.

---

# 🗺️ Record What You See

Do not record confidential tenant information.

Simply mark which technologies you can locate:

```text
[ ] Microsoft Authenticator

[ ] Passkey / FIDO2

[ ] SMS

[ ] Voice

[ ] Temporary Access Pass

[ ] Certificate-Based Authentication

[ ] Other
```

---

# 🧠 Part 3 — Classify Authentication Factors

For each example, identify the factor.

Choices:

```text
Something You Know

Something You Have

Something You Are
```

## Password

```text
______________________________
```

## Hardware Security Key

```text
______________________________
```

## Fingerprint

```text
______________________________
```

## PIN

```text
______________________________
```

## Phone

```text
______________________________
```

---

# 📱 Part 4 — Explore Microsoft Authenticator

Select or inspect the Microsoft Authenticator method policy if your permissions allow read-only viewing.

Do not change it.

Look for information related to:

```text
Who can use the method

Authentication mode

Configuration options
```

You may also encounter features associated with:

```text
Push Notifications

Number Matching

Passwordless Authentication
```

---

# 🧠 Scenario

A user receives an Authenticator prompt but is not currently signing in.

What should the user do?

```text
A. Approve it

B. Deny it
```

Answer:

```text
______________________________
```

Why?

```text
____________________________________

____________________________________
```

---

# 🔐 Part 5 — Explore Passkey / FIDO2

Locate the passkey or FIDO2 authentication method area.

Do not change the policy.

At a high level, remember:

```text
PASSKEY / FIDO2
      ↓
Strong Authentication
      ↓
Phishing Resistance
      ↓
Reduced Password Dependence
```

You will study this in more detail in Lesson 06.

---

# 🎟️ Part 6 — Find Temporary Access Pass

Locate:

```text
Temporary Access Pass
```

Do not enable or configure it.

Think about this scenario:

```text
New Employee
      ↓
Needs to register
a strong authentication method
```

How could a Temporary Access Pass help?

```text
____________________________________

____________________________________
```

---

# 💪 Part 7 — Find Authentication Strength

Look for an area related to:

```text
Authentication strengths
```

Depending on the portal layout, this may be associated with authentication or Conditional Access capabilities.

You may encounter concepts such as:

```text
Multifactor Authentication Strength

Passwordless MFA Strength

Phishing-Resistant MFA Strength
```

Do not create or modify a custom authentication strength.

---

# 🧠 Think About It

Which resource should generally require stronger authentication?

```text
A. Public company website

B. Global Administrator access
```

Answer:

```text
______________________________
```

Why?

```text
____________________________________

____________________________________
```

---

# 🛡️ Part 8 — Find Security Defaults

Locate the tenant's Security Defaults area.

Do **not** enable or disable Security Defaults.

Changing this setting can affect authentication across the organization.

At a high level:

```text
SECURITY DEFAULTS
=
Baseline Identity Protection
```

Record whether you were able to locate the setting:

```text
[ ] Located

[ ] Not visible with my permissions
```

Do not publish whether your real organization has Security Defaults enabled or disabled.

---

# 🔑 Part 9 — Explore Password Protection

Look for password protection settings.

Depending on your permissions and portal layout, you may see concepts related to:

```text
Banned Passwords

Custom Banned Passwords

Lockout
```

Do not change them.

---

# 🧠 Password Challenge

Which password is more predictable?

```text
A. CompanyName2026!

B. A strong unique password not based on company information
```

Answer:

```text
______________________________
```

Why might a company name be a poor password component?

```text
____________________________________

____________________________________
```

---

# 🚦 Part 10 — Find Conditional Access

Locate:

```text
Conditional Access
```

Do not create, enable, disable, or edit a production policy.

For now, observe the relationship:

```text
ACCESS REQUEST
      ↓
CONDITIONAL ACCESS
      ↓
REQUIRE MFA
or
REQUIRE AUTHENTICATION STRENGTH
      ↓
ACCESS DECISION
```

Conditional Access will receive its own lesson and lab later.

---

# 🔎 Part 11 — Explore Sign-In Information

If your permissions allow it, locate sign-in information or sign-in logs.

Do not record or publish real user details.

Look for the types of information administrators may be able to review.

Examples can include:

```text
User

Application

Time

Location

Device Information

Authentication Requirement

Status
```

The exact information available depends on permissions, licensing, and the current portal experience.

---

# 🛡️ Why Are Sign-In Logs Useful?

Consider:

```text
Employee Normally Signs In
from Missouri
        ↓
Sudden Suspicious Sign-In
from Another Region
        ↓
Security Team Investigates
```

Logs and risk signals can help administrators understand authentication activity.

---

# 🧠 Part 12 — MFA or Not MFA?

Decide whether each example represents true MFA.

## Scenario 1

```text
Password
+
Authenticator Approval
```

MFA?

```text
YES / NO
```

---

## Scenario 2

```text
Password
+
PIN
```

MFA?

```text
YES / NO
```

For this simplified fundamentals exercise, both are treated as knowledge factors.

---

## Scenario 3

```text
Password
+
Hardware Security Key
```

MFA?

```text
YES / NO
```

---

## Scenario 4

```text
Password #1
+
Password #2
```

MFA?

```text
YES / NO
```

---

# 🎣 Part 13 — Phishing Scenario

Contoso receives a phishing email.

The attacker tricks an employee into entering a username and password into a fake website.

Without MFA:

```text
PASSWORD STOLEN
      ↓
ATTACKER SIGNS IN
```

With stronger authentication:

```text
PASSWORD STOLEN
      ↓
ADDITIONAL AUTHENTICATION REQUIRED
      ↓
ATTACK MAY BE BLOCKED
```

Answer:

### Which control adds another authentication barrier?

```text
______________________________
```

### Which types of authentication are specifically designed to provide stronger phishing resistance?

```text
____________________________________

____________________________________
```

---

# 🧱 Part 14 — Build an Authentication Strategy

Contoso has three types of users:

```text
Normal Employees

IT Administrators

External Contractors
```

Design a simple authentication approach.

| User Type | Authentication Requirement |
|---|---|
| Normal Employees | __________________________ |
| IT Administrators | __________________________ |
| External Contractors | __________________________ |

There is not one perfect answer.

Think about:

```text
Risk

MFA

Authentication Strength

Least Privilege

Conditional Access
```

---

# 🔐 Part 15 — Zero Trust Connection

Which Zero Trust principle most directly connects to authentication?

```text
Verify Explicitly

Use Least Privilege

Assume Breach
```

Answer:

```text
______________________________
```

Now explain why:

```text
____________________________________

____________________________________
```

---

# 🗺️ Part 16 — Build Your Authentication Map

Complete the table:

| Feature | Purpose |
|---|---|
| Password | __________________________ |
| MFA | __________________________ |
| Microsoft Authenticator | __________________________ |
| Passkey / FIDO2 | __________________________ |
| Temporary Access Pass | __________________________ |
| Authentication Strength | __________________________ |
| Security Defaults | __________________________ |
| Password Protection | __________________________ |
| Conditional Access | __________________________ |

---

# ✅ Suggested Answers

## Authentication Factors

```text
Password
=
Something You Know

Hardware Security Key
=
Something You Have

Fingerprint
=
Something You Are

PIN
=
Something You Know

Phone
=
Something You Have
```

---

## Authenticator Scenario

```text
B — Deny it
```

Users should not approve authentication requests they did not initiate.

---

## Authentication Strength Scenario

```text
B — Global Administrator access
```

Highly privileged access presents greater risk and should generally receive stronger protection.

---

## Password Challenge

```text
A — CompanyName2026!
```

Company names and predictable patterns may be easier for attackers to guess.

---

## MFA Scenarios

```text
Scenario 1
Password + Authenticator
=
YES


Scenario 2
Password + PIN
=
NO
for this simplified factor-category example


Scenario 3
Password + Security Key
=
YES


Scenario 4
Two Passwords
=
NO
```

---

## Phishing Scenario

Additional barrier:

```text
MFA
```

Examples of phishing-resistant approaches include:

```text
Passkeys / FIDO2

Windows Hello for Business

Certificate-Based Authentication
```

depending on configuration.

---

## Zero Trust

```text
Verify Explicitly
```

Strong authentication helps verify that the identity requesting access is legitimate.

---

# 🎓 What You Should Have Learned

You should now understand:

```text
AUTHENTICATION
=
Who are you?
```

```text
MFA
=
Multiple authentication factors
```

```text
AUTHENTICATION METHODS
=
Ways users prove identity
```

```text
AUTHENTICATION STRENGTH
=
Require methods appropriate to risk
```

and:

```text
PASSWORD ALONE
=
Not the ideal end state for strong identity security
```

---

# ✅ Lab Completion Checklist

Before marking the lab complete, make sure you can answer:

- [ ] What is authentication?
- [ ] How is authentication different from authorization?
- [ ] What are the three classic authentication factor categories?
- [ ] What makes MFA truly multifactor?
- [ ] What does Microsoft Authenticator do?
- [ ] What is a Temporary Access Pass?
- [ ] What is authentication strength?
- [ ] What are Security Defaults?
- [ ] What does password protection help prevent?
- [ ] Why can legacy authentication be risky?
- [ ] How can Conditional Access interact with MFA?
- [ ] Which Zero Trust principle is closely connected to authentication?

If you can answer these, Lab 05 is complete.

---

# ➡️ Next

Continue to:

## 📘 Lesson 06 — Passwordless Authentication

You will take a closer look at:

- Passkeys
- FIDO2
- Windows Hello for Business
- Microsoft Authenticator
- Temporary Access Pass
- Phishing-resistant authentication

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Authentication Methods](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods)
- [Microsoft Entra MFA](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-mfa-howitworks)
- [Authentication Strengths](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-strengths)
- [Security Defaults](https://learn.microsoft.com/en-us/entra/fundamentals/security-defaults)

---

# 📚 Course Navigation

⬅️ **[Lesson 05 — Authentication & Multifactor Authentication](../lessons/%F0%9F%93%98%20Lesson%2005%20%E2%80%94%20Authentication%20&%20Multifactor%20Authentication.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
