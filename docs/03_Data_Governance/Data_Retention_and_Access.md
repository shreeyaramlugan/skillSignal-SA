# SkillSignal SA — Data Retention and Access Policy

**Project ID:** SSA-001
**Document ID:** SSA-DOC-008
**Version:** 0.1
**Status:** Initial policy — source-specific rules pending

---

## 1. Purpose

This policy describes how project data should be accessed,
stored, retained and reviewed.

It supports the approved requirement that public outputs contain
aggregated findings and permitted materials only.

## 2. Access Principles

- The individual project owner is the authorised project user.
- Restricted raw data must remain private.
- Credentials must never be committed to version control.
- Access to restricted material must be limited to what is necessary.
- Public repository contents must be reviewed before release.

## 3. Data Storage Categories

| Data category | Project location | Access |
|---|---|---|
| Raw | data/raw/ | Private and restricted |
| Interim | data/interim/ | Project owner |
| Processed | data/processed/ | Project owner; release only after review |
| External | data/external/ | Subject to source terms and restrictions |
| Reference | data/reference/ | Subject to applicable permissions |
| Published outputs | reports/final/ | Approved public materials only |

The directory location does not override a source's legal,
contractual or licensing restrictions.

## 4. Retention Rules

No universal retention period is approved at this stage.

Before retaining acquired material, record:
- Applicable source terms.
- Permission or licence conditions.
- Required retention period, if specified.
- Deletion or renewal requirements.
- Whether derived data may be retained.
- Whether aggregate publication is permitted.

Where source conditions require deletion or restrict retention,
those conditions take precedence.

## 5. Deletion and Review

When data is no longer permitted or necessary:
- Stop using the affected material.
- Identify dependent interim and processed records.
- Review whether derived outputs are also affected.
- Delete or restrict material as required.
- Record the action and reason in project documentation.

Deletion must consider local copies and relevant backups.

## 6. Publication Review

Before any public release, verify that:
- No restricted raw data is included.
- No unnecessary personal information is exposed.
- No credentials or secrets are present.
- Source terms permit the material being released.
- Aggregations do not inadvertently expose restricted information.
- Findings are accurately described and limitations disclosed.

## 7. Backups and Version Control

- Do not commit restricted datasets to Git.
- Do not store secrets in notebooks or configuration files.
- Review `.gitignore` before adding data files.
- Keep backup arrangements consistent with source restrictions.
- Do not assume that Git history is an appropriate data-retention mechanism.

## 8. Outstanding Decisions

The following remain pending:
- Source-specific retention periods.
- Backup implementation.
- Database access controls.
- Data deletion procedures for each source.
- Long-term storage arrangements.
- Legal and contractual review of each source.

---
**Status note:** This policy establishes a baseline. It does not
authorise indefinite retention or redistribution of acquired data.
