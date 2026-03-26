# Scan Result Analysis

## Example Scenario

Target: 192.168.1.45

Open Ports:
- 21 (FTP)
- 80 (HTTP)

---

## Analysis Approach

### Port 21 (FTP)
- Check for anonymous login
- Identify service version
- Search for known vulnerabilities

### Port 80 (HTTP)
- Identify web server version
- Enumerate directories
- Check for outdated components

---

## Filtered Ports

Indicates firewall dropping packets.
Cannot determine open or closed state.

---

## Defensive View

SYN scans may appear in logs as:
- Multiple connection attempts
- Half-open TCP connections
- Suspicious network activity
