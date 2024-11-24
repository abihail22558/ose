


# Tasks for Basic Network Analysis

## Overview
This guide outlines the steps to perform a **basic network analysis** using the **Nmap** tool. The tasks include identifying active hosts, listing open ports and services, and detecting the operating systems on network devices.

---

## Prerequisites
1. Install **Nmap** on your local machine.
2. Open a terminal or command prompt.
3. Determine the IP address and subnet of your computer.

---

## Tasks

### Task 1: Perform a Basic Network Scan
1. **Find the IP Address and Subnet**:
   - Run the following command to get the IP address and subnet of the host computer:
     ```bash
     ipconfig
     ```
     ![image](https://github.com/user-attachments/assets/82675d65-5eff-4d15-b37e-43a5e72b6e2f)


2. **Scan the Network**:
   - Use the following command to perform a basic scan of the network:
     ```bash
     nmap [HostIPAddress/NetworkRange]
     ```
   - Example:
     ```bash
     nmap 192.168.1.0/24
     ```

---

### Task 2: Identify Active Hosts
To discover all active hosts on the network:
- Run the following command:
  ```bash
  nmap -sn [HostIPAddress/NetworkRange]
  ```
- Replace `[HostIPAddress/NetworkRange]` with the actual IP address and range.
- Example:
  ```bash
  nmap -sn 192.168.1.0/24
  ```

---

### Task 3: List Open Ports and Running Services
To detect open ports and services on each host:
- Run the following command:
  ```bash
  nmap -sV [HostIPAddress/NetworkRange]
  ```
- Replace `[HostIPAddress/NetworkRange]` with the actual IP address and range.
- Example:
  ```bash
  nmap -sV 192.168.1.0/24
  ```

---

### Task 4: Detect Operating Systems
To identify the operating system of each device on the network:
- Run the following command:
  ```bash
  nmap -O [HostIPAddress/NetworkRange]
  ```
- Replace `[HostIPAddress/NetworkRange]` with the actual IP address and range.
- Example:
  ```bash
  nmap -O 192.168.1.0/24
  ```

---

## Tools Used
- **Nmap**: Open-source tool for network discovery and security scanning.

---

## Notes
- Ensure that you have permission to scan the network.
- Use this guide within a controlled environment or for authorized professional purposes.

---

## Disclaimer
This guide is for educational purposes only. Unauthorized use of Nmap on networks without permission is illegal and can lead to severe consequences under applicable laws.
