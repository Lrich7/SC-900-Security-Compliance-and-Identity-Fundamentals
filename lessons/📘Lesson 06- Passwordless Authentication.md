# 📘 Lesson 06 — Passwordless Authentication

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 06  
**Lab:** 🔵 Explore the Tool — Passwordless Authentication  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain passwordless authentication
- Describe why organizations are reducing dependence on passwords
- Describe passkeys and FIDO2 security keys
- Describe Windows Hello for Business
- Describe passwordless sign-in with Microsoft Authenticator
- Explain the purpose of Temporary Access Pass
- Explain phishing-resistant authentication
- Distinguish common passwordless methods
- Explain how passwordless authentication supports Zero Trust
- Locate passwordless authentication settings in Microsoft Entra

---

# 🔑 The Password Problem

Passwords have been used for decades, but they create significant security and usability challenges.

Common problems include:

```text
Weak Passwords

Password Reuse

Phishing

Credential Theft

Password Spraying

Forgotten Passwords

Password Reset Costs
```

Even strong passwords can be stolen.

For example:

```text
User Creates Strong Password
        ↓
Attacker Creates Fake Login Page
        ↓
User Enters Password
        ↓
Attacker Steals Password
```

The password itself may have been strong, but the authentication method was still vulnerable to phishing.

---

# 🚫 What Is Passwordless Authentication?

Passwordless authentication allows a user to authenticate without entering a traditional password.

Instead, authentication can rely on:

```text
A Trusted Device

Cryptographic Keys

Biometrics

PIN

Security Key

Passkey
```

Conceptually:

```text
Traditional
Username + Password
        ↓
Authentication
```

becomes:

```text
Passwordless
Trusted Device / Key
        +
User Verification
        ↓
Authentication
```

---

# 🧠 Passwordless Does Not Mean Security-Free

Removing the password does **not** mean removing authentication.

The user still needs to prove identity.

Passwordless technologies can use:

```text
Device Possession

Cryptographic Keys

Biometric Verification

Local PIN
```

The difference is that the user does not need to send or type a reusable password during normal authentication.

---

# 🎣 Why Passwordless Helps Against Phishing

Traditional phishing often attempts to steal:

```text
Username

Password
```

A phishing-resistant passwordless method is designed so that simply tricking a user into typing a secret into a fake website is not enough.

Conceptually:

```text
PASSWORD
=
Reusable Secret
```

versus:

```text
PASSKEY / FIDO2
=
Cryptographic Authentication
```

This can significantly reduce credential-phishing risk.

---

# 🔐 Major Microsoft Passwordless Methods

For SC-900, become familiar with:

```text
Passkeys / FIDO2

Windows Hello for Business

Microsoft Authenticator

Temporary Access Pass
```

Temporary Access Pass is primarily a bootstrap or recovery method rather than the user's long-term passwordless credential.

---

# 🔑 Passkeys

A **passkey** is a modern authentication credential based on public-key cryptography.

Instead of sending a reusable password to a service:

```text
User
  ↓
Passkey
  ↓
Cryptographic Proof
  ↓
Authentication
```

The private key remains protected on the user's device or authenticator.

---

# 🧠 Public and Private Keys — Simplified

You do not need deep cryptography knowledge for SC-900.

At a high level:

```text
PUBLIC KEY
=
Can be known by the service
```

```text
PRIVATE KEY
=
Protected by the authenticator/device
```

The user proves possession of the private key without sending the private key itself to the service.

---

# 🛡️ FIDO2

**FIDO2** is a standards-based approach for strong authentication.

FIDO2 credentials can be used with:

```text
Security Keys

Passkeys

Supported Devices
```

A hardware security key might look conceptually like:

```text
User
  ↓
Physical Security Key
  ↓
Touch / PIN
  ↓
Cryptographic Authentication
```

FIDO2 methods are important because they can provide **phishing-resistant authentication**.

