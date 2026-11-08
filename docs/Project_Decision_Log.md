# SkillSignal SA — Project Decision Log

**Project ID:** SSA-001  
**Document ID:** SSA-DOC-002  
**Version:** 2.0  
**Status:** Active — Section A and Section B Decisions Recorded  
**Project:** SkillSignal SA  
**Ownership:** Individual  
**Budget:** R0  
**Baseline Timeline:** 10 weeks  
**Approved Timeline:** 8–12 weeks  

---

## 1. Purpose

This document records decisions affecting the planning, research, architecture, implementation and delivery of SkillSignal SA.

It serves as the central decision register for the project and provides traceability between approved decisions, unresolved proposals and the relevant project documentation.

Confirmed decisions are distinguished from proposals awaiting investigation or approval.

The decision log must:

- Preserve previously approved decisions.
- Record new decisions using unique identifiers.
- Identify the reasoning and implications of significant decisions.
- Distinguish approved requirements from technical proposals.
- Track unresolved matters until they are formally resolved.
- Provide traceability to the relevant project documents.
- Prevent silent changes to approved project scope or methodology.

This document covers the original Section A project decisions and the subsequently approved Section B research and governance decisions.

It is not intended to replace detailed specifications. The relevant research, architecture, governance and implementation documents remain authoritative for their respective technical and methodological details.

---

## 2. Decision Status Definitions

| Status | Meaning |
|---|---|
| Confirmed | Explicitly approved and treated as authoritative. |
| Proposed | Suggested but not yet approved. |
| Pending | Requires further investigation, review or approval. |
| Deferred | Intentionally postponed until a later project stage. |
| Rejected | Considered and explicitly not selected. |
| Superseded | Replaced by a later approved decision. |

A proposed or deferred item must not be treated as an approved project requirement.

Where a decision changes, the original entry must remain in the historical record and be marked as superseded, with a reference to the replacement decision.

---

## 3. Section A — Confirmed Project Decisions

### 3.1 Project Identity and Ownership

| ID | Decision | Approved Value | Status |
|---|---|---|---|
| DEC-001 | Project name | SkillSignal SA | Confirmed |
| DEC-002 | Ownership | Individual | Confirmed |
| DEC-003 | Budget | R0 | Confirmed |
| DEC-004 | Timeline | 8–12 weeks, with a 10-week baseline and optional Weeks 11–12 contingency | Confirmed |
| DEC-005 | Geographic scope | South Africa, including qualifying international remote opportunities | Confirmed |
| DEC-006 | Research window | 12 months, subsequently fixed under Section B as 1 November 2025–31 October 2026 inclusive | Confirmed |
| DEC-007 | Data acquisition | Hybrid acquisition approach | Confirmed |
| DEC-008 | Primary audience | Students and graduates | Confirmed |
| DEC-009 | Publication | Aggregate findings and permitted materials | Confirmed |
| DEC-010 | Technical ambition | Advanced | Confirmed |
| DEC-011 | Product identity | Analytics portfolio and standalone product concept | Confirmed |

### 3.2 Project Positioning

| ID | Decision | Approved Value | Status |
|---|---|---|---|
| DEC-012 | Project ID | SSA-001 | Confirmed |
| DEC-013 | Project tagline | Turning job-market signals into career intelligence. | Confirmed |
| DEC-014 | Secondary audience | Recruiters, employers and educational institutions | Confirmed |
| DEC-015 | Research orientation | Applied, quantitative and analytical | Confirmed |
| DEC-016 | Research principles | Evidence over assumptions, data quality, reproducibility, statistical integrity, responsible acquisition, provenance and transparent limitations | Confirmed |

### 3.3 Project Constraints

| ID | Decision | Approved Value | Status |
|---|---|---|---|
| DEC-017 | Budget constraint | No paid services or infrastructure are assumed; proposed implementation must remain compatible with the R0 budget. | Confirmed |
| DEC-018 | Research integrity | No fabricated records, findings, source permissions or statistical results. | Confirmed |
| DEC-019 | Data publication boundary | Public aggregate findings and other permitted materials; raw data remains private where redistribution is restricted. | Confirmed |
| DEC-020 | Project duration | The 10-week baseline is the planning reference; Weeks 11–12 are contingency rather than mandatory extensions. | Confirmed |

