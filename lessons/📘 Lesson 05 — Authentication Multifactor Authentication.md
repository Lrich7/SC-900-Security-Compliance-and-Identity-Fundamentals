# 📘 Lesson 05 — Authentication & Multifactor Authentication

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 05  
**Lab:** 🔵 Explore the Tool — Authentication & MFA  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Explain authentication
- Distinguish authentication from authorization
- Describe common authentication factors
- Explain multifactor authentication (MFA)
- Describe common Microsoft Entra authentication methods
- Explain Security Defaults at a fundamentals level
- Describe Microsoft Entra authentication method policies
- Explain authentication strength
- Describe password protection concepts
- Explain why stronger authentication supports Zero Trust
- Locate authentication-related areas in the Microsoft Entra admin center

---

# 🔐 What Is Authentication?

Authentication answers:

> **Who are you?**

Before a system gives a user access, it usually needs to verify the user's identity.

Conceptually:

```text
USER
  ↓
Claims an Identity
  ↓
AUTHENTICATION
  ↓
Identity Verified
```

Examples include signing in with:

```text
Password

Microsoft Authenticator

Passkey

Security Key

Windows Hello

Certificate
```

---

# 🪪 Authentication vs Authorization

These terms sound similar but mean different things.

## Authentication

```text
WHO ARE YOU?
```

Authentication verifies identity.

## Authorization

```text
WHAT ARE YOU ALLOWED TO DO?
```

Authorization determines permissions after identity is established.

Example:

```text
Employee Badge
      ↓
AUTHENTICATION
      ↓
"This is Alex."
      ↓
AUTHORIZATION
      ↓
"Alex can enter the IT office,
but not the server room."
```

---

# 🧠 Memory Trick

```text
AuthN
=
Name
=
Who are you?
```

```text
AuthZ
=
Permission
=
What can you do?
```

---

# 🔑 Authentication Factors

Authentication can use different categories of evidence.

Three classic factors are:

```text
Something You KNOW

Something You HAVE

Something You ARE
```

---

# 🧠 Something You Know

Examples:

```text
Password

PIN
```

This information is known by the user.

---

# 📱 Something You Have

Examples:

```text
Phone

Hardware Security Key

Smart Card
```

This is a physical item the user possesses.

---

# 👆 Something You Are

Examples:

```text
Fingerprint

Face

Other Biometrics
```

This uses a characteristic of the person.

---

# 🛡️ What Is Multifactor Authentication?

**Multifactor authentication (MFA)** requires more than one authentication factor.

Example:

```text
PASSWORD
   +
AUTHENTICATOR APPROVAL
```

This combines:

```text
Something You Know
        +
Something You Have
```

If an attacker steals only the password, the attacker may still be unable to complete authentication.

---

# ❗ Two Passwords Are Not MFA

This is an important concept.

Suppose a system asks for:

```text
Password #1
+
Password #2
```

Both are:

```text
Something You Know
```

That is not true multifactor authentication.

MFA uses multiple **factor categories**, not simply multiple credentials from the same category.

---

# 🌎 Why MFA Matters

Passwords can be compromised through:

```text
Phishing

Password Reuse

Credential Theft

Malware

Data Breaches

Social Engineering
```

MFA adds another barrier.

Conceptually:

```text
Password Stolen
      ↓
Attacker Attempts Sign-In
      ↓
Additional Factor Required
      ↓
ACCESS MAY BE BLOCKED
```

MFA is an important part of modern identity security.

---

# 🔷 Microsoft Entra Authentication Methods

Microsoft Entra supports multiple authentication methods.

Depending on configuration and licensing, these can include technologies such as:

```text
Passwords

Microsoft Authenticator

Passkeys / FIDO2 Security Keys

Windows Hello for Business

Temporary Access Pass

Certificate-Based Authentication

SMS

Voice
```

Different methods provide different levels of security and different user experiences.

---

# 📱 Microsoft Authenticator

