# ⚡ ACTION REQUIRED: REVIEW TECHNICAL CASE STUDIES

### Klicka på knappen nedan för att verifiera min kompetens inom IAM, ServiceNow och Active Directory genom en interaktiv simulering.

[![KLICKA HÄR FÖR ATT STARTA](https://img.shields.io/badge/ÖPPNA_INTERAKTIV_PORTFOLIO-0047AB?style=for-the-badge&logo=microsoft-azure&logoColor=white)](https://hamdan-source.github.io/Identity-Access-Management-IT-Support-Project/)

---

> **NOTERA:** Denna miljö visar konkreta lösningar på P1-incidenter och infrastruktur-konfigurationer som är relevanta för din rekrytering.




# Identity and Access Management -IT Support Project

There is a difference between resolving a technical issue and understanding what that issue means for the person affected.

## Overview

This project documents how IT support work is handled in practice from the moment a user reports an issue through to resolution and follow-up.

When Carol Johnson contacted the service desk at 8am unable to access her workstation, the technical fix was straightforward. But Carol works in HR, and payroll processing was about to begin. That changed the priority completely.

The issue was no longer just about restoring access. It was about understanding the impact on business operations, acting quickly, and communicating clearly and that approach is what this project is built around.

## Tech Stack

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud virtual machine hosting |
| Windows Server 2025 | Server operating system and domain controller |
| Active Directory | Identity and access management |
| Microsoft Entra ID | Cloud identity, MFA, and hybrid authentication |
| Intune | Mobile Device Management (MDM) and endpoint compliance|
| ServiceNow | Incident tracking and service desk workflow |
| Git & GitHub | Documentation and version control |
| RDP | Remote administration of server environment |


## Repository Structure
```
IAM-IT-Support-Project/
│
├── README.md
├── docs/
│   ├── azure-setup.md
│   ├── active-directory-setup.md
│   ├── entra-id-setup.md
│   ├── IntuneSetup.md
│   └── tickets/
│       ├── INC0010001.md
│       ├── INC0010002.md
│       ├── INC0010003.md
│       ├── INC0010004.md
│       ├── INC0010005.md
│       └── INC0010006.md
│
└── screenshots/
    ├── azure/
    ├── active-directory/
    ├── entra-id/
    ├── intune/
    └── tickets/
```
## Environment Setup

A Windows Server 2025 virtual machine was deployed in Microsoft Azure and configured as a Domain Controller for the `PROJECT.LOCAL` domain.

**Active Directory** was used to manage users, groups, and access control across the environment.

**Microsoft Entra ID** was integrated to simulate hybrid identity, including MFA and cloud authentication scenarios.

**Microsoft Intune** was configured as the Mobile Device Management solution, used to enrol devices, apply compliance policies and push software update policies to managed endpoints.

This environment allowed investigation and troubleshooting of identity and access issues in a structured way, mirroring how they would be handled within a real IT operations team.

<img width="795" height="465" alt="azure-vm-deployment-complete" src="https://github.com/user-attachments/assets/3b9b975f-4b51-4ff3-a695-c5903f90d30c" />

*Azure VM deployed as the foundation of the lab environment*

## Incidents Handled

| Ticket | User | Issue | Priority | Outcome |
|---|---|---|---|---|
| INC0010001 | Carol Johnson | HR account access blocked during payroll cycle | 🔴 Critical | Resolved within SLA after investigation |
| INC0010002 | Erik Larsson | New employee unable to access system on first day | 🟡 Moderate | Account created and verified |
| INC0010003 | Maria Andersson | No access to Finance applications | 🟡 Moderate | Correct security group assigned |
| INC0010004 | Anna Lindqvist | Employee offboarding and access removal | 🟡 Moderate | Account disabled following process |
| INC0010005 | Bjorn Larsson | MFA device lost and account lockout | 🟡 Moderate | MFA reset through Entra ID |
| INC0010006 | Jonas Eriksson | New employee device onboarding and Intune MDM compliance | 🟡 Moderate | Device enrolled, compliance and update policy applied |

&nbsp;

<img width="1187" height="703" alt="Ticket List" src="https://github.com/user-attachments/assets/dceecd26-a99d-4fc5-912c-14349348b0bd" />

*All incidents tracked and resolved in ServiceNow*

## Support Approach

Each ticket follows the same structured flow:

1. **Understand before acting** — Identify what is actually happening and what the impact is
2. **Assess urgency** — Determine priority based on who is affected and what processes are impacted
3. **Investigate** — Identify the root cause before applying any fix
4. **Resolve carefully** — Apply the fix in a controlled way to avoid creating additional issues
5. **Communicate throughout** — Keep the user informed at every stage
6. **Confirm before closing** — The ticket is only closed once the user confirms resolution

A locked account is not just a technical issue when it affects payroll, onboarding, or compliance processes.

## What This Project Demonstrates

Working through Active Directory, Entra ID, Azure, Intune, and ServiceNow required understanding how identity systems connect and how access issues can occur across them.

Each incident required investigation, troubleshooting, and careful resolution to avoid impacting other users or systems.

Working with Intune added an endpoint management dimension — ensuring devices meet security compliance before users can access company resources.

At the same time, each ticket required communication, prioritisation, and awareness of business impact.

The combination of technical execution and decision-making under pressure is what this project is designed to show.

## Foundation Knowledge

Alongside this project, I studied Linux and networking fundamentals to support my understanding of how systems behave behind the tools.

This includes Linux system structure, SSH, DNS, TCP and UDP, subnetting, VPN concepts, and basic cloud networking principles. This knowledge supports troubleshooting and helps connect what happens at the application level with what is happening at the network and system level.

## Conclusion

This project represents how I approach IT support work. I focus on understanding the issue first, investigating it properly, and resolving it in a way that considers both the technical system and the person affected.

If this approach aligns with what your team is looking for, I would welcome the opportunity to speak further.

Hamdan

Hamdan.suleiman@hotmail.com