---

## 4. Section B — Research Design and Methodology Decisions

### 4.1 B1 — Research Problem and Justification

**DEC-021 — Research problem**

The following research problem statement is approved:

> There is a need for a structured, evidence-based understanding of the South African technology labour market, particularly the skills, qualifications, experience requirements, employment opportunities, salary transparency and geographic patterns reflected in technology job advertisements. Existing information is fragmented across recruitment platforms and inconsistently presented, limiting the ability of stakeholders to identify and compare meaningful labour-market patterns. SkillSignal SA seeks to address this information gap by developing a reproducible data analytics solution that transforms job advertisement data into accessible technology labour-market intelligence.

**DEC-022 — Research evidence boundary**

Job advertisements are treated as evidence of advertised labour-market demand.

They do not directly establish:

- Actual hiring outcomes.
- The number of people hired.
- The complete number of vacancies in South Africa.
- The full state of the South African technology labour market.

**Status:** Confirmed.

### 4.2 B2 — Research Aim

**DEC-023 — Approved research aim**

> To develop and apply a reproducible data analytics framework for investigating the South African technology labour market through the systematic collection, processing and analysis of technology job advertisements, generating evidence-based insights into skills demand, qualifications, experience requirements, employment opportunities, salary transparency, geographic distribution and temporal trends.

**Status:** Confirmed.

### 4.3 B2 — Research Objectives

**DEC-024 — Approved research objectives**

The following twelve research objectives are confirmed:

| ID | Objective |
|---|---|
| RO-01 | Establish a research framework defining the South African technology labour-market scope, research period, job families and analytical boundaries. |
| RO-02 | Identify, evaluate and document suitable job advertisement sources according to relevance, accessibility, reliability, coverage and permitted use. |
| RO-03 | Acquire a defensible sample using documented and reproducible collection procedures. |
| RO-04 | Design and implement a processing pipeline to clean, standardise, validate and deduplicate acquired records. |
| RO-05 | Develop a structured classification framework for assigning advertisements to seven technology job families. |
| RO-06 | Extract and standardise technical and professional skills, qualifications, experience requirements, salary information, locations and employment characteristics. |
| RO-07 | Analyse the frequency and distribution of advertised skills, differences between job families and commonly requested skill combinations. |
| RO-08 | Investigate qualification, experience and entry-level requirements across selected job families. |
| RO-09 | Examine the geographic distribution and characteristics of advertised opportunities in South Africa. |
| RO-10 | Investigate salary transparency, available salary ranges and differences across relevant job characteristics. |
| RO-11 | Analyse changes and patterns in advertised technology requirements over the selected research period. |
| RO-12 | Develop an interactive labour-market intelligence report and supporting research publication communicating findings, limitations and implications. |

**Status:** Confirmed.

### 4.4 B4 — Research Scope and Boundaries

**DEC-025 — Geographic coverage**

Include all nine South African provinces, major cities and smaller towns, and qualifying on-site, hybrid and remote opportunities.

**DEC-026 — International remote eligibility**

International employers may be included only where advertisements explicitly permit candidates working from South Africa.

Domestic and qualifying international remote opportunities must be distinguishable.

**DEC-027 — Employment types**

Include:

- Permanent positions.
- Fixed-term positions.
- Temporary positions.
- Graduate programmes.
- Graduate positions.
- Internships.
- Learnerships.
- Apprenticeships.
- Part-time positions.
- Genuine paid freelance opportunities.
- Project-based contracts.

**DEC-028 — Exclusions**

Exclude:

- Volunteer positions.
- Unpaid speculative projects.
- Training without an employment opportunity.
- Generic company promotions without a specific vacancy.
- Opportunities outside the research period.
- Opportunities outside the approved job families.
- International roles explicitly excluding South African candidates.
- Invalid or unverifiable records.
- Duplicate copies after review.
- Records acquired through prohibited methods.

