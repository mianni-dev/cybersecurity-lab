# Samba usermap_script Exploit Lab

## Objective
Exploit vulnerable Samba service on Metasploitable.

## Tools
- Kali Linux
- Metasploit Framework
- Nmap

## Target
Metasploitable2

## Discovery
nmap -sV 192.168.56.102

Ports:
139/tcp
445/tcp

Service:
Samba 3.x

## Exploit
exploit/multi/samba/usermap_script

## Result
Obtained root shell on target machine.

## Key Takeaways
- Old Samba versions contain critical RCE vulnerabilities
- Enumeration is essential before exploitation
