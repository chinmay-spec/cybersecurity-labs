# Linux Permissions & chmod

## Objective
Understand file permissions and access control in Linux.

---

## Permission Structure

-rwxr-xr--

- User (Owner)
- Group
- Others

---

## Commands Used

- chmod u+x filename
- chmod g-r filename
- chmod o+r filename
- chmod ugo-rwx filename

---

## Permission Types

- r (read)
- w (write)
- x (execute)

---

## Security Importance

Misconfigured permissions can lead to:
- Privilege escalation
- Unauthorized access
- Data leakage

Understanding permissions is critical for:
- Server hardening
- Incident response
- System security audits