**DEC-029 — Missing information**

Missing salary, qualification, experience or skills information does not automatically disqualify an otherwise eligible advertisement.

**DEC-030 — Multi-family classification**

An advertisement may be assigned to more than one job family when its responsibilities and requirements support the assignments.

**DEC-031 — Unit of analysis**

One unique advertised job opportunity, represented by one canonical analytical record.

**DEC-032 — Research limitations**

The project must disclose:

- Advertisement data is a proxy for advertised demand.
- The accessible dataset is not necessarily representative of all South African technology vacancies.
- Advertisement counts are not hiring counts.
- Multi-family assignments create overlapping totals.
- Missing data affects analytical coverage.
- Source selection may create coverage bias.
- Historical availability may be incomplete.
- Duplicate identification may be imperfect.

**Status:** Confirmed.

### 4.5 B6 — Research Period

**DEC-033 — Fixed research period**

The research period is:

**1 November 2025 to 31 October 2026 inclusive.**

This is a retrospective 12-month research window.

**DEC-034 — Publication-date eligibility**

Original publication date determines research-period eligibility.

Closing date and collection date must not replace publication date.

Advertisements discovered after the research period may qualify if their original publication date can be credibly verified within the approved period.

**DEC-035 — Temporal fields**

Maintain the following fields:

- `publication_date`
- `closing_date`
- `first_seen_date`
- `collection_date`
- `last_verified_date`
- `repost_date`

Preserve original date wording and evidence where permitted.

**DEC-036 — Collection model**

Use one planned collection exercise, potentially involving multiple sources, queries and batches.

**DEC-037 — Historical recovery**

Historical records may be recovered from permitted archives, employer records or other authorised sources.

Historical information must not be fabricated or reconstructed without evidence.

**DEC-038 — Repost management**

Preserve permitted publication-instance evidence, link reposts and maintain one canonical record per unique opportunity.

Genuinely different opportunities must remain separate.

**DEC-039 — Collection completion**

Collection completion requires approved-source acquisition, eligibility assessment, duplicate review, justified supplementary searches, historical recovery attempts and coverage and quality assessment.

If the intended collection target is not met, document the shortfall rather than including unsuitable advertisements.

**Status:** Confirmed.

---

## 5. Section B — Research Questions and Hypotheses

### 5.1 B3 — Approved Research Questions

**DEC-040 — Twelve research questions**

| ID | Research Question |
|---|---|
| RQ-01 | Which technical and professional skills are most frequently requested in South African technology job advertisements during the research period? |
| RQ-02 | How does advertised skills demand differ across the seven technology job families? |
| RQ-03 | Which skills commonly occur together in job advertisements, and how do these combinations differ by job family? |
| RQ-04 | What educational qualifications and professional certifications are requested across the technology job families? |
| RQ-05 | How do experience requirements differ across job families and seniority levels? |
| RQ-06 | What proportion and characteristics of advertised opportunities are accessible to graduates and entry-level candidates, and which skills, qualifications and experience requirements are associated with them? |
| RQ-07 | How are advertised opportunities distributed geographically across South African provinces and major locations, and how do requirements vary geographically? |
| RQ-08 | To what extent do technology job advertisements disclose salary information, and how does disclosure vary by job family, experience and location? |
| RQ-09 | Among advertisements with usable salary information, how do advertised salary ranges differ by job family, experience and location? |
| RQ-10 | What employment arrangements and working conditions are advertised, and how do these vary by role and location? |
| RQ-11 | How do advertised skills, qualifications, experience requirements and opportunity characteristics change over the research period? |
| RQ-12 | What relationships exist between job family, experience, location and advertised skills, qualifications, salary information and employment requirements? |

**Status:** Confirmed.

### 5.2 B3 — Approved Hypotheses

**DEC-041 — Seven hypotheses**

