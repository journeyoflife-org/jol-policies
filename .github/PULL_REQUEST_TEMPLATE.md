<!-- markdownlint-disable-file MD041 -->
<!--
Thank you for contributing to the JOL ISMS policy suite.
Substantive changes require policy-owner review and JOL Governance Board approval.
-->

## Summary

<!-- What does this pull request change, and why? Reference the driving issue. -->

Closes #<!-- issue number -->

## Type of Change

- [ ] New policy or major revision (version bump required)
- [ ] Minor revision / clarification
- [ ] Control-mapping update
- [ ] Editorial (typos, links, formatting)
- [ ] Tooling / CI

## Compliance Impact

<!-- List the control identifiers affected. Leave blank if editorial only. -->

| Framework | Control(s) |
|-----------|------------|
| SOC 2 | e.g. CC6.1 |
| ISO/IEC 27001:2022 | e.g. A.5.15 |
| GDPR | e.g. Art. 32 |

## Checklist

- [ ] Document-Control block updated (version, effective date, Change History) for each policy touched.
- [ ] `docs/control-mapping-matrix.md` updated if control coverage changed.
- [ ] `docs/document-control.md` register updated.
- [ ] `CHANGELOG.md` entry added.
- [ ] `make check` passes locally (markdownlint, detect-secrets, whitespace/tabs).
- [ ] No secrets, credentials, personal data, internal hostnames, or tenant identifiers included.
- [ ] Owners/approvers referenced by **role**, not personal name.
- [ ] Commits are signed (GPG/SSH) and follow Conventional Commits.

## Reviewer Notes

<!-- Anything a reviewer should focus on; open questions; links to evidence. -->
