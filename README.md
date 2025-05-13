# Active-Directory-AD-Lab-Environment

## 🧪 Active Directory Lab Build

A step-by-step project to build a virtualized Active Directory (AD) lab for learning, testing, or cybersecurity training purposes. This project uses virtual machines (VMs) to simulate a Windows domain environment, including a Domain Controller, workstations, and optionally a Linux attacker box (e.g., Kali Linux).

## 🗂️ Lab Overview

This lab includes:

- **Domain Controller** (Windows Server 2022)
- **Windows Workstation(s)** (Windows 10)
- **Attacker VM** (Kali Linux)
- **Virtualization Platform:** VMware Workstation
- **Networking:** Internal NAT

## ⚙️ Requirements

- 16+ GB RAM (32 GB recommended)
- 100+ GB disk space
- VirtualBox / VMware / Proxmox
- Windows Server ISO (2019 or 2022)
- Windows 10/11 ISO
- Optional: Kali Linux ISO

## 🔧 Installation Steps

- Setting up the Domain Controller

- Create new Virtual machine
- Configuration - Typical(Recommended)

  ![image](https://github.com/user-attachments/assets/a4ccd351-aebb-46dc-ae52-b166c9e47ffd)

- Select the drive

  ![image](https://github.com/user-attachments/assets/336d17fb-e0eb-4975-bf9d-d3752cc15599)

- Select split virtual disk into multiple files
- Finish
- Edit this virtual machine
- Increase ram from 2gb to 4/8gb
  
  ![image](https://github.com/user-attachments/assets/8d668cfe-742a-4001-adf9-f1bf136c075f)

- Power on
- windows server setup

  ![image](https://github.com/user-attachments/assets/27f6cbfb-2175-45f5-af7c-03dc39720087)

- Select Standard Evaluation (Desktop Experience)

  ![image](https://github.com/user-attachments/assets/03bcc4fd-1f93-4769-a656-768e42878b91)

- Parition and Install the operating system
- Set Password for the Admin account

  ![image](https://github.com/user-attachments/assets/6abdaea3-a13a-4bfa-89f7-1350d7c8c2b3)

- Login
- In Server Manager, Manage > Add roles and Features

  ![image](https://github.com/user-attachments/assets/7785f95b-a654-4d9c-8b84-a38a3993ccd2)

- Role based installation

  ![image](https://github.com/user-attachments/assets/a83a0468-a24c-43f1-affc-3923ad058723)

- Add Actice directory domain services

  ![image](https://github.com/user-attachments/assets/e9f2b040-6c08-4752-9d08-d1a44c672b44)

- Install
- Promote this server to Domain Controller
- Add new forest

![image](https://github.com/user-attachments/assets/42d70761-3ee9-438b-9f35-28cf297c58f3)

- Add your password

  ![image](https://github.com/user-attachments/assets/441de5f2-7d2c-4192-981b-35b420d89bdd)

- NetBIOS Name

  ![image](https://github.com/user-attachments/assets/1ab35b00-ef70-4fcf-9620-2ac727b495f8)

- Install Restart and Login
- Server Manager > Manage > Add roles and features
- Add Active Directory Cerificate Services
- Make sure the Certificate Authority is checked
- Install
- Configure Active Directory Certificate Services

  ![image](https://github.com/user-attachments/assets/8af4fd1d-06e6-4df3-b2e9-48d7dcebab1d)

- Rest stays default
- Restart thr server

- Domain Controller Setup is now completed 

- Install the other workstations
- Setup Users, Groups and Policies
- Join user machines to the domain

Active Directory (AD) lab environment is ready to use.


