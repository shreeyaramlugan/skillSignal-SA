# SkillSignal SA — Data Governance Plan

**Project ID:** SSA-001
**Document ID:** SSA-DOC-005
**Version:** 0.1
**Status:** Initial baseline — subject to refinement
**Related document:** Section A — Project Foundation

---

## 1. Purpose

This document establishes the governance principles and operational
controls for data used in SkillSignal SA.

The project investigates advertised technology employment demand
in South Africa over a 12-month research window.

Data governance supports responsible acquisition, data quality,
provenance, reproducibility, statistical integrity and responsible
publication.

## 2. Governance Principles

1. Evidence over assumptions.
2. Data quality over quantity.
3. Reproducibility over convenience.
4. Full data provenance.
5. Transparent limitations.
6. Responsible data acquisition.
7. Statistical integrity.
8. No fabricated findings.
9. Zero-budget implementation.
10. Publication of aggregated findings and permitted materials only.

## 3. Data Classification

| Classification | Description | Intended handling |
|---|---|---|
| Raw | Original acquired records and source material | Restricted; preserve where permitted |
| Interim | Data undergoing extraction, cleaning or transformation | Controlled working access |
| Processed | Standardised and validated analytical records | Controlled project access |
| Reference | Approved taxonomies, mappings and supporting reference material | Retain provenance and applicable licence details |
| Published | Approved aggregate tables, figures and research outputs | Public release subject to review |

## 4. Data Acquisition

Every potential source must be assessed before acquisition.

The assessment must consider:
- Source identity and ownership.
- Access method and technical restrictions.
- Terms of service and applicable permissions.
- Copyright and database rights considerations.
- Personal information and privacy risks.
- Permitted storage, processing and retention.
- Whether derived aggregate findings may be published.

The final source list and acquisition methods remain subject to
Section C.

No source is automatically approved merely because its content
is publicly accessible.

## 5. Provenance Requirements

Where available, acquired records should be traceable to:
- Source name and source identifier.
- Original source URL or record reference.
- Acquisition timestamp.
- Acquisition method.
- Original publication date.
- Processing date.
- Transformation history.
- Relevant permission or restriction notes.

Credentials, access tokens and private account information
must not be stored in source code or published repository files.

## 6. Data Quality Controls

The processing pipeline should assess:
- Missing mandatory fields.
- Invalid dates and values.
- Duplicate advertisements.
- Inconsistent job titles and locations.
- Inconsistent employment and seniority classifications.
- Invalid or malformed records.
- Unusable or incomplete records.
- Transformation and extraction errors.

Quality checks, exclusions and their reasons must be recorded.

## 7. Privacy and Personal Information

The project should collect only information necessary for its
research objectives.

Personal information must not be unnecessarily collected,
retained or exposed.

Personal information must not be included in public outputs.
Where a dataset contains unnecessary personal information,
the project should exclude or appropriately remove it before
analytical use, subject to applicable requirements.

## 8. Storage and Access

- Raw data must remain private where redistribution is not permitted.
- Restricted data must not be committed to public Git repositories.
- Interim and processed datasets must be managed separately.
- Access should be limited to the project owner.
- Credentials and secrets must remain outside version control.
- Public repository contents must be reviewed before publication.

## 9. Publication Controls

Public outputs may include:
- Aggregated statistical findings.
- Approved visualisations.
- Research methodology.
- Permitted code and documentation.
- Non-restricted reference materials.

Public outputs must not expose restricted raw records,
unnecessary personal information, credentials or material
that cannot legally or contractually be redistributed.

## 10. Reproducibility

The project should preserve:
- Version-controlled source code.
- Documented transformation procedures.
- Classification and taxonomy versions.
- Data-quality rules.
- Research methodology.
- Analytical assumptions.
- Relevant software dependencies.

Results must be traceable to the methodology and permitted
underlying data.

## 11. Governance Responsibilities

The individual project owner is responsible for:
- Evaluating data sources.
- Recording acquisition decisions.
- Applying access restrictions.
- Maintaining data provenance.
- Reviewing quality controls.
- Protecting restricted material.
- Reviewing public outputs.

## 12. Outstanding Governance Decisions

The following remain open:
- Final data sources and acquisition permissions.
- Source-specific retention periods.
- Final dataset schema.
- Final data-quality thresholds.
- Final anonymisation or exclusion procedures, where applicable.
- Database access and backup implementation.

These decisions must be resolved in the relevant project sections.

## 13. Review

This document must be reviewed when material changes occur to
data sources, acquisition methods, processing, storage or publication.

---
**Status note:** This is the initial governance baseline. It does not
constitute approval of any specific external data source.
