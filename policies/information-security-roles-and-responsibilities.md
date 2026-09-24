# Information Security Roles and Responsibilities

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | POL-GOV-002                        |
| Title            | Information Security Roles & Responsibilities |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Chief Information Security Officer |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Last Review      | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

### Change History

| Version | Date       | Author (role) | Summary of Change    | Approved By (role) |
|---------|------------|---------------|----------------------|--------------------|
| 1.0.0   | 2026-09-24 | CISO          | Initial release      | JOL Governance Board |

## 1. Purpose

This policy assigns information security roles and responsibilities across JOL, ensuring
accountability, segregation of duties, and management leadership. It implements ISO/IEC 27001:2022
Annex A controls **A.5.2**, **A.5.3**, and **A.5.4**, and SOC 2 criteria **CC1.2–CC1.5**.

## 2. Scope

Applies to all JOL personnel, contractors, and third parties within the
[ISMS scope](../docs/scope-statement.md). Roles are described **by role, not by personal name**.

## 3. Definitions

| Term | Meaning |
|------|---------|
| Segregation of duties | Separating conflicting responsibilities to reduce risk of error or misuse |
| Accountable | The role ultimately answerable for an outcome (one per outcome) |
| DPO | Data Protection Officer (GDPR Art. 37–39) |
| CAB | Change Advisory Board |

## 4. Roles and Responsibilities

| Role | Primary information security responsibilities |
|------|-----------------------------------------------|
| JOL Governance Board | Accountable for the ISMS; approves policy, risk appetite, and resources |
| Chief Information Security Officer (CISO) | Owns the ISMS and this policy suite; advises the Board; oversees controls |
| Data Protection Officer (DPO) | Independent oversight of GDPR compliance; DPIAs; data-subject rights |
| Head of DevOps / CAB | Secure operations and change management; owns POL-CHG-004 |
| Engineering & Operations leads | Implement and operate controls; enforce least privilege |
| People/HR | Background checks, contracts, security awareness, sanctions process |
| All personnel | Comply with policies; report incidents and weaknesses |

## 5. Principles

- Every security obligation has a single **accountable** role and defined **responsible** roles.
- Conflicting duties are **segregated**; where segregation is impractical, compensating controls
  (e.g. logging, independent review) are applied and documented.
- Security responsibilities are documented in role descriptions and contracts.

## 6. Policy Statements

### 6.1 Assignment of Information Security Roles

1. Information security roles and responsibilities **must** be defined, assigned, and documented.
2. Accountability for the ISMS **must** rest with the Governance Board; day-to-day ownership with
   the CISO.
3. Role holders **must** acknowledge their security responsibilities at assignment.

### 6.2 Segregation of Duties

1. Conflicting duties and areas of responsibility **must** be segregated to reduce the risk of
   unauthorised or unintentional modification or misuse.
2. Where full segregation is not feasible, compensating controls **must** be documented, approved
   by the CISO, and monitored (e.g. activity logging, dual authorisation).
3. No single individual **must** be able to both authorise and implement a production change
   without an independent check (see [POL-CHG-004](change-management-policy.md)).

### 6.3 Management Responsibilities

1. Managers **must** ensure personnel understand and fulfil their security responsibilities.
2. Managers **must** promote the ISMS, enforce this policy suite, and escalate risks and
   nonconformities to the CISO.
3. Management **must** lead by example and provide the resources required for compliance.

### 6.4 Data Protection Officer Independence

1. Where required by GDPR Art. 37, JOL **must** designate a DPO who operates independently,
   reports to the highest management level, and has no conflicting duties.
2. The DPO **must** be consulted on all matters relating to the protection of personal data and
   **must** oversee DPIAs (coordinated with the `jol-privacy` repository).

## 7. Enforcement and Sanctions

Failure to fulfil assigned responsibilities is treated as a policy breach under
[POL-ISM-001 §7](information-security-policy.md) and may result in disciplinary action.

## 8. Exceptions

Exceptions **must** be time-bound, risk-assessed, and approved via the
[Policy Exception Request](../templates/policy-exception-request.md) form.

## 9. Review

The CISO reviews this policy at least annually and upon organisational change affecting roles.

## 10. Control Mapping

| Framework | Controls |
|-----------|----------|
| ISO/IEC 27001:2022 | A.5.2, A.5.3, A.5.4 |
| SOC 2 TSC | CC1.2, CC1.3, CC1.4, CC1.5, CC5.3 |
| GDPR | Art. 24, Art. 37–39 |

Full clause-level traceability: [Control-Mapping Matrix](../docs/control-mapping-matrix.md).

## 11. References

- ISO/IEC 27001:2022 Annex A.5.2–A.5.4; clause 5.3 (roles, responsibilities and authorities).
- AICPA SOC 2 TSC CC1.
- GDPR Art. 24, 37–39.
- [POL-ISM-001](information-security-policy.md), [POL-CHG-004](change-management-policy.md).
