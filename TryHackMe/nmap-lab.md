# TryHackMe – Nmap Lab

## Objective

Learn how to scan networks and identify open ports using Nmap.

---

## Commands Used

nmap <target>
nmap -sS <target>
nmap -sV <target>
nmap -p- <target>

---

## Command Explanation

* `nmap` → Performs a basic scan
* `-sS` → Stealth (SYN) scan
* `-sV` → Detects service versions
* `-p-` → Scans all ports

---

## Example Results

* Port 22 → SSH
* Port 80 → HTTP
* Port 443 → HTTPS

---

## Why Nmap is Important

Nmap is used to discover open ports and services running on a system.
These services can contain vulnerabilities that attackers may exploit.

---

## Key Takeaways

* Port scanning is the first step in penetration testing
* Open ports indicate potential attack surfaces
* Nmap is one of the most important tools in cybersecurity

---
