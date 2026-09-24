# Contributing to JOL Policies

This repository contains the **Journey of Life (JOL) ISMS policy suite** — a public "trust"
repository. Contributions here change the security and compliance commitments JOL makes to its
member institutions, customers, auditors, and regulators, so they follow a controlled, auditable
lifecycle.

Please read [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) and [`SECURITY.md`](SECURITY.md) before
contributing.

## Types of Contribution

| Type | Channel |
|------|---------|
| Propose a policy change | [*Policy Change Request*](.github/ISSUE_TEMPLATE/policy-change-request.yml) issue, then a pull request |
| Report a gap, ambiguity, or missing control mapping | [*Policy Gap or Finding*](.github/ISSUE_TEMPLATE/policy-gap-or-finding.yml) issue |
| Report a security vulnerability | **Private** channel only — see [`SECURITY.md`](SECURITY.md) |
| Fix typos, links, or formatting | Pull request directly |

## Policy Change Lifecycle

1. **Raise an issue** describing the change and its compliance driver (control, audit finding,
   regulatory change, or incident lesson).
2. **Open a draft pull request** against `main` from a branch named `feature/<doc-id>-<summary>`,
   `fix/<doc-id>-<summary>`, or `chore/<summary>`.
3. **Update the document-control block**: bump the policy version, set the new effective date, and
   add a Change-History row.
4. **Update the mapping**: if the change affects control coverage, update
   [`docs/control-mapping-matrix.md`](docs/control-mapping-matrix.md) and the register in
   [`docs/document-control.md`](docs/document-control.md).
5. **Record the release** in [`CHANGELOG.md`](CHANGELOG.md).
6. **Review**: the policy owner (via CODEOWNERS) reviews first; substantive changes additionally
   require JOL Governance Board approval.
7. **Merge**: only after CI passes, reviews are complete, and commits are signed.

## Documentation Standards

- **Markdown lint clean** — run `make lint` (or `make check`) before pushing.
- **Document-Control block required** on every policy (see
  [`templates/policy-template.md`](templates/policy-template.md)).
- **Traceability** — every numbered policy statement must map to a control in the
  control-mapping matrix.
- **Roles, not names** — refer to owners and approvers by role (e.g. "CISO", "Data Protection
  Officer"), never by personal name.
- **Plain, testable statements** — use "must"/"must not" for requirements; avoid ambiguity.
- **Conventional Commits** — e.g. `docs(POL-ACC-003): add MFA requirement for privileged access`.

## Data Protection (GDPR)

This is a **public** repository. Never commit:

- Personal data or real institution/tenant identifiers.
- Credentials, keys, tokens, or other secrets (enforced by `detect-secrets` and GitHub secret
  scanning).
- Internal hostnames, IP addresses, network topology, or vendor contract terms.
- Real incident details.

Use synthetic examples only. Privacy-specific artefacts (DPIAs, records of processing) belong in
the `jol-privacy` repository and are **linked**, not duplicated.

## Local Quality Checks

```bash
make install   # install pre-commit + detect-secrets into .venv
make check     # run the full pre-commit suite against all files
make lint      # markdown lint only
make links     # link check only
make secrets   # secret scan against the baseline
```

## Licence

By contributing, you agree that your contributions will be licensed under
[CC-BY-4.0](LICENSE), consistent with the rest of the policy suite.
