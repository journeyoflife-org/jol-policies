# Changelog

All notable changes to the JOL ISMS policy suite are documented in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this
repository adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Policy
versions are tracked individually in [`docs/document-control.md`](docs/document-control.md);
this changelog records releases of the suite as a whole.

## [1.0.0] - 2026-09-24

### Added

- Initial public release of the JOL ISMS policy suite ("trust" repository).
- `POL-ISM-001` Information Security Policy (Tier-1 ISMS policy).
- `POL-GOV-002` Information Security Roles & Responsibilities.
- `POL-ACC-003` Access Control Policy.
- `POL-CHG-004` Change Management Policy.
- `POL-AUP-005` Acceptable Use Policy.
- `POL-CLS-006` Data Classification & Handling Policy.
- Governance spine: policy framework, ISMS scope statement, document-control register,
  authoritative control-mapping matrix (SOC 2 / ISO 27001:2022 / GDPR), and review schedule.
- Policy authoring template and policy-exception (waiver) request form.
- Repository governance: `README`, `SECURITY`, `CONTRIBUTING`, `CODE_OF_CONDUCT`, and `LICENSE`
  (CC-BY-4.0).
- Documentation CI (`docs-ci.yml`) and compliance-coverage CI (`compliance-check.yml`).
- Pre-commit configuration (markdown linting, secret detection, whitespace/tab/CRLF hygiene).

[1.0.0]: https://github.com/journeyoflife-org/jol-policies/releases/tag/v1.0.0
