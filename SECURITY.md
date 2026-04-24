# Security Policy

## Supported Projects

| Project | Repository | Supported |
|---------|-----------|-----------|
| 🎮 The Cordite Wars: Six Fronts | [cordite](https://github.com/KoshkiKode/cordite) | ✅ Active development |
| 📚 Unshelv'd | [unshelvd](https://github.com/KoshkiKode/unshelvd) | ✅ Active development |
| 🌿 Vetviona | [vetviona](https://github.com/KoshkiKode/vetviona) | ✅ Active development |

Security fixes are applied to the latest release of each project. We do not backport security patches to older versions.

---

## Reporting a Vulnerability

**Please do not open a public GitHub issue for security vulnerabilities.**

If you discover a security vulnerability in any KoshkiKode project, please report it responsibly:

1. **Email:** Use the contact form at [koshkikode.com](https://koshkikode.com) with the subject line `[SECURITY] <repo name>`.
2. **Include in your report:**
   - A clear description of the vulnerability
   - Steps to reproduce or a proof-of-concept
   - The potential impact (data exposure, authentication bypass, etc.)
   - Any suggestions for a fix, if you have them

---

## Response Timeline

| Stage | Target |
|-------|--------|
| Acknowledgement | Within 3 business days |
| Initial assessment | Within 7 days |
| Fix / mitigation | Dependent on severity — critical issues prioritized |
| Public disclosure | Coordinated with reporter after fix is released |

We will keep you informed at each stage. If you do not hear back within 3 business days, please follow up.

---

## Scope

Reports are accepted for:

- **Authentication and authorization flaws** in Unshelv'd (backend, payments, admin)
- **Data exposure** in any KoshkiKode app or service
- **RootLoop™ sync encryption weaknesses** in Vetviona
- **Supply-chain / dependency vulnerabilities** in any active project
- **Payment flow vulnerabilities** in Unshelv'd (Stripe Connect, PayPal)

Out of scope:

- Issues in third-party libraries where the fix must come from the upstream maintainer
- Social-engineering attacks
- Rate limiting or denial-of-service on development/staging environments
- Issues requiring physical access to a device

---

## Disclosure Policy

KoshkiKode follows coordinated disclosure. We ask that you give us reasonable time to address a vulnerability before making it public. In return, we will acknowledge your contribution in the release notes (unless you prefer to remain anonymous).

---

© 2026 [KoshkiKode](https://koshkikode.com). All rights reserved.
