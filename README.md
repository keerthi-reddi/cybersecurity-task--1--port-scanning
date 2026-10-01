# Network Reconnaissance & Port Scanning (Task 1)
## Overview
This repository contains network reconnaissance and port scanning analysis conducted for Task 1 of the Cybersecurity Internship at Elevate Labs.
## Objective
* Discover live hosts on the local network subnet.
* Scan open network ports using TCP SYN Stealth Scanning (`-sS`).
* Document findings and evaluate potential security risks.
## Tools Used
* **Nmap:** Network discovery and stealth SYN scanning
* **Wireshark:** Network packet capture and protocol analysis
## Command Executed
nmap -sS 192.168.43.0/24 -oN scan_results.txt
tcp.flags.syn == 1

Summary of Findings
Target Subnet: 192.168.43.0/24
Target Host Identified: 192.168.43.1
Discovered Open Ports & Services:
Port Number	state	service	description
135/TCP	open	msrpc	Microsoft Windows RPC Endpoint Mapper
139/TCP	open	netbios-ssn	NetBIOS Session Service
445/TCP	open	microsoft-ds	SMB (Server Message Block) File Sharing
902/TCP	open	iss-realsecure	VMware Authentication Daemon