Microsoft Authenticator can support sign-in and MFA scenarios.

Depending on configuration, it can provide experiences such as:

```text
Push Notifications

Number Matching

Passwordless Sign-In
```

Example:

```text
User Signs In
     ↓
Authentication Request
     ↓
Microsoft Authenticator
     ↓
User Verifies Request
```

---

# 🔢 Number Matching

With number matching, the sign-in experience displays a number that the user must match in Microsoft Authenticator.

Conceptually:

```text
Sign-In Screen
      ↓
Shows: 42
      ↓
Authenticator
      ↓
User selects/enters 42
```

This helps the user verify that the authentication request corresponds to the sign-in they are actually performing.

---

# 📲 SMS and Voice

Microsoft Entra can support phone-based authentication methods such as:

```text
SMS

Voice Call
```

These may be useful in some environments, but organizations should understand that not all authentication methods provide the same security strength.

More phishing-resistant methods are preferred for higher-risk or privileged scenarios when practical.

---

# 🔐 Passkeys and FIDO2

Passkeys and FIDO2 security keys can provide strong, phishing-resistant authentication.

Examples include:

```text
Hardware Security Key

Device-Based Passkey
```

These methods reduce dependence on traditional passwords.

We will examine passwordless authentication more closely in:

> **Lesson 06 — Passwordless Authentication**

---

# 💻 Windows Hello for Business

Windows Hello for Business allows users to authenticate using methods such as:

```text
PIN

Face

Fingerprint
```

The credential is tied to the device and backed by cryptographic keys.

The PIN is not simply a traditional password sent to Microsoft over the network.

---

# 🎟️ Temporary Access Pass

A **Temporary Access Pass (TAP)** is a time-limited passcode that can help users register or recover strong authentication methods.

Conceptually:

```text
New User
   ↓
Temporary Access Pass
   ↓
Registers Strong Authentication
   ↓
Normal Authentication Method
```

TAP can be useful during onboarding and recovery scenarios.

---

# 🪪 Certificate-Based Authentication

Certificate-Based Authentication can use digital certificates to authenticate users.

At the SC-900 level, remember:

```text
CERTIFICATE
     ↓
Can be used as an authentication method
```

You do not need to become a public key infrastructure expert for this course.

---

# 🧱 Authentication Method Policy

Administrators can manage which authentication methods are available to users through Microsoft Entra authentication method policies.

Conceptually:

```text
ORGANIZATION
      ↓
AUTHENTICATION METHOD POLICY
      ↓
Which users/groups
can use which methods
```

This allows organizations to move toward stronger authentication methods in a controlled way.

---

# 💪 Authentication Strength

**Authentication strength** allows organizations to define which combinations of authentication methods satisfy a particular access requirement.

Example idea:

```text
Normal Resource
      ↓
MFA Required
```

while a highly sensitive resource might require:

```text
Sensitive Resource
      ↓
Phishing-Resistant MFA
```

Authentication strength can work with Conditional Access.

You will explore Conditional Access more deeply in Lesson 07.

---

# 🚦 Authentication Strength + Conditional Access

Conceptually:

```text
USER REQUESTS ACCESS
        ↓
CONDITIONAL ACCESS
        ↓
Authentication Requirement
        ↓
Required Authentication Strength
        ↓
ALLOW / BLOCK
```

This allows organizations to require stronger authentication for more sensitive scenarios.

---

# 🛡️ Security Defaults

**Security Defaults** provide baseline identity security settings for organizations that may not have configured more advanced identity security controls.

Security Defaults are designed to help protect organizations from common identity-related attacks.

At a fundamentals level, associate Security Defaults with protections such as:

```text
MFA Registration

MFA for Administrative Access

Blocking Legacy Authentication
```

The exact sign-in behavior can depend on Microsoft's current implementation and risk evaluation.

---

# 🧠 Security Defaults vs Conditional Access

