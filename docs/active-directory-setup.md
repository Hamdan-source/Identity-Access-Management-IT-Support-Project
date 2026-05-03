# Active Directory Setup

## What This Document Covers

This document explains how Active Directory Domain Services were installed and configured on the Azure Windows Server 2025 virtual machine. It covers the promotion of the server to a Domain Controller for the PROJECT.LOCAL domain and the reasoning behind each configuration decision.

## Why Active Directory

Active Directory is the foundation of identity and access management in enterprise environments. It controls how users authenticate, what they can access, and how permissions are structured across an organisation.

In most Microsoft-based environments, Active Directory is the central system behind user management, security enforcement, and access control.

## Why a Domain Controller

Installing Active Directory alone does not create a functional identity system. Promoting the server to a Domain Controller allows it to:

- Authenticate users
- Enforce domain policies
- Manage user and computer accounts centrally
- Control access to resources within the domain

This is what transforms a standard server into an identity management system.

## Configuration Overview

| Setting | Value |
|---|---|
| Domain Name | PROJECT.LOCAL |
| NetBIOS Name | PROJECT |
| Forest Functional Level | Windows Server 2025 |
| Domain Functional Level | Windows Server 2025 |
| DNS Role | Enabled |
| Global Catalog | Enabled |

## Setup Steps

1. Installed Active Directory Domain Services role via Server Manager
2. Promoted the server to Domain Controller using AD DS Configuration Wizard
3. Created a new forest with root domain PROJECT.LOCAL
4. Configured DNS during domain controller promotion
5. Set Directory Services Restore Mode (DSRM) password
6. Completed installation and restarted the server
7. Verified Active Directory installation using Active Directory Users and Computers
8. Created an Organisational Unit named IT USERS under the domain
9. Created user accounts for simulated employees

## Why the IT USERS Organisational Unit

Organisational Units are used in enterprise environments to structure and manage identity objects.

Instead of placing users in default containers, a dedicated OU allows:

- Better organisation of accounts
- Easier policy management
- Scalable structure for departments such as HR, Finance, and IT

In this project, IT USERS represents the starting structure for a real enterprise-style environment.

## Users Created

| Name | Username | Department |
|---|---|---|
| Carol Johnson | carol.johnson | HR |
| Erik Larsson | erik.larsson | Unassigned |
| Maria Andersson | maria.andersson | Finance |
| Anna Lindqvist | anna.lindqvist | Operations |
| Bjorn Larsson | bjorn.larsson | Unassigned |

## Issues and Resolution

**Prerequisites Check Failure**

The initial attempt to promote the server to a Domain Controller failed due to a system state conflict. The issue was resolved by restarting the server and rerunning the promotion wizard.

**Organisational Unit Visibility**

The IT USERS OU was not immediately visible under the expected structure. Enabling advanced features in Active Directory Users and Computers confirmed correct placement within the domain hierarchy.

## Key Takeaway

Active Directory is the core of enterprise identity management. Every subsequent action in this project, including onboarding, access control, and authentication, depends on the structure created here.

Understanding Active Directory is essential for working in any Microsoft-based IT support environment.
