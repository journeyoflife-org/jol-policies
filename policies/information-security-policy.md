# Information Security Policy

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | POL-ISM-001                        |
| Title            | Information Security Policy        |
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

This is the Tier-1 governing policy of the Journey of Life (JOL) Information Security Management
System (ISMS). It states management's direction, commitment, and objectives for information
security, and gives effect to ISO/IEC 27001:2022 clause 5.2 and Annex A control **A.5.1**. All
other JOL security policies derive from this document.

## 2. Scope

This policy applies to all JOL personnel, contractors, and third parties, and to all information,
systems, services, and environments used to deliver the JOL platform, as defined in the
[ISMS Scope Statement](../docs/scope-statement.md).

## 3. Definitions

| Term | Meaning |
|------|---------|
| ISMS | Information Security Management System |
| Information asset | Any data, system, or service of value to JOL or its member institutions |
| Confidentiality | Information is accessible only to those authorised to access it |
| Integrity | Information and systems are accurate, complete, and protected from improper modification |
| Availability | Information and systems are accessible and usable when required |
| Personal data | Any information relating to an identified or identifiable natural person (GDPR Art. 4) |

## 4. Roles and Responsibilities

The JOL Governance Board is accountable for this policy. The Chief Information Security Officer
(CISO) owns it. All personnel are responsible for complying with it. Detailed responsibilities are
defined in [POL-GOV-002 Roles & Responsibilities](information-security-roles-and-responsibilities.md).

## 5. Principles

JOL information security is founded on the following principles:

- **Confidentiality, integrity, and availability** of member-institution and congregant data.
- **Least privilege** — access is the minimum necessary for the role and is time-bounded.
- **Defence in depth** — no single point of trust; multiple, layered controls.
- **Fail-safe defaults** — new tenants and services inherit the most restrictive configuration.
- **Data residency and privacy by design** — EU data stays in EU regions; GDPR is designed in.
- **Accountability and observability** — actions are attributable and logged.

## 6. Policy Statements

### 6.1 Management Commitment and ISMS Objectives

1. Management **must** establish, document, communicate, and maintain an ISMS proportionate to
   JOL's size, regulatory obligations, and risk profile.
2. The ISMS **must** preserve the confidentiality, integrity, and availability of all JOL and
   member-institution information.
3. Management **must** provide the resources, authority, and visibility required to operate and
   improve the ISMS.
4. Information security objectives **must** be established, be consistent with this policy, and be
   reviewed at each management review.

### 6.2 Information Security Objectives and Measurement

1. Objectives **must** be specific, measurable, and assigned to accountable roles.
2. Progress against objectives **must** be monitored and reported to the Governance Board at
   least annually and upon material change.

### 6.3 Continual Improvement and ISMS Review

1. The ISMS **must** be reviewed at planned intervals (see
   [Review Schedule](../docs/review-schedule.md)) and continually improved.
2. Nonconformities **must** be corrected, and corrective actions **must** address root cause.
3. Lessons from incidents, audits, and exceptions **must** feed policy and control improvements.

### 6.4 Communication of the Policy

1. This policy **must** be published in this repository and communicated to all personnel and
   relevant third parties.
2. Personnel **must** confirm awareness of this policy and the
   [Acceptable Use Policy](acceptable-use-policy.md) at onboarding and at least annually.

## 7. Enforcement and Sanctions

Breaches of this policy **must** be reported to the CISO. Violations may result in disciplinary
action up to and including termination of employment or contract, and, where warranted, civil or
criminal proceedings.

## 8. Exceptions

Any exception to this policy **must** be time-bound (maximum 12 months), risk-assessed,
compensated, and approved using the
[Policy Exception Request](../templates/policy-exception-request.md) form (see
[Policy Framework §5](../docs/policy-framework.md)).

## 9. Review

The CISO reviews this policy at least annually and upon any material change. Reviews and changes
follow the lifecycle in [CONTRIBUTING](../CONTRIBUTING.md) and require Governance Board approval.

## 10. Control Mapping

| Framework | Controls |
|-----------|----------|
| ISO/IEC 27001:2022 | A.5.1, A.5.2, A.5.4, A.5.37; clauses 5.2, 9.3 |
| SOC 2 TSC | CC1.1–CC1.5, CC2.1–CC2.3, CC5.1 |
| GDPR | Art. 24, Art. 32 |

Full clause-level traceability: [Control-Mapping Matrix](../docs/control-mapping-matrix.md).

## 11. References

- ISO/IEC 27001:2022, *Information security management systems — Requirements*.
- AICPA SOC 2 Trust Services Criteria.
- Regulation (EU) 2016/679 (GDPR).
- [POL-GOV-002](information-security-roles-and-responsibilities.md),
  [DOC-FWK-001](../docs/policy-framework.md),
  [DOC-SCP-001](../docs/scope-statement.md).