---

# 🔌 Hardware Security Keys

A FIDO2 security key is a physical authenticator.

Examples can connect using technologies such as:

```text
USB

NFC

Bluetooth
```

depending on the device and key.

A user may:

```text
Insert / Tap Security Key
        ↓
Verify with PIN or Touch
        ↓
Authenticate
```

Security keys can be especially useful for:

```text
Administrators

High-Risk Users

Users Without Company Phones

Phishing-Resistant Authentication Requirements
```

---

# 💻 Windows Hello for Business

**Windows Hello for Business** provides strong authentication for Windows users.

A user may sign in using:

```text
PIN

Fingerprint

Face
```

The important concept is:

> The Windows Hello PIN is tied to the device and is not simply a normal password transmitted to Microsoft.

Conceptually:

```text
USER
  ↓
Windows Device
  ↓
PIN / Biometrics
  ↓
Cryptographic Credential
  ↓
Authentication
```

---

# 🧠 PIN vs Password

A password may be reusable across devices and services.

A Windows Hello for Business PIN is associated with a particular device.

Think:

```text
PASSWORD
=
Reusable secret
```

```text
WINDOWS HELLO PIN
=
Unlocks protected credentials
on a specific device
```

This is an important distinction.

---

# 📱 Microsoft Authenticator Passwordless Sign-In

Microsoft Authenticator can also support passwordless authentication scenarios.

Conceptually:

```text
User Enters Account
       ↓
Authenticator Receives Request
       ↓
User Verifies
       ↓
Authentication Completes
```

The exact experience depends on configuration and supported authentication methods.

---

# 🎟️ Temporary Access Pass — TAP

A **Temporary Access Pass** is a time-limited passcode that can help a user onboard or recover authentication methods.

Example:

```text
New Employee
      ↓
Receives Temporary Access Pass
      ↓
Signs In
      ↓
Registers Passkey / Security Key /
Windows Hello / Other Strong Method
      ↓
Uses Normal Authentication Method
```

Think of TAP as:

> **A temporary bridge to stronger authentication.**

---

# 🆕 Onboarding Example

Imagine Contoso hires Jordan.

Instead of giving Jordan a permanent password that must later be changed:

```text
IT Creates Jordan's Identity
        ↓
Temporary Access Pass
        ↓
Jordan Signs In
        ↓
Registers Strong Authentication
        ↓
Passwordless Sign-In
```

This can support a more modern onboarding process.

---

# 🆘 Recovery Example

Suppose a user loses the device containing their authentication credential.

An authorized recovery process might use a Temporary Access Pass to help the user register a replacement authentication method.

Conceptually:

```text
Authentication Method Lost
        ↓
Identity Verified Through
Approved Recovery Process
        ↓
Temporary Access Pass
        ↓
Register New Method
```

Organizations should protect recovery processes carefully because attackers may try to exploit them.

---

# 🛡️ Phishing-Resistant Authentication

Not all MFA methods provide the same level of protection.

For example, an attacker may sometimes socially engineer users into approving an authentication prompt.

Phishing-resistant methods are designed to provide stronger protection against these attacks.

Microsoft technologies associated with phishing-resistant authentication can include:

```text
Passkeys / FIDO2

Windows Hello for Business

Certificate-Based Authentication
```

depending on configuration and policy.

---

# 💪 Authentication Strength

From Lesson 05:

**Authentication strength** can specify which authentication methods satisfy an access requirement.

For example:

```text
Normal User
     ↓
MFA Requirement
```

while:

```text
Privileged Administrator
        ↓
Phishing-Resistant
Authentication Requirement
```

This lets organizations match authentication strength to risk.

---

# 🚦 Passwordless + Conditional Access

Conditional Access can help enforce authentication requirements.

Conceptually:

```text
USER REQUESTS ACCESS
        ↓
CONDITIONAL ACCESS
        ↓
RESOURCE IS SENSITIVE
        ↓
REQUIRE STRONGER
AUTHENTICATION
        ↓
ACCESS DECISION
```

