# theHarvester – OSINT Email & Subdomain Enumeration

## Purpose

theHarvester is an open-source intelligence (OSINT) tool used to collect publicly available information about a target domain. It gathers emails, subdomains, IP addresses, and hostnames from search engines and public sources.

---

## Command Used

```bash
theHarvester -d example.com -l 200 -b all
```

### Explanation:
- `-d` → Target domain
- `-l` → Limit number of results
- `-b` → Data source (google, bing, yahoo, etc.)

---

## What It Collects

- Email addresses associated with the domain
- Subdomains
- Hostnames
- Public IP addresses
- Employee-related information (if indexed)

---

## Security Relevance (Offensive Perspective)

theHarvester is used in the reconnaissance phase of penetration testing to:

- Identify potential phishing targets
- Map external attack surface
- Discover exposed services
- Gather intelligence before exploitation

---

## Defensive Mitigation

Organizations should:

- Avoid publishing internal email addresses publicly
- Use generic contact emails (info@, support@)
- Remove sensitive employee data from public pages
- Monitor exposure using OSINT tools
- Implement DMARC, SPF, and DKIM to reduce phishing risks

---

## Lab Environment

Performed in a controlled lab environment using Parrot OS.
