# Task 4 – Firewall Configuration with UFW

## 📌 Objective
The goal of this task was to configure and manage firewall rules using **UFW (Uncomplicated Firewall)** on Kali Linux.  
We implemented security best practices by **allowing only required ports** and **blocking insecure services** like Telnet (port 23).

---

## 🔹 What is UFW?
**UFW** is a user-friendly command-line interface for managing firewall rules in Linux.  
It is a front-end for **iptables** and allows simple configuration of incoming and outgoing network traffic rules.

---

## 🛠 Steps Performed

### 1️⃣ Enable UFW
     ```bash
     sudo ufw enable

### 2️⃣ Check Current Rules
     ```bash
     sudo ufw status verbose
     
### 3️⃣ Block Telnet (Port 23)
     ```bash
     sudo ufw deny 23
### 4️⃣ Verify Rule Added
     ```bash
     sudo ufw status verbose
### 5️⃣ Test Connection Block
     ```bash
     telnet localhost 23
### 6️⃣ Remove the Deny Rule
     ```bash
     sudo ufw delete deny 23
### 7️⃣ Export Firewall Rules
     ```bash
     sudo ufw status numbered > firewall_rules.txt

     
✅ Outcome

By completing this task:

1. UFW was successfully enabled and configured.

2. Insecure Telnet access was blocked.

3. The rules were tested, documented, and exported.

4. Demonstrated basic Linux firewall management skills.
