# Policy Review Schedule

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | DOC-REV-001                        |
| Title            | Policy Review Schedule             |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

## 1. Purpose

This schedule defines the review cadence for the JOL ISMS policy suite and the events that trigger
an out-of-cycle review. It gives effect to ISO/IEC 27001:2022 clause 9.3 (*Management review*) and
Annex A **A.5.1**, and to SOC 2 **CC4.1–CC4.2** (*Monitoring Activities*).

## 2. Cadence

| Doc ID | Document | Cycle | Last Review | Next Review |
|--------|----------|-------|-------------|-------------|
| POL-ISM-001 | Information Security Policy | Annual | 2026-09-24 | 2027-09-24 |
| POL-GOV-002 | Roles & Responsibilities | Annual | 2026-09-24 | 2027-09-24 |
| POL-ACC-003 | Access Control Policy | Annual | 2026-09-24 | 2027-09-24 |
| POL-CHG-004 | Change Management Policy | Annual | 2026-09-24 | 2027-09-24 |
| POL-AUP-005 | Acceptable Use Policy | Annual | 2026-09-24 | 2027-09-24 |
| POL-CLS-006 | Data Classification & Handling | Annual | 2026-09-24 | 2027-09-24 |
| DOC-FWK-001 | ISMS Policy Framework | Annual | 2026-09-24 | 2027-09-24 |
| DOC-SCP-001 | ISMS Scope Statement | Annual | 2026-09-24 | 2027-09-24 |
| DOC-MAP-001 | Control-Mapping Matrix | Annual + on control change | 2026-09-24 | 2027-09-24 |

## 3. Out-of-Cycle Review Triggers

A review is initiated immediately, regardless of schedule, when any of the following occurs:

- A **security incident** with lessons affecting policy (coordinated with `jol-incident-response`).
- An **audit finding** or external assessment observation (SOC 2, ISO 27001, or customer audit).
- A **regulatory or standard change** (e.g. GDPR guidance, ISO 27001 revision, new TSC).
- A **material change** to the platform, architecture, scope, or processing activities.
- An **organisational change** affecting roles, ownership, or accountability.
- A recurring **exception** indicating a policy is impractical or misaligned.

## 4. Review Process

1. Owner re-reads the document against current practice, controls, and frameworks.
2. Owner confirms or updates the control mapping in
   [`control-mapping-matrix.md`](control-mapping-matrix.md).
3. Changes follow the lifecycle in [`../CONTRIBUTING.md`](../CONTRIBUTING.md) and require
   Governance Board approval for substantive edits.
4. The Document-Control block, this schedule, and
   [`document-control.md`](document-control.md) are updated with the new review dates.
5. A "no change" review still records the review date and reviewer role.

## 5. Management Review

The complete suite is presented to the JOL Governance Board at least annually as part of ISMS
management review (ISO/IEC 27001:2022 clause 9.3), covering policy status, exceptions, incidents,
audit results, and improvement opportunities.
