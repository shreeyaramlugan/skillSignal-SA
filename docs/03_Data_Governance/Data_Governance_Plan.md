# SkillSignal SA — Data Governance Plan

| Document Attribute | Details |
|---|---|
| Project Name | SkillSignal SA |
| Project ID | SSA-001 |
| Document | Data Governance Plan |
| Document Location | `docs/03_Data_Governance/Data_Governance_Plan.md` |
| Version | 2.0 |
| Status | Approved — Section B Finalised |
| Ownership | Individual project |
| Budget | R0 |
| Research Period | 1 November 2025 – 31 October 2026 inclusive |
| Publication Model | Public aggregate findings and permitted materials |
| Raw Data Access | Private; restricted where source conditions require |
| Related Documents | Research Design; Sampling Strategy; Data Dictionary; Statistical Methodology; Data Retention and Access; Data Source Register |

---

## 1. Purpose

This document defines the data-governance principles and operational requirements for SkillSignal SA.

It establishes how research data must be sourced, acquired, documented, processed, stored, accessed, analysed, published and retained.

The governance framework supports:

- Responsible data acquisition.
- Source provenance.
- Respect for source terms and access restrictions.
- Data minimisation.
- Raw-data preservation.
- Data quality and traceability.
- Restricted access to raw and sensitive material.
- Aggregate public reporting.
- Reproducibility.
- Transparent limitations.
- Responsible disposal and retention.

The purpose is to ensure that the project produces useful technology labour-market intelligence without treating publicly accessible information as automatically unrestricted for collection, redistribution or publication.

## 2. Governance Objectives

SkillSignal SA adopts the following governance objectives:

1. Acquire information through approved and permitted methods.
2. Maintain traceable provenance for collected advertisements.
3. Preserve original source information where permitted.
4. Minimise unnecessary personal and confidential information.
5. Keep restricted raw data private.
6. Publish aggregate findings and materials that may legitimately be shared.
7. Maintain data quality and classification traceability.
8. Prevent unauthorised disclosure or redistribution.
9. Maintain reproducible processing and analysis.
10. Document limitations and governance decisions.
11. Apply retention and disposal requirements consistently.
12. Ensure that public outputs do not misrepresent the underlying dataset.

---

## 3. Governance Principles

### 3.1 Responsible acquisition

Information must only be acquired through sources and methods that are approved for the project.

Public accessibility does not automatically establish permission for unrestricted automated extraction, storage or redistribution.

### 3.2 Purpose limitation

Data collection must support the approved research objectives.

Information unrelated to the analysis must not be collected or retained without a documented justification.

### 3.3 Data minimisation

Collect only the information reasonably necessary to:

- Establish advertisement eligibility.
- Preserve provenance.
- Classify opportunities.
- Extract relevant job requirements.
- Conduct approved analyses.
- Validate research outputs.

Unnecessary personal information must not be collected.

### 3.4 Provenance and accountability

Each analytical record must be traceable to its source and collection process to the extent permitted.

Material transformations, exclusions and classification decisions must be documented.

### 3.5 Integrity and transparency

Raw source values must be distinguishable from standardised and derived values.

Research findings must accurately reflect the collected data and its limitations.

### 3.6 Controlled publication

Public outputs must use aggregate findings and other materials that are permitted for publication.

Raw data must not be published merely because the underlying advertisement was publicly accessible.

### 3.7 Reproducibility

Data-processing and analytical decisions must be documented sufficiently to support review and reproducibility without disclosing restricted source content.

---

## 4. Data Classification

### 4.1 Classification framework

SkillSignal SA uses the following logical data classifications.

| Classification | Description | Access and Publication |
|---|---|---|
| Public | Approved material intended for public release. | May be published following review. |
| Internal | Project documentation, non-sensitive processing information and internal working material. | Restricted to authorised project access. |
| Restricted | Raw advertisements, source evidence or other information subject to access or redistribution restrictions. | Private; access limited to authorised use. |
| Confidential / Sensitive | Information that could expose personal, confidential or otherwise protected information. | Avoid collection where unnecessary; tightly restrict any unavoidable handling. |

These are project governance classifications. They do not replace source-specific conditions or applicable legal requirements.

### 4.2 Examples