| ID | Research Area | Null Hypothesis (H0) | Alternative Hypothesis (H1) |
|---|---|---|---|
| H-01 | Skills by job family | Advertised skill distributions do not differ across job families. | Advertised skill distributions differ across job families. |
| H-02 | Qualifications | Qualification requirements are independent of job family. | Qualification requirements are associated with job family. |
| H-03 | Experience | Experience requirements are independent of job family. | Experience requirements are associated with job family. |
| H-04 | Geographic distribution | Advertised opportunities are uniformly distributed across South African provinces. | Advertised opportunities are not uniformly distributed across South African provinces. |
| H-05 | Salary disclosure | Salary disclosure rates are equal across job families. | Salary disclosure rates differ across job families. |
| H-06 | Salary distributions | Comparable advertised salary distributions do not differ across job-family and experience groups. | At least some comparable advertised salary distributions differ across job-family and experience groups. |
| H-07 | Skills and job characteristics | Advertised skills demand is not associated with the examined job characteristics. | Advertised skills demand is associated with at least some examined job characteristics. |

**DEC-042 — Hypothesis-testing standards**

- Significance level: α = 0.05.
- Two-sided testing unless justified otherwise.
- Exact p-values where available.
- Effect sizes and confidence intervals where appropriate.
- Sample sizes and explicit denominators.
- Benjamini–Hochberg false discovery rate adjustment for suitable exploratory test families.
- Report raw and adjusted p-values.
- Assess assumptions and data adequacy.
- Distinguish statistical significance from practical importance.
- Do not change methods solely to obtain significance.
- Do not infer causation from observational advertisement data.

**Status:** Confirmed.

---

## 6. Section B — Population and Sampling Decisions

### 6.1 B5 — Population

**DEC-043 — Target population**

All qualifying technology employment opportunities advertised during the approved research period and accessible to candidates working in South Africa, across the approved job families and employment types.

**DEC-044 — Accessible population**

The discoverable subset of qualifying advertisements available through approved sources and permitted acquisition methods, subject to source accessibility and the R0 budget.

**DEC-045 — Sampling frame**

A consolidated collection of discovered advertisements with sufficient metadata to assess eligibility, date, family, location, provenance and duplication.

### 6.2 B5 — Sampling Approach

**DEC-046 — Hybrid census and stratified analytical approach**

Collect all eligible discoverable advertisements from approved sources where feasible, establish canonical records and preserve the natural distribution of the accessible dataset.

Use stratified subsets or controlled comparisons where analytically appropriate.

Do not artificially balance job families or other categories.

**DEC-047 — Sample-size decision**

No fixed numerical sample size is approved before source discovery and pilot assessment.

The final target must be justified using:

- Eligible advertisement volume.
- Source coverage.
- Completeness.
- Data quality.
- Duplicate rates.
- Time feasibility.
- R0 budget constraints.

**DEC-048 — Supplementary collection**

Targeted supplementary collection may address underrepresented job families, geographic areas or employment types.

Supplementary records must meet the same eligibility criteria and be identified through `collection_purpose`.

They must not be used to create artificial population balance.

**DEC-049 — Candidate grouping variables**

The following are candidate grouping or stratification variables:

1. Job family.
2. Province or geographic category.
3. Employer geography.
4. Employment type.
5. Experience or seniority.
6. Work arrangement.
7. Source platform.
8. Publication month.

These are not automatically mandatory formal strata.

**DEC-050 — Sampling limitations**

The dataset must be described as a census or collection of accessible eligible advertisements, not as a representative sample of all South African technology vacancies.

No weighting adjustment is approved.

**DEC-051 — Analysis-specific adequacy**

Sample adequacy must be evaluated separately for each analysis.

There is no universal minimum sample size for the entire project.

Where data is insufficient, use descriptive reporting, justified category consolidation, reduced complexity or non-performance of unsuitable analyses.

Categories must not be combined merely to obtain statistical significance.

**DEC-052 — Sampling audit trail**

Maintain traceability for source discovery, acquisition, provenance, eligibility, dates, duplicates, canonical records, classification, supplementary searches, exclusions and manual changes.

**Status:** Confirmed.

