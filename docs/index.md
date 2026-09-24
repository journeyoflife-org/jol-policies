# Policy Suite Index

This document maps the structure of the JOL Information Security Management System (ISMS) policy
suite and defines the order in which the documents should be read.

## Policy Hierarchy

The suite is organised in three tiers. This repository publishes **Tier 1 and Tier 2**; Tier 3
procedures live in the operational repositories they govern and are linked, not duplicated.

```text
Tier 1 — Governing policy
└── POL-ISM-001  Information Security Policy
                 (sets direction, objectives, and management commitment)

Tier 2 — Topic policies (derive from Tier 1)
├── POL-GOV-002  Information Security Roles & Responsibilities
├── POL-ACC-003  Access Control Policy
├── POL-CHG-004  Change Management Policy
├── POL-AUP-005  Acceptable Use Policy
└── POL-CLS-006  Data Classification & Handling Policy

Tier 3 — Procedures, standards, guidelines (external repositories)
├── jol-security            → technical security standards & hardening
├── jol-incident-response   → incident handling runbooks
├── jol-privacy             → DPIAs, records of processing, data-subject rights
├── jol-compliance-evidence → control evidence collection
└── jol-dr                  → backup, resilience, and disaster recovery
```

## Reading Order

| # | Audience | Read |
|---|----------|------|
| 1 | Everyone | [`README`](../README.md) → [`scope-statement.md`](scope-statement.md) → [`POL-AUP-005`](../policies/acceptable-use-policy.md) |
| 2 | Management / auditors | [`POL-ISM-001`](../policies/information-security-policy.md) → [`POL-GOV-002`](../policies/information-security-roles-and-responsibilities.md) → [`policy-framework.md`](policy-framework.md) |
| 3 | Engineering / operations | [`POL-ACC-003`](../policies/access-control-policy.md) → [`POL-CHG-004`](../policies/change-management-policy.md) → [`POL-CLS-006`](../policies/data-classification-and-handling.md) |
| 4 | Compliance / audit | [`control-mapping-matrix.md`](control-mapping-matrix.md) → [`document-control.md`](document-control.md) → [`review-schedule.md`](review-schedule.md) |

## Document Map

| Document | Type | Purpose |
|----------|------|---------|
| [`policy-framework.md`](policy-framework.md) | Framework | How the ISMS policy suite is structured, versioned, and governed |
| [`scope-statement.md`](scope-statement.md) | Framework | Boundaries and applicability of the ISMS (ISO 27001 cl. 4.3) |
| [`document-control.md`](document-control.md) | Register | Master list of every policy with version, owner, and review dates |
| [`control-mapping-matrix.md`](control-mapping-matrix.md) | Crosswalk | Authoritative SOC 2 / ISO 27001:2022 / GDPR mapping |
| [`review-schedule.md`](review-schedule.md) | Schedule | Review cadence and out-of-cycle review triggers |
