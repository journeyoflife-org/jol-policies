# Control-Mapping Matrix

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | DOC-MAP-001                        |
| Title            | Control-Mapping Matrix             |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

This is the **authoritative** crosswalk between the JOL ISMS policy suite and its governing
frameworks: **SOC 2 Trust Services Criteria (TSC)**, **ISO/IEC 27001:2022 Annex A**, and the
**EU GDPR**. Every numbered policy requirement must appear here. Standards identifiers are the
property of AICPA, ISO/IEC, and the European Union respectively and are referenced for mapping only.

## 1. Policy-Level Mapping

| Doc ID | Policy | ISO/IEC 27001:2022 | SOC 2 TSC | GDPR |
|--------|--------|--------------------|-----------|------|
| POL-ISM-001 | Information Security Policy | A.5.1, A.5.2, A.5.4, A.5.37 | CC1.1–CC1.5, CC2.1–CC2.3, CC5.1 | Art. 24, Art. 32 |
| POL-GOV-002 | Roles & Responsibilities | A.5.2, A.5.3, A.5.4 | CC1.2, CC1.3, CC1.4, CC1.5 | Art. 24, Art. 37–39 |
| POL-AUP-005 | Acceptable Use | A.5.10, A.5.11, A.6.3 | CC1.1, CC2.2, CC2.3 | Art. 29, Art. 32(4) |
| POL-ACC-003 | Access Control | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.5 | CC6.1–CC6.5, CC6.7, CC6.8 | Art. 5(1)(f), Art. 25, Art. 32 |
| POL-CHG-004 | Change Management | A.8.32, A.8.9, A.8.29, A.8.31, A.5.37 | CC8.1, CC3.4, CC4.1, CC5.2 | Art. 25, Art. 32, Art. 35 |
| POL-CLS-006 | Data Classification & Handling | A.5.12, A.5.13, A.5.14, A.5.10 | CC2.1, CC6.1, CC6.5 | Art. 5, Art. 30, Art. 32 |

> **Scope note:** the governance anchor for this suite is SOC 2 **CC1–CC2** and ISO 27001
> **A.5.1–A.5.4**. Access control and change management additionally and necessarily map to
> **CC6 / A.5.15+** and **CC8.1 / A.8.32** respectively; omitting these would leave the crosswalk
> indefensible under audit. Both the anchor and the extended mappings are shown.

## 2. Clause-Level Mapping

Each policy requirement (clause) traces to at least one control.

### POL-ISM-001 Information Security Policy

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Management commitment & ISMS objectives | A.5.1, A.5.4 | CC1.1, CC1.2 | Art. 24 |
| 6.2 | Information security objectives & measurement | A.5.1 | CC1.5, CC4.1 | — |
| 6.3 | Continual improvement & ISMS review | A.5.1 | CC4.1, CC4.2 | Art. 24 |
| 6.4 | Communication of the policy | A.5.1, A.6.3 | CC2.2, CC2.3 | — |

### POL-GOV-002 Roles & Responsibilities

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Assignment of information security roles | A.5.2 | CC1.3 | Art. 24 |
| 6.2 | Segregation of duties | A.5.3 | CC1.4, CC5.3 | — |
| 6.3 | Management responsibilities | A.5.4 | CC1.2, CC1.5 | Art. 24 |
| 6.4 | Data Protection Officer independence | A.5.2 | CC1.3 | Art. 37–39 |

### POL-AUP-005 Acceptable Use

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Acceptable use of assets & systems | A.5.10 | CC1.1, CC2.2 | Art. 29 |
| 6.2 | Return of assets on termination | A.5.11 | CC6.5 | — |
| 6.3 | Security awareness & training | A.6.3 | CC1.4, CC2.2 | Art. 32(4) |
| 6.4 | Sanctions for misuse | A.5.10 | CC1.1 | — |

### POL-ACC-003 Access Control

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Access control policy & business rules | A.5.15 | CC6.1 | Art. 5(1)(f) |
| 6.2 | Identity management & provisioning | A.5.16, A.5.18 | CC6.2, CC6.3 | Art. 25 |
| 6.3 | Authentication & secure sign-on (MFA) | A.5.17, A.8.5 | CC6.1, CC6.7 | Art. 32 |
| 6.4 | Least privilege & privileged access | A.8.2, A.8.3 | CC6.1, CC6.4 | Art. 25 |
| 6.5 | Access review & de-provisioning | A.5.18 | CC6.2, CC6.3, CC6.5 | Art. 32 |

### POL-CHG-004 Change Management

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Documented change process & authorisation | A.8.32, A.5.37 | CC8.1 | Art. 32 |
| 6.2 | Risk & impact assessment (incl. DPIA trigger) | A.8.32 | CC3.4 | Art. 35 |
| 6.3 | Segregation of dev/test/prod & config mgmt | A.8.31, A.8.9 | CC8.1, CC6.4 | Art. 25 |
| 6.4 | Security testing before release | A.8.29 | CC8.1, CC4.1 | — |
| 6.5 | Emergency changes & rollback | A.8.32 | CC8.1, CC7.4 | Art. 32 |

### POL-CLS-006 Data Classification & Handling

| Clause | Requirement | ISO 27001 | SOC 2 | GDPR |
|--------|-------------|-----------|-------|------|
| 6.1 | Classification scheme & levels | A.5.12 | CC2.1 | Art. 5, Art. 30 |
| 6.2 | Labelling of information | A.5.13 | CC2.1 | — |
| 6.3 | Handling & transfer by level | A.5.14, A.5.10 | CC6.1, CC6.5 | Art. 32 |
| 6.4 | Personal-data handling & retention | A.5.12 | CC6.5 | Art. 5(1)(e), Art. 32 |

## 3. Reverse Index (Control → Policy)

| Control | Covered by |
|---------|------------|
| ISO A.5.1 | POL-ISM-001, DOC-FWK-001 |
| ISO A.5.2–A.5.4 | POL-GOV-002, POL-ISM-001 |
| ISO A.5.10–A.5.14 | POL-CLS-006, POL-AUP-005 |
| ISO A.5.15–A.5.18 | POL-ACC-003 |
| ISO A.6.3 | POL-AUP-005 |
| ISO A.8.2, A.8.3, A.8.5 | POL-ACC-003 |
| ISO A.8.9, A.8.29, A.8.31, A.8.32 | POL-CHG-004 |
| SOC 2 CC1.x | POL-ISM-001, POL-GOV-002, POL-AUP-005 |
| SOC 2 CC2.x | POL-ISM-001, POL-AUP-005, POL-CLS-006 |
| SOC 2 CC3.4, CC4.1 | POL-CHG-004 |
| SOC 2 CC5.x | POL-ISM-001, POL-GOV-002, POL-CHG-004 |
| SOC 2 CC6.x | POL-ACC-003, POL-CLS-006 |
| SOC 2 CC8.1 | POL-CHG-004 |
| GDPR Art. 5, 24, 25, 29, 30, 32, 35 | POL-CLS-006, POL-ISM-001, POL-ACC-003, POL-CHG-004, POL-AUP-005 |

## 4. Coverage Gaps

No policy requirement in this suite is unmapped. Controls outside the scope of these six policies
(for example physical security A.7.x, or supplier relationships A.5.19–A.5.23) are addressed by
Tier 3 procedures in the operational repositories and are tracked in the Statement of Applicability
in `jol-control`.
