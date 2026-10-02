# 🔵 Lab 06 — Explore Passwordless Authentication

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Related Lesson:** Lesson 06 — Passwordless Authentication  
**Lab Type:** 🔵 Explore the Tool  
**Difficulty:** Beginner  
**Configuration Changes:** None required

---

# 🎯 Lab Objectives

By completing this lab, you should be able to:

- Locate passwordless authentication methods in Microsoft Entra
- Locate passkey/FIDO2 settings
- Locate Microsoft Authenticator settings
- Locate Windows Hello for Business settings
- Locate Temporary Access Pass
- Recognize authentication strength policies
- Compare major passwordless methods
- Explain why passwordless authentication can reduce phishing risk
- Connect passwordless authentication to Zero Trust

---

# 🧪 Lab Philosophy

This is a:

# 🔵 Explore the Tool Lab

You will not enroll yourself in a new authentication method or modify organization-wide authentication settings.

The goal is:

```text
FIND
  ↓
OBSERVE
  ↓
UNDERSTAND
  ↓
COMPARE
```

---

# ⚠️ Production Safety

Authentication configuration can affect whether users and administrators can sign in.

For this lab:

```text
DO NOT:

Enable methods

Disable methods

Change target groups

Change authentication strengths

Delete registered methods

Change Conditional Access
```

unless you are specifically authorized to do so in a test environment.

---

# 📋 What You Need

Ideally:

- A Microsoft work or school account
- Access to Microsoft Entra admin center
- Permission to view authentication settings

Some features may require:

```text
Specific Administrative Roles

Licensing

Tenant Configuration
```

If you cannot view a setting, continue with the conceptual portion of the lab.

---

# 🚀 Part 1 — Open Microsoft Entra

Open:

```text
https://entra.microsoft.com
```

Sign in using an authorized account.

Locate:

```text
Entra ID
```

---

# 🔐 Part 2 — Open Authentication Methods

Find:

```text
Authentication methods
```

Then locate the authentication method policies.

Depending on the current portal design, the navigation may vary.

Look for methods such as:

```text
Passkey / FIDO2

Microsoft Authenticator

Temporary Access Pass

Certificate-Based Authentication

SMS

Voice
```

---

# 🗺️ Authentication Method Inventory

Mark what you can locate.

```text
[ ] Passkey / FIDO2

[ ] Microsoft Authenticator

[ ] Temporary Access Pass

[ ] Certificate-Based Authentication

[ ] SMS

[ ] Voice

[ ] Other
```

Do not record whether your organization's real security configuration is good or bad in a public repository.

---

# 🔑 Part 3 — Explore Passkey / FIDO2

Open the passkey or FIDO2 method policy in read-only fashion.

Do not change:

```text
Enable / Disable

Target Groups

Configuration Options
```

Look for the types of settings available.

---

# 🧠 Passkey Review

Complete:

```text
Passkeys use:
______________________________
```

```text
Passkeys reduce dependence on:
______________________________
```

```text
Passkeys are designed to provide strong resistance to:
______________________________
```

---

# 🔌 Part 4 — Hardware Security Key Scenario

Contoso gives IT administrators FIDO2 security keys.

The administrator:

```text
Attempts Sign-In
      ↓
Uses Security Key
      ↓
Performs User Verification
      ↓
Cryptographic Authentication
```

Why might Contoso choose this for administrators?

```text
____________________________________

____________________________________
```

---

# 📱 Part 5 — Explore Microsoft Authenticator

Return to the authentication methods list.

Open:

```text
Microsoft Authenticator
```

in read-only mode.

Look for configuration areas related to who can use the method and what capabilities are available.

Do not change the policy.

---

# 🧠 Authenticator Review

Microsoft Authenticator can participate in:

```text
MFA

Passwordless Authentication
```

These are related but not identical concepts.

Complete:

```text
MFA
=
____________________________________
```

```text
Passwordless
=
____________________________________
```

---

# 💻 Part 6 — Find Windows Hello for Business

Look for references to:

```text
Windows Hello for Business
```

Depending on your environment, some Windows Hello configuration may be managed through other Microsoft administration tools rather than entirely from the Entra authentication methods page.

For this lab, focus on the concept.

---

# 🧠 Windows Hello Scenario

