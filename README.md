# Enterprise IAM Architecture

### Learn how enterprise Identity and Access Management (IAM) is architected across modern organizations, from core identity components to authentication, authorization, governance, privileged access, and cloud integration.

---

<p align="center">

# Haris Trust

### *Guarding Digital Trust.*

**Enterprise Identity Security Portfolio**

</p>

---

## Repository Information

| Category | Details |
|----------|---------|
| Level | Beginner → Advanced |
| Reading Time | 45–60 Minutes |
| Hands-on Lab | Yes |
| Enterprise Focus | Yes |
| Interview Preparation | Yes |

---

## Repository Overview

Identity and Access Management (IAM) is far more than creating user accounts or resetting passwords. In modern enterprises, IAM serves as the security foundation that ensures the right individuals have the right access to the right resources at the right time.

Whether employees are accessing on-premises applications, cloud services, VPNs, or privileged systems, IAM provides the controls that authenticate identities, authorize access, enforce security policies, and maintain compliance.

This repository explains how enterprise IAM environments are designed, how different identity components work together, and how organizations secure identities across hybrid infrastructures.

---

# Learning Objectives

By the end of this repository, you will understand:

- What Enterprise IAM Architecture is
- Core IAM building blocks
- Identity lifecycle management
- Authentication vs Authorization
- Single Sign-On (SSO)
- Multi-Factor Authentication (MFA)
- Identity Federation
- Directory Services
- Identity Governance
- Privileged Access Management (PAM)
- Access Review processes
- Enterprise IAM workflows
- Common IAM attack paths
- Defensive security controls
- Enterprise architecture best practices

---

# Why This Matters

Modern organizations may manage:

- 5,000 employees
- 20,000 contractors
- Thousands of servers
- Hundreds of SaaS applications
- Cloud workloads
- Service accounts
- APIs
- Privileged administrators

Without a well-designed IAM architecture:

- Unauthorized access increases
- Insider threats become difficult to detect
- Compliance requirements fail
- Manual access management becomes unmanageable
- Privileged accounts become high-value attack targets

IAM enables organizations to scale securely while maintaining visibility and control over identities and access.

---

# Core Concepts

## Identity

An identity represents a user, service account, application, or device that interacts with enterprise resources.

Examples:

- Employee
- Contractor
- Vendor
- Service Account
- Administrator
- API Identity
- Device Identity

Everything starts with identity.

---

## Authentication

Authentication answers:

> Who are you?

Examples:

- Username + Password
- Smart Card
- MFA
- Windows Login
- Certificate Authentication
- Biometrics

Authentication verifies identity before access is granted.

---

## Authorization

Authorization answers:

> What are you allowed to do?

Examples:

- Read files
- Modify database records
- Restart servers
- Access HR systems
- View payroll data

Authorization occurs after successful authentication.

---

## Identity Repository

The identity repository stores user information and access attributes.

Examples:

- Active Directory
- Microsoft Entra ID
- LDAP
- HR Systems

It acts as the central source of identity information.

---

## Identity Lifecycle Management

Every identity follows a lifecycle:

Joiner

↓

Mover

↓

Leaver

Joiners receive initial access.

Movers have access updated based on role changes.

Leavers have all access removed promptly to prevent unauthorized access.

---

## Role-Based Access Control (RBAC)

Instead of assigning permissions individually, users receive access based on their role.

Example:

HR Manager

↓

HR Role

↓

HR Applications

↓

Payroll Access

↓

Employee Records

RBAC simplifies administration and reduces access errors.

---

## Least Privilege

Users receive only the permissions necessary to perform their job responsibilities.

Benefits include:

- Reduced attack surface
- Lower insider risk
- Improved compliance
- Easier auditing

---

## Segregation of Duties (SoD)

Critical tasks are separated among different users to prevent fraud or misuse.

Example:

One employee creates a payment.

Another employee approves it.

This separation reduces the risk of abuse.

---

# Enterprise IAM Components

## Active Directory

Stores user identities, groups, and computer objects for Windows environments.

Functions include:

- Authentication
- Authorization
- Group Policy
- Kerberos
- LDAP

---

## Microsoft Entra ID

Provides cloud identity services.

Capabilities include:

- Cloud authentication
- Conditional Access
- MFA
- SaaS integration
- Identity Protection

---

## Identity Governance (IGA)

IGA focuses on:

- Access requests
- Approval workflows
- Certifications
- Access reviews
- Compliance reporting

Popular solutions:

- SailPoint
- Saviynt
- One Identity

---

## Privileged Access Management (PAM)

Protects administrative accounts.

Functions include:

- Password vaulting
- Session recording
- Just-In-Time access
- Credential rotation
- Privileged session monitoring

Popular solutions:

- Delinea
- CyberArk
- BeyondTrust

---