---

## 7. Section B — Job-Family Classification Decisions

**DEC-053 — Seven approved job families**

| Code | Job Family |
|---|---|
| JF01 | Software Development |
| JF02 | Data and Analytics |
| JF03 | Cybersecurity |
| JF04 | IT Infrastructure and Support |
| JF05 | Cloud and DevOps |
| JF06 | Quality Assurance and Testing |
| JF07 | Business Technology |

**DEC-054 — Classification approach**

Job-family assignment must be based on role responsibilities and requirements rather than job title alone.

Maintain raw and standardised titles, assignment method, confidence and review status.

Multiple family assignments are permitted when supported by evidence.

**DEC-055 — Seniority categories**

- Entry-level.
- Junior.
- Intermediate.
- Senior.
- Lead/Principal.
- Management/Executive.
- Unknown.

**DEC-056 — Graduate accessibility categories**

- Graduate-specific.
- Entry-level accessible.
- Experience required.
- Not established.

Graduate accessibility must not be inferred solely from a job title or employment type.

**Status:** Confirmed.

---

## 8. Section B — Data Dictionary Decisions

### 8.1 B7 — Data Layers

**DEC-057 — Three-layer data model**

Maintain separate logical layers:

1. Raw source data.
2. Standardised data.
3. Derived analytical data.

Raw values must remain distinguishable from standardised and derived values. Silent overwriting is not permitted.

### 8.2 B7 — Provenance and Employer Data

**DEC-058 — Provenance requirements**

Maintain stable advertisement identifiers, source information, source record identifiers, source URLs where permitted, collection batches, collection purpose, canonical status, duplicate groups, provenance status and record versions.

Internal advertisement identifiers must not depend on job titles or URLs.

**DEC-059 — Employer information**

Distinguish the advertising organisation from the actual hiring organisation where known.

Do not infer employer identity, size or industry without reliable evidence.

Minimise recruiter personal information.

### 8.3 B7 — Skills

**DEC-060 — Skills representation**

Maintain raw and standardised skill names, identifiers, categories, technical/professional types, requirement levels, context, extraction method, confidence, evidence and review status.

Count each unique advertisement-skill relationship once while preserving relevant context and requirement levels.

### 8.4 B7 — Qualifications and Certifications

**DEC-061 — Qualification representation**

Maintain qualification text, standardised name, level, field, requirement level, restrictions and equivalent-experience acceptance.

Distinguish formal qualifications from professional certifications.

Use separate three-state indicators:

- `formal_qualification_required`
- `professional_certification_required`

Values must distinguish yes, no and not stated.

### 8.5 B7 — Experience

**DEC-062 — Experience representation**

Preserve original experience wording and capture minimum and maximum years only where supported.

Missing experience must not be treated as zero.

Vague wording must not be converted into invented numeric values.

The approved provisional categories are:

- No experience specified.
- No prior experience required.
- Graduate/trainee.
- 0–1 years.
- 1–2 years.
- 3–5 years.
- 6–10 years.
- 10+ years.
- Unclear/unclassifiable.

Exact category boundaries and overlap handling remain to be finalised before implementation.

### 8.6 B7 — Salary

**DEC-063 — Salary representation**

Preserve original salary wording, disclosure status, minimum and maximum values, currency, remuneration period, salary type, benefits inclusion and negotiability.

Distinguish exact amounts, ranges, minimums, maximums, negotiable amounts without figures, commission, stipends, benefits-only disclosures, undisclosed values and unclear information.

Do not invent salary values, replace ranges with midpoints or perform unsupported currency conversions.

Currency conversion requires a documented source, rate and date.

### 8.7 B7 — Geography

**DEC-064 — Geographic representation**

Distinguish employer location from work location.

Capture province, city, location category, work arrangement, remote eligibility, remote scope, international remote status, South African eligibility, location flexibility, relocation and travel requirements where supported.

Do not infer geography or remote eligibility from incomplete information.

### 8.8 B7 — Employment Characteristics

**DEC-065 — Employment representation**

