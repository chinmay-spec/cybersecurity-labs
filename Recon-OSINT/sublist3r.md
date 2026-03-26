# Sublist3r – Subdomain Enumeration Tool

## Purpose

Sublist3r is a Python-based OSINT tool used to discover subdomains of a target domain using search engines and passive enumeration techniques.

---

## Command Used

```bash
python3 sublist3r.py -d example.com -v -o results.txt
```

### Explanation:
- `-d` → Target domain
- `-v` → Verbose output
- `-o` → Save output to file

---

## What It Collects

- Publicly accessible subdomains
- Development or staging environments
- Forgotten or misconfigured services

Examples:
- dev.example.com
- mail.example.com
- test.example.com

---

## Security Relevance (Offensive Perspective)

Subdomain enumeration helps identify:

- Hidden services
- Vulnerable staging servers
- Misconfigured DNS records
- Expanded attack surface

Attackers often target less monitored subdomains.

---

## Defensive Mitigation

Organizations should:

- Regularly audit subdomains
- Remove unused or outdated subdomains
- Restrict access to development environments
- Monitor DNS changes
- Use attack surface management tools

---

## Lab Environment

Enumeration performed in a controlled testing environment.
