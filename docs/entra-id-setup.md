# Microsoft Entra ID Setup

## What This Document Covers

This document explains how Microsoft Entra ID was configured as the cloud identity layer in this project and how it integrates with on-premises Active Directory in a hybrid identity model.

It covers setup decisions, authentication management, and how Entra ID is used in real IT support scenarios.

## Why Microsoft Entra ID

Active Directory manages identity within a local network environment, while Microsoft Entra ID extends identity management to cloud services.

In real enterprise environments, both systems are used together to support hybrid identity.

Entra ID is responsible for:

- Cloud authentication
- Microsoft 365 access
- Multi-factor authentication (MFA)
- Remote user sign-in management

Understanding both systems is essential for modern IT support and IAM roles.

## Why Hybrid Identity Matters

Most organisations do not operate purely on-premises or purely cloud-based systems. Instead, identity is split across:

- Active Directory (on-premises identity)
- Microsoft Entra ID (cloud identity)

This creates a hybrid identity model where users can access both local and cloud resources using a unified identity structure.

## Entra ID Configuration

| Setting | Value |
|---|---|
| Tenant Name | Default Directory |
| Primary Domain | onmicrosoft.com |
| License Type | Microsoft Entra ID Free |
| Admin Role | Global Administrator |

## Setup Steps

1. Accessed Microsoft Entra ID via Azure portal
2. Confirmed Default Directory tenant configuration
3. Verified Global Administrator access
4. Created a test user account (Bjorn Larsson)
5. Navigated to Authentication Methods section
6. Configured MFA settings for user authentication control
7. Performed MFA reset for simulated support incident (INC0010005)
8. Verified user authentication changes applied successfully

## Example Support Scenario

A user lost access to their account due to a missing authenticator app.

The issue was not related to Active Directory. The resolution was handled entirely in Microsoft Entra ID by resetting multi-factor authentication and allowing the user to re-register their device.

This demonstrates how cloud identity issues are handled separately from on-premises identity systems.

## Why MFA Management Matters

Multi-factor authentication is a core security control in modern environments. It ensures that even if a password is compromised, access cannot be granted without a second verification method.

IT support teams are responsible for:

- Resetting MFA when users lose devices
- Re-enrolling authentication methods
- Ensuring secure access recovery without weakening security

## Key Takeaway

Microsoft Entra ID is a critical part of modern identity management. It handles cloud authentication, security verification, and user access to Microsoft services.

In real IT support environments, knowing whether an issue belongs to Active Directory or Entra ID is essential for fast and accurate resolution.
