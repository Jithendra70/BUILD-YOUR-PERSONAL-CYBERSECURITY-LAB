# BUILD-YOUR-PERSONAL-CYBERSECURITY-LAB
You can use this **GitHub README.md** content for your Task-2 repository:

````markdown
# Build Your Personal Cybersecurity Lab

## Overview
This project demonstrates the creation of a safe and isolated cybersecurity lab environment using virtualization technology. The lab is designed for learning penetration testing, vulnerability assessment, web application security testing, and network traffic analysis without affecting real-world systems.

## Objective
The objective of this project is to build a personal cybersecurity lab that provides hands-on experience with:

- Virtualization
- Network configuration
- Vulnerability assessment
- Traffic analysis
- Web application security testing

## Lab Architecture

Host System (Windows 11)
│
├── Kali Linux VM (Attacker Machine)
│
├── NAT Adapter (Internet Access)
│
├── Host-Only Adapter (Lab Communication)
│
└── OWASP Juice Shop (Vulnerable Target)

## Technologies Used

| Tool | Purpose |
|--------|---------|
| Oracle VirtualBox / VMware | Virtualization Platform |
| Kali Linux | Attacker Machine |
| Docker | Container Platform |
| OWASP Juice Shop | Vulnerable Web Application |
| Nmap | Network Scanning |
| Wireshark | Packet Analysis |
| Burp Suite | Web Security Testing |

## System Requirements

- RAM: 8 GB Minimum
- Storage: 40 GB Free Space
- Operating System: Windows 11
- Internet Connection

## Implementation Steps

### Step 1: Setup Virtualization Environment
- Installed Oracle VirtualBox / VMware
- Configured virtual networking

### Step 2: Configure Kali Linux
- Imported Kali Linux virtual machine
- Configured:
  - Adapter 1 → NAT
  - Adapter 2 → Host-Only

### Step 3: Update Kali Linux

```bash
sudo apt update
sudo apt upgrade -y
````

### Step 4: Install Docker

```bash
sudo apt install docker.io -y
sudo systemctl start docker
```

### Step 5: Deploy OWASP Juice Shop

```bash
sudo docker run -d -p 3000:3000 bkimminich/juice-shop
```

Access Application:

```text
http://localhost:3000
```

### Step 6: Network Scanning using Nmap

```bash
nmap -sV localhost
```

### Step 7: Traffic Analysis using Wireshark

* Captured network packets
* Analyzed HTTP traffic
* Verified network communication

### Step 8: Web Application Testing using Burp Suite

* Configured browser proxy
* Intercepted HTTP requests
* Analyzed web traffic

## Results

* Successfully created an isolated cybersecurity lab.
* Deployed OWASP Juice Shop using Docker.
* Performed network scanning using Nmap.
* Captured and analyzed packets using Wireshark.
* Intercepted web requests using Burp Suite.

## Screenshots

* Virtual Machine Setup
* Kali Linux Environment
* Network Configuration
* Docker Container Status
* OWASP Juice Shop Homepage
* Nmap Scan Results
* Wireshark Packet Capture
* Burp Suite Interception

## Learning Outcomes

* Understanding of virtualization concepts
* NAT and Host-Only networking
* Vulnerable application deployment
* Network reconnaissance
* Packet analysis
* Web application security testing

## References

* Kali Linux Documentation
* OWASP Juice Shop Documentation
* Docker Documentation
* Nmap Documentation
* Wireshark Documentation
* Burp Suite Documentation

## Author

**Bhavirisetti Jithendra Manideep**

Cybersecurity Internship – Maincrafts Technology

