# 🔴 Week 04: Lateral Movement & SMB Internal Network Attacks

## 📌 Overview
This project demonstrates how attackers exploit the SMB (Server Message Block) protocol to perform internal network attacks and lateral movement. It includes SMB enumeration, accessing shared resources, traffic analysis, and credential reuse within a controlled lab environment.

---

## 🎯 Objectives
- Understand SMB protocol weaknesses
- Perform SMB enumeration using different tools
- Access shared folders and extract sensitive data
- Analyze SMB traffic using Wireshark
- Simulate lateral movement using discovered credentials

---

## 🛠️ Tools Used
- Kali Linux
- Nmap
- smbclient
- Wireshark
- Windows (Victim Machine)

---

## 🌐 Lab Setup
- **Attacker Machine:** Kali Linux  
- **Victim Machine:** Windows  
- **Network Type:** NAT (Same Network)

---

## 🔍 Task 01: SMB Enumeration & Exploitation

### 1️⃣ SMB Port Scanning
```bash
nmap -p 139,445 -sV 192.168.88.129