Think of the broad distinction:

```text
SECURITY DEFAULTS
=
Microsoft-provided baseline protections
```

```text
CONDITIONAL ACCESS
=
More customizable policy-based access control
```

Organizations should understand their licensing and security requirements before changing either.

---

# 🔑 Password Protection

Passwords remain common, so Microsoft Entra includes password protection capabilities.

Password protection can help prevent users from selecting weak or commonly attacked passwords.

Examples of passwords organizations should avoid include:

```text
Password123!

CompanyName2026!

Welcome123!
```

A password can meet traditional complexity requirements and still be predictable.

---

# 🚫 Banned Passwords

Microsoft Entra password protection uses banned-password concepts to help prevent weak password choices.

Organizations may also use custom banned-password terms in supported configurations.

Examples might include:

```text
Company Name

Product Name

Local Sports Team

Office Location
```

These terms may be easy for attackers to guess if they are associated with the organization.

---

# 🧠 Password Complexity Is Not Everything

Historically, organizations often focused on requirements such as:

```text
Uppercase

Lowercase

Number

Symbol
```

But:

```text
Summer2026!
```

may technically satisfy complexity requirements while still being predictable.

Modern authentication strategy should not depend on passwords alone.

---

# 🚫 Legacy Authentication

Older authentication protocols may not support modern protections such as MFA.

This creates additional risk.

Conceptually:

```text
MODERN AUTHENTICATION
      ↓
Can support stronger controls


LEGACY AUTHENTICATION
      ↓
May bypass or lack modern controls
```

Reducing or blocking legacy authentication is an important identity-security concept.

---

# 🛡️ Authentication and Zero Trust

Authentication supports the first Zero Trust principle:

# Verify Explicitly

Remember:

```text
VERIFY EXPLICITLY
=
Use available signals to make access decisions
```

Authentication can provide important signals such as:

```text
Identity

Authentication Method

MFA Status

Authentication Strength

Risk
```

---

# 🏢 Real-World Example

Contoso has an HR application containing sensitive employee data.

Originally:

```text
Username
   +
Password
   ↓
ACCESS
```

Contoso improves the design:

```text
Username
   +
Password
   +
MFA
   ↓
Conditional Access Evaluation
   ↓
ACCESS
```

For administrators, Contoso may require even stronger authentication.

```text
ADMINISTRATOR
      ↓
Phishing-Resistant Authentication
      ↓
Administrative Resource
```

This is an example of matching authentication requirements to risk.

---

# ⚠️ MFA Fatigue

Attackers may repeatedly trigger authentication requests hoping that a user eventually approves one.

This is sometimes called:

> **MFA fatigue** or **MFA push bombing**

Users should never approve an authentication request they did not initiate.

Features such as number matching help users better identify legitimate authentication requests.

---

# 🎣 Phishing Resistance

Traditional passwords can be stolen by phishing.

Some MFA methods can also be socially engineered.

Phishing-resistant authentication methods are designed to provide stronger protection against credential phishing.

Examples include technologies based on:

```text
FIDO2 / Passkeys

Windows Hello for Business

Certificate-Based Authentication
```

depending on configuration.

---

# 🎯 Exam Focus

Know these relationships:

```text
AUTHENTICATION
=
Who are you?
```

```text
AUTHORIZATION
=
What can you do?
```

```text
MFA
=
Two or more authentication factors
```

```text
SECURITY DEFAULTS
=
Baseline identity security protections
```

```text
AUTHENTICATION STRENGTH
=
Controls which authentication methods
can satisfy an access requirement
```

```text
PASSWORD PROTECTION
=
Helps prevent weak or banned passwords
```

---

# 🧠 Memory Tricks

### Authentication

```text
AUTH-N
=
NAME
=
WHO ARE YOU?
```

### Authorization

```text
AUTH-Z
=
ACCESS
=
WHAT CAN YOU DO?
```

### MFA

