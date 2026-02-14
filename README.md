# IT Help Desk & Active Directory Project
## 🎫 osTicket + Active Directory (Hybrid IT Support Lab)

---

## 📌 Overview

This project simulates a real-world enterprise IT Help Desk environment using:

- Windows Server (Active Directory Domain Services)
- Windows 11 Domain-Joined Client
- Ubuntu Linux (osTicket Help Desk System)
- UTM Virtualization (Apple Silicon)

The lab demonstrates structured Tier 1 / Tier 2 IT support workflows including:

- Account lockouts and password resets
- Group-based access control (RBAC)
- Domain join troubleshooting
- DNS resolution failures
- RDP configuration
- User deprovisioning
- Security-related investigations

This environment mirrors common support operations in corporate IT departments and managed service providers (MSPs).

---

## 🏗 Lab Architecture

The lab environment consists of:

Windows Server (Domain Controller)
- Active Directory Domain Services (AD DS)
- DNS Server
- Group Policy Management

Windows 11 Client
- Domain-joined workstation
- Simulated end-user environment

Ubuntu Linux Server
- Apache
- PHP
- MariaDB
- osTicket (Ticketing platform)

All systems operate within a NAT-based virtual network inside UTM.

---

## 🛠 Environment Details

Host System
- macOS (Apple Silicon – M3)
- UTM (QEMU ARM64 Virtualization)

Resource Allocation
- Windows Server: 4–6 GB RAM
- Windows Client: 4 GB RAM
- Ubuntu Server: 4–6 GB RAM
- Disk: 20–60 GB per VM
- Network Mode: NAT (Internal Lab Network)

---

## 🧠 Active Directory Configuration

- Installed and configured Active Directory Domain Services
- Created:
  - Users
  - Security Groups
  - Organizational Units (OUs)
- Implemented Group Policy Objects (GPOs)
- Configured account lockout policies
- Simulated:
  - Account lockouts
  - Password resets
  - Group membership access changes
  - Domain join failures
  - RDP access permissions
- Applied Least Privilege and Role-Based Access Control (RBAC) principles

---

## 🎫 Ticketing System (osTicket)

Deployed osTicket on Ubuntu to simulate structured help desk workflows.

Configuration Performed
- Created departments (IT Support, Security)
- Defined agent roles and permissions
- Configured ticket priorities and SLAs
- Implemented escalation workflows
- Customized notification templates

---

## 🧪 Example Tickets Handled

Active Directory
- User account locked out
- Password reset requests
- Security group access provisioning
- User deprovisioning

Networking
- DNS resolution failure
- Domain join troubleshooting
- RDP access issues

Security
- Suspicious login investigation
- Privilege escalation review

Each ticket included:
- Issue description
- Impact assessment
- Step-by-step troubleshooting
- Root cause identification
- Resolution documentation
- Closure summary

---

## 🔑 Core Competencies Demonstrated

- Active Directory Administration
- Group Policy Management
- RBAC Implementation
- Tier 1 / Tier 2 Troubleshooting
- Domain Authentication & DNS Diagnostics
- Linux Server Deployment (LAMP)
- Ticket Lifecycle Documentation
- Security Awareness & Incident Triage

---

## 📁 Project Structure

screenshots/
│
├── 00-setup/
├── 01-active-directory/
├── 02-ticketing/
└── 03-scenarios/

tickets/
│
└── README.md

Each folder documents a specific stage of infrastructure deployment and support workflows.

---

## 🎥 Project Walkthrough

3-minute lab demonstration includes:

- Ticket #001 – Account Lockout Resolution
- Ticket #003 – Group-Based Access Provisioning

(Video link coming soon)

---

## 📈 Key Takeaways

- Structured troubleshooting reduces resolution time.
- DNS misconfiguration is a common root cause in domain environments.
- Group-based access control simplifies permission management.
- Proper documentation improves escalation and auditing workflows.

---

## 🎯 Career Relevance

This project aligns with responsibilities in roles such as:

- Help Desk Technician
- IT Support Specialist
- Service Desk Analyst
- Desktop Support Technician
- Junior Systems Administrator
- SOC Analyst (Entry-Level)

It demonstrates hands-on experience with:

- Active Directory environments
- Ticket-based IT operations
- Hybrid infrastructure troubleshooting
- Identity and access management
