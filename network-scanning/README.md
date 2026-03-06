# Network Scanning Lab

## Objective
The goal of this lab is to practice network reconnaissance using common security scanning tools. Network scanning is one of the first steps in penetration testing and security assessments because it helps identify live hosts, open ports, and exposed services.

## Lab Environment

Attacker Machine  
- Kali Linux

Virtualization  
- VirtualBox

Target Machines  
- Local lab network (additional vulnerable machines will be added later)

## Tools Used

- Nmap

## Key Concepts

This lab explores several core network discovery concepts:

- Host discovery
- Port scanning
- Service enumeration
- OS detection

These techniques help security professionals understand the attack surface of a system.

## Basic Scan Example

Example command used with Nmap:

nmap -sS -A 192.168.56.0/24

Explanation:

- -sS performs a SYN stealth scan
- -A enables OS detection, version detection, and traceroute
- 192.168.56.0/24 scans the local virtual network

## Expected Output

The scan should identify:

- Active hosts on the network
- Open ports
- Running services
- Potential operating system fingerprints

Example findings may include services such as:

- SSH (22)
- HTTP (80)
- FTP (21)

## Security Relevance

Network scanning is used by both attackers and defenders.

Attackers use scanning to locate vulnerable services.  
Defenders use scanning to audit networks and detect unnecessary exposures.

## Future Additions

This lab will expand to include:

- Detailed Nmap scan types
- Service version enumeration
- Vulnerability scanning
- Analysis of vulnerable lab machines

## Screenshots

Screenshots of scan results will be stored in the `/screenshots` directory.
