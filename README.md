# Active Directory Lab in Azure
## Overview
This project demonstrates the setup and configuration of an Active Directory environment hosted on a Microsoft Azure Virtual Machine.
The lab simulates a basic enterprise environment by deploying a Windows Server VM, promoting it to a Domain Controller, and organizing directory objects using Organizational Units (OUs).

## Technologies Used
- Microsoft Azure (virtual machines)
- Windows Server 2025
- Active Directory Services (AD DS)

## Step 1: Creating the Azure Virtual Machine
I created a Windows Server VM in Azure to host the Active Directory environment.
### Key Configuration
- OS: Windows Server 2025 Datacenter (Azure Edition)
- Size: Standard E2s v3 (2 vCPUs, 16 GiB RAM)
- Region: East US

This VM acts as the domain controller for the lab environment

![VM info](/imgs/VM_info.jpeg)
![Resource Group](/imgs/resource_group.jpeg)

## Step 2: Installing Active Directory Domain Services
After connecting the VM, I installed the Active Directory Domain Services role using Server Manager.

![Server Services](/imgs/server_groups.jpeg)

## Step 3: Promoting to Domain Controller
The server was promoted to a domain controller and a new domain was created:
- Domain Name: lab.local

## Step 4: Creating Organizational Units (OUs)
To simulate a structured enviornment, I created a Branch OU and organized it into sub-OUs:
- Branch 1
  - Users
  - Computers
  - Groups

![AD Structure](/imgs/AD.jpeg)

## Step 5: Creating a User
A test user account was created within the Users OU to simulate user management.

![AD New User](/imgs/AD_user.jpeg)