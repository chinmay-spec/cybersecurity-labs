# Networking Basics

## Objective

Understand fundamental networking concepts required for cybersecurity, including how devices communicate and how attackers enumerate networks.

---

## 1. What is Networking?

Networking enables devices to communicate and exchange data over wired or wireless connections using defined protocols.

In cybersecurity, understanding networking is essential for:
- Identifying attack surfaces
- Detecting malicious traffic
- Performing reconnaissance
- Analyzing logs

---

## 2. OSI Model (7 Layers)

1. Physical  
2. Data Link  
3. Network  
4. Transport  
5. Session  
6. Presentation  
7. Application  

### Security Relevance:
- Attacks occur at different layers (e.g., ARP spoofing at Layer 2, SQL injection at Layer 7).
- Network defenders monitor traffic across multiple layers.

---

## 3. TCP/IP Model

1. Network Interface  
2. Internet  
3. Transport  
4. Application  

### Key Protocols:
- TCP (Reliable communication)
- UDP (Faster, connectionless)
- ICMP (Used for ping and diagnostics)
- DNS (Domain resolution)
- HTTP/HTTPS (Web communication)

---

## 4. IP Addressing

### Types:
- Public IP
- Private IP (e.g., 192.168.x.x, 10.x.x.x)

### CIDR Notation Example:
192.168.1.0/24

Indicates 256 possible IP addresses in subnet.

---

## 5. Common Networking Commands Practiced

### Check Interface Information
```
ifconfig
ip a
```

### Ping Test
```
ping 192.168.1.1
```

### Traceroute
```
traceroute google.com
```

### Host Discovery
```
nmap -sn 192.168.1.0/24
```

---

## 6. Ports & Services

Common Ports:

- 21 → FTP
- 22 → SSH
- 25 → SMTP
- 53 → DNS
- 80 → HTTP
- 443 → HTTPS

Open ports represent potential attack vectors.

---

## 7. Defensive Perspective

From a SOC perspective:

- Multiple SYN packets may indicate port scanning.
- ICMP sweeps may indicate host discovery attempts.
- Unusual outbound connections may indicate malware.

Understanding networking fundamentals helps both attackers and defenders.

---

## Lab Environment

Practiced in Parrot OS (UTM – Mac M1) and TryHackMe virtual labs.
