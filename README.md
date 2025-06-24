# Internship-Task
---
Task 1:

Project Title: Local Network Scanning Using Nmap on Kali Linux**

This project focuses on scanning a local network using *Nmap* to identify live devices, open ports, and running services. It's aimed at *beginners in cybersecurity* who are learning the basics of *ethical hacking, **penetration testing, and **network enumeration*. Scan results are saved in a file for review and analysis, helping users understand potential vulnerabilities in their network.

---

### 🧭 *Step-by-Step Process*

*⿡ Install Nmap*
First, install Nmap on Kali Linux by running:

bash
sudo apt update && sudo apt install nmap


*⿢ Identify Your IP Range*
Find your local IP address and subnet using:

bash
ip a
hostname -I


➡ Example: If your IP is 192.168.1.10/24, scan the network range 192.168.1.0/24.

*⿣ Run a TCP SYN (Stealth) Scan*
Use Nmap to perform a stealth scan:

bash
nmap -sS 192.168.1.0/24


This reveals active hosts and their open TCP ports.

*⿤ Record Discovered Hosts & Ports*
Document the IP addresses of live systems and their open ports.

*⿥ (Optional) Monitor with Wireshark*
Capture live network traffic with *Wireshark* while scanning to observe packet flow and behavior.

*⿦ Understand the Services*
Research the services running on open ports (e.g., port 22 = SSH, port 80 = HTTP) to understand their roles.

*⿧ Assess Potential Risks*
Analyze which open ports or services might be vulnerable due to weak configurations or outdated software.

*⿨ Save Your Scan Output*
Store scan results in a text file for later reference:

bash
nmap -sS 192.168.1.0/24 -oN scan.txt


You can also use -oX (XML) or -oA (all formats) for other export options.

---

### 🛠 *Tools Utilized*

* *Kali Linux*
* *Nmap*
* *Wireshark* (optional)

---

### 🎯 *Learning Goals*

By completing this project, you will gain hands-on experience in:

* Scanning and mapping local networks
* Detecting active devices and open ports
* Interpreting service and port data
* Identifying basic security concerns
* Documenting scan results for analysis

---