| Data | Suggested Classification |
|---|---|
| Public research methodology | Public, if approved for release |
| Aggregate skill-frequency charts | Public, after disclosure review |
| Aggregate job-family comparisons | Public, after disclosure review |
| Approved public research report | Public |
| Raw advertisement text | Restricted where source conditions require |
| Source URLs and acquisition evidence | Internal or restricted, depending on source conditions |
| Candidate acquisition records | Internal or restricted |
| Duplicate-review evidence | Internal or restricted |
| Raw extracted datasets | Restricted where source conditions require |
| Cleaned analytical datasets | Internal or restricted, depending on source rights |
| Internal data-quality reports | Internal |
| Credentials and access tokens | Confidential / Sensitive |
| Unnecessary recruiter or contact personal information | Must not be collected or retained |

Classification must be determined according to the actual content, source conditions and intended use.

---

## 5. Data Sources and Acquisition Governance

### 5.1 Source approval

Potential sources include:

- Public recruitment platforms.
- Employer career pages.
- Public job listings.
- Other authorised recruitment and employment information sources.

These are candidate source categories, not confirmation that every source has been approved.

Each individual source must be assessed before acquisition.

### 5.2 Source assessment requirements

The source assessment should consider:

- Relevance to the research objectives.
- Geographic coverage.
- Job-family coverage.
- Historical advertisement availability.
- Data reliability.
- Accessibility.
- Terms of use.
- Collection restrictions.
- Redistribution restrictions.
- Privacy considerations.
- Technical feasibility.
- Zero-budget feasibility.

### 5.3 Permitted acquisition

Acquisition must respect applicable source conditions and approved methods.

The project must not assume permission to:

- Bypass access controls.
- Circumvent technical restrictions.
- Access private or restricted accounts.
- Use unauthorised credentials.
- Collect information in violation of source conditions.
- Redistribute content beyond permitted use.

Where the permission status or acquisition method is uncertain, acquisition must be deferred until the issue is resolved.

### 5.4 Source register

The Data Source Register must document the approved source inventory and its assessment.

Relevant information should include:

- Source name.
- Source category.
- Source location or URL.
- Geographic relevance.
- Research-period coverage.
- Source assessment.
- Access method.
- Permission or terms assessment.
- Acquisition status.
- Restrictions.
- Notes and limitations.

A source must not be represented as approved merely because it appears in the register as a candidate.

### 5.5 Acquisition records

Each collection batch must preserve sufficient permitted metadata to identify:

- Source.
- Acquisition method.
- Collection date.
- Search criteria.
- Collection batch.
- Collection purpose.
- Candidate volume.
- Eligibility outcomes.
- Duplicate outcomes.
- Exclusion reasons.

The physical implementation of acquisition logs remains subject to technical design.

---

## 6. Research Scope and Data Eligibility

### 6.1 Research period

The approved research period is:

**1 November 2025 to 31 October 2026 inclusive.**

The original publication date determines eligibility.

Collection date, first-seen date and closing date must remain separate.

Advertisements discovered after the end of the research period may qualify if their original publication date can be credibly verified within the approved period.

### 6.2 Geographic eligibility

The research covers:

- All nine South African provinces.
- Major cities and smaller towns.
- On-site opportunities.
- Hybrid opportunities.
- Remote opportunities.
- Qualifying international remote opportunities explicitly open to candidates working in South Africa.

### 6.3 Employment eligibility

Qualifying employment types include:

- Permanent.
- Fixed-term.
- Temporary.
- Graduate programmes.
- Graduate positions.
- Internships.
- Learnerships.
- Apprenticeships.
- Part-time.
- Genuine paid freelance.
- Project-based contracts.

Volunteer positions, unpaid speculative projects and training without an employment opportunity are excluded.

### 6.4 Job-family eligibility

Advertisements must fall within at least one of the seven approved job families:

| Code | Job Family |
|---|---|
| JF01 | Software Development |
| JF02 | Data and Analytics |
| JF03 | Cybersecurity |
| JF04 | IT Infrastructure and Support |
| JF05 | Cloud and DevOps |
| JF06 | Quality Assurance and Testing |
| JF07 | Business Technology |

Advertisements may receive multiple assignments where justified by their responsibilities and requirements.

### 6.5 Eligibility governance

- Missing salary information does not disqualify an advertisement.
- Missing qualification information does not disqualify an advertisement.
- Missing experience information does not disqualify an advertisement.
- Missing skills information does not automatically disqualify an advertisement.
- Uncertain date, location or eligibility information must be reviewed.
- Exclusions must have documented reasons.
- Prohibited acquisition must not be used to improve sample coverage.