You will explore Conditional Access in Lesson 07.

---

# 🧱 Passwordless and Zero Trust

Passwordless authentication supports:

# Verify Explicitly

Zero Trust does not assume that a password alone proves identity strongly enough for every scenario.

Modern access decisions can consider:

```text
Identity

Authentication Method

Authentication Strength

Device

Risk

Application

Location
```

---

# 🏢 Real-World Example

Contoso has three groups:

```text
Normal Employees

IT Administrators

Executives
```

The company could design different authentication requirements.

Example:

```text
Normal Employees
      ↓
Strong MFA / Passwordless Options


IT Administrators
      ↓
Phishing-Resistant Authentication


Executives
      ↓
Strong Authentication
+
Additional Risk Controls
```

The exact policy depends on the organization's requirements.

---

# ⚖️ Passwordless Method Comparison

| Method | Typical Use | Passwordless | Phishing Resistant |
|---|---|---:|---:|
| Passkey / FIDO2 | Strong modern authentication | Yes | Yes |
| Windows Hello for Business | Windows device authentication | Yes | Yes |
| Microsoft Authenticator passwordless | Mobile-based passwordless sign-in | Yes | Not the same phishing-resistant category as FIDO2/WHfB |
| Temporary Access Pass | Bootstrap/recovery | Temporary method | Used to establish stronger methods |

The exact capabilities and policy behavior can evolve, so always consult current Microsoft documentation when designing a production authentication strategy.

---

# 🚫 Passwordless Does Not Mean Remove Every Password Immediately

Organizations may transition gradually.

A realistic path might be:

```text
PASSWORDS
   ↓
MFA
   ↓
STRONGER MFA
   ↓
PASSWORDLESS
   ↓
PHISHING-RESISTANT AUTHENTICATION
```

Different users, applications, and devices may move at different speeds.

---

# 🧩 Authentication Method Policy

Microsoft Entra administrators can control which authentication methods are available.

Conceptually:

```text
AUTHENTICATION METHOD
        ↓
TARGET USERS / GROUPS
        ↓
ALLOWED OR NOT ALLOWED
```

This helps organizations roll out methods gradually.

Example:

```text
IT Pilot Group
      ↓
Enable New Authentication Method
      ↓
Test
      ↓
Expand Deployment
```

---

# 🧪 Pilot Before Broad Deployment

Authentication changes can affect whether users can sign in.

A good operational approach is:

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

This is especially important in production environments.

---

# 🎯 Exam Focus

Know these relationships:

```text
PASSWORDLESS
=
Authenticate without entering
a traditional password
```

```text
PASSKEY / FIDO2
=
Cryptographic,
phishing-resistant authentication
```

```text
WINDOWS HELLO FOR BUSINESS
=
Strong device-bound Windows authentication
```

```text
TEMPORARY ACCESS PASS
=
Temporary bootstrap/recovery credential
```

```text
AUTHENTICATION STRENGTH
=
Require appropriate authentication
methods for an access scenario
```

---

# 🧠 Memory Tricks

### FIDO2

```text
FIDO2
=
PHISHING-RESISTANT KEY-BASED AUTH
```

### Windows Hello

```text
HELLO
=
DEVICE + USER VERIFICATION
```

### TAP

```text
TAP
=
TEMPORARY ACCESS PATH
```

### Passwordless

```text
NO REUSABLE PASSWORD
      ↓
STRONGER MODERN AUTHENTICATION
```

---

# ❓ Knowledge Check

### 1.

What is passwordless authentication?

A. Access without authentication  
B. Authentication without entering a traditional password  
C. Using two passwords  
D. Disabling identity security

---

### 2.

Which technology uses public-key cryptography and can provide phishing-resistant authentication?

