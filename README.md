# ⚡ REVIEW TECHNICAL CASE STUDIES

[![OPEN INTERACTIVE PORTFOLIO](https://img.shields.io/badge/OPEN_INTERACTIVE_PORTFOLIO-0047AB?style=for-the-badge&logo=microsoft-azure&logoColor=white)](https://hamdan-source.github.io/Identity-Access-Management-IT-Support-Project/)

> This portfolio shows practical examples of IT support, identity management, security auditing, and automation in a Microsoft environment.

---

# Identity and Access Management - IT Support Project

This project shows how I approach IT support: understand the issue, investigate properly, and resolve it with business impact in mind.

## Start Here

1. **Overview** — what the project is about.
2. **Tech Stack** — the tools and systems used.
3. **Incidents Handled** — the main case studies.
4. **Environment Setup** — how the lab was built.
5. **Support Approach** — how each ticket was handled.

## Overview

This project documents how IT support work is handled in practice, from the moment a user reports an issue through to resolution and follow-up.

The focus is not only on fixing the technical issue, but also on understanding what the issue means for the user and for the business.

## Tech Stack

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud virtual machine hosting |
| Windows Server 2025 | Server operating system and domain controller |
| Active Directory | Identity and access management |
| Microsoft Entra ID | Cloud identity, MFA, and hybrid authentication |
| Intune | Mobile Device Management (MDM) and endpoint compliance |
| ServiceNow | Incident tracking and service desk workflow |
| PowerShell | Identity automation and administrative scripting |
| Git & GitHub | Documentation and version control |
| RDP | Remote administration of server environment |

## Repository Structure

```text
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
│       ├── INC0010006.md
│       ├── INC0010007.md
│       └── INC0010008.md
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

**Microsoft Intune** was configured as the Mobile Device Management solution, used to enrol devices, apply compliance policies, and push software update policies to managed endpoints.

This environment allowed investigation and troubleshooting of identity and access issues in a structured way, mirroring how they would be handled within a real IT operations team.

![Azure VM setup](https://github.com/user-attachments/assets/3b9b975f-4b51-4ff3-a695-c5903f90d30c)

*Azure VM deployed as the foundation of the lab environment*

## Incidents Handled

| Ticket | User | Issue | Priority | Outcome |
|---|---|---|---|---|
| INC0010001 | Carol Johnson | HR account access blocked during payroll cycle | Critical | Resolved within SLA after investigation |
| INC0010002 | Erik Larsson | New employee unable to access system on first day | Moderate | Account created and verified |
| INC0010003 | Maria Andersson | No access to Finance applications | Moderate | Correct security group assigned |
| INC0010004 | Anna Lindqvist | Employee offboarding and access removal | Moderate | Account disabled following process |
| INC0010005 | Bjorn Larsson | MFA device lost and account lockout | Moderate | MFA reset through Entra ID |
| INC0010006 | Jonas Eriksson | New employee device onboarding and Intune MDM compliance | Moderate | Device enrolled, compliance and update policy applied |
| INC0010007 | Internal Security Review | Ghost Identity Audit and shadow admin account discovery | High | Shadow admin disabled after Event ID 4624 verification |
| INC0010008 | Internal Process Improvement | Automated onboarding pipeline with PowerShell | Moderate | AD account creation, group assignment, password policy, and audit trail automated |

## ServiceNow Tracking

This screenshot shows the incident workflow and ticket tracking used across the project.

![ServiceNow ticket tracking](https://raw.githubusercontent.com/Hamdan-source/Identity-Access-Management-IT-Support-Project/main/screenshots/tickets/Ticket_List.png)

*All incidents tracked and resolved in ServiceNow*

## Highlighted Case Studies

### INC0010001 - Payroll Access Incident

This case shows how a simple account issue became a critical support problem because it affected payroll processing.

### INC0010007 - Ghost Identity Audit

This case shows proactive identity auditing. A shadow admin account was discovered through Event Viewer analysis and then mitigated.

![INC0010007 Event Viewer evidence](https://raw.githubusercontent.com/Hamdan-source/Identity-Access-Management-IT-Support-Project/main/screenshots/tickets/INC0010007_Forensics.png)

### INC0010008 - Automated Onboarding Pipeline

This case shows how PowerShell was used to automate onboarding steps and reduce manual work.

## Support Approach

Each ticket follows the same structured flow:

1. Understand before acting.
2. Assess urgency.
3. Investigate root cause.
4. Resolve carefully.
5. Communicate throughout.
6. Confirm before closing.

A locked account is not just a technical issue when it affects payroll, onboarding, or compliance processes.

## What This Project Demonstrates

Working through Active Directory, Entra ID, Azure, Intune, and ServiceNow required understanding how identity systems connect and how access issues can occur across them.

The combination of technical execution, identity auditing, and automation under pressure is what this project is designed to show.

## Foundation Knowledge

Alongside this project, I studied Linux and networking fundamentals to support my understanding of how systems behave behind the tools.

This includes Linux system structure, SSH, DNS, TCP and UDP, subnetting, VPN concepts, and basic cloud networking principles.

## Conclusion

This project represents how I approach IT support work. I focus on understanding the issue first, investigating it properly, and resolving it in a way that considers both the technical system and the person affected.

If this approach aligns with what your team is looking for, I would welcome the opportunity to speak further.

Hamdan  
[Hamdan.suleiman@hotmail.com](mailto:Hamdan.suleiman@hotmail.com)