Capture standardised employment type, duration, renewal possibility, graduate programme, internship, learnership, apprenticeship, part-time, freelance and project-contract characteristics, working hours, shifts, working days, benefits and work-authorisation requirements.

Genuine paid freelance opportunities may qualify.

Do not infer unstated benefits or employment conditions.

### 8.9 B7 — Temporal Variables

**DEC-066 — Temporal representation**

Maintain the six approved date fields and derive publication month, quarter, year, advertisement age and days until closing only where supported by the underlying dates.

Publication date determines eligibility.

### 8.10 B7 — Missing Data and Quality

**DEC-067 — Approved data-status vocabulary**

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

Conflicts, uncertainty and review requirements must be traceable.

### 8.11 B7 — Logical Entities and Counting

**DEC-068 — Logical data entities**

- Advertisement.
- Employer.
- Job-family assignment.
- Skill relationship.
- Qualification relationship.
- Certification relationship.
- Experience requirement.
- Location relationship.
- Employment characteristic.

These are logical entities, not an approved physical database schema.

**DEC-069 — Counting rules**

- Unique advertisements: distinct canonical advertisement identifiers.
- Family demand: unique advertisements assigned to each family.
- Skill demand: unique advertisement-skill relationships.
- Qualification and certification demand: unique relevant relationships.
- Geographic demand: unique advertisements associated with the relevant location.

Overlapping family and relationship totals may exceed unique advertisement totals and must be explained.

**Status:** Confirmed.

---

## 9. Section B — Statistical Methodology Decisions

### 9.1 B8 — Analytical Principles

**DEC-070 — Descriptive-first analysis**

Descriptive analysis precedes comparative, inferential and multivariable analysis.

Methods must be appropriate to variable types, distributions, independence, assumptions and sample adequacy.

**DEC-071 — Descriptive statistics**

Approved descriptive methods include:

- Frequencies and counts.
- Percentages and proportions.
- Mean, median and mode.
- Minimum and maximum.
- Standard deviation.
- Interquartile range.
- Percentiles.
- Cross-tabulations.
- Missingness summaries.
- Unique counts.

Denominators must be explicit.

### 9.2 Skills and Co-occurrence

**DEC-072 — Skills analysis**

Analyse overall and job-family skill frequencies, technical/professional categories, requirement levels, diversity and graduate-accessible profiles.

Repeated mentions within an advertisement must not inflate unique advertisement-skill counts.

**DEC-073 — Co-occurrence analysis**

Potential methods include pair counts, conditional probability, Jaccard similarity, lift, association rules and network representations.

Thresholds must be established after data assessment.

Co-occurrence must not be interpreted as causation.

### 9.3 Qualifications, Experience and Geography

**DEC-074 — Qualification analysis**

Analyse qualification levels, fields, certifications, requirement levels, equivalent experience and graduate accessibility.

**DEC-075 — Experience analysis**

Analyse experience distributions, seniority, family differences, internship acceptance and graduate accessibility.

Missing experience is not zero experience.

**DEC-076 — Geographic analysis**

Analyse provincial and city distributions, job-family patterns, skills, graduate accessibility, work arrangements and domestic versus qualifying international remote opportunities.

Distinguish opportunity-location analysis from employer-location analysis.

### 9.4 Salary and Employment

**DEC-077 — Two-track salary analysis**

Track A: Salary transparency and disclosure.

Track B: Advertised remuneration values and ranges.

Comparisons must use sufficiently comparable salary information.

Preserve original currency, period and remuneration wording.

No midpoint substitution or unsupported currency conversion.

**DEC-078 — Employment analysis**

Analyse employment types, working arrangements, duration, hours, shifts, benefits and work-authorisation characteristics.

Do not create an unsupported composite employment-quality score.

### 9.5 Hypothesis Testing and Multivariable Analysis

**DEC-079 — Hypothesis-testing standards**

Use α = 0.05, two-sided testing unless justified, exact p-values where available, effect sizes, confidence intervals, sample sizes and appropriate multiple-testing adjustment.