---

## 7. Data Lifecycle Governance

### 7.1 Lifecycle stages

The project applies governance controls throughout the following lifecycle:

1. Source discovery.
2. Source assessment and approval.
3. Candidate acquisition.
4. Provenance recording.
5. Eligibility assessment.
6. Duplicate review.
7. Raw data handling.
8. Cleaning and standardisation.
9. Classification and extraction.
10. Validation and quality review.
11. Analytical dataset preparation.
12. Statistical analysis.
13. Aggregate reporting.
14. Retention and disposal.

### 7.2 Raw data

Raw source information must be preserved where permitted and distinguishable from later processing.

Raw information must not be silently overwritten by standardised or derived values.

Where source restrictions prevent retention of certain content, the project must retain only the permitted information needed for provenance and auditability.

### 7.3 Standardised data

Standardisation must follow documented rules.

Examples include:

- Normalised job titles.
- Standardised employer names.
- Job-family assignments.
- Skill names.
- Qualification categories.
- Experience categories.
- Geographic classifications.
- Employment-type classifications.

The original source wording must remain distinguishable wherever retention is permitted.

### 7.4 Derived data

Derived variables must have documented definitions and calculation rules.

Examples include:

- Publication month.
- Publication quarter.
- Salary disclosure flag.
- Graduate accessibility classification.
- Skill prevalence.
- Advertisement counts.
- Statistical summaries.

Derived values must not be presented as direct source observations.

### 7.5 Analytical datasets

Analytical datasets must be created from eligible canonical advertisements.

They must retain the information needed to:

- Identify the relevant dataset version.
- Reproduce the analysis.
- Understand exclusions.
- Validate classifications.
- Trace analytical results to their underlying records where permitted.

### 7.6 Publication datasets

Public outputs should contain only approved aggregate results or other material that has passed publication review.

Restricted raw records must not be embedded in public dashboards, reports, repositories or downloadable files.

---

## 8. Access Control and Data Security

### 8.1 Access model

The project is individually owned and managed.

Access must remain limited to the project owner and any explicitly authorised administrators or collaborators, if such access is later introduced.

Raw and restricted data must not be made publicly accessible.

### 8.2 Access principles

- Grant access only where necessary.
- Avoid public access to raw data.
- Separate public outputs from restricted working data.
- Avoid embedding credentials in source code or documentation.
- Do not commit secrets or access tokens to version control.
- Restrict access to source evidence where required.
- Review access if project ownership or collaboration arrangements change.

### 8.3 Security safeguards

The implementation should provide appropriate safeguards for:

- Local project files.
- Stored datasets.
- Backups.
- Credentials.
- Remote repositories.
- Analytical environments.
- Public dashboards and exports.

Specific technical controls, encryption choices, backup mechanisms and access-control implementations remain subject to technical implementation decisions.

### 8.4 Unauthorised access or disclosure

If restricted information is accidentally exposed:

1. Stop further disclosure where feasible.
2. Restrict access to the affected material.
3. Identify the affected records and information.
4. Assess the source conditions and potential impact.
5. Preserve relevant incident details.
6. Take corrective action.
7. Document the incident and resolution.
8. Review whether the governance process requires changes.

Any notification obligations must be assessed against applicable requirements and the circumstances of the incident.

---

## 9. Privacy and Personal Information

### 9.1 Data minimisation

The research focuses on advertised job opportunities, not applicants, employees or recruiters as individuals.

Personal information must not be collected unless genuinely necessary for an approved research or operational purpose.

### 9.2 Personal information safeguards

- Avoid collecting recruiter contact details.
- Avoid collecting applicant information.
- Avoid collecting personal identifiers unrelated to the research.
- Avoid retaining personal information included incidentally in advertisement content.
- Remove or exclude unnecessary personal information from analytical and public outputs.
- Restrict unavoidable personal information.
- Follow applicable retention and access requirements.

### 9.3 Employer and recruiter information

Employer identity may be relevant to the analysis, but recruiter identity is not automatically relevant.

The project must distinguish:

- Employer organisation.
- Recruitment agency.
- Individual recruiter or contact person.

Where an advertisement is posted by an agency, the identity of the actual hiring organisation may remain unknown.

### 9.4 Privacy review

Before publication, review outputs for:

- Personal information.
- Confidential employer information.
- Restricted source content.
- Small-cell disclosure risks.
- Unintended identification through combinations of variables.