## Single Sign-On (SSO)

SSO allows users to authenticate once and access multiple applications without repeatedly entering credentials.

Benefits:

- Better user experience
- Reduced password fatigue
- Fewer helpdesk tickets
- Centralized authentication

---

## Multi-Factor Authentication (MFA)

MFA requires multiple verification factors.

Examples:

- Password
- Mobile approval
- OTP
- Hardware token
- Biometrics

Even if passwords are compromised, MFA significantly reduces unauthorized access.

---

## Federation

Federation enables trusted authentication between organizations and cloud providers.

Common protocols include:

- SAML
- OAuth 2.0
- OpenID Connect (OIDC)

This enables seamless access across multiple domains without maintaining separate credentials.

---

# Enterprise IAM Flow

```
HR Creates Employee

        ↓

Identity Created

        ↓

Account Provisioned

        ↓

Access Assigned

        ↓

Authentication

        ↓

Authorization

        ↓

Application Access

        ↓

Logging & Monitoring

        ↓

Access Reviews

        ↓

Role Changes

        ↓

Deprovisioning
```

---

# Enterprise Perspective

A typical enterprise IAM ecosystem includes:

- HR System
- Active Directory
- Microsoft Entra ID
- Identity Governance Platform
- PAM Solution
- MFA Provider
- SSO Portal
- Cloud Applications
- VPN
- SIEM
- ITSM Platform

These systems integrate to automate identity management, improve security, and support regulatory compliance.

---

# Detection & Defense

## Common IAM Attacks

- Password Spraying
- Credential Stuffing
- Phishing
- Pass-the-Hash
- Golden Ticket attacks
- Privilege Escalation
- Excessive permissions
- Stale accounts
- Service account abuse
- Insider threats

---

## Defensive Controls

- MFA
- Conditional Access
- Least Privilege
- RBAC
- Just-In-Time Administration
- PAM
- Access Reviews
- Password Rotation
- Identity Governance
- SIEM Monitoring
- Behavioral Analytics
- Zero Trust principles

---

# Hands-on Lab

## Objective

Understand how an enterprise IAM architecture supports identity lifecycle management.

### Lab Tasks

- Identify each IAM component in your environment.
- Map the Joiner–Mover–Leaver lifecycle.
- Create a simple IAM architecture diagram on paper or digitally.
- List systems involved in user provisioning.
- Identify where authentication and authorization occur.
- Determine where logs are generated.
- Note where access reviews and approvals take place.

---

# Interview Questions

### Beginner

- What is IAM?
- What is authentication?
- What is authorization?
- What is RBAC?
- What is MFA?
- What is SSO?
- What is Active Directory?

### Intermediate

- Explain the Joiner-Mover-Leaver process.
- How does IAM improve enterprise security?
- What is Identity Governance?
- Why is Least Privilege important?
- What is Segregation of Duties?

### Advanced

- Describe a modern enterprise IAM architecture.
- How do AD and Entra ID work together?
- What is the role of PAM?
- How do SAML, OAuth 2.0, and OIDC differ?
- How would you secure privileged identities in a hybrid environment?

---

# From the Field

In enterprise environments, IAM is not a single product but an integrated ecosystem. HR systems trigger identity creation, directories store user accounts, governance platforms manage approvals, PAM protects privileged accounts, SSO simplifies access, MFA strengthens authentication, and SIEM solutions monitor identity events. Security teams rely on this architecture to reduce risk, automate operations, and maintain compliance at scale.

---

# Key Takeaways

- IAM is the foundation of enterprise security.
- Authentication verifies identity.
- Authorization determines access.
- RBAC simplifies permission management.
- Least Privilege minimizes risk.
- Identity Governance enforces compliance.
- PAM secures privileged accounts.
- Federation enables secure cross-domain access.
- Monitoring and auditing are essential for detecting identity-based threats.
- Well-designed IAM architecture supports secure business growth.

---

# References

- Microsoft Identity Documentation
- Microsoft Entra ID Documentation
- SailPoint Documentation
- Delinea Documentation
- NIST Cybersecurity Framework
- NIST SP 800-63 Digital Identity Guidelines
- OWASP Identity and Access Control Resources

---

# Revision List (Version 1.1+)

- Add enterprise architecture diagrams
- Add Mermaid diagrams
- Add hybrid AD + Entra architecture
- Add Zero Trust identity model
- Add authentication flow diagrams
- Add SAML/OAuth/OIDC comparison table
- Add PowerShell examples
- Add KQL detection examples
- Add Sigma detection rules
- Add IAM maturity model
- Add enterprise case studies
- Add screenshots
- Add interview scenario walkthroughs

---

# Next Repository

➡️ **Repository #9 – Identity-Incident-Response-Playbooks**

---

**Haris Trust**

*Guarding Digital Trust.*
