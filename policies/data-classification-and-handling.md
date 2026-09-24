# Data Classification and Handling Policy

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | POL-CLS-006                        |
| Title            | Data Classification & Handling Policy |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Data Protection Officer            |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Last Review      | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

### Change History

| Version | Date       | Author (role) | Summary of Change    | Approved By (role) |
|---------|------------|---------------|----------------------|--------------------|
| 1.0.0   | 2026-09-24 | DPO           | Initial release      | JOL Governance Board |

## 1. Purpose

This policy defines how JOL classifies information and the handling requirements for each class, so
that protection is proportionate to sensitivity and legal obligation. It implements ISO/IEC
27001:2022 Annex A controls **A.5.12**, **A.5.13**, and **A.5.14**, and supports SOC 2 **CC2.1**
and **CC6**, and GDPR principles of integrity/confidentiality and storage limitation.

## 2. Scope

Applies to all information JOL creates, receives, stores, processes, transmits, or disposes of, in
any format or location, within the [ISMS scope](../docs/scope-statement.md).

## 3. Definitions

| Term | Meaning |
|------|---------|
| Personal data | GDPR Art. 4 — information relating to an identified or identifiable person |
| Special-category data | GDPR Art. 9 — e.g. data revealing religious beliefs |
| Handler | Any person or system that processes information |

> Given that JOL serves religious institutions, much congregant data may constitute
> **special-category data under GDPR Art. 9** and is treated at the highest classification.

## 4. Roles and Responsibilities

- **Data Protection Officer** — owns this policy; advises on classification of personal data.
- **Data/asset owners** — classify their assets and approve handling exceptions.
- **All handlers** — apply the correct classification and handling requirements.

## 5. Classification Scheme

| Level | Label | Examples | Baseline handling |
|-------|-------|----------|-------------------|
| 1 | **Public** | This policy suite, marketing material | No special handling; integrity still protected |
| 2 | **Internal** | Operational docs, internal metrics | Access restricted to JOL personnel |
| 3 | **Confidential** | Personal data, security configurations, contracts | Encrypted in transit and at rest; least-privilege access; logged |
| 4 | **Restricted** | Secrets/keys, special-category data, payment data | Strongest controls; vault storage; MFA; strict need-to-know; no local copies |

## 6. Policy Statements

### 6.1 Classification Scheme and Levels

1. All JOL information **must** be classified into one of the four levels in §5.
2. Data owners **must** assign and record classification; where unclear, the **higher** level
   **must** be applied until resolved (fail-safe default).
3. Personal data **must** be classified at least **Confidential**; special-category and payment data
   **must** be **Restricted**.

### 6.2 Labelling of Information

1. Confidential and Restricted information **must** be labelled (metadata, headers, or repository
   markers) so handlers can identify the required protections.
2. Labels **must** travel with the information when copied or transmitted.
3. This repository is labelled **Public**; Confidential/Restricted material **must not** be committed
   here (see [POL-AUP-005 §6.1](acceptable-use-policy.md)).

### 6.3 Handling and Transfer by Level

1. Handling, storage, transmission, and disposal controls **must** match the classification level,
   including encryption in transit (TLS 1.3) and at rest (AES-256) for Confidential and above.
2. Transfer of Confidential/Restricted information outside the EEA **must** use a lawful GDPR
   transfer mechanism and be approved by the DPO.
3. Secure disposal **must** render information unrecoverable at end of retention.

### 6.4 Personal-Data Handling and Retention

1. Personal data **must** be processed only with a lawful basis, for specified purposes, and
   minimised to what is necessary (GDPR Art. 5).
2. Retention periods **must** be defined per data category and enforced; data **must** be deleted or
   anonymised when retention expires (storage limitation, Art. 5(1)(e)).
3. Records of processing and DPIAs **must** be maintained in the `jol-privacy` repository and
   referenced, not duplicated, here.

## 7. Enforcement and Sanctions

Mishandling of classified information — especially Confidential or Restricted — is a policy breach
under [POL-ISM-001 §7](information-security-policy.md) and may trigger incident response and
disciplinary or regulatory action.

## 8. Exceptions

Exceptions **must** be time-bound, risk-assessed, and approved via the
[Policy Exception Request](../templates/policy-exception-request.md) form, with DPO sign-off for any
exception involving personal data.

## 9. Review

The DPO reviews this policy at least annually and upon changes to law, processing activities, or
data flows.

## 10. Control Mapping

| Framework | Controls |
|-----------|----------|
| ISO/IEC 27001:2022 | A.5.12, A.5.13, A.5.14, A.5.10 |
| SOC 2 TSC | CC2.1, CC6.1, CC6.5 |
| GDPR | Art. 5, Art. 30, Art. 32 |

Full clause-level traceability: [Control-Mapping Matrix](../docs/control-mapping-matrix.md).

## 11. References

- ISO/IEC 27001:2022 Annex A.5.12–A.5.14.
- AICPA SOC 2 TSC CC2, CC6.
- GDPR Art. 4, 5, 9, 30, 32, 35.
- `jol-privacy` (DPIA template and records of processing),
  [POL-AUP-005](acceptable-use-policy.md).
