# 📘 Lesson 02 — Shared Responsibility, Defense in Depth & Zero Trust

**Course:** Microsoft SC-900 — Security, Compliance, and Identity Fundamentals  
**Lesson:** 02  
**Lab:** 🟡 Scenario Lab — Apply Zero Trust  
**Difficulty:** Beginner

---

# 🎯 Learning Objectives

By the end of this lesson, you should be able to:

- Describe the shared responsibility model
- Explain how responsibility changes between on-premises, IaaS, PaaS, and SaaS
- Describe defense in depth
- Explain the Zero Trust model
- Identify the three Zero Trust principles
- Recognize the major Zero Trust pillars
- Explain encryption and hashing
- Distinguish data at rest, in transit, and in use
- Explain Governance, Risk, and Compliance (GRC)
- Describe data residency, data sovereignty, and data privacy
- Apply these concepts to basic security scenarios

---

# 🤝 The Shared Responsibility Model

Moving to the cloud does **not** mean that the cloud provider becomes responsible for everything.

Security responsibilities are shared between:

```text
Microsoft
    +
Customer
```

Exactly who is responsible depends on the type of cloud service being used.

---

# 🏢 On-Premises

In a traditional on-premises environment, the organization manages nearly everything.

```text
CUSTOMER RESPONSIBILITY

Data
Applications
Runtime
Operating System
Virtualization
Servers
Storage
Networking
Physical Datacenter
```

The organization must secure and maintain the entire environment.

---

# ☁️ Infrastructure as a Service — IaaS

With IaaS, the cloud provider manages the physical infrastructure.

The customer still manages much of what runs on top of it.

A common example is an Azure virtual machine.

```text
Microsoft
────────────
Physical Datacenter
Physical Network
Physical Hosts

Customer
────────────
Operating System
Applications
Configuration
Accounts
Data
```

Think:

> Microsoft protects the physical cloud infrastructure, while you still have significant responsibility for what you deploy on it.

---

# ☁️ Platform as a Service — PaaS

With PaaS, the provider manages more of the underlying platform.

The customer focuses more heavily on:

```text
Applications
Data
Access
Configuration
```

and less on maintaining operating systems and physical infrastructure.

---

# ☁️ Software as a Service — SaaS

With SaaS, the provider manages most of the technical platform.

A familiar example is Microsoft 365.

The customer still has important responsibilities.

Examples include:

```text
Users
Passwords
Authentication
Access
Permissions
Data
Device Security
Configuration
```

Using SaaS does **not** remove the customer's security responsibilities.

---

# 🧠 Shared Responsibility Memory Trick

As you move:

```text
On-Premises
     ↓
IaaS
     ↓
PaaS
     ↓
SaaS
```

the provider generally manages **more** of the underlying technology.

But the customer always retains important responsibilities.

In particular, customers remain responsible for areas such as their:

```text
Data
Identities
Accounts
Access decisions
Configurations
```

depending on the service.

---

# 🛡️ Defense in Depth

Defense in depth means:

> Using multiple layers of security instead of depending on one control.

Imagine protecting a castle.

You would not rely on one door.

You might have:

```text
Outer Wall
    ↓
Moat
    ↓
Gate
    ↓
Guards
    ↓
Inner Wall
    ↓
Locked Rooms
```

Cybersecurity uses the same basic idea.

---

# 🧱 Security Layers

A simplified defense-in-depth model might include:

```text
PHYSICAL SECURITY
        ↓
IDENTITY
        ↓
PERIMETER
        ↓
NETWORK
        ↓
COMPUTE
        ↓
APPLICATION
        ↓
DATA
```

If one control fails, another layer may still prevent or limit an attack.

---

# 🌎 Defense-in-Depth Example

Suppose an attacker obtains an employee's password.

If password security were the only protection:

```text
Password Stolen
      ↓
Account Compromised
```

But with multiple controls:

```text
Password Stolen
      ↓
MFA
      ↓
Conditional Access
      ↓
Device Requirements
      ↓
Least Privilege
      ↓
Data Protection
```

the stolen password alone may not be enough.

That is defense in depth.

---

# 🔺 CIA Triad and Defense in Depth

Remember from Lesson 01:

```text
Confidentiality
Integrity
Availability
```

Defense-in-depth controls help protect all three.

Examples:

| Control | Security Benefit |
|---|---|
| MFA | Helps protect confidentiality |
| Encryption | Helps protect confidentiality |
| Hashing | Helps verify integrity |
| Backups | Helps support availability |
| DDoS protection | Helps support availability |
| Access controls | Helps protect confidentiality and integrity |

---

# 🚫 Zero Trust

Traditional security often assumed:

```text
Inside Network
=
Trusted
```

and:

```text
Outside Network
=
Untrusted
```

Modern environments make that assumption much less useful.

Users can work from anywhere.

Applications may exist in multiple clouds.

Devices may be:

```text
Corporate
Personal
Managed
Unmanaged
Remote
Mobile
```

Zero Trust uses a different approach.

---

# 🛡️ The Zero Trust Model

The basic idea is:

> Do not automatically trust an access request simply because of its location or previous access.

Instead, access decisions should be continuously informed by available signals and policy.

Microsoft describes three guiding Zero Trust principles:

```text
1. Verify explicitly

2. Use least privilege access

3. Assume breach
```

These are very important for SC-900.

---

# 1️⃣ Verify Explicitly

Verify explicitly means making access decisions using relevant information.

Signals might include:

```text
User identity
Location
Device
Application
Authentication method
Risk
Resource being accessed
```

Example:

```text
User requests access
       ↓
Who is the user?
       ↓
Is MFA satisfied?
       ↓
Is the device acceptable?
       ↓
Is the sign-in risky?
       ↓
What resource is requested?
       ↓
Policy Decision
```

Do not trust solely because:

> "They're inside the office."

---

# 2️⃣ Use Least Privilege Access

Least privilege means:

> Give identities only the access they need, for only as long as they need it.

Example:

A help desk technician may need to reset user passwords.

That does not automatically mean the technician should receive unrestricted access to every administrative function.

Think:

```text
NEEDED ACCESS
=
GRANTED

UNNEEDED ACCESS
=
NOT GRANTED
```

Reducing privileges can reduce the impact of:

```text
Compromised Accounts
Mistakes
Malware
Insider Threats
```

---

# 3️⃣ Assume Breach

Assume breach means designing security as though an attacker may already have gained some level of access.

This does **not** mean assuming every employee is malicious.

It means designing systems so one compromised account or device does not automatically compromise everything else.

Examples include:

```text
Segmentation
Monitoring
Encryption
Least Privilege
Threat Detection
Logging
Incident Response
```

Think:

```text
One System Compromised
        ↓
LIMIT THE DAMAGE
        ↓
DETECT ACTIVITY
        ↓
RESPOND
```

---

# 🧠 Remember Zero Trust

```text
VERIFY
   ↓
Verify Explicitly

LIMIT
   ↓
Least Privilege

EXPECT
   ↓
Assume Breach
```

---

# 🏛️ Zero Trust Pillars

Microsoft's Zero Trust approach considers multiple areas of an environment.

Important pillars include:

```text
Identities

Endpoints

Applications

Networks

Infrastructure

Data
```

Microsoft also treats visibility, automation, and orchestration as important across these areas.

For SC-900, understand that Zero Trust is an organization-wide security strategy rather than a single Microsoft product.

---

# ❌ Zero Trust Is NOT a Product

This is important.

You do not simply purchase:

```text
Microsoft Zero Trust
```

and turn it on.

Zero Trust is a:

> **Security model and strategy.**

Microsoft technologies can help implement it.

Examples include:

```text
Microsoft Entra
        ↓
Identity and access

Conditional Access
        ↓
Policy-based access

Microsoft Defender
        ↓
Threat protection

Microsoft Sentinel
        ↓
Detection and response

Microsoft Purview
        ↓
Data protection
```

---

# 🔐 Encryption

Encryption transforms readable information into a protected form using cryptographic algorithms and keys.

Conceptually:

```text
Readable Data
     ↓
Encryption
     ↓
Unreadable Ciphertext
```

With the appropriate key:

```text
Ciphertext
     ↓
Decryption
     ↓
Readable Data
```

Encryption primarily helps protect:

> **Confidentiality**

---

# 💾 Data at Rest

Data at rest is data being stored.

Examples:

```text
Hard Drive
Database
Storage Account
Backup
USB Drive
Cloud Storage
```

Encryption at rest helps protect stored information.

---

# 🌐 Data in Transit

Data in transit is moving between locations.

Examples:

```text
Laptop → Website

Application → Database

Office → Cloud Service
```

Protocols such as HTTPS/TLS can help protect data while it travels across networks.

---

# ⚙️ Data in Use

Data in use is data currently being processed or accessed.

Think:

```text
Stored
=
At Rest

Moving
=
In Transit

Being Processed
=
In Use
```

---

# #️⃣ Hashing

Hashing is different from encryption.

A hash function takes input and produces a fixed-size hash value.

Conceptually:

```text
Input Data
    ↓
Hash Function
    ↓
Hash Value
```

A small change to the input should produce a different hash.

Hashes are useful for purposes such as:

```text
Integrity Verification
Password Protection Techniques
Digital Signatures
File Verification
```

---

# 🔐 Encryption vs Hashing

A useful exam distinction:

## Encryption

Designed so protected information can be recovered with the appropriate key.

```text
Plaintext
   ↓
Encrypt
   ↓
Ciphertext
   ↓
Decrypt
   ↓
Plaintext
```

## Hashing

Designed as a one-way transformation.

```text
Data
 ↓
Hash
 ↓
Digest
```

You generally do not "decrypt" a hash to recover the original input.

---

# 🧠 Memory Trick

```text
ENCRYPTION
=
Protect secrecy

HASHING
=
Check integrity / represent data
```

---

# 🏛️ Governance, Risk & Compliance — GRC

GRC stands for:

```text
Governance
Risk
Compliance
```

These concepts help organizations manage security and business requirements systematically.

---

# 📜 Governance

Governance establishes how an organization makes decisions and sets expectations.

Examples:

```text
Policies
Standards
Roles
Responsibilities
Oversight
Processes
```

Example policy:

> Administrative accounts must use multifactor authentication.

---

# ⚠️ Risk

Risk considers the possibility that something could negatively affect the organization.

A simplified model is:

```text
Asset
  +
Threat
  +
Vulnerability
      ↓
Risk
```

Organizations identify risks and decide how to handle them.

Possible approaches include:

```text
Reduce
Avoid
Transfer
Accept
```

---

# 📋 Compliance

Compliance involves meeting applicable requirements.

These might come from:

```text
Laws
Regulations
Industry Standards
Contracts
Internal Policies
```

Compliance does not automatically guarantee perfect security.

Security and compliance support each other, but they are not identical.

---

# 🌍 Data Residency

Data residency concerns:

> Where data is physically or geographically stored.

For example, an organization may need to know whether data is stored in:

```text
United States
European Union
Canada
Australia
```

---

# ⚖️ Data Sovereignty

Data sovereignty concerns:

> The laws and regulations that apply to data because of the jurisdiction where it is stored or processed.

Location can therefore have legal implications.

---

# 🔏 Data Privacy

Data privacy concerns how personal or sensitive information is:

```text
Collected
Used
Shared
Stored
Protected
Retained
Deleted
```

Organizations need policies and controls governing appropriate use of information.

---

# 🧠 Residency vs Sovereignty vs Privacy

Remember:

```text
RESIDENCY
=
WHERE is the data?


SOVEREIGNTY
=
WHICH jurisdiction's laws apply?


PRIVACY
=
HOW is personal/sensitive data handled?
```

---

# 🌎 Real-World Scenario

Suppose Contoso moves its employee portal to the cloud.

The organization asks:

### Who patches the physical servers?

Under a cloud service:

> The cloud provider may be responsible for the underlying physical infrastructure.

### Who controls employee accounts?

> Contoso still has responsibility for its identities and access configuration.

### Should a user be trusted simply because they are in the office?

> No. Zero Trust says access should be explicitly verified based on relevant signals.

### Should every administrator receive Global Administrator?

> No. Least privilege says users should receive only necessary access.

### Should sensitive stored information be protected?

> Encryption can help protect data at rest.

### How can Contoso detect whether a downloaded file changed?

> Hashing can help verify integrity.

These concepts work together.

---

# 🎯 Exam Focus

Make sure you can recognize these relationships:

```text
Shared Responsibility
=
Provider + Customer
```

```text
Defense in Depth
=
Multiple security layers
```

```text
Zero Trust
=
Verify Explicitly
Use Least Privilege
Assume Breach
```

```text
Encryption
=
Protect confidentiality
```

```text
Hashing
=
One-way transformation useful for integrity
```

```text
GRC
=
Governance
Risk
Compliance
```

---

# ❓ Knowledge Check

### 1.

