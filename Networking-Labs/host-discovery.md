# Host Discovery Techniques

## Objective
Identify active devices in a network.

---

## Tools Used

- ping
- fping
- netdiscover
- nmap -sn

---

## Techniques

### Ping Sweep
`nmap -sn 192.168.1.0/24`

Identifies live hosts without scanning ports.

### ARP Discovery
`netdiscover -r 192.168.1.0/24`

Discovers devices using ARP requests.

---

## Security Perspective

Host discovery is the first phase of:
- Penetration testing
- Red team operations
- Network mapping

From a defensive perspective:
- Repeated scanning may indicate reconnaissance activity.