**DEC-080 — Candidate multivariable methods**

Potential methods include:

- Logistic regression.
- Ordinal logistic regression.
- Multinomial logistic regression.
- Multiple regression.
- Robust alternatives where justified.

Final model specifications depend on data quality, suitability and diagnostics.

**DEC-081 — Predictive modelling is not mandatory**

The project does not require predictive modelling.

It may be considered only where justified by the research objectives and available data.

### 9.6 Temporal Analysis, Diagnostics and Reporting

**DEC-082 — Temporal analysis**

Use publication dates for monthly and quarterly analysis.

Twelve monthly observations do not establish seasonality or automatically justify complex forecasting.

**DEC-083 — Diagnostics**

Assess relevant categorical, numerical and model assumptions, including sparse data, independence, distributions, outliers, multicollinearity, residual behaviour, heteroscedasticity, influence, model specification, separation and calibration where relevant.

**DEC-084 — Analysis-specific adequacy**

There is no universal minimum sample size for the project.

Use descriptive reporting, justified alternatives or non-performance of unsuitable analyses where data is inadequate.

**DEC-085 — Reporting and reproducibility**

Record research questions, dataset versions, variables, sample sizes, missingness, methods, assumptions, parameters, results, effect sizes, confidence intervals, interpretation and limitations.

Maintain traceability through version-controlled scripts or notebooks and relevant dataset and taxonomy versions.

**Status:** Confirmed.

---

## 10. Section B — Data Governance Decisions

**DEC-086 — Responsible data acquisition**

Sources and acquisition methods must be assessed for relevance, accessibility, reliability, coverage and permitted use.

Public accessibility does not automatically establish permission for unrestricted collection, storage or redistribution.

**DEC-087 — Private raw data**

Raw advertisements and restricted source evidence remain private where redistribution is not permitted.

**DEC-088 — Aggregate publication**

Public outputs are limited to aggregate findings and other permitted materials.

**DEC-089 — Data minimisation**

Avoid unnecessary personal information, including recruiter and applicant information unrelated to the research.

**DEC-090 — Provenance and integrity**

Maintain traceability for source records, collection batches, transformations, classifications, duplicate decisions and manual corrections.

**DEC-091 — Retention and disposal**

Retention and disposal must follow the separate Data Retention and Access document and applicable source restrictions.

No new fixed retention period is approved by this decision.

**DEC-092 — Disclosure review**

Review public outputs for small-cell risks, personal information, confidential information and restricted source content.

No universal numerical small-cell suppression threshold is approved.

**Status:** Confirmed.

---

## 11. Unresolved Proposals and Deferred Decisions

The following matters remain unresolved or are intentionally deferred.

Previously proposed matters that have since been approved are no longer listed as pending.

| ID | Proposal / Outstanding Matter | Resolution Section | Status |
|---|---|---|---|
| PROP-001 | Final individual research-source approvals and source-specific permissions | C | Pending |
| PROP-002 | Final dataset-size target after source discovery and pilot assessment | B–C | Deferred |
| PROP-003 | Exact experience-category boundaries and overlap rules | B–C | Pending |
| PROP-004 | Final skill taxonomy and versioning details | B–C | Deferred |
| PROP-005 | Salary standardisation and currency-conversion policy | B–C | Deferred |
| PROP-006 | Final statistical test selection and model specifications | B–F | Deferred |
| PROP-007 | NLP methods and their implementation | G | Pending |
| PROP-008 | Physical database implementation and final schema | D | Pending |
| PROP-009 | BI implementation and dashboard technology | H | Pending |
| PROP-010 | Final technology and package versions | E | Pending |
| PROP-011 | Predictive modelling beyond the approved optional position | F–G | Deferred |
| PROP-012 | Publishing and hosting implementation | J | Pending |
| PROP-013 | Exact retention periods and disposal schedule | C | Pending |
| PROP-014 | Final small-cell disclosure threshold | C–J | Pending |
| PROP-015 | Technical access-control, encryption and backup implementation | D–E | Deferred |
| PROP-016 | Final acquisition-log and audit-trail implementation | C–D | Deferred |
| PROP-017 | Final source coverage and collection completion target | B–C | Deferred |