---

## 10. Data Quality and Integrity Governance

### 10.1 Quality objectives

Data quality must be managed throughout acquisition and processing.

The project should assess:

- Accuracy.
- Completeness.
- Consistency.
- Validity.
- Uniqueness.
- Timeliness.
- Provenance.
- Classification confidence.

### 10.2 Validation requirements

Validation should cover:

- Research-period eligibility.
- Geographic eligibility.
- Job-family eligibility.
- Employment-type eligibility.
- Canonical-record status.
- Duplicate relationships.
- Date validity.
- Numeric salary values.
- Currency and remuneration period.
- Skill classification.
- Qualification classification.
- Experience classification.
- Geographic classification.
- Employment classification.

### 10.3 Missing and conflicting information

Use the approved data-status vocabulary:

- `observed`
- `extracted`
- `standardised`
- `derived`
- `not_stated`
- `not_applicable`
- `unclear`
- `conflicting`
- `not_verified`
- `not_processed`

Missing information must not be interpreted as a negative value.

Conflicting evidence must be documented and reviewed.

### 10.4 Manual review

Manual review must be used where automated processing cannot reliably establish:

- Eligibility.
- Publication date.
- Duplicate status.
- Job-family assignment.
- Skill equivalence.
- Qualification level.
- Experience requirements.
- Salary interpretation.
- Geographic eligibility.
- Employment type.

Manual corrections must be traceable.

### 10.5 No silent changes

Changes to classifications, standardisation rules or source records must be documented.

Where a material correction affects analysis, the relevant analytical output must be reviewed or regenerated.

---

## 11. Duplicate and Canonical Record Governance

### 11.1 Approved approach

One unique advertised opportunity must have one canonical analytical record.

The same opportunity may appear on multiple sources or be reposted.

### 11.2 Duplicate handling

- Preserve permitted source provenance.
- Identify potential duplicate groups.
- Retain duplicate evidence.
- Establish a canonical record.
- Link duplicate publication instances.
- Record material changes.
- Preserve repost information.
- Review uncertain cases manually.

### 11.3 Distinct opportunities

Similar advertisements must not automatically be merged.

Different vacancies may share:

- Employer.
- Job title.
- Description.
- Source.
- Location.

A separate record is required where evidence supports a genuinely different opportunity.

### 11.4 Counting safeguards

Duplicate publication instances must not inflate unique advertisement counts.

Multiple family, skill, qualification or location relationships must not be confused with additional advertisements.

---

## 12. Retention, Archiving and Disposal

### 12.1 General principle

Data must be retained only for as long as justified by the approved research, audit, reproducibility and governance requirements, subject to source restrictions and applicable obligations.

### 12.2 Retention requirements

The project must distinguish between:

- Raw advertisement content.
- Source evidence.
- Provenance metadata.
- Standardised records.
- Derived analytical data.
- Statistical outputs.
- Public reports.
- Internal documentation.
- Credentials and access information.

Different categories may require different retention treatment.

### 12.3 Source restrictions

Where a source restricts storage or retention:

- Respect the applicable restriction.
- Avoid retaining prohibited content.
- Preserve permitted provenance metadata where possible.
- Ensure downstream analytical use remains within permitted conditions.
- Review whether the source can continue to support the research.

### 12.4 Retention schedule

Exact retention periods and disposal procedures are governed by the separate Data Retention and Access document.

This plan does not introduce a new fixed retention period.

### 12.5 Disposal

When information reaches the end of its approved retention period or must be removed:

- Identify the affected information.
- Apply the approved disposal procedure.
- Consider copies and backups.
- Preserve only information that may legitimately be retained.
- Document disposal where required.

---

## 13. Publication and Disclosure Governance

### 13.1 Approved publication model

The project adopts public aggregate findings and permitted materials.

The following may be considered for publication after review:

- Aggregate skill frequencies.
- Job-family comparisons.
- Qualification and experience summaries.
- Geographic distributions.
- Salary disclosure rates.
- Comparable aggregate salary summaries.
- Employment-type distributions.
- Work-arrangement summaries.
- Temporal summaries.
- Research methodology.
- Data-quality and limitations statements.
- Approved visualisations and dashboard outputs.

### 13.2 Restricted publication material

The following must not be published unless a clear permission or other valid basis allows it:

- Restricted raw advertisement text.
- Restricted source extracts.
- Personal information.
- Confidential employer information.
- Credentials or access tokens.
- Unauthorised source data.
- Restricted datasets or downloadable exports.

### 13.3 Aggregate disclosure review

Before publication, review:

- Small group sizes.
- Rare combinations of variables.
- Potential identification of individuals.
- Potential identification of confidential opportunities.
- Source redistribution restrictions.
- Whether the output reveals restricted raw information.
- Whether the result could be misleading due to missingness or sample limitations.

No universal small-cell suppression threshold is approved at this stage.

The publication review must assess the actual disclosure risk and document the decision.

### 13.4 Statistical transparency

Public findings must:

- Identify the relevant research period.
- Explain the accessible sample.
- Distinguish advertisements from actual hires.
- Disclose multi-family assignment.
- State denominators.
- Describe material missingness.
- Identify source and sampling limitations.
- Avoid unsupported causal claims.
- Avoid unsupported claims of market representativeness.

### 13.5 Dashboard governance

An interactive dashboard must use approved publication-ready data.

It must not expose restricted raw records through:

- Visible tables.
- Drill-down interactions.
- Download functions.
- API responses.
- Embedded source content.
- Hidden client-side data.

The dashboard must be checked for accidental disclosure before public release.

---

## 14. Research Reproducibility and Version Control

### 14.1 Reproducibility objectives

The project must be able to explain how a published result was produced from the available permitted data and documented processing rules.

### 14.2 Versioning requirements

Maintain traceability for:

- Dataset versions.
- Source register versions.
- Job-family taxonomy.
- Skill taxonomy.
- Qualification taxonomy.
- Experience categories.
- Standardisation rules.
- Processing scripts.
- Statistical analysis.
- Report outputs.

### 14.3 Analytical traceability

Each material output should identify:

- Research question.
- Dataset version.
- Relevant variables.
- Transformation rules.
- Analytical method.
- Relevant limitations.
- Output version.

### 14.4 Restricted data and version control

Restricted raw data must not be committed to a public repository.

Repository documentation and source code must not expose:

- Secrets.
- Credentials.
- Restricted source content.
- Unauthorised data exports.
- Personal information.

Public repository content should contain approved documentation, code and permitted aggregate outputs.

---

## 15. Governance Roles and Responsibilities

### 15.1 Project ownership

SkillSignal SA is an individual project.

The project owner is responsible for:

- Source assessment.
- Acquisition decisions.
- Governance compliance.
- Data quality.
- Access control.
- Retention and disposal.
- Analytical integrity.
- Publication review.
- Documentation.
- Change management.

### 15.2 Future collaborators

If collaborators or administrators are introduced:

- Their responsibilities must be documented.
- Access must be limited to their role.
- Restricted information must remain controlled.
- Source restrictions must be communicated.
- Any new access arrangement must be reviewed.

No additional project owner, data controller, external reviewer or administrator is assumed by this document.

---

## 16. Governance Risk Register

| ID | Risk | Potential Impact | Governance Response |
|---|---|---|---|
| DG-R01 | Source terms do not permit intended acquisition. | Unauthorised collection or use. | Assess and document source permissions before acquisition. |
| DG-R02 | Public source content is redistributed without permission. | Breach of source restrictions. | Publish only permitted materials and approved aggregates. |
| DG-R03 | Raw data is exposed publicly. | Unauthorised disclosure. | Restrict raw-data access and review publication outputs. |
| DG-R04 | Personal information is collected unnecessarily. | Privacy risk. | Apply data minimisation and remove unnecessary personal information. |
| DG-R05 | Source provenance is incomplete. | Reduced traceability and reproducibility. | Maintain source and batch metadata. |
| DG-R06 | Duplicate advertisements inflate counts. | Misleading statistical findings. | Use canonical records and duplicate review. |
| DG-R07 | Incorrect classifications affect analysis. | Misleading findings. | Maintain evidence, confidence and manual review. |
| DG-R08 | Missing data is treated as a negative value. | Incorrect interpretation. | Use explicit missing-data statuses. |
| DG-R09 | Historical dates are unreliable. | Incorrect research-period inclusion. | Verify publication dates and document uncertainty. |
| DG-R10 | Restricted information enters public dashboards. | Unauthorised disclosure. | Use publication-ready datasets and disclosure review. |
| DG-R11 | Retention restrictions are overlooked. | Unauthorised continued storage. | Apply the Data Retention and Access schedule. |
| DG-R12 | Analytical outputs cannot be reproduced. | Reduced research credibility. | Version datasets, taxonomies, scripts and outputs. |
| DG-R13 | Small groups enable indirect identification. | Disclosure of sensitive or confidential information. | Review small-cell and variable-combination disclosure risks. |
| DG-R14 | Source availability creates coverage bias. | Misleading market interpretation. | Document source coverage and sampling limitations. |

