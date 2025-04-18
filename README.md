# 🕵️ Kali Linux - Hands-on – Internship Task

This repository contains essential Linux commands, tool usage, and penetration testing steps documented as part of a Cybersecurity Internship at Future Interns. This task aimed to provide a hands-on foundation for command-line operations and practical cybersecurity assessments using Kali Linux.

---

## 📌 Task Overview

- **Intern Name:** Shezan Ahmad Khan
- **Internship Role:** Cybersecurity Intern  
- **Reporting Date:** April 18, 2025  
- **Task ID:** TASK 1 
- **Task Title:** Kali Linux - Hands-on – Internship Task
---

## 🎯 Objective

To understand and apply basic Linux commands, install Kali Linux tools, and perform reconnaissance and attacks on a vulnerable website using CLI-based techniques.

---

## 📂 Covered Topics

### 🔧 File & Directory Management

- ls           # List directory contents
- cd           # Change directory
- pwd          # Print working directory
- mkdir dir    # Create new directory
- rm file      # Delete a file

---

## 📄 File Handling

- cat file.txt            # Read file
- cp file1.txt file2.txt  # Copy file
- mv file1.txt newdir/    # Move file
- nano file.txt           # Edit file

---

## 🔐 Permissions & Ownership

- chmod +x script.sh      # Add execute permission
- chown user:user file    # Change file owner

---

## 🖥️ System & Process Info

- uname -a       # System info
- df -h          # Disk usage
- top            # Running processes

---

## 🌐 Networking Commands

- ifconfig       # Show network interfaces
- ping google.com # Ping test
- netstat -tulnp  # List open ports

---

## ⚙️ Package & Tool Installation

### 🔄 Update & Install Packages

- sudo apt update
- sudo apt install nmap sqlmap dirb

## 🛠️ Kali Tools from GitHub

### 🔎 XSStrike (XSS Detection Tool)

- git clone https://github.com/s0md3v/XSStrike.git
- cd XSStrike
- pip install -r requirements.txt
- python3 xsstrike.py

### 🛡️ Nikto (Web Vulnerability Scanner)

- git clone https://github.com/sullo/nikto.git
- cd nikto/program

---

## 🎯 Reconnaissance & Attack Execution

### 📍 Nmap Scan

- nmap -sV testphp.vulnweb.com

### 🧬 SQL Injection with sqlmap

- sqlmap -u "http://testphp.vulnweb.com/artists.php?artist=1" --dbs --batch

---

✅ **Findings**

- Vulnerable Parameter: artist (GET)
- Injection Types Detected:
    - Boolean-based
    - Error-based
    - Time-based
    - UNION-based
    - Backend DBMS: MySQL ≥ 5.6
    - Web Server: Nginx 1.19.0, PHP 5.6.40
    - Databases Found:
      - 1. acuart
      - 2. Information_schema

---

### 🔍 Directory Bruteforce with dirb

- dirb http://testphp.vulnweb.com/

---

## 📂 Discovered Resources

- /admin/ → Potential login page
- /CVS/ → Version control files
- /secured/, /vendor/ → Sensitive directories
- crossdomain.xml, index.php, favicon.icc

---

✅ **Key Takeaways**

- Mastery of essential Linux commands for real-world use
- Installed and used popular Kali Linux tools
- Hands-on recon & exploitation using command-line tools
- Practical understanding of web vulnerabilities

---

## 📌 Acknowledgment

Thanks to Future Interns for offering this hands-on cybersecurity learning journey. This task helped solidify my command-line skills and tool-based offensive security knowledge.