### 11.1 Resolved Proposals

The following matters were previously unresolved but are now approved:

| Original Proposal | Resolution | Current Status |
|---|---|---|
| PROP-001 — Exact research dates | Fixed as 1 November 2025–31 October 2026 inclusive. | Resolved — Confirmed |
| PROP-003 — Target dataset size | No fixed target before source discovery and pilot assessment; establish a feasibility-based target. | Resolved — Approach Confirmed |
| PROP-004 — Final job-family rules | Seven job families and codes approved; detailed classification rules remain subject to implementation. | Resolved — Framework Confirmed |
| PROP-005 — Final research hypotheses | Seven hypotheses with H0 and H1 approved. | Resolved — Confirmed |
| PROP-006 — Statistical methods | Statistical framework and standards approved; exact tests depend on data. | Resolved — Framework Confirmed |
| PROP-011 — Predictive modelling | Explicitly optional and not mandatory. | Resolved — Position Confirmed |

The original proposal identifiers are retained for traceability. Their resolution does not imply that every related implementation detail is complete.

---

## 12. Decision Management Rules

1. Confirmed decisions must not be changed silently.
2. New decisions must have unique IDs.
3. Proposals must not be treated as approved requirements.
4. Material changes require formal change control.
5. Decisions must be traceable to project documentation.
6. Superseded decisions must remain in the historical record.
7. Changes affecting multiple documents must be reflected consistently.
8. Decisions must not claim source permissions, technical implementations or research findings that have not been established.
9. Deferred decisions must be revisited at the appropriate project stage.
10. Approval of a specification does not automatically mean that it has been implemented.

---

## 13. Related Project Documentation

| Document | Purpose |
|---|---|
| `docs/02_Research_Methodology/Research_Design.md` | Research problem, aim, objectives, scope and design |
| `docs/02_Research_Methodology/Research_Questions_and_Hypotheses.md` | Approved research questions and hypotheses |
| `docs/02_Research_Methodology/Sampling_Strategy.md` | Population, sampling frame and sampling approach |
| `docs/02_Research_Methodology/Statistical_Methodology.md` | Statistical analysis framework |
| `docs/03_Data_Governance/Data_Dictionary.md` | Variables, definitions and operationalisation |
| `docs/03_Data_Governance/Data_Governance_Plan.md` | Data governance and publication controls |
| `docs/03_Data_Governance/Data_Source_Register.csv` | Source inventory and assessment |
| `docs/03_Data_Governance/Data_Retention_and_Access.md` | Data retention and access requirements |

---

## 14. New Decision Entry Template

Use this template for significant new decisions.

| Field | Details |
|---|---|
| Decision ID | DEC-XXX |
| Date | YYYY-MM-DD |
| Description | |
| Options considered | |
| Selected option | |
| Reason | |
| Impact | |
| Status | Proposed / Confirmed / Rejected / Deferred |
| Related section | |
| Related documents | |
| Supersedes | If applicable |

---

## 15. Section B Approval Record

The following Section B documents have received explicit approval of their proposed contents:

| No. | Document | Approval Status |
|---|---|---|
| 1 | Research Design | Approved |
| 2 | Research Questions and Hypotheses | Approved |
| 3 | Sampling Strategy | Approved |
| 4 | Data Dictionary | Approved |
| 5 | Statistical Methodology | Approved |
| 6 | Data Governance Plan | Approved |

The approval record reflects acceptance of the proposed documentation content. It does not claim that the files have been saved, implemented or committed to version control.

---

## 16. Document Maintenance

This decision log must be updated whenever a material project decision is approved, rejected, deferred or superseded.

The project owner is responsible for maintaining the log and ensuring that related documents remain consistent.

**Current document version:** 2.0  
**Current decision coverage:** Section A project decisions and Section B research and governance decisions  
**Document status:** Active  
**Next update:** When subsequent project sections introduce or resolve material decisions.