Which security model defines responsibilities shared between a cloud provider and customer?

A. Zero Trust  
B. Shared responsibility  
C. Federation  
D. RBAC

---

### 2.

Which cloud model generally leaves the customer with the greatest responsibility?

A. SaaS  
B. PaaS  
C. IaaS  
D. On-premises

---

### 3.

What is the main idea behind defense in depth?

A. Use one extremely strong security control  
B. Use multiple layers of security controls  
C. Trust internal network traffic  
D. Remove authentication requirements

---

### 4.

Which is one of Microsoft's three Zero Trust principles?

A. Trust internal users  
B. Verify explicitly  
C. Allow permanent administrator access  
D. Disable monitoring

---

### 5.

Which Zero Trust principle focuses on minimizing permissions?

A. Assume breach  
B. Verify explicitly  
C. Use least privilege access  
D. Shared responsibility

---

### 6.

Which Zero Trust principle encourages organizations to limit the impact of a successful compromise?

A. Assume breach  
B. Trust but verify  
C. High availability  
D. Federation

---

### 7.

Which technology is designed to protect readable information by converting it into ciphertext that can later be decrypted with the appropriate key?

A. Hashing  
B. Encryption  
C. Federation  
D. Auditing

---

### 8.

Which technology commonly helps verify that data has not changed?

A. Hashing  
B. SaaS  
C. Federation  
D. Authorization

---

### 9.

What does GRC stand for?

A. Governance, Risk, and Compliance  
B. Global Resource Control  
C. Governance, Recovery, and Cybersecurity  
D. General Regulatory Controls

---

### 10.

Which term refers primarily to where data is geographically stored?

A. Data sovereignty  
B. Data residency  
C. Data privacy  
D. Data authorization

---

# ✅ Knowledge Check Answers

```text
1. B — Shared responsibility

2. D — On-premises

3. B — Use multiple layers of security controls

4. B — Verify explicitly

5. C — Use least privilege access

6. A — Assume breach

7. B — Encryption

8. A — Hashing

9. A — Governance, Risk, and Compliance

10. B — Data residency
```

---

# 📌 Lesson Summary

You learned:

```text
SHARED RESPONSIBILITY
        ↓
Security is shared between
provider and customer


DEFENSE IN DEPTH
        ↓
Use multiple security layers


ZERO TRUST
        ↓
Verify Explicitly
Least Privilege
Assume Breach


ENCRYPTION
        ↓
Protect confidentiality


HASHING
        ↓
Help verify integrity


GRC
        ↓
Governance
Risk
Compliance
```

These concepts are foundational to Microsoft's security approach and are explicitly part of the current SC-900 skills measured.

---

# 🧪 Lab

This lesson has a useful lab:

## 🟡 Lab 02 — Apply Zero Trust

You will act as the security reviewer for a fictional company and decide how shared responsibility, defense in depth, and Zero Trust should be applied.

➡️ **[Lab 02 — Apply Zero Trust](../labs/Lab%2002%20—%20Apply%20Zero%20Trust.md)**

---

# ➡️ Next Lesson

## 📘 Lesson 03 — Microsoft Entra ID & Identity Types

Next you'll move from general security concepts into Microsoft's identity platform.

You'll learn about:

- Microsoft Entra ID
- Cloud identities
- Hybrid identities
- External identities
- Workload and agent identities
- Tenants and directories

Lesson 03 will include:

> 🔵 **Explore the Tool — Microsoft Entra admin center**

---

# 🔗 Official Microsoft Resources

- [SC-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/sc-900)
- [Describe security and compliance concepts](https://learn.microsoft.com/en-us/training/modules/describe-security-concepts-methodologies/)
- [SC-900 Security, Compliance, and Identity Concepts Learning Path](https://learn.microsoft.com/en-us/training/paths/m365-security-compliance-capabilities/)

---

# 📚 Course Navigation

⬅️ **[Lesson 01](%F0%9F%93%98%20Lesson%2001%20%E2%80%94%20Security,%20Compliance%20&%20Identity%20Fundamentals.md)**

🧪 **[Lab 02 — Apply Zero Trust](../labs/Lab%2002%20—%20Apply%20Zero%20Trust.md)**

📘 **[Lessons](README.md)**

🧪 **[Labs](../labs/README.md)**

📖 **[References](../references/)**

🔗 **[Resources](../resources/)**

🏠 **[Return to Main README](../README.md)**
