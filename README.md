## Nmap-Network-Scanning-and-Enumeration-Lab
## 1. Introduction
Nmap (Network Mapper) is an open-source tool used for network discovery and security auditing. It helps identify active hosts, open ports, running services, service versions, and operating systems.

This project demonstrates different Nmap scanning techniques using Kali Linux and Metasploitable 2 in a virtual lab environment. It includes Host Discovery, Port Scanning, Service and Version Detection, OS Detection, Vulnerability Scanning, and Aggressive Scanning.

The main purpose of this project is to gain practical knowledge of network scanning, understand exposed services, and learn basic security assessment techniques in an authorized environment.
## 2. Objectives

- To understand Nmap scanning techniques.
- To discover active hosts.
- To identify open ports.
- To detect services and versions.
- To identify the operating system.
- To perform vulnerability scanning.
- To analyze scan results.
 ## 3. Tools and Technologies Used
| **Tool** | **Purpose** |
|---|---|
| Kali Linux | Scanning Machine |
| Nmap | Network Scanning |
| Metasploitable 2 | Lab Target |
| VMware | Virtual Machine Environment |
| Terminal | Execute Commands |

## 4. Lab Setup and Target Identification

**Target IP Address**: 192.168.124.130 

**Command:**
ip addr

<img width="747" height="430" alt="Screenshot 2026-10-29 003513" src="https://github.com/user-attachments/assets/385f0711-91cd-44f5-a557-fb6d32a2ca49" />

## 5. Host Discovery Scan

**Command:**

nmap -sn 192.168.124.130

**Purpose:** To check whether the target host is active.

**Expected Result**
If the target is active, Nmap will show:

Host is up.

This confirms that the target machine is reachable and ready for further scanning.

<img width="667" height="176" alt="Screenshot 2026-10-29 005830" src="https://github.com/user-attachments/assets/a6af703f-0c13-4f2b-8805-bf2a380ad545" />

## 6. Port Scanning

**Command:**

nmap -p- 192.168.72.130

**Purpose**: To scan all TCP ports and identify open ports.

| **Port** | **Common Service** |
|---:|---|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 25 | SMTP |
| 80 | HTTP |
| 445 | SMB |
| 3306 | MySQL |









