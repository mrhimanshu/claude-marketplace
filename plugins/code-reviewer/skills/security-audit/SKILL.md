---
description: Deep security audit of code for OWASP Top 10 and common vulnerabilities
disable-model-invocation: true
---

Perform a focused security audit on the selected code or recent changes. Check against:

**OWASP Top 10**
- A01: Broken Access Control
- A02: Cryptographic Failures
- A03: Injection (SQL, NoSQL, OS command, LDAP)
- A04: Insecure Design
- A05: Security Misconfiguration
- A06: Vulnerable and Outdated Components
- A07: Identification and Authentication Failures
- A08: Software and Data Integrity Failures
- A09: Security Logging and Monitoring Failures
- A10: Server-Side Request Forgery (SSRF)

**Additional Checks**
- Hardcoded secrets, API keys, or credentials
- Insecure deserialization
- Path traversal vulnerabilities
- Improper error handling that leaks information
- Missing rate limiting or DoS protection
- Insecure direct object references

For each finding, provide:
- **Severity**: Critical / High / Medium / Low
- **Location**: File and line number
- **Description**: What the vulnerability is
- **Remediation**: How to fix it with a code example

If no issues found, confirm the code passes the security audit.