A. FIDO2/passkeys  
B. Plain SMS only  
C. Traditional password only  
D. Username only

---

### 3.

Which is a Microsoft passwordless authentication technology for Windows devices?

A. Windows Hello for Business  
B. Windows Firewall  
C. Microsoft Paint  
D. Azure Storage

---

### 4.

What is the Windows Hello PIN primarily associated with?

A. Every website on the internet  
B. A particular device and protected credential  
C. A user's email mailbox only  
D. Azure billing

---

### 5.

What is a Temporary Access Pass primarily useful for?

A. Permanently replacing every authentication policy  
B. Bootstrapping or recovering authentication methods  
C. Managing virtual networks  
D. Encrypting SharePoint documents

---

### 6.

Which method is strongly associated with phishing resistance?

A. FIDO2 security key  
B. Password only  
C. Username only  
D. Security question only

---

### 7.

Why might an organization use an authentication method policy?

A. To control which users can use specific authentication methods  
B. To create network cables  
C. To manage printer toner  
D. To configure physical locks

---

### 8.

What can authentication strength help an organization do?

A. Require specific classes of authentication methods for access  
B. Increase internet speed  
C. Create user job titles  
D. Manage Azure invoices

---

### 9.

Which Zero Trust principle is most directly supported by strong passwordless authentication?

A. Verify explicitly  
B. Trust every internal user  
C. Disable monitoring  
D. Give permanent administrator access

---

### 10.

Why should organizations pilot authentication changes?

A. Authentication changes can affect user sign-in  
B. Passwordless always requires new servers  
C. MFA cannot be tested  
D. Microsoft Entra has no policies

---

# ✅ Knowledge Check Answers

```text
1. B — Authentication without entering a traditional password

2. A — FIDO2/passkeys

3. A — Windows Hello for Business

4. B — A particular device and protected credential

5. B — Bootstrapping or recovering authentication methods

6. A — FIDO2 security key

7. A — Control which users can use specific authentication methods

8. A — Require specific classes of authentication methods for access

9. A — Verify explicitly

10. A — Authentication changes can affect user sign-in
```

---

# 📌 Lesson Summary

You learned:

```text
PASSWORDLESS
=
Authentication without a traditional password
```

```text
PASSKEY / FIDO2
=
Key-based phishing-resistant authentication
```

```text
WINDOWS HELLO FOR BUSINESS
=
Device-bound strong authentication
```

```text
MICROSOFT AUTHENTICATOR
=
Can support passwordless sign-in
```

```text
TEMPORARY ACCESS PASS
=
Temporary onboarding/recovery method
```

Passwordless authentication can reduce dependence on reusable secrets and help organizations move toward stronger identity security.

---

# 🧪 Lab

This lesson benefits from a lab.

## 🔵 Lab 06 — Explore Passwordless Authentication

This is a read-only exploration lab.

You will locate and compare:

- Passkeys / FIDO2
- Microsoft Authenticator
- Windows Hello for Business
- Temporary Access Pass
- Authentication strengths
- Authentication method policies

No production authentication changes are required.

➡️ **[Lab 06 — Explore Passwordless Authentication](../labs/Lab%2006%20—%20Explore%20Passwordless%20Authentication.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 07 — Conditional Access & RBAC

Next you will learn how Microsoft can use signals and policies to decide whether access should be:

```text
Allowed

Blocked

Allowed with Requirements
```

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Passwordless Authentication Options](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-passwordless)
- [Passkeys in Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-enable-passkey-fido2)
- [Windows Hello for Business](https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/)
- [Temporary Access Pass](https://learn.microsoft.com/en-us/entra/identity/authentication/howto-authentication-temporary-access-pass)

---

# 📚 Course Navigation

⬅️ **Lesson 05 — Authentication & Multifactor Authentication**

🧪 **[Lab 06 — Explore Passwordless Authentication](../labs/Lab%2006%20—%20Explore%20Passwordless%20Authentication.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
