# Infoga – Email Intelligence Gathering Tool

## Purpose

Infoga is an OSINT tool used to gather intelligence about email addresses associated with a target domain.

It helps identify whether emails exist and whether they appear in public data breaches.

---

## Command Used

```bash
python3 infoga.py -d example.com
```

---

## What It Collects

- Email addresses linked to domain
- Email validation status
- Possible breach exposure
- Associated services

---

## Security Relevance (Offensive Perspective)

Email intelligence can be used to:

- Identify phishing targets
- Perform credential stuffing attacks
- Conduct social engineering
- Assess email exposure risk

---

## Defensive Mitigation

Organizations should:

- Enforce strong password policies
- Enable multi-factor authentication (MFA)
- Monitor breach exposure
- Conduct phishing awareness training
- Avoid publicly exposing employee email addresses

---

## Lab Environment

Testing performed strictly in controlled lab conditions.
