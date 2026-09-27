# Network-Reconnaissance-Traffic-Analysis-using-Nmap-and-Wireshark

## 📌 Project Title

**Network Reconnaissance, Port Scanning & Traffic Analysis using Nmap and Wireshark

- **Project Type:** Network Security & Network Analysis
- **Environment:r** Authorized Virtual Lab Environment

---

## 📖 Introduction

This project demonstrates practical network reconnaissance, port scanning, service enumeration, and network traffic analysis using **Nmap** and **Wireshark** in an authorized virtual laboratory environment.

Nmap is an open-source network scanning tool used to discover hosts, identify open ports, detect running services, and perform operating system detection.

Wireshark is an open-source network protocol analyzer used to capture and inspect network packets and understand communication between systems.

The project combines both tools to provide practical experience in network enumeration and packet-level traffic analysis.

---

## 🎯 Project Objectives

- Understand network reconnaissance techniques
- Perform host and port discovery
- Identify running network services
- Perform TCP and UDP scanning
- Detect operating system information
- Analyze network traffic using Wireshark
- Understand TCP three-way handshake
- Analyze DNS, HTTP, HTTPS/TLS, ICMP, and UDP traffic
- Learn basic network security assessment techniques
- Develop practical cybersecurity and SOC analyst skills

---

## 🛠️ Tools and Environment

| Tool / Platform | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| Nmap | Network reconnaissance and port scanning |
| Wireshark | Packet capture and traffic analysis |
| VirtualBox | Virtual lab environment |
| Ubuntu / Metasploitable | Authorized target VM |
| Web Browser | Generate network traffic |
| Terminal | Network testing |

---

## 🏗️ Lab Architecture

```text
+-------------------------+
|       Kali Linux        |
|   Nmap + Wireshark      |
+------------+------------+
             |
             | Virtual Lab Network
             |
             v
+-------------------------+
| Ubuntu / Metasploitable |
|       Target VM         |
+-------------------------+
