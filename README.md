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

nmap -p- 192.168.124.130

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

These are common examples; actual results may differ

<img width="667" height="662" alt="Screenshot 2026-10-29 011156" src="https://github.com/user-attachments/assets/20f26f1d-04c5-49e3-9cbe-4ae18276b480" />

<img width="627" height="155" alt="Screenshot 2026-10-29 012423" src="https://github.com/user-attachments/assets/c5c65541-b142-4887-a3c1-ea3fff14829a" />

## 7. Service and Version Detection

**Command:**

nmap -sV 192.168.124.130

**Purpose:** To identify running services and their versions.

| **Option** | **Meaning** |
|---|---|
| `-sV` | Service and Version Detection |


<img width="1017" height="612" alt="Screenshot 2026-10-29 013104" src="https://github.com/user-attachments/assets/397c5b4a-d63d-4314-a9a8-548deb81096c" />


<img width="622" height="147" alt="Screenshot 2026-10-29 013306" src="https://github.com/user-attachments/assets/250a8239-6092-4b5f-858e-6d956943d217" />

## 8. Operating System Detection
**Command:**

nmap -O 192.168.124.130

**Purpose:** To estimate the target operating system.

<img width="732" height="661" alt="image" src="https://github.com/user-attachments/assets/d79862fa-5647-4b2a-af6f-343d67d50682" />

<img width="611" height="152" alt="image" src="https://github.com/user-attachments/assets/c718fc57-13df-41eb-ac9c-b03429d62946" />


## 9. Vulnerability Scanning Using NSE
**Command:**

nmap --script vuln 192.168.124.130

**Purpose:** To check for potential security vulnerabilities.


<img width="946" height="760" alt="image" src="https://github.com/user-attachments/assets/a3e5300e-c82b-442c-95ef-6f16f1fa7137" />

<img width="746" height="735" alt="image" src="https://github.com/user-attachments/assets/c4f0598a-caae-4c56-a435-91b7f7a5d618" />

<img width="777" height="786" alt="image" src="https://github.com/user-attachments/assets/e77180b1-2316-4087-a167-e233474716c4" />

<img width="1010" height="782" alt="image" src="https://github.com/user-attachments/assets/3a0ca8c7-79b1-4b9c-8b22-fe97fb1713eb" />

<img width="997" height="770" alt="image" src="https://github.com/user-attachments/assets/63108072-c38f-40a2-8807-1502a6903479" />


















