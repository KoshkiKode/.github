# Security Policy

## Supported Versions

| Project | Supported Versions |
|---------|------------------|
| Unshelv'd | Latest release on `main` |
| Vetviona | Latest release on `main` |
| Cordite Wars | Latest release on `main` |

Only the latest version of each project receives security updates. If you're running an older version, please update before reporting.

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, report them privately via one of the following:

- **GitHub Private Security Advisory** — use the "Report a vulnerability" button on the Security tab of the affected repository.
- **Email** — send details to the organisation maintainer. Check the repository `README.md` for contact information.

### What to Include

Please provide as much of the following as possible:

- The repository and component affected
- A description of the vulnerability and its potential impact
- Steps to reproduce or a proof-of-concept
- Any suggested mitigations

---

## Response Timeline

| Stage | Target Time |
|-------|------------|
| Acknowledgement | Within 72 hours |
| Initial assessment | Within 7 days |
| Fix or mitigation | Depends on severity |
| Public disclosure | After fix is released |

---

## Scope

### In Scope

- Authentication and authorisation flaws
- Payment processing vulnerabilities (Unshelv'd)
- Data exposure or privacy leaks
- Remote code execution
- Injection vulnerabilities (SQL, command, etc.)
- Dependency vulnerabilities with a clear exploitation path

### Out of Scope

- Issues in third-party services (Stripe, PayPal, GoDaddy, etc.) — report those to the vendor directly
- Social engineering attacks
- Vulnerabilities requiring physical access to a device
- Issues on unsupported versions
- Spam or denial-of-service without a clear security impact

---

## Responsible Disclosure

We commit to:
- Acknowledging your report promptly
- Keeping you informed of progress
- Crediting you in the release notes (unless you prefer anonymity)
- Not taking legal action against good-faith security researchers

We ask that you:
- Give us reasonable time to fix the issue before public disclosure
- Not access, modify, or delete data that isn't yours
- Not disrupt service availability
