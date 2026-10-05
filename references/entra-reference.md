# 👤 Microsoft Entra Reference

A quick-reference guide for the Microsoft Entra concepts covered by
SC-900.

------------------------------------------------------------------------

# 🧠 Main Purpose

``` text
MICROSOFT ENTRA
=
IDENTITY & ACCESS
```

Microsoft Entra ID is Microsoft's cloud identity and access management
service.

It was previously called:

``` text
Azure Active Directory
Azure AD
```

------------------------------------------------------------------------

# 👥 Identity Types

## Human Identities

Employees, administrators, guests, partners, and contractors.

## Device Identities

``` text
Entra Registered
Entra Joined
Entra Hybrid Joined
```

## Workload Identities

Identities used by applications, services, scripts, and automation.

Examples:

``` text
Service Principals
Managed Identities
Applications
```

## External Identities

Users outside the organization who require access to resources.

## Agent Identities

Identities associated with AI agents or agent-based workloads.

------------------------------------------------------------------------

# 👤 Users

Common user information includes:

``` text
Display Name
User Principal Name
User Type
Job Title
Department
Manager
Account Status
```

## Member

Usually an internal organizational user.

## Guest

Typically an external user invited to collaborate.

------------------------------------------------------------------------

# 👥 Groups

Groups simplify access management.

## Security Group

Primarily used for:

``` text
Permissions
Access
Security
```

## Microsoft 365 Group

Primarily supports collaboration across Microsoft 365 services.

## Membership

``` text
Assigned
→ Membership manually managed

Dynamic
→ Membership based on rules/attributes
```

------------------------------------------------------------------------

# 🔐 Authentication

``` text
AUTHENTICATION
→ Who are you?
```

Common methods:

``` text
Password
Microsoft Authenticator
Passkey / FIDO2
Windows Hello for Business
Temporary Access Pass
Certificate-Based Authentication
SMS
Voice
```

------------------------------------------------------------------------

# 🔑 MFA

MFA uses two or more different authentication factor types.

``` text
KNOW
→ Password/PIN

HAVE
→ Phone/security key

ARE
→ Fingerprint/face
```

------------------------------------------------------------------------

# 🔓 Passwordless

Important methods:

``` text
Passkeys / FIDO2
Windows Hello for Business
Microsoft Authenticator
Temporary Access Pass
```

Remember:

``` text
PASSWORDLESS
≠
AUTHENTICATION-FREE
```

------------------------------------------------------------------------

# 🚦 Conditional Access

Conditional Access evaluates access requests using signals and controls.

``` text
IF
User
Device
Location
Application
Risk

THEN
Allow
Block
Require MFA
Require compliant device
Require authentication strength
```

Conditional Access supports Zero Trust:

``` text
VERIFY EXPLICITLY
```

------------------------------------------------------------------------

# 🛡️ Security Defaults

Provides baseline identity-security protections for organizations that
do not use more customized Conditional Access policies.

Think:

``` text
SECURITY DEFAULTS
→ Simpler baseline protection

CONDITIONAL ACCESS
→ Granular/custom access policies
```

------------------------------------------------------------------------

# 👑 Microsoft Entra Roles

Used to control administrative access to identity/directory resources.

Examples:

``` text
Global Administrator
User Administrator
Groups Administrator
Authentication Administrator
Application Administrator
```

Use:

``` text
LEAST PRIVILEGE
```

Do not give Global Administrator when a smaller role is sufficient.

------------------------------------------------------------------------

# ☁️ Entra Roles vs Azure RBAC

``` text
ENTRA ROLE
→ Identity/directory administration

AZURE RBAC
→ Azure resource authorization
```

------------------------------------------------------------------------

# ⚠️ Identity Protection

Detects identity-related risk.

``` text
USER RISK
→ Is this identity likely compromised?

SIGN-IN RISK
→ Is this particular sign-in suspicious?

RISK DETECTION
→ Signal/event contributing to risk
```

Risk can be used with Conditional Access.

------------------------------------------------------------------------

# 🏛️ Identity Governance

Ensures the right identities have the right access for the right amount
of time.

``` text
RIGHT IDENTITY
RIGHT ACCESS
RIGHT RESOURCE
RIGHT TIME
```

## PIM

``` text
PRIVILEGED IDENTITY MANAGEMENT
→ Just-in-time privileged access
```

## Access Reviews

``` text
DOES THIS USER STILL NEED ACCESS?
```

## Entitlement Management

Uses access packages to manage access to groups, apps, and resources.

## Lifecycle Workflows

Supports:

``` text
JOINER
MOVER
LEAVER
```

------------------------------------------------------------------------

# 🔄 Identity Lifecycle

``` text
JOINER
→ Create/provision access

MOVER
→ Update access as role changes

LEAVER
→ Remove access
```

------------------------------------------------------------------------

# 🧠 Entra Decision Map

``` text
SIGN IN?
→ Authentication

EXTRA VERIFICATION?
→ MFA

NO PASSWORD?
→ Passwordless

ACCESS CONDITIONS?
→ Conditional Access

ADMIN PRIVILEGES?
→ Entra Roles / PIM

SUSPICIOUS IDENTITY?
→ Identity Protection

REVIEW ACCESS?
→ Access Reviews

PACKAGE ACCESS?
→ Entitlement Management

JOINER/MOVER/LEAVER?
→ Lifecycle Workflows
```

------------------------------------------------------------------------

# 📚 Navigation

⬅️ **[References](README.md)**\
🏠 **[Main README](../README.md)**
