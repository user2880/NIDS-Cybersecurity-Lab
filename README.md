# NIDS-Cybersecurity-Lab

Overview
This project demonstrates the setup of a Network Intrusion Detection System (NIDS) using Security Onion in a virtualized environment. The lab setup includes VMware Workstation Pro, Security Onion, Kali Linux, and Metasploitable. The goal is to simulate various cyber-attacks and monitor them using Security Onion to detect and analyze the threats.

Prerequisites

VMware Workstation Pro: Virtualization platform used for running virtual machines.
Security Onion: A free and open-source Linux distribution for intrusion detection, network security monitoring, and log management.
Kali Linux: A Debian-based Linux distribution used for penetration testing and ethical hacking.
Metasploitable: A deliberately vulnerable virtual machine used to test security tools and demonstrate vulnerabilities.

Lab Setup

1. Setting Up VMware Workstation Pro
Installation: Download and install VMware Workstation Pro from the official site.
Create Virtual Machines:
Security Onion: Allocate at least 4 CPUs, 16GB of RAM, and 200GB of disk space.
Kali Linux: Allocate at least 1 CPU, 2GB of RAM, and 10GB of disk space.
Metasploitable: Allocate at least 1 CPU, 512MB of RAM, and 8GB of disk space.
2. Network Configuration
Security Onion:
Interface 1 (Management): IP 192.168.253.10 (Replace with your setup).
Interface 2 (Sniffing): No IP, set to promiscuous mode.
Kali Linux: IP 192.168.253.129 (Replace with your setup).
Metasploitable: IP 192.168.253.128 (Replace with your setup).
3. Installing and Configuring Security Onion
Follow the installation guide provided in the Security Onion documentation.
Configure network interfaces according to your lab setup.
Deploy Security Onion with the necessary monitoring and alerting tools (e.g., Suricata, Zeek, Kibana).
4. Simulating Attacks with Kali Linux
Example Attacks:
SQL Injection: Target vulnerable web applications on Metasploitable.
Denial of Service (DoS): Flood the Metasploitable server with traffic.
Exploitation: Use Metasploit on Kali Linux to exploit known vulnerabilities on Metasploitable.
6. Monitoring and Analyzing with Security Onion
Zeek (formerly Bro): Monitor network traffic and generate logs.
Suricata: Analyze network traffic for signs of intrusion.
Kibana: Visualize and analyze the logs and alerts generated by Zeek and Suricata.

Results

Detection: Demonstrate how Security Onion detects various attacks.
Analysis: Analyze the logs and alerts generated by Security Onion.
Mitigation: Discuss potential mitigations for the detected attacks.

Future Work

Expanding the lab to include more complex scenarios and additional tools.
Integrating additional logging and monitoring tools.
Automating the deployment and configuration process.

Resources

Security Onion Documentation
Kali Linux Official Website
Metasploitable Download

License

This project is licensed under the MIT License - see the LICENSE file for details.

