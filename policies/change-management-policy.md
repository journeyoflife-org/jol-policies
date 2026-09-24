# Change Management Policy

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | POL-CHG-004                        |
| Title            | Change Management Policy           |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | Head of DevOps / Change Advisory Board |
| Approver (role)  | JOL Governance Board               |
| Effective Date   | 2026-09-24                         |
| Last Review      | 2026-09-24                         |
| Next Review      | 2027-09-24                         |
| Review Cycle     | Annual, or upon material change    |

### Change History

| Version | Date       | Author (role) | Summary of Change    | Approved By (role) |
|---------|------------|---------------|----------------------|--------------------|
| 1.0.0   | 2026-09-24 | Head of DevOps | Initial release     | JOL Governance Board |

## 1. Purpose

This policy governs how changes to JOL systems, services, infrastructure, and security controls are
requested, assessed, authorised, tested, deployed, and reviewed. It implements ISO/IEC 27001:2022
Annex A controls **A.8.32**, **A.8.9**, **A.8.29**, **A.8.31**, and **A.5.37**, and SOC 2 Common
Criterion **CC8.1**.

## 2. Scope

Applies to all changes affecting production systems, shared services, infrastructure-as-code,
security controls, and anything processing member-institution or personal data, within the
[ISMS scope](../docs/scope-statement.md).

## 3. Definitions

| Term | Meaning |
|------|---------|
| Change | Any addition, modification, or removal that affects a system, service, or control |
| Standard change | Pre-authorised, low-risk, repeatable change following a documented procedure |
| Normal change | Requires assessment and authorisation before implementation |
| Emergency change | Urgent change to restore service or remediate a critical risk |
| CAB | Change Advisory Board — authorising body for normal/emergency changes |
| Rollback | Reverting a change to a known-good prior state |

## 4. Roles and Responsibilities

- **Change requester** — raises, documents, and tests the change.
- **CAB** — assesses risk and authorises normal and emergency changes.
- **Head of DevOps** — owns the change process and tooling.
- **CISO** — assesses security impact; **DPO** — assesses data-protection impact (DPIA trigger).
- **Independent approver** — someone other than the implementer (segregation of duties).

## 5. Principles

No unauthorised change reaches production. Changes are risk-assessed, tested, authorised by someone
independent of the implementer, reversible, and recorded. Artefacts are immutable; promotion across
`development → staging → production` is by configuration change, not rebuild.

## 6. Policy Statements

### 6.1 Documented Change Process and Authorisation

1. All changes **must** be recorded in a change-management system with a unique identifier, scope,
   rationale, and risk assessment.
2. Normal and emergency changes **must** be authorised by the CAB (or delegate) **before**
   implementation; standard changes **must** follow a pre-approved documented procedure.
3. Authorisation **must** be independent of implementation (see
   [POL-GOV-002 §6.2](information-security-roles-and-responsibilities.md)).

### 6.2 Risk and Impact Assessment (including DPIA trigger)

1. Each change **must** be assessed for security, operational, and compliance impact before
   authorisation.
2. Changes that introduce or materially alter personal-data processing **must** trigger a DPIA under
   GDPR Art. 35, coordinated with the DPO and the `jol-privacy` repository, **before** approval.
3. High-risk changes **must** include a tested rollback plan.

### 6.3 Segregation of Environments and Configuration Management

1. Development, test, and production environments **must** be separated; production data **must not**
   be used in lower environments without approval and masking.
2. Configuration **must** be managed as code, version-controlled, and reviewed (see `jol-iac`);
   undocumented configuration drift **must** be detected and reconciled.

### 6.4 Security Testing Before Release

1. Changes **must** pass automated build, lint, test, and security scans (SAST, dependency, and
   secret scanning) before promotion.
2. Security-relevant changes **must** undergo security review and, where applicable, penetration or
   acceptance testing before release.

### 6.5 Emergency Changes and Rollback

1. Emergency changes **must** be authorised (verbally or asynchronously where necessary), documented,
   and retrospectively ratified by the CAB within 5 business days.
2. A tested rollback **must** be available for changes affecting availability or integrity; failed
   changes **must** be rolled back or remediated promptly.
3. Post-implementation review **must** occur for emergency and failed changes; lessons feed
   improvement (see [POL-ISM-001 §6.3](information-security-policy.md)).

## 7. Enforcement and Sanctions

Unauthorised or unrecorded production changes are a policy breach under
[POL-ISM-001 §7](information-security-policy.md) and may result in disciplinary action.

## 8. Exceptions

Exceptions **must** be time-bound, risk-assessed, and approved via the
[Policy Exception Request](../templates/policy-exception-request.md) form.

## 9. Review

The Head of DevOps and CISO review this policy at least annually and following any failed or
high-impact change.

## 10. Control Mapping

| Framework | Controls |
|-----------|----------|
| ISO/IEC 27001:2022 | A.8.32, A.8.9, A.8.29, A.8.31, A.5.37 |
| SOC 2 TSC | CC8.1, CC3.4, CC4.1, CC5.2, CC7.4 |
| GDPR | Art. 25, Art. 32, Art. 35 |

Full clause-level traceability: [Control-Mapping Matrix](../docs/control-mapping-matrix.md).

## 11. References

- ISO/IEC 27001:2022 Annex A.8.9, A.8.29, A.8.31, A.8.32, A.5.37.
- AICPA SOC 2 TSC CC8.1, CC3.4.
- GDPR Art. 25, 32, 35.
- [POL-GOV-002](information-security-roles-and-responsibilities.md),
  [POL-ISM-001](information-security-policy.md).
