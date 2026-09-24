# ISMS Scope Statement

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | DOC-SCP-001                        |
| Title            | ISMS Scope Statement               |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

## 1. Purpose

This statement defines the scope of the Journey of Life (JOL) Information Security Management
System (ISMS), as required by ISO/IEC 27001:2022 clause 4.3. It establishes the boundaries and
applicability of the policy suite published in this repository.

## 2. Organisational Scope

The ISMS applies to the JOL platform operated by `journeyoflife-org`, including all functions that
design, build, operate, secure, and support the platform serving approximately 400,000 religious
institution websites across 27 EU member states.

## 3. Scope of the ISMS

The ISMS covers:

- All **information assets** used to deliver the JOL platform, regardless of format or location
  (production, staging, development, endpoints, backups, and third-party hosted systems).
- All **personnel** — employees, contractors, and temporary staff — who access JOL systems or data.
- All **third parties and processors** that access, store, or process JOL or member-institution data
  on JOL's behalf.
- All **services, environments, and infrastructure** (including cloud regions) used to deliver the
  platform, across the `development → staging → production` lifecycle.
- The **governance, risk, and compliance processes** that manage information security.

## 4. Applicability of This Repository

This repository publishes the **Tier 1 and Tier 2** policy documents that apply organisation-wide
across the scope above. Implementation procedures (Tier 3) are maintained in the operational
repositories referenced in [`index.md`](index.md).

## 5. Interfaces and Dependencies

| Interface | Description |
|-----------|-------------|
| Member institutions | Data controllers whose congregants' data JOL processes as a processor |
| Cloud providers | EU-region infrastructure hosting tenant services and data stores |
| Payment services | Card processing scoped separately (see `jol-payments-scope`) |
| Sub-processors | Third parties engaged under GDPR Art. 28 agreements |

## 6. Exclusions

The following are explicitly out of scope of this repository (governed elsewhere):

- Payment-card environment specifics — governed by `jol-payments-scope` (PCI-DSS).
- Privacy artefacts (DPIAs, records of processing, data-subject rights) — governed by `jol-privacy`.
- Operational incident runbooks — governed by `jol-incident-response`.
- Infrastructure topology and secrets management implementation — governed by `jol-iac` and
  `jol-secrets` respectively.

## 7. Boundaries and Risk Acceptance

Where a control in ISO/IEC 27001:2022 Annex A is not applicable, the justification is recorded in
the Statement of Applicability maintained in `jol-control`. Public visibility of governance
repositories is a documented, owner-accepted risk that is re-evaluated before any sensitive content
is published.

## 8. Control Mapping

| Framework | Reference |
|-----------|-----------|
| ISO/IEC 27001:2022 | Clause 4.1–4.3 (context and scope), A.5.1 |
| SOC 2 | CC1.1, CC3.1–CC3.4 (risk assessment context) |
| GDPR | Art. 24, Art. 28, Art. 30 |