Jordan uses a company Windows laptop.

Jordan signs in using:

```text
Fingerprint
or
PIN
```

The PIN is associated with the device and protected cryptographic credentials.

Is this the same as sending a traditional password to a website?

```text
YES / NO
```

Answer:

```text
______________________________
```

---

# 🎟️ Part 7 — Explore Temporary Access Pass

Return to:

```text
Authentication methods
```

Locate:

```text
Temporary Access Pass
```

Do not enable it or create a TAP.

Observe the types of controls that exist.

---

# 🆕 Onboarding Scenario

A new employee needs to register a passkey.

Arrange the process:

```text
A. User registers strong authentication

B. Administrator provides approved Temporary Access Pass

C. New identity is created

D. User signs in using the temporary credential
```

Write the correct order:

```text
____ → ____ → ____ → ____
```

---

# 🆘 Recovery Scenario

A user loses the device containing their authentication credential.

Why could a Temporary Access Pass be useful?

```text
____________________________________

____________________________________
```

Why must the recovery process still verify the user's identity?

```text
____________________________________

____________________________________
```

---

# 💪 Part 8 — Explore Authentication Strengths

Locate:

```text
Authentication strengths
```

You may see built-in strength categories or related policies.

Examples can include concepts such as:

```text
Multifactor Authentication

Passwordless MFA

Phishing-Resistant MFA
```

Do not create or edit a policy.

---

# 🎯 Match the Risk

Choose the most reasonable requirement.

## Public Information Portal

```text
Normal Authentication
or
Highest Privileged Authentication Requirement?
```

Answer:

```text
______________________________
```

## Global Administrator Access

```text
Normal Authentication
or
Phishing-Resistant Authentication?
```

Answer:

```text
______________________________
```

---

# 🎣 Part 9 — Phishing Comparison

Consider two users.

## User A

Uses:

```text
Username
+
Password
```

## User B

Uses:

```text
Passkey / FIDO2
```

An attacker creates a fake Microsoft sign-in page.

Which user's authentication approach is designed to provide stronger phishing resistance?

```text
User A / User B
```

Answer:

```text
______________________________
```

---

# 🧠 Why?

Write a short explanation:

```text
____________________________________

____________________________________
```

Think about:

```text
Reusable Password
vs
Cryptographic Authentication
```

---

# 🛡️ Part 10 — Zero Trust Connection

Recall the Zero Trust principles:

```text
VERIFY EXPLICITLY

USE LEAST PRIVILEGE

ASSUME BREACH
```

Which principle most directly relates to strong authentication?

```text
______________________________
```

Explain:

```text
____________________________________

____________________________________
```

---

# 🚦 Part 11 — Conditional Access Preview

Locate:

```text
Conditional Access
```

Do not change anything.

Imagine a policy:

```text
IF
User is accessing
a sensitive admin resource

THEN
Require
phishing-resistant authentication
```

This combines:

```text
Conditional Access
        +
Authentication Strength
```

You will study this in Lesson 07.

---

# 🏗️ Part 12 — Design a Passwordless Rollout

Contoso wants to reduce password use.

It has:

```text
150 Employees

10 IT Administrators

20 Remote Employees

New Employees Every Month
```

Design a basic rollout order.

Example choices:

```text
Pilot IT Users

Pilot Small User Group

Expand to Employees

Use TAP for New-User Registration

Require Stronger Methods for Administrators
```

Your plan:

```text
1. ____________________________________

2. ____________________________________

3. ____________________________________

4. ____________________________________

5. ____________________________________
```

---

# 🧠 Why Pilot?

Authentication is critical.

A poorly planned change could result in:

```text
Users Cannot Sign In

Administrators Locked Out

Unsupported Devices

Application Problems

Help Desk Surge
```

A safer strategy is:

```text
PLAN
 ↓
PILOT
 ↓
TEST
 ↓
MONITOR
 ↓
EXPAND
```

---

# 🗺️ Part 13 — Build Your Passwordless Map

Complete:

| Technology | Primary Purpose |
|---|---|
| Passkey / FIDO2 | __________________________ |
| Windows Hello for Business | __________________________ |
| Microsoft Authenticator | __________________________ |
| Temporary Access Pass | __________________________ |
| Authentication Strength | __________________________ |

---

