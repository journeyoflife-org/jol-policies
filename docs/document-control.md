# Document-Control Register

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | DOC-REG-001                        |
| Title            | Document-Control Register          |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

This is the master register of all documents in the JOL ISMS policy suite. It is the single source
of truth for document identity, ownership, version, and review status. It satisfies ISO/IEC
27001:2022 clause 7.5 (*Documented information*) and supports SOC 2 **CC2.1**.

## 1. Policy Documents

| Doc ID | Title | Ver | Classification | Owner (role) | Approver (role) | Effective | Next Review | Status |
|--------|-------|-----|----------------|--------------|-----------------|-----------|-------------|--------|
| POL-ISM-001 | Information Security Policy | 1.0.0 | Public | CISO | Governance Board | 2026-09-24 | 2027-09-24 | Approved |
| POL-GOV-002 | Information Security Roles & Responsibilities | 1.0.0 | Public | CISO | Governance Board | 2026-09-24 | 2027-09-24 | Approved |
| POL-ACC-003 | Access Control Policy | 1.0.0 | Public | CISO / IAM Lead | Governance Board | 2026-09-24 | 2027-09-24 | Approved |
| POL-CHG-004 | Change Management Policy | 1.0.0 | Public | Head of DevOps / CAB | Governance Board | 2026-09-24 | 2027-09-24 | Approved |
| POL-AUP-005 | Acceptable Use Policy | 1.0.0 | Public | CISO / HR | Governance Board | 2026-09-24 | 2027-09-24 | Approved |
| POL-CLS-006 | Data Classification & Handling Policy | 1.0.0 | Public | Data Protection Officer | Governance Board | 2026-09-24 | 2027-09-24 | Approved |

## 2. Framework Documents

| Doc ID | Title | Ver | Classification | Owner (role) | Effective | Next Review | Status |
|--------|-------|-----|----------------|--------------|-----------|-------------|--------|
| DOC-FWK-001 | ISMS Policy Framework | 1.0.0 | Public | CISO | 2026-09-24 | 2027-09-24 | Approved |
| DOC-SCP-001 | ISMS Scope Statement | 1.0.0 | Public | CISO | 2026-09-24 | 2027-09-24 | Approved |
| DOC-MAP-001 | Control-Mapping Matrix | 1.0.0 | Public | CISO | 2026-09-24 | 2027-09-24 | Approved |
| DOC-REG-001 | Document-Control Register | 1.0.0 | Public | CISO | 2026-09-24 | 2027-09-24 | Approved |
| DOC-REV-001 | Review Schedule | 1.0.0 | Public | CISO | 2026-09-24 | 2027-09-24 | Approved |

## 3. Register Rules

- Every document has a unique, never-reused identifier and a single accountable owner **by role**.
- A document is **Approved** only after owner and Governance Board sign-off; until then it is
  **Draft** and must not be relied upon.
- Any change to a document updates its version and the Change-History block within the document,
  and is reflected in this register and in [`../CHANGELOG.md`](../CHANGELOG.md).
- A document past its Next Review date without a completed review is flagged **Overdue** and
  escalated to the owner and the Governance Board.
- **Retired** documents are retained for audit history and marked as such; their identifiers are
  never reused.

## 4. Status Legend

| Status | Meaning |
|--------|---------|
| Draft | In authoring/review; not approved |
| Approved | Owner + Governance Board sign-off complete; current |
| Overdue | Past Next Review without a completed review |
| Retired | Superseded or withdrawn; retained for history |