---

## 17. Governance Monitoring and Review

Governance should be reviewed at relevant project milestones.

### 17.1 Source review

Confirm:

- Source approval status.
- Permission and access conditions.
- Acquisition method.
- Source restrictions.
- Coverage limitations.

### 17.2 Data processing review

Confirm:

- Raw data preservation where permitted.
- Standardisation traceability.
- Duplicate handling.
- Missing-data treatment.
- Manual review records.
- Data-quality issues.

### 17.3 Analytical review

Confirm:

- Dataset version.
- Variable definitions.
- Denominators.
- Statistical method suitability.
- Treatment of overlapping categories.
- Limitations.

### 17.4 Publication review

Confirm:

- Aggregate-only publication model.
- Permitted source use.
- Personal information minimisation.
- Small-cell disclosure review.
- No restricted raw data.
- Accurate methodological limitations.

### 17.5 Change review

Material changes to:

- Sources.
- Acquisition methods.
- Data categories.
- Retention.
- Access permissions.
- Publication practices.
- Statistical reporting.

must be documented and assessed for their effect on governance and research validity.

---

## 18. Confirmed Decisions and Unresolved Implementation Matters

### 18.1 Confirmed decisions

The following are approved or established project requirements:

- Individual project ownership.
- Zero-budget constraint.
- Aggregate public publication.
- Private handling of raw data where redistribution is restricted.
- Responsible and permitted data acquisition.
- Source provenance.
- Data minimisation.
- Raw, standardised and derived data separation.
- Canonical advertisement records.
- Duplicate-review traceability.
- Missing-data and classification safeguards.
- Restricted access to raw data.
- Public-output disclosure review.
- Reproducibility and version traceability.
- Governance alignment with the approved research period and seven job families.

### 18.2 Unresolved implementation matters

The following must be confirmed through the relevant project stages:

- Individual source approvals and terms assessments.
- Source-specific retention restrictions.
- Exact retention periods, as governed by the Data Retention and Access document.
- Final technical access controls.
- Encryption and backup implementation.
- Exact security and incident-management procedures.
- Final small-cell disclosure thresholds.
- Physical audit-log implementation.
- Final dashboard publication controls.
- Any future collaborator access arrangements.

These items must not be represented as already implemented or approved.

---

## 19. Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| DG-AC-01 | Governance purpose and objectives are documented. |
| DG-AC-02 | Data classification framework is defined. |
| DG-AC-03 | Responsible acquisition and source approval requirements are documented. |
| DG-AC-04 | Source restrictions and redistribution considerations are explicit. |
| DG-AC-05 | Research-period and eligibility governance align with the approved research design. |
| DG-AC-06 | Raw, standardised and derived data are governed separately. |
| DG-AC-07 | Access-control requirements protect restricted data. |
| DG-AC-08 | Privacy and data-minimisation requirements are documented. |
| DG-AC-09 | Data-quality and integrity controls are defined. |
| DG-AC-10 | Duplicate and canonical-record governance is documented. |
| DG-AC-11 | Retention and disposal are aligned with the separate retention document. |
| DG-AC-12 | Aggregate publication requirements are explicit. |
| DG-AC-13 | Dashboard and public-output disclosure risks are addressed. |
| DG-AC-14 | Reproducibility and version-control requirements are documented. |
| DG-AC-15 | Individual ownership and responsibilities are defined. |
| DG-AC-16 | Governance risks and responses are documented. |
| DG-AC-17 | Monitoring and review requirements are included. |
| DG-AC-18 | Confirmed decisions are distinguished from unresolved implementation matters. |

---

## 20. Approval and Document Control

This document consolidates the approved governance implications arising from Section B.

It establishes the governance requirements for data acquisition, processing, access, analysis, retention and publication.

Source-specific permissions, retention periods and technical controls must be confirmed through their respective project documents and implementation decisions.

**Approval Status:** Approved — Section B Finalised

**Document Status:** Ready for incorporation into the SkillSignal SA repository following review and acceptance.