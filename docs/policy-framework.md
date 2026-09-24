# ISMS Policy Framework

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | DOC-FWK-001                        |
| Title            | ISMS Policy Framework              |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

## 1. Purpose

This framework defines how the Journey of Life (JOL) Information Security Management System (ISMS)
policy suite is structured, authored, approved, versioned, communicated, reviewed, and retired. It
gives effect to ISO/IEC 27001:2022 clause 7.5 (*Documented information*) and Annex A control
**A.5.1** (*Policies for information security*), and to SOC 2 criteria **CC1** and **CC2**.

## 2. Policy Tiers

| Tier | Name | Purpose | Approval |
|------|------|---------|----------|
| 1 | Governing policy | Management direction, objectives, and commitment | JOL Governance Board |
| 2 | Topic policy | Binding requirements for a security domain | Policy owner + Governance Board |
| 3 | Procedure / standard / guideline | How a requirement is implemented operationally | Domain owner (external repo) |

Tier 1 and Tier 2 documents are published in this repository. Tier 3 documents are maintained in
the operational repositories they govern (see [`index.md`](index.md)).

## 3. Document Conventions

### 3.1 Identification

Every document has a stable identifier: `POL-<DOMAIN>-<NNN>` for policies and `DOC-<DOMAIN>-<NNN>`
for framework documents. Identifiers are never reused, even after retirement.

### 3.2 Document-Control block

Every policy and framework document begins with a Document-Control block stating: Document ID,
Title, Version, Classification, Owner (role), Approver (role), Effective Date, Last Review, Next
Review, and Review Cycle; followed by a Change-History table. See
[`../templates/policy-template.md`](../templates/policy-template.md).

### 3.3 Versioning

Versions follow Semantic Versioning applied to documents:

- **MAJOR** — substantive change to requirements, scope, or control obligations (requires
  Governance Board re-approval).
- **MINOR** — clarification, added detail, or non-binding guidance that does not alter obligations.
- **PATCH** — editorial fixes (typos, links, formatting).

### 3.4 Authoring rules

- Owners and approvers are referenced by **role**, never by personal name (public repository).
- Requirements use "must"/"must not"; recommendations use "should".
- Every numbered requirement must be traceable to a control in
  [`control-mapping-matrix.md`](control-mapping-matrix.md).
- No secrets, personal data, tenant identifiers, internal hostnames, or network topology.

## 4. Review and Approval

- Policies are reviewed **at least annually** and upon any material change (see
  [`review-schedule.md`](review-schedule.md)).
- Substantive changes follow the lifecycle in [`../CONTRIBUTING.md`](../CONTRIBUTING.md): issue →
  draft PR → owner review → Governance Board approval → merge → CHANGELOG + version bump.
- Review outcomes are recorded in the document's Change-History table and the master register in
  [`document-control.md`](document-control.md).

## 5. Exceptions

A requirement may be waived only through a time-bound, risk-assessed exception recorded on the
[`../templates/policy-exception-request.md`](../templates/policy-exception-request.md) form.
Exceptions must state the compensating controls, an expiry date (maximum 12 months), and the
approving authority. Expired exceptions lapse automatically and must be re-approved or remediated.

## 6. Communication and Training

Approved policies are published in this repository and communicated to all personnel. Awareness of
the Acceptable Use Policy is confirmed during onboarding and at least annually (ISO 27001
**A.6.3**; SOC 2 **CC2.2**).

## 7. Control Mapping

| Framework | Controls satisfied by this framework |
|-----------|--------------------------------------|
| ISO/IEC 27001:2022 | A.5.1, A.5.2, A.5.4, A.5.37; clause 7.5 |
| SOC 2 | CC1.1–CC1.5, CC2.1–CC2.3 |
| GDPR | Art. 24 (accountability) |
