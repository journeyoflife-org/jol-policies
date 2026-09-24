# Security Policy

## Supported Versions

Only the latest release on the `main` branch reflects the current, approved JOL ISMS policy suite.
Prior versions are retained for audit history but are not actively maintained.

| Version         | Supported |
|-----------------|-----------|
| `main` (latest) | Yes       |
| Older releases  | Historical reference only |

## Reporting a Vulnerability

**Do not open a public issue for security vulnerabilities.**

If you discover a vulnerability in a JOL system, or a security weakness implied by these policies,
report it through one of the following private channels:

1. **GitHub Security Advisories** — use the "Report a vulnerability" button on the repository's
   *Security* tab (preferred).
2. **Email** — send an encrypted message to `security@journeyoflife.org` using the organisation's
   published PGP key.

Please include:

- A description of the vulnerability and its potential impact.
- Steps to reproduce or a proof-of-concept where feasible.
- The affected component, policy document ID, file path, and version.
- Any suggested remediation.

## Reporting a Policy Gap or Compliance Finding

Non-vulnerability concerns — for example a missing control mapping, an ambiguous policy statement,
or a gap against SOC 2 / ISO 27001 / GDPR — should be raised through the
[*Policy Gap or Finding*](.github/ISSUE_TEMPLATE/policy-gap-or-finding.yml) issue template. These
are public by design and feed the documented policy-change process.

## Response Timeline

| Phase                | Target SLA              |
|----------------------|-------------------------|
| Acknowledgement      | 2 business days         |
| Triage and severity  | 5 business days         |
| Remediation plan     | 10 business days        |
| Patch deployment     | Proportional to severity |

## Severity Classification

Severity is assessed using CVSS v3.1:

| Rating   | Score    | Response                                    |
|----------|----------|---------------------------------------------|
| Critical | 9.0–10.0 | Immediate remediation; emergency release    |
| High     | 7.0–8.9  | Prioritised remediation within one sprint   |
| Medium   | 4.0–6.9  | Scheduled remediation in next release cycle |
| Low      | 0.1–3.9  | Tracked; remediated as capacity allows      |

## Disclosure Policy

- The reporter receives credit unless they request anonymity.
- Public disclosure occurs only after a fix is available and affected parties have been notified.
- A minimum 90-day embargo applies unless the vulnerability is actively exploited.

Incident handling itself is governed by the `jol-incident-response` repository; this document
covers disclosure of vulnerabilities affecting, or described by, this policy suite.

## Security Controls Applied to This Repository

- **Signed commits** — all commits to `main` are GPG- or SSH-signed.
- **Secret scanning** — GitHub secret scanning and push protection are enabled.
- **Least privilege** — GitHub Actions workflows declare explicit, minimal `permissions`.
- **Reviewed changes** — all policy changes require CODEOWNERS approval (see `.github/CODEOWNERS`).