```text
KNOW
+
HAVE
+
ARE

Use at least two different factors
```

### Security Defaults

```text
DEFAULT
=
BASELINE PROTECTION
```

---

# ❓ Knowledge Check

### 1.

What question does authentication answer?

A. What can you do?  
B. Who are you?  
C. Where is the data stored?  
D. What license is assigned?

---

### 2.

What question does authorization answer?

A. Who are you?  
B. What are you allowed to do?  
C. What is your password?  
D. Where is the datacenter?

---

### 3.

Which is an example of something you have?

A. Password  
B. PIN  
C. Hardware security key  
D. Username

---

### 4.

Which combination is true MFA?

A. Password + PIN  
B. Password + security key  
C. Two passwords  
D. Two PINs

---

### 5.

What is Microsoft Authenticator used for?

A. Physical network cabling  
B. Authentication  
C. Data residency  
D. Azure billing only

---

### 6.

What is a Temporary Access Pass designed to help with?

A. Physical building access  
B. Registering or recovering strong authentication methods  
C. Creating virtual networks  
D. Managing backups

---

### 7.

What do Security Defaults provide?

A. Baseline identity security protections  
B. Physical server maintenance  
C. Database development  
D. Email archiving only

---

### 8.

What does authentication strength help define?

A. The physical strength of a security key  
B. Which authentication methods satisfy an access requirement  
C. The size of a password database  
D. The number of users in a group

---

### 9.

Why can legacy authentication be risky?

A. It may not support modern protections such as MFA  
B. It requires too many security keys  
C. It always uses biometrics  
D. It automatically deletes accounts

---

### 10.

Which Zero Trust principle is most directly supported by strong authentication?

A. Assume nothing is encrypted  
B. Verify explicitly  
C. Give everyone administrator rights  
D. Disable logging

---

# ✅ Knowledge Check Answers

```text
1. B — Who are you?

2. B — What are you allowed to do?

3. C — Hardware security key

4. B — Password + security key

5. B — Authentication

6. B — Registering or recovering strong authentication methods

7. A — Baseline identity security protections

8. B — Which authentication methods satisfy an access requirement

9. A — It may not support modern protections such as MFA

10. B — Verify explicitly
```

---

# 📌 Lesson Summary

You learned:

```text
AUTHENTICATION
=
Verify identity
```

```text
AUTHORIZATION
=
Determine access
```

```text
MFA
=
Use multiple authentication factors
```

```text
AUTHENTICATION METHODS
=
Ways an identity can prove who it is
```

```text
AUTHENTICATION STRENGTH
=
Require appropriate methods for the scenario
```

and:

```text
STRONG IDENTITY SECURITY
=
More than just passwords
```

---

# 🧪 Lab

This lesson benefits from a lab.

## 🔵 Lab 05 — Explore Authentication & MFA

This is a read-only exploration lab.

You will locate:

- Authentication methods
- Authentication method policies
- MFA-related areas
- Security Defaults
- Password protection
- Conditional Access
- Sign-in and authentication information

No production configuration changes are required.

➡️ **[Lab 05 — Explore Authentication & MFA](../labs/Lab%2005%20—%20Explore%20Authentication%20&%20MFA.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 06 — Passwordless Authentication

Next you will go deeper into:

- Passkeys
- FIDO2 security keys
- Windows Hello for Business
- Microsoft Authenticator
- Temporary Access Pass
- Passwordless authentication strategy

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Authentication Methods in Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods)
- [Microsoft Entra MFA](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-mfa-howitworks)
- [Authentication Strengths](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-strengths)
- [Security Defaults](https://learn.microsoft.com/en-us/entra/fundamentals/security-defaults)

---

# 📚 Course Navigation

⬅️ **Lesson 04 — Users, Groups & Identity Management**

🧪 **[Lab 05 — Explore Authentication & MFA](../labs/Lab%2005%20—%20Explore%20Authentication%20&%20MFA.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
