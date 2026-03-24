# Reconnaissance & OSINT Lab – Day 3

## Objective

Learn and practice reconnaissance techniques including network analysis, OSINT tools, and anonymity tools used in cybersecurity.

---

## Lab Environment

Operating System: Parrot OS
Platform: UTM (Mac M1)

---

## Topics Covered

### 1. VPN & Anonymity

Installed and used VPN for secure and private browsing.

* Installed ProtonVPN
* Connected using OpenVPN configuration files

Also explored TOR Browser for anonymous communication.

---

### 2. Networking Commands

Practiced basic network reconnaissance:

* `whois tata.com` → domain registration info
* `traceroute google.com` → path tracking
* `ip a` → IP address info

---

### 3. OSINT Tools

#### theHarvester

Used for gathering emails, subdomains, and hosts.

Example:
theHarvester -d microsoft.com -l 200 -b all

---

#### Sublist3r

Used to enumerate subdomains.

Example:
python3 sublist3r.py -d tesla.com

---

#### Infoga

Used for email intelligence gathering.

Example:
python3 infoga.py -d infosys.com

---

### 4. Google Dorking

Used advanced search queries for information gathering:

Examples:

* `site:tata.com`
* `filetype:pdf ethical hacking`
* `intitle:"ethical hacking"`
* `inurl:"elon-musk"`

---

### 5. Automation Tools

#### Shell-GPT (sgpt)

Used for executing commands and automating tasks.

Example:
sgpt --shell "What is my IP address"

---

#### tgpt

CLI-based GPT tool for quick queries.

---

## Key Takeaways

* Reconnaissance is the first and most critical phase in cybersecurity
* OSINT tools help gather valuable public information about targets
* VPN and TOR improve privacy and anonymity
* Automation tools can speed up analysis and reconnaissance

---

## Cybersecurity Relevance

* Used in penetration testing (footprinting phase)
* Used by SOC analysts for threat intelligence
* Helps identify attack surfaces before exploitation

---

## Next Steps

* Learn Nmap for network scanning
* Practice web reconnaissance techniques
* Start vulnerability scanning labs
