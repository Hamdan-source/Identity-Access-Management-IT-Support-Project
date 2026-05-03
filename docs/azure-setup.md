# Azure VM Setup

## What This Document Covers

This document explains how I deployed a Windows Server 2025 virtual machine in Microsoft Azure and configured it as a Domain Controller for the PROJECT.LOCAL domain. It includes the decisions made during setup and how they reflect real enterprise infrastructure practices.

## Why Azure

Azure is widely used by Swedish organisations as their primary cloud platform. It supports compliance requirements such as GDPR, provides scalability, and integrates naturally with Microsoft 365 and Active Directory environments.

Working in Azure reflects how modern IT infrastructure is actually built and managed in enterprise environments.

## Why Windows Server 2025

Windows Server 2025 is the current server operating system in the Microsoft ecosystem. Using it ensures the environment reflects current enterprise standards for identity, authentication, and domain management.

## VM Configuration

| Setting | Value |
|---|---|
| VM Name | ProjectD1 |
| Region | Australia East |
| Availability Zone | Zone 1 |
| Image | Windows Server 2025 Datacenter Azure Edition Gen2 |
| Size | Standard D2s v3 (2 vCPUs, 8 GiB RAM) |
| Admin Username | projadmin |
| Inbound Port | RDP (3389) |
| Auto-shutdown | Midnight |
| Resource Group | ProjectD1 |

## Why Australia East

The free-tier subscription limited available VM sizes in some European regions. Australia East was the most stable option for deployment under these constraints.

In a production environment, Sweden Central would be the correct choice due to latency, compliance, and data residency requirements.

## Why Auto-Shutdown

Auto-shutdown was configured to control costs. Cloud resources run continuously unless managed, and cost awareness is a standard part of working in cloud environments.

## Why RDP (Port 3389)

RDP is the standard protocol for remote administration of Windows servers. Port 3389 was enabled to allow secure remote access during configuration. In production environments, this would typically be restricted through VPN or IP allowlisting.

## Deployment Steps

1. Created a dedicated resource group (ProjectD1)
2. Selected Azure region based on available compute resources
3. Deployed Windows Server 2025 Datacenter Edition
4. Chose Standard D2s v3 VM size for stability
5. Enabled RDP access for administration
6. Configured auto-shutdown for cost control
7. Deployed and connected using Microsoft Remote Desktop on Mac

## Issues and Resolution

**VM Size Availability**

Some regions restricted VM sizes due to subscription limitations. Changing regions resolved the deployment constraint.

**RDP Access on Mac**

Remote Desktop was not natively available on macOS. Microsoft Remote Desktop was installed and used for server access.

## Key Takeaway

Every configuration decision in this setup had a purpose. In cloud environments, understanding why a choice is made is as important as the configuration itself.
