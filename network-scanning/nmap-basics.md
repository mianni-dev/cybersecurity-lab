# Nmap Basics Lab

## Objective

Perform basic network discovery and port scanning using Nmap.

## Lab Environment

Attacker Machine  
Kali Linux running in VirtualBox

Local IP  
10.0.2.15

Network Range  
10.0.2.0/24

## Host Discovery

Command:

nmap -sn 10.0.2.0/24

Result:

The scan identified several active hosts including the VirtualBox NAT gateway and DNS service.

## Port Scan

Command:

nmap -sS -A 10.0.2.2

Purpose:

This scan attempts to identify open ports, running services, and operating system details.

## Observations

The VirtualBox gateway responded but did not expose many open services. This is expected for a NAT gateway device.

## Security Insight

Network scanning is commonly used by security professionals to identify potential attack surfaces. Understanding what services are exposed helps defenders harden systems and detect unauthorized access attempts.

## Tools Used

Nmap
