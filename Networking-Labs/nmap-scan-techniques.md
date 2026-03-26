# Nmap Scan Techniques

## Objective

Understand different Nmap scanning techniques used during network reconnaissance and how they are detected from a defensive perspective.

---

## 1. Host Discovery (Ping Sweep)

### Command
```
nmap -sn 192.168.1.0/24
```

### Purpose
Identify live hosts without scanning ports.

### Security Impact
Used during initial reconnaissance to map active devices.

### Detection
May appear as multiple ICMP echo requests or ARP requests in logs.

---

## 2. TCP Connect Scan (-sT)

### Command
```
nmap -sT 192.168.1.45
```

### How It Works
Completes full TCP 3-way handshake.

### Characteristics
- Reliable
- Easily logged
- No root privileges required

### Detection
Very easy to detect in firewall and IDS logs.

---

## 3. SYN Scan (-sS)

### Command
```
sudo nmap -sS 192.168.1.45
```

### How It Works
Sends SYN packet and waits for SYN-ACK response without completing handshake.

### Why Used
- Faster than connect scan
- Considered stealthier

### Detection
Can still be detected by IDS due to abnormal SYN patterns.

---

## 4. UDP Scan (-sU)

### Command
```
sudo nmap -sU 192.168.1.45
```

### Purpose
Identify open UDP services (DNS, SNMP, etc.)

### Challenges
- Slower
- Often unreliable
- No response does not always mean closed

---

## 5. NULL Scan (-sN)

### Command
```
sudo nmap -sN 192.168.1.45
```

### Concept
Sends TCP packets with no flags set.

### Purpose
Attempt to bypass poorly configured firewalls.

### Limitation
Not reliable against modern systems.

---

## 6. FIN Scan (-sF)

### Command
```
sudo nmap -sF 192.168.1.45
```

### Concept
Sends FIN flag packets to identify open ports.

---

## 7. XMAS Scan (-sX)

### Command
```
sudo nmap -sX 192.168.1.45
```

### Concept
Sets FIN, PSH, and URG flags simultaneously.

### Purpose
Firewall evasion testing in lab environments.

---

## 8. Version Detection (-sV)

### Command
```
sudo nmap -sV 192.168.1.45
```

### Purpose
Identify service versions running on open ports.

### Security Use
Helps identify known CVEs associated with specific versions.

---

## 9. OS Detection (-O)

### Command
```
sudo nmap -O 192.168.1.45
```

### How It Works
Uses TCP/IP stack fingerprinting.

### Reliability
Moderately accurate; can be affected by firewalls and NAT.

---

## 10. Aggressive Scan (-A)

### Command
```
sudo nmap -A 192.168.1.45
```

### Enables
- OS detection
- Version detection
- Script scanning
- Traceroute

### Risk
High detectability.

---

## 11. Timing Templates (-T)

Examples:
```
-T3 (Normal)
-T4 (Aggressive)
-T5 (Insane)
```

Higher timing = faster scan but higher detection risk.

---

## 12. Output Saving

```
-oN output.txt   (Normal output)
-oX output.xml   (XML format)
```

Important for documentation and reporting.

---

# Defensive Perspective

From a SOC viewpoint, Nmap scans may generate:

- Multiple connection attempts
- Incomplete TCP handshakes
- Unusual traffic patterns
- Sequential port probing

Monitoring tools such as IDS/IPS can detect these behaviors.

---

# Ethical Note

All scanning performed in controlled lab environments (TryHackMe / local lab).
