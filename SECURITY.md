# Security Policy

## Overview

Nasiko values the work of the security community and welcomes submissions of potential security vulnerabilities. Responsible disclosure helps us keep our products, infrastructure, and users safe.

We encourage good-faith security research and ask that you follow the guidelines below when reporting issues.

## Scope

This policy applies to submissions of potential security vulnerabilities related to Nasiko-owned or operated digital assets.

### What's In Scope

- **Nasiko Platform** — [https://nasiko.com](https://nasiko.com/)
- **Nasiko Documentation** — [https://docs.nasiko.com](https://docs.nasiko.com/)
- High-usage Nasiko-maintained open-source repositories (including `nasiko`, `nasiko-agent-sdk`, and similar core projects)
- Nasiko-owned applications, services, APIs, and infrastructure
- Public-facing Nasiko branded websites

Assets not explicitly listed are considered out of scope unless approved by Nasiko. If you're unsure whether a repository or service is in scope, contact `security@nasiko.com` before extensive testing.

### What's Out of Scope

**Always out of scope:**
- Social engineering or phishing
- Physical attacks or data-center access
- Attacks against third-party services
- Issues that only impact Nasiko users without a Nasiko-controlled vulnerability

**Usually out of scope** *(No bounty or acceptance unless additional, concrete security impact is demonstrated)*
- Automated scanning or indiscriminate fuzzing
- Rate limiting issues without demonstrated impact
- Password policy or complexity issues
- Error pages, banners, stack traces, or version disclosure
- Common public files (e.g. `robots.txt`, `.well-known`)
- Missing security headers or TLS/SSL best practices without exploitation
- Self-XSS, spam, or tabnabbing
- Open redirects without additional impact
- Issues requiring MITM or access to a user's device
- Known vulnerable libraries without a working proof of concept
- Prompt injection without demonstrated exploitability
- Issues affecting outdated or unsupported browsers

> If you are unsure whether an issue is in scope, please contact `security@nasiko.com` before performing extensive testing.

## How to Report a Vulnerability

If you believe you've found a security issue affecting Nasiko, please submit it using the appropriate channel below.

### Public Open-Source Repositories

For vulnerabilities in Nasiko public GitHub repositories, follow the security reporting instructions provided in the relevant repository or reach out to `security@nasiko.com`.

### All Other Systems

For vulnerabilities affecting Nasiko applications, services, infrastructure, or any non-public systems, email **[security@nasiko.com](mailto:security@nasiko.com)**.

## Reporting Guidelines

To help us validate and fix issues quickly, please follow these guidelines when submitting a vulnerability report.

### What to Include

Reports should include enough detail for us to **reproduce and assess the issue**. At a minimum, please provide:

- A clear description of the vulnerability
- The affected system, application, or repository
- Steps to reproduce the issue, or a working proof of concept
- An explanation of the security impact
- Any relevant screenshots, logs, or code snippets (if applicable)

Reports that lack sufficient detail to reproduce the issue may not be accepted or eligible for a bounty.

### Proof of Impact

We prioritize reports that clearly demonstrate **realistic security impact**.

Where possible, show:

- How the issue could be exploited in practice
- What an attacker could gain (e.g., access level, data exposure, privilege escalation)
- Any constraints or prerequisites required for exploitation

Theoretical issues or best-practice gaps without demonstrated impact are generally out of scope.

### Testing Expectations

Please conduct testing responsibly:

- Only test against assets listed as in scope
- Do not access, modify, or delete data that does not belong to you
- Do not intentionally degrade service availability
- Stop testing immediately if you believe your actions could impact other users or production systems

### Submission Rules

- Submit **one vulnerability per report**, unless chaining is required to demonstrate impact
- If multiple issues share a single root cause, they may be treated as one finding
- Duplicate submissions are awarded based on the **first reproducible report received**
- Vulnerabilities discovered through automated scanning must include **manual validation and demonstrated impact**
- Nasiko **does not accept** AI-generated submissions or reports generated primarily by automated tools

### Disclosure Expectations

- **Do not publicly disclose vulnerabilities without Nasiko's explicit written permission**
- Allow reasonable time for us to investigate and remediate reported issues
- Coordinated disclosure may be permitted after remediation at Nasiko's discretion

## Response Targets

Nasiko makes a best-effort attempt to meet the following timelines:

- **Initial response:** within 4 business days
- **Initial triage:** within 15 business days
- **Resolution time:** varies based on severity and complexity

Timelines are best-effort and may vary based on report quality, severity, and volume.

## Safe Harbor

Security research conducted **in good faith and in accordance with this policy** is considered authorized.

Nasiko will not initiate legal action against researchers who comply with this policy.

If a third party initiates legal action related to compliant research, Nasiko will make reasonable efforts to clarify that the activity was authorized.

## Bug Bounty Rewards

Severity is based on what an attacker can realistically achieve, not theoretical or worst-case impact. We evaluate findings based on the level of access gained, data sensitivity, and likelihood of exploitation.

Reports should clearly demonstrate real-world impact. Theoretical issues or best-practice gaps without a demonstrated exploit are generally out of scope.

Final severity and bounty decisions are made by Nasiko.

### Reward Scale

| Severity | What This Means | Typical Impact | Example Findings | Reward |
| --- | --- | --- | --- | --- |
| **Low** | Minimal security impact with little attacker value | No user data access. No production or privileged system access. Limited to individual accounts or non-sensitive assets. | Leaked API key with minimal scoped permissions | **$200** |
| **Moderate** | Real security weakness with constrained scope or impact | No user data access. Limited internal access or functionality. Impact constrained by permissions or additional requirements. | Access to internal endpoints or metadata without privilege escalation | **$500** |
| **High** | Meaningful compromise of Nasiko systems or infrastructure | Access to production systems or internal services. No confirmed user data exposure. Clear exploitability. | RCE or environment access exposing only low-sensitivity secrets | **$1,000–$2,000** |
| **Severe / Critical** | Significant compromise of infrastructure or user trust | User data access, cross-tenant impact, or highly privileged system access | Read/write access to internal systems or user data | **$2,000–$5,000+** |

### Payment Methods

Nasiko currently supports the following payment options:

- **Wire transfer** (via Accounts Payable)
- **Cryptocurrency** (Bitcoin, Ethereum)
- **PayPal** or other payment processors

Payment method availability may vary by country. Additional information may be required to comply with legal, tax, or payment regulations.

## Other Security Concerns

For any other security concerns, please contact us at `security@nasiko.com`.

You can also reach out via:
- **Discord:** [Nasiko Discord Community](https://discord.gg/DTNPxhDjD)
- **GitHub:** [Nasiko GitHub](https://github.com/Nasiko-Labs/nasiko)

---

Thank you for helping keep Nasiko and our community safe! 🔒
