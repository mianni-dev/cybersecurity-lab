# Metasploitable Network Scan Lab

## Objective

Identify services running on a vulnerable Linux machine using Nmap.

## Lab Environment

Attacker:
Kali Linux

Target:
Metasploitable 2

Virtualization:
VirtualBox Host-Only Network

## Host Discovery

Command used:

nmap -sn 192.168.56.0/24

Result:

The scan identified multiple hosts including the Metasploitable machine.

## Port Scan

Command:

nmap 192.168.56.102

Open services discovered:

- FTP (21)
- SSH (22)
- Telnet (23)
- HTTP (80)
- SMB (445)
- MySQL (3306)

## Service Enumeration

Command:

nmap -sS -sV -O 192.168.56.102

The scan revealed numerous outdated and vulnerable services intentionally included in Metasploitable.

## Security Insight

Service enumeration allows attackers to identify exposed services that may contain vulnerabilities. Security teams use similar scans to identify unnecessary services and reduce attack surface.

## Tools Used

Nmap
