# Security Policy

## Supported Versions

We actively maintain security patches for the following versions:

| Version | Supported |
|---------|-----------|
| Latest release | ✅ |
| Previous minor | ✅ |
| Older versions | ❌ |

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub Issues.**

If you discover a security vulnerability in any Evice Labs repository, we ask that you report it responsibly. We take all security reports seriously and will respond as quickly as possible.

### How to Report

**Option 1 — GitHub Private Vulnerability Reporting (preferred)**

Use GitHub's built-in private reporting feature:
1. Go to the affected repository
2. Click **Security** → **Advisories** → **Report a vulnerability**
3. Fill in the details

This keeps the report confidential and lets us coordinate a fix before public disclosure.

**Option 2 — Email**

Send a report to: *will be updated soon*

Encrypt your message using our PGP key if the information is highly sensitive.

---

## What to Include in Your Report

To help us triage and reproduce the issue quickly, please include:

- **Description** — a clear summary of the vulnerability
- **Affected component** — which repository, module, or function
- **Steps to reproduce** — detailed reproduction steps
- **Impact** — what an attacker could achieve by exploiting this
- **Suggested fix** *(optional)* — if you have a proposed remediation

---

## Our Commitment to You

- We will **acknowledge your report within 48 hours**
- We will **provide a status update within 5 business days**
- We will **notify you when the vulnerability is patched**
- We will **credit you** in the security advisory (unless you prefer anonymity)

We ask that you:
- Give us **reasonable time to address** the issue before public disclosure
- Avoid exploiting the vulnerability or accessing user data
- Not disclose the issue publicly until a fix has been released

---

## Disclosure Policy

We follow **coordinated disclosure**:

1. Reporter submits vulnerability privately
2. We confirm and assess severity (CVSS scoring)
3. We develop and test a fix
4. We release the fix and publish a GitHub Security Advisory
5. We credit the reporter (with their consent)

Typical turnaround: **14–30 days** depending on severity. Critical vulnerabilities are prioritized and may be patched sooner.

---

## Scope

The following are **in scope** for security reports:

- All repositories under the [evice-labs](https://github.com/evice-labs) organization
- Smart contracts / on-chain programs
- ZK circuits and cryptographic primitives
- SDKs and libraries published by Evice Labs

The following are **out of scope**:

- Third-party dependencies (report these to the upstream project)
- Social engineering attacks
- Vulnerabilities requiring physical access to a device
- Issues in forks not maintained by Evice Labs

---

## Bug Bounty

We currently **do not operate a formal bug bounty program**. However, we genuinely appreciate responsible disclosure and will publicly acknowledge reporters in our security advisories.

---

*Thank you for helping keep Evice Labs and its users safe.*
