# Microsoft Intune — Device Onboarding and MDM Setup

## What This Document Covers
This document explains how Microsoft Intune was configured 
as the Mobile Device Management (MDM) solution in this 
project and how it was used to enrol, secure and manage 
a macOS device on behalf of a new employee.

It covers setup decisions, compliance policy configuration, 
device enrolment and update policy management.

## Why Microsoft Intune
Microsoft Intune is a cloud-based endpoint management 
platform that allows IT teams to manage and secure devices 
across an organisation from a single admin center.

In real enterprise environments, Intune is used to:
- Enrol company devices into centralised management
- Apply compliance policies to enforce security standards
- Push software and update policies to managed devices
- Verify devices meet security requirements before 
  granting access to company resources

Understanding Intune is essential for modern IT support, 
endpoint management and device security roles.

## Why MDM Matters
Organisations cannot rely on users to self-manage device 
security. Mobile Device Management ensures that:

- Every device meets minimum security requirements
- Encryption and password policies are enforced
- Software updates are pushed and controlled by IT
- Devices can be monitored and wiped remotely if needed

Without MDM, a single unmanaged device can become a 
security risk to the entire organisation.

## Intune Configuration

| Setting | Value |
|---|---|
| Tenant Name | Default Directory |
| Admin Account | admin@Hamdansuleimanhotmail.onmicrosoft.com |
| License Type | Microsoft Intune Plan 1 (Trial) |
| MDM Authority | Microsoft Intune |
| Platform Managed | macOS |
| Apple MDM Push Certificate | Active — Expires May 7 2027 |

## Setup Steps
1. Accessed Microsoft Intune admin center at intune.microsoft.com
2. Activated Microsoft Intune Plan 1 free trial licence
3. Assigned Global Administrator and Intune Administrator 
   roles to admin account
4. Configured Apple MDM Push Certificate via Apple Push 
   Certificates Portal using Apple ID
5. Created compliance policy requiring password protection 
   and device encryption
6. Enrolled MacBook Air into Intune via Company Portal app
7. Verified device appeared as compliant in Intune device list
8. Created and assigned software update policy using 
   DDM Settings Catalog

## Compliance Policy

| Setting | Value |
|---|---|
| Policy Name | Compliance-Policy-INC0010006 |
| Platform | macOS |
| Password Required | Yes |
| Minimum Password Length | 8 characters |
| Encryption Required | Yes |
| Action on Noncompliance | Mark device noncompliant immediately |
| Assignment | All devices |

## Update Policy

| Setting | Value |
|---|---|
| Policy Name | UpdatePolicy-INC0010006 |
| Platform | macOS |
| Method | Declarative Device Management (DDM) |
| Target OS Version | 14.8.5 |
| Target Date | 01/01/2027 |
| Assignment | All devices and all users |

## Example Support Scenario
A new employee, Jonas Eriksson, was given a company laptop 
on his first day. IT was required to enrol the device into 
Intune, apply a compliance policy and push a software update 
policy before he could access company resources.

The device was enrolled using Company Portal on macOS. 
The compliance policy immediately enforced password and 
encryption requirements on the device in real time, 
confirming successful MDM enrolment and policy application.

## Why Compliance Policies Matter
Compliance policies are the foundation of zero-trust 
security in endpoint management. They ensure that:

- Devices must prove they meet security standards before 
  accessing company resources
- Password and encryption are enforced at the device level
- IT has visibility into which devices are compliant and 
  which are not
- Noncompliant devices can be automatically blocked

## Key Takeaway
Microsoft Intune is a critical tool in modern IT 
environments. It gives IT teams full visibility and 
control over company devices, ensuring security policies 
are enforced consistently across all managed endpoints.

In real IT support environments, knowing how to enrol 
devices, apply compliance policies and troubleshoot MDM 
issues is essential for endpoint management and 
security roles.
