# Access Control Policy

## Document Control

| Field            | Value                              |
|------------------|------------------------------------|
| Document ID      | POL-ACC-003                        |
| Title            | Access Control Policy              |
| Version          | 1.0.0                              |
| Classification   | Public                             |
| Owner (role)     | CISO / Identity & Access Management Lead |
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

This policy establishes the rules for controlling logical access to JOL information, systems, and
services. It implements ISO/IEC 27001:2022 Annex A controls **A.5.15–A.5.18**, **A.8.2**,
**A.8.3**, and **A.8.5**, and SOC 2 Common Criteria **CC6**.

## 2. Scope

Applies to all JOL systems, applications, data stores, infrastructure, and services, and to all
users, service accounts, and third parties that access them, within the
[ISMS scope](../docs/scope-statement.md).

## 3. Definitions

| Term | Meaning |
|------|---------|
| Least privilege | Granting only the access necessary to perform a task, for only as long as needed |
| MFA | Multi-factor authentication |
| Privileged access | Access that can alter systems, data, or security controls |
| Service account | Non-human identity used by a system or workload |
| De-provisioning | Removal of access and identities |

## 4. Roles and Responsibilities

- **CISO / IAM Lead** — owns this policy; defines standards; oversees access governance.
- **Resource owners** — authorise access to their systems and data.
- **Managers** — request, justify, and review access for their teams.
- **All users** — protect their credentials and use only authorised access.

## 5. Principles

Access is granted on the basis of **least privilege**, **need-to-know**, and **fail-safe defaults**.
Identity is verified before access is granted, privileged access is minimised and monitored, and all
access is reviewed and revocable.

## 6. Policy Statements

### 6.1 Access Control Policy and Business Rules

1. Access to JOL information and systems **must** be controlled in accordance with this policy and
   documented business rules approved by resource owners.
2. An access-control standard **must** define technical enforcement (RBAC/ABAC) for each system.
3. Rules **must** reflect data classification (see
   [POL-CLS-006](data-classification-and-handling.md)) and multi-tenant isolation.

### 6.2 Identity Management and Provisioning

1. Each user **must** have a unique identity; shared accounts **must not** be used except for
   tightly controlled, logged, and approved system accounts.
2. Access **must** be provisioned only after approval by the resource owner and the user's manager,
   and **must** be recorded.
3. Joiner/mover/leaver processes **must** trigger timely provisioning, adjustment, and revocation.

### 6.3 Authentication and Secure Sign-On (MFA)

1. Authentication information (passwords, keys, tokens) **must** be protected, stored using strong
   cryptographic mechanisms, and never shared or logged in plaintext.
2. **MFA must** be enforced for all remote access, all privileged access, and all access to
   production systems.
3. Password standards **must** enforce sufficient length/complexity and screening against breached
   credentials; secrets **must** be stored in an approved vault (see `jol-secrets`), never in source
   control.

### 6.4 Least Privilege and Privileged Access

1. Access **must** be the minimum necessary for the role and time-bounded where possible.
2. Privileged access **must** be granted just-in-time, separately from standard accounts, logged,
   and monitored.
3. Access to information **must** be restricted in line with classification and need-to-know;
   default-deny **must** apply.

### 6.5 Access Review and De-provisioning

1. Access rights **must** be reviewed at defined intervals (at least quarterly for privileged
   access, at least annually otherwise) and upon role change.
2. Access **must** be revoked immediately on termination or when no longer required, coordinated
   with the leaver process in [POL-AUP-005 §6.2](acceptable-use-policy.md).
3. Reviews and revocations **must** be recorded as control evidence (see `jol-compliance-evidence`).

## 7. Enforcement and Sanctions

Unauthorised access, credential sharing, or abuse of privilege is a policy breach under
[POL-ISM-001 §7](information-security-policy.md) and may result in disciplinary or legal action.

## 8. Exceptions

Exceptions **must** be time-bound, risk-assessed, compensated, and approved via the
[Policy Exception Request](../templates/policy-exception-request.md) form.

## 9. Review

The CISO / IAM Lead reviews this policy at least annually and upon material change to systems,
identity tooling, or threat landscape.

## 10. Control Mapping

| Framework | Controls |
|-----------|----------|
| ISO/IEC 27001:2022 | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.5 |
| SOC 2 TSC | CC6.1, CC6.2, CC6.3, CC6.4, CC6.5, CC6.7, CC6.8 |
| GDPR | Art. 5(1)(f), Art. 25, Art. 32 |

Full clause-level traceability: [Control-Mapping Matrix](../docs/control-mapping-matrix.md).

## 11. References

- ISO/IEC 27001:2022 Annex A.5.15–A.5.18, A.8.2, A.8.3, A.8.5.
- AICPA SOC 2 TSC CC6.
- GDPR Art. 5(1)(f), 25, 32.
- [POL-CLS-006](data-classification-and-handling.md), [POL-AUP-005](acceptable-use-policy.md).
