# JOL Policies — Information Security & Compliance Trust Centre

The public **trust** repository for the **Journey of Life (JOL)** platform. It publishes the
Information Security Management System (ISMS) policy suite that governs how JOL protects the
confidentiality, integrity, and availability of the data entrusted to it by approximately
**400,000 religious-institution websites across 27 EU member states**.

This repository exists so that customers, member institutions, auditors, and regulators can
inspect JOL's governing security and compliance commitments directly.

## Compliance Coverage

| Framework | Scope in this repository |
|-----------|--------------------------|
| **ISO/IEC 27001:2022** | Annex A organisational, people, and technological controls (A.5.x, A.6.x, A.8.x) |
| **SOC 2 (Trust Services Criteria)** | Control Environment (CC1), Communication & Information (CC2), Logical Access (CC6), Change Management (CC8) |
| **GDPR (EU 2016/679)** | Accountability, security of processing, and data-protection-by-design principles (Art. 5, 24, 25, 32, 35) |

A clause-by-clause crosswalk is maintained in
[`docs/control-mapping-matrix.md`](docs/control-mapping-matrix.md).

## Policy Index

| Doc ID | Policy | Owner (role) | Classification |
|--------|--------|--------------|----------------|
| [POL-ISM-001](policies/information-security-policy.md) | Information Security Policy | CISO | Public |
| [POL-GOV-002](policies/information-security-roles-and-responsibilities.md) | Information Security Roles & Responsibilities | CISO | Public |
| [POL-ACC-003](policies/access-control-policy.md) | Access Control Policy | CISO | Public |
| [POL-CHG-004](policies/change-management-policy.md) | Change Management Policy | Head of DevOps | Public |
| [POL-AUP-005](policies/acceptable-use-policy.md) | Acceptable Use Policy | CISO | Public |
| [POL-CLS-006](policies/data-classification-and-handling.md) | Data Classification & Handling Policy | Data Protection Officer | Public |

Supporting governance documents:

| Document | Purpose |
|----------|---------|
| [`docs/index.md`](docs/index.md) | Policy hierarchy map and reading order |
| [`docs/policy-framework.md`](docs/policy-framework.md) | ISMS structure, tiers, review cadence, exception process |
| [`docs/scope-statement.md`](docs/scope-statement.md) | ISMS scope, boundaries, applicability, exclusions |
| [`docs/document-control.md`](docs/document-control.md) | Master document-control register |
| [`docs/control-mapping-matrix.md`](docs/control-mapping-matrix.md) | Authoritative SOC 2 / ISO 27001 / GDPR crosswalk |
| [`docs/review-schedule.md`](docs/review-schedule.md) | Review cadence and next-review dates |

## Document Control

Every policy carries a Document-Control block stating its ID, version, owner (by **role**, never
by personal name), approver, effective date, and next-review date. All policies in this repository
are classified **Public** and are reviewed **at least annually** or upon material change. The
consolidated register is at [`docs/document-control.md`](docs/document-control.md).

## Providing Feedback / Requesting a Change

Policies are maintained through a public, auditable change process:

- **Propose a policy change** — open an issue using the
  [*Policy Change Request*](.github/ISSUE_TEMPLATE/policy-change-request.yml) template.
- **Report a gap or finding** — open an issue using the
  [*Policy Gap or Finding*](.github/ISSUE_TEMPLATE/policy-gap-or-finding.yml) template.
- **Contribution workflow** — see [`CONTRIBUTING.md`](CONTRIBUTING.md).

All substantive changes require review and approval by the policy owner and the JOL Governance
Board, and are recorded in [`CHANGELOG.md`](CHANGELOG.md).

## Reporting a Security Vulnerability

**Do not open a public issue for security vulnerabilities.** See [`SECURITY.md`](SECURITY.md) for
the private disclosure channel, response SLAs, and severity classification.

## Related JOL Repositories

Privacy governance (DPIAs, records of processing, data-subject rights) is maintained separately in
the `jol-privacy` repository; incident response in `jol-incident-response`; and control evidence in
`jol-compliance-evidence`. This repository links to, and does not duplicate, those artefacts.

## Licence

The policy text in this repository is licensed under
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). See [`LICENSE`](LICENSE).