# 🧩 Part 14 — Choose the Technology

Choose from:

```text
Passkey / FIDO2

Windows Hello for Business

Microsoft Authenticator

Temporary Access Pass
```

## Scenario 1

A new employee needs a temporary method to register stronger authentication.

```text
______________________________
```

## Scenario 2

An administrator needs a hardware-based phishing-resistant sign-in method.

```text
______________________________
```

## Scenario 3

A Windows employee wants device-bound biometric or PIN authentication.

```text
______________________________
```

## Scenario 4

A user wants to use a supported mobile application for passwordless sign-in.

```text
______________________________
```

---

# ✅ Suggested Answers

## Passkey Review

```text
Passkeys use:
Public-key cryptography

Passkeys reduce dependence on:
Passwords / reusable secrets

Passkeys are designed to resist:
Phishing
```

---

## Security Key Scenario

FIDO2 security keys can provide strong phishing-resistant authentication, which is valuable for highly privileged accounts.

---

## MFA vs Passwordless

```text
MFA
=
Uses multiple authentication factors
```

```text
Passwordless
=
Authenticates without entering
a traditional password
```

---

## Windows Hello

```text
NO
```

Windows Hello uses device-bound cryptographic credentials rather than simply transmitting a reusable traditional password.

---

## TAP Onboarding Order

```text
C → B → D → A
```

```text
Create Identity
      ↓
Provide TAP
      ↓
User Signs In
      ↓
Register Strong Authentication
```

---

## Authentication Strength

For highly privileged administrative access:

```text
Phishing-Resistant Authentication
```

is the stronger choice.

---

## Phishing Comparison

```text
User B
```

Passkeys/FIDO2 use cryptographic authentication designed to resist credential-phishing attacks.

---

## Zero Trust

```text
Verify Explicitly
```

Strong authentication helps establish confidence in the identity requesting access.

---

## Choose the Technology

```text
Scenario 1
=
Temporary Access Pass

Scenario 2
=
Passkey / FIDO2 Security Key

Scenario 3
=
Windows Hello for Business

Scenario 4
=
Microsoft Authenticator
```

---

# 🎓 What You Should Have Learned

You should now understand:

```text
PASSWORDLESS
=
No traditional password required
during normal authentication
```

```text
PASSKEY / FIDO2
=
Phishing-resistant
cryptographic authentication
```

```text
WINDOWS HELLO
=
Device-bound authentication
```

```text
TEMPORARY ACCESS PASS
=
Bootstrap / recovery
```

and:

```text
STRONGER AUTHENTICATION
      ↓
HELPS VERIFY IDENTITY
      ↓
SUPPORTS ZERO TRUST
```

---

# ✅ Lab Completion Checklist

Before marking this lab complete, make sure you can answer:

- [ ] What is passwordless authentication?
- [ ] Why can passwords be risky?
- [ ] What is a passkey?
- [ ] What is FIDO2?
- [ ] What is Windows Hello for Business?
- [ ] Why is a Windows Hello PIN different from a traditional password?
- [ ] What can Microsoft Authenticator do?
- [ ] What is Temporary Access Pass?
- [ ] What does phishing-resistant authentication mean?
- [ ] What is authentication strength?
- [ ] Why should authentication changes be piloted?
- [ ] How does passwordless authentication support Zero Trust?

If you can answer these, Lab 06 is complete.

---

# ➡️ Next

Continue to:

## 📘 Lesson 07 — Conditional Access & RBAC

Next you will learn how identity, device, location, application, and risk signals can be evaluated to make access decisions.

---

# 🔗 Official Microsoft Resources

- [Microsoft Entra Admin Center](https://entra.microsoft.com/)
- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Passwordless Authentication Options](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-passwordless)
- [Passkeys in Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-enable-passkey-fido2)
- [Windows Hello for Business](https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/)
- [Temporary Access Pass](https://learn.microsoft.com/en-us/entra/identity/authentication/howto-authentication-temporary-access-pass)

---

# 📚 Course Navigation

⬅️ **[Lesson 06 — Passwordless Authentication](../lessons/%F0%9F%93%98%20Lesson%2006%20%E2%80%94%20Passwordless%20Authentication.md)**

📘 **[Lessons](../lessons/README.md)**

🧪 **[Labs](README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
