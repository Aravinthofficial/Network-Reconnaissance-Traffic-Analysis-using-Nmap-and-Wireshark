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
 Installation Procedure

### Install Wireshark in Ubuntu/Kali Linux

```bash
sudo apt update
sudo apt install wireshark -y
```

### Verify Installation

```bash
wireshark --version
```

---

## 🚀 Project Implementation

### Step 1: Open Wireshark

Launch Wireshark application.

```bash
wireshark
```

---

### Step 2: Select Network Interface

Choose active interface:

- `eth0` → Ethernet
- `wlan0` → WiFi
- `lo` → Loopback

Click **Start Capturing Packets**.

---

### Step 3: Generate Network Traffic

Perform activities:

- Open Google
- Visit websites
- Watch YouTube
- Ping domains
- Download files

Example:

```bash
ping google.com
```

---

## 🔍 Protocol Analysis

### 1. DNS Analysis

#### Purpose
DNS converts domain names into IP addresses.

#### Filter

```text
dns
```

#### Observation

- Query Request
- DNS Response
- Resolved IP Address

Example:

```text
google.com → 142.xx.xx.xx
```

---

### 2. TCP Analysis

#### Purpose
TCP ensures reliable communication.

#### Filter

```text
tcp
```

### TCP 3-Way Handshake

```text
SYN
SYN ACK
ACK
```

#### Analysis

- Source Port
- Destination Port
- Session Establishment

---

### 3. HTTP Analysis

#### Purpose
HTTP transfers website data.

#### Filter

```text
http
```

#### Observation

- GET Request
- POST Request
- HTTP Response Code
- Website Host

---

### 4. HTTPS / TLS Analysis

#### Purpose
Secure encrypted communication.

#### Filter

```text
tls
```

#### Observation

- TLS Handshake
- Certificate Information
- Secure Traffic

---

### 5. ICMP Analysis

#### Purpose
Connectivity testing.

#### Generate Traffic

```bash
ping google.com
```

#### Filter

```text
icmp
```

#### Observation

- Echo Request
- Echo Reply

---

### 6. UDP Analysis

#### Purpose
Connectionless communication.

#### Filter

```text
udp
```

#### Observation

- DNS Traffic
- Streaming Packets

---

## 🎯 Important Wireshark Filters

### DNS

```text
dns
```

### TCP

```text
tcp
```

### UDP

```text
udp
```

### HTTP

```text
http
```

### HTTPS/TLS

```text
tls
```

### ICMP

```text
icmp
```

### Specific IP

```text
ip.addr == 192.168.1.1
```

### Specific Port

```text
tcp.port == 80
```

---

## 📊 Observations

During packet analysis, the following information was identified:

- Source IP Address
- Destination IP Address
- Packet Size
- Protocol Type
- Communication Flow
- Request and Response Packets

---

## ⚠️ Challenges Faced

- Large number of packets
- Packet filtering difficulty
- Understanding TCP handshake
- HTTPS encrypted traffic visibility

---

## ✅ Results

Successfully captured and analyzed:

- DNS packets
- TCP communication
- HTTP traffic
- HTTPS encrypted traffic
- ICMP packets
- UDP traffic

