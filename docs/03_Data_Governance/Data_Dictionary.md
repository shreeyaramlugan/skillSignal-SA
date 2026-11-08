# SkillSignal SA — Data Dictionary

| Document Attribute | Details |
|---|---|
| Project Name | SkillSignal SA |
| Project ID | SSA-001 |
| Document | Data Dictionary |
| Document Location | `docs/03_Data_Governance/Data_Dictionary.md` |
| Version | 2.0 |
| Status | Approved — Section B Finalised |
| Research Period | 1 November 2025 – 31 October 2026 inclusive |
| Unit of Analysis | One unique job advertisement representing one advertised opportunity |
| Geographic Scope | South Africa, including qualifying international remote opportunities |
| Related Documents | Research Design; Research Questions and Hypotheses; Sampling Strategy; Data Governance Plan; Statistical Methodology |

---

## 1. Purpose

This document defines the variables required to represent, process, validate and analyse the job advertisements collected for SkillSignal SA.

It establishes a shared reference for:

- Data acquisition.
- Raw data preservation.
- Data cleaning.
- Standardisation.
- Classification.
- Feature extraction.
- Derived-variable calculation.
- Data-quality assessment.
- Statistical analysis.
- Reporting and visualisation.

The dictionary describes the logical data requirements. It does not prescribe a final physical database schema, programming language, database engine or extraction library.

Those technical implementation decisions remain subject to the relevant architecture and implementation stages.

## 2. Data Dictionary Principles

### 2.1 Three-layer data model

The project uses three logical data layers.

| Layer | Purpose | Example |
|---|---|---|
| Raw source | Preserve information as obtained from the advertisement | `job_title_raw` |
| Standardised | Represent source information consistently | `job_title_standardised` |
| Derived | Represent calculated or classified information | `publication_month` |

These layers must remain distinguishable throughout processing.

### 2.2 Raw data preservation

- Preserve original source values where permitted.
- Never silently overwrite raw source information.
- Keep source wording available for verification.
- Record standardisation and extraction methods.
- Retain evidence supporting classifications.
- Document material corrections and manual changes.
- Apply retention restrictions to source content and personal information.

### 2.3 Missing-data principles

A missing value must not automatically be interpreted as a negative response.

For example:

- No salary information does not mean the position is unpaid.
- No qualification information does not mean no qualification is required.
- No experience information does not mean no prior experience is required.
- No location information does not mean the position is remote.

Missing, not stated, unclear, conflicting and not applicable must remain distinguishable.

### 2.4 Confidence and review

Extracted or classified information should include confidence, evidence or review information where applicable.

Automated extraction does not automatically establish that a value is correct.

### 2.5 Logical rather than physical definitions

Field names and groupings in this document represent logical data requirements.

Exact database types, nullability, table names, indexes, constraints, relationships and implementation-specific naming remain subject to technical design.

---

## 3. Advertisement Identity and Provenance

### 3.1 Purpose

These variables identify an advertisement, preserve its source history and support canonical-record and duplicate management.

### 3.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `advertisement_id` | Standardised | Stable internal identifier for one canonical advertised opportunity. Must not depend on title, employer or source URL. |
| `source_name` | Raw / Standardised | Name of the platform, employer website or other approved source. |
| `source_record_id` | Raw | Identifier assigned by the original source, where available. |
| `source_url` | Raw | Original advertisement URL, subject to access and retention restrictions. |
| `employer_reference` | Raw | Employer or recruitment reference number, where available. |
| `original_job_title` | Raw | Original job title as displayed by the source. |
| `first_seen_date` | Raw / Standardised | Date the project first identified the advertisement. |
| `collection_date` | Standardised | Date the project acquired or recorded the advertisement. |
| `collection_batch_id` | Standardised | Identifier linking the record to its acquisition batch. |
| `collection_purpose` | Standardised | `primary_collection` or `targeted_supplementary`. |
| `canonical_record_status` | Standardised | Indicates whether a record is a canonical opportunity, duplicate instance or unresolved candidate. |
| `duplicate_group_id` | Standardised | Identifier linking records believed to represent the same opportunity. |
| `provenance_status` | Standardised | Indicates whether source origin and supporting provenance have been sufficiently established. |
| `record_version` | Standardised | Version or revision identifier used to track material record changes. |

### 3.3 Operational rules

1. Every canonical opportunity receives one stable `advertisement_id`.
2. Source-specific identifiers must not replace the internal identifier.
3. Multiple source instances may be linked to one canonical opportunity.
4. Duplicate decisions must preserve evidence and review history.
5. Collection purpose must be recorded for primary and supplementary collection.
6. A record must not be considered verified solely because it has a URL.
7. Changes to canonical records must be traceable.
8. Where source information cannot legally or practically be retained, preserve permitted provenance metadata instead.

---

## 4. Employer Variables

### 4.1 Purpose

Employer variables describe the organisation advertising or offering the opportunity.

The advertising organisation and actual hiring organisation may be different.

### 4.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `employer_name_raw` | Raw | Employer or organisation name as displayed in the source. |
| `employer_name_standardised` | Standardised | Consistent employer name after documented cleaning. |
| `employer_id` | Standardised | Internal employer identifier where identity can be established confidently. |
| `employer_country` | Standardised | Country associated with the employer, where verified. |
| `employer_type` | Standardised | Employer classification where supported by evidence. |
| `industry` | Standardised | Employer industry where reliable information is available. |
| `company_size_category` | Standardised | Employer-size category where reliable evidence exists. |
| `employer_website` | Raw / Standardised | Public employer website, where available and permitted. |
| `recruitment_agency_flag` | Standardised | Indicates whether a recruitment agency is advertising the opportunity. |
| `employer_identity_confidence` | Derived / Review | Confidence in the identification and standardisation of the employer. |

### 4.3 Operational rules

- Preserve the original employer name.
- Standardise names only where the identity is sufficiently established.
- Do not merge organisations merely because their names are similar.
- Do not infer company size or industry from an advertisement's wording alone.
- Distinguish recruitment agencies from direct employers.
- Distinguish the organisation advertising the role from the organisation employing the successful candidate where evidence permits.
- Avoid collecting unnecessary recruiter or employee personal information.
- An `employer_id` may remain unavailable where the identity cannot be reliably established.

---

## 5. Job Title, Job Family and Seniority Variables

### 5.1 Purpose

These variables classify advertised opportunities into the approved technology job families and support comparisons by role and seniority.

### 5.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `job_title_raw` | Raw | Original job title exactly as obtained. |
| `job_title_standardised` | Standardised | Normalised job title using documented naming rules. |
| `job_title_family` | Standardised | Human-readable job-family classification. |
| `job_family_code` | Standardised | Approved job-family code. |
| `job_family_name` | Standardised | Approved job-family name. |
| `job_family_assignment_method` | Standardised | Manual, rule-based, NLP-assisted or hybrid assignment method. |
| `job_family_confidence` | Derived / Review | Confidence in the job-family assignment. |
| `job_family_review_status` | Standardised | Indicates whether classification has been reviewed or requires review. |
| `seniority_level` | Standardised | Normalised seniority classification. |
| `graduate_entry_level_flag` | Derived | Indicates the advertisement's assessed accessibility to graduates or entry-level applicants. |
| `role_description_text` | Raw | Original role description, where collection and retention are permitted. |
| `role_summary_standardised` | Standardised | Concise normalised summary of the advertised responsibilities, where required. |

### 5.3 Approved job-family taxonomy

| Code | Job Family | Description |
|---|---|---|
| JF01 | Software Development | Software engineering, application development and related software creation roles. |
| JF02 | Data and Analytics | Data analysis, business intelligence, data engineering and related analytics roles. |
| JF03 | Cybersecurity | Information security, cyber defence, security operations and related security roles. |
| JF04 | IT Infrastructure and Support | IT support, systems administration, infrastructure operations and related technical support roles. |
| JF05 | Cloud and DevOps | Cloud engineering, platform engineering, DevOps and related automation or deployment roles. |
| JF06 | Quality Assurance and Testing | Software testing, quality assurance and test engineering roles. |
| JF07 | Business Technology | Business systems, enterprise technology, technology analysis and related business-facing roles. |

### 5.4 Seniority categories

| Category | Definition |
|---|---|
| Entry-level | Explicitly entry-level opportunity. |
| Junior | Early-career role with some expected capability or experience. |
| Intermediate | Role requiring established professional competence. |
| Senior | Role requiring substantial experience or advanced responsibility. |
| Lead/Principal | Technical leadership or principal-level responsibility. |
| Management/Executive | Management, departmental or executive responsibility. |
| Unknown | Seniority cannot be established reliably. |

### 5.5 Graduate accessibility categories

| Category | Definition |
|---|---|
| Graduate-specific | Explicitly intended for graduates or graduate programme participants. |
| Entry-level accessible | No substantial prior experience is required or the advertisement explicitly welcomes entry-level applicants. |
| Experience required | Requirements indicate that prior relevant experience is necessary. |
| Not established | Available evidence does not support a reliable determination. |

### 5.6 Operational rules

- Job-family classification must consider responsibilities and requirements, not job title alone.
- Multiple family assignments are permitted where justified.
- Each assignment must be independently supported by evidence.
- Uncertain assignments must be flagged for review.
- Seniority must not be inferred solely from years of experience.
- Graduate accessibility must not be inferred solely from the word "junior".
- A graduate programme is not automatically equivalent to an entry-level accessible position.
- Family taxonomy changes must be version-controlled.
- The assignment method and confidence must remain traceable.

---

## 6. Skills Variables

### 6.1 Purpose

Skills variables identify the technical and professional capabilities requested in advertisements.

They support frequency analysis, job-family comparisons, graduate skill profiles and skill co-occurrence analysis.

### 6.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `skills_text_raw` | Raw | Original section or text containing advertised skills. |
| `skill_name_raw` | Raw | Skill wording as stated in the advertisement. |
| `skill_name_standardised` | Standardised | Normalised skill name. |
| `skill_id` | Standardised | Internal identifier for a standardised skill. |
| `skill_category` | Standardised | Approved or documented skill category. |
| `skill_type` | Standardised | Technical or professional skill. |
| `skill_requirement_level` | Standardised | Required, preferred, advantageous or unspecified. |
| `skill_context` | Raw / Standardised | Context in which the skill is mentioned. |
| `skill_extraction_method` | Standardised | Manual, rule-based, NLP-assisted or hybrid extraction. |
| `skill_extraction_confidence` | Derived / Review | Confidence in extraction and normalisation. |
| `skill_evidence_text` | Raw / Evidence | Supporting advertisement wording, where permitted. |
| `skill_review_status` | Standardised | Indicates whether the extracted skill has been reviewed. |

### 6.3 Technical skill categories

| Category | Examples |
|---|---|
| Programming languages | Python, Java, JavaScript, C#, SQL |
| Frameworks and libraries | React, Angular, Django, Spring |
| Databases and data management | PostgreSQL, MySQL, MongoDB, data modelling |
| Data analytics and visualisation | Power BI, Tableau, Excel, statistical analysis |
| Cloud platforms | AWS, Azure, Google Cloud |
| DevOps and infrastructure | Docker, Kubernetes, CI/CD, infrastructure automation |
| Cybersecurity | SIEM, penetration testing, incident response, vulnerability management |
| Networking and systems | TCP/IP, Linux, Windows Server, network administration |
| Software engineering practices | Version control, API development, system design |
| Testing and quality assurance | Selenium, automated testing, test planning |
| Enterprise and business systems | ERP, CRM, SAP, business applications |
| Tools and development environments | Git, IDEs, command-line tools and relevant technical utilities |

These categories are an initial approved classification framework. They may be refined through documented taxonomy development without silently changing previously recorded raw skill values.

### 6.4 Professional skill categories

- Communication.
- Problem-solving.
- Critical thinking.
- Teamwork and collaboration.
- Leadership.
- Project management.
- Stakeholder management.
- Adaptability.
- Analytical thinking.
- Written communication.

### 6.5 Operational rules

1. A skill must be supported by advertisement evidence.
2. Generic words must not automatically be treated as skills.
3. Equivalent skill names may be standardised to one canonical label.
4. Raw wording must remain available.
5. Requirement level must be preserved where distinguishable.
6. A skill may occur in several contexts within one advertisement.
7. For advertisement-level frequency, count each unique standardised skill once per canonical advertisement.
8. Preserve multiple contexts or requirement levels where they convey meaningful information.
9. Do not treat repeated mentions as separate advertisements or independent skill observations.
10. Record extraction method and confidence.
11. Maintain a versioned skill taxonomy.
12. Uncertain skill mappings must be reviewed.

### 6.6 Counting rule

For skill frequency:

\[
\text{Skill frequency} =
\text{Number of unique canonical advertisements containing the skill}
\]

A single advertisement mentioning Python five times contributes one advertisement-level occurrence of Python.

---

## 7. Qualification and Certification Variables

### 7.1 Purpose

These variables capture formal educational requirements and professional certifications.

Educational qualifications and professional certifications must be analysed separately.

### 7.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `qualification_text_raw` | Raw | Original qualification wording. |
| `qualification_name_standardised` | Standardised | Normalised qualification name. |
| `qualification_level` | Standardised | Qualification level or category. |
| `qualification_field` | Standardised | Academic or professional field, where stated. |
| `qualification_requirement_level` | Standardised | Required, preferred, advantageous or unspecified. |
| `qualification_field_restriction` | Standardised | Indicates whether a specific study field is required or accepted. |
| `certification_name_raw` | Raw | Original certification wording. |
| `certification_name_standardised` | Standardised | Normalised certification name. |
| `certification_provider` | Standardised | Certification issuer or provider where identifiable. |
| `certification_requirement_level` | Standardised | Required, preferred, advantageous or unspecified. |
| `equivalent_experience_accepted` | Standardised | Indicates whether equivalent experience is explicitly accepted. |
| `qualification_extraction_method` | Standardised | Method used to extract qualification information. |
| `qualification_evidence_text` | Raw / Evidence | Supporting advertisement wording, where permitted. |
| `qualification_confidence` | Derived / Review | Confidence in extraction and classification. |
| `qualification_review_status` | Standardised | Review state. |

### 7.3 Qualification categories

| Category | Examples |
|---|---|
| Matric / NSC | National Senior Certificate or equivalent school-leaving qualification |
| Other school qualification | Other stated school-level qualification |
| Higher Certificate | Higher Certificate |
| Diploma | Diploma |
| Advanced Diploma | Advanced Diploma |
| Bachelor's degree | Relevant bachelor's qualification |
| Honours degree | Honours qualification |
| Postgraduate Diploma | Postgraduate Diploma |
| Master's degree | Master's qualification |
| Doctorate | Doctoral qualification |
| Not specified | No educational level can be established |

### 7.4 Certification categories

Certifications may be classified as:

- Vendor-specific certification.
- Industry-recognised certification.
- Other professional certification.
- Not specified.
- Unclear.

The certification provider and actual certification name should be retained separately where identifiable.

### 7.5 Qualification requirement indicators

The following three-state indicators must be maintained separately:

| Variable | Allowed values |
|---|---|
| `formal_qualification_required` | Yes, No, Not stated |
| `professional_certification_required` | Yes, No, Not stated |

### 7.6 Operational rules

- Distinguish educational qualifications from certifications.
- Distinguish required qualifications from preferred qualifications.
- Preserve alternative qualifications and equivalent-experience statements.
- Do not assume a degree is mandatory when an advertisement merely says it is advantageous.
- Do not treat an omitted qualification as a negative requirement.
- Record field restrictions where explicitly stated.
- Retain evidence supporting the assigned level.

---

## 8. Experience and Seniority Requirement Variables

### 8.1 Purpose

These variables capture prior experience requirements and support analysis of experience expectations, seniority and graduate accessibility.

### 8.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `experience_text_raw` | Raw | Original experience requirement wording. |
| `minimum_experience_years` | Standardised | Minimum numeric experience requirement where reliably extractable. |
| `maximum_experience_years` | Standardised | Maximum numeric experience requirement where reliably extractable. |
| `experience_range_type` | Standardised | Exact, minimum-only, bounded range, maximum-only or unclear. |
| `experience_requirement_level` | Standardised | Required, preferred, advantageous or unspecified. |
| `experience_category` | Standardised | Normalised experience grouping. |
| `seniority_level` | Standardised | Approved seniority category. |
| `graduate_accessibility` | Derived | Assessed accessibility to graduates or entry-level applicants. |
| `experience_internship_accepted` | Standardised | Indicates whether internship experience is explicitly accepted or recognised. |
| `experience_equivalent_accepted` | Standardised | Indicates whether equivalent experience is explicitly accepted. |
| `experience_relevant_domain` | Standardised | Domain in which experience is required. |
| `experience_extraction_method` | Standardised | Extraction method used. |
| `experience_evidence_text` | Raw / Evidence | Supporting advertisement wording. |
| `experience_confidence` | Derived / Review | Confidence in extracted experience information. |
| `experience_review_status` | Standardised | Review state. |

### 8.3 Provisional experience categories

| Category | Description |
|---|---|
| No experience specified | Advertisement does not state an experience requirement. |
| No prior experience required | Advertisement explicitly states that prior experience is unnecessary. |
| Graduate/trainee | Explicit graduate or trainee experience pathway. |
| 0–1 years | Numeric requirement within the stated range. |
| 1–2 years | Numeric requirement within the stated range. |
| 3–5 years | Numeric requirement within the stated range. |
| 6–10 years | Numeric requirement within the stated range. |
| 10+ years | Requirement explicitly exceeding ten years or equivalent. |
| Unclear/unclassifiable | Available wording does not support reliable categorisation. |

**Boundary and overlap rules remain to be finalised before implementation.**

The final categorisation must establish how boundary values and overlapping ranges are handled. The categories must not be implemented as mutually exclusive numeric bins until those rules are approved.

### 8.4 Operational rules

- Preserve original experience wording.
- Do not convert vague terms into invented numeric values.
- Missing experience information is not equivalent to zero years.
- Distinguish no experience required from experience not stated.
- Preserve minimum and maximum values separately.
- Distinguish required and preferred experience.
- Record relevant domain experience where stated.
- Seniority must not be derived solely from numeric experience.
- Graduate accessibility must consider the complete advertisement, not just experience wording.
- Flag uncertain extraction for review.

---

## 9. Salary and Remuneration Variables

### 9.1 Purpose

These variables support two separate analytical areas:

1. Salary transparency: whether and how advertisements disclose remuneration.
2. Advertised remuneration patterns: the amounts or ranges explicitly stated.

### 9.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `salary_text_raw` | Raw | Original salary or remuneration wording. |
| `salary_disclosed_flag` | Derived | Indicates whether the advertisement discloses a remuneration amount or other identifiable remuneration information. |
| `salary_minimum_raw` | Raw | Original minimum salary amount, where stated. |
| `salary_maximum_raw` | Raw | Original maximum salary amount, where stated. |
| `salary_currency` | Raw / Standardised | Original remuneration currency. |
| `salary_period` | Raw / Standardised | Original remuneration period. |
| `salary_minimum_standardised` | Standardised | Normalised minimum numeric amount where reliably extractable. |
| `salary_maximum_standardised` | Standardised | Normalised maximum numeric amount where reliably extractable. |
| `salary_period_standardised` | Standardised | Normalised remuneration period. |
| `salary_type` | Standardised | Salary, hourly rate, daily rate, commission, stipend, allowance or other remuneration type. |
| `salary_includes_benefits` | Standardised | Indicates whether the disclosed amount explicitly includes benefits. |
| `salary_negotiable_flag` | Standardised | Indicates whether remuneration is stated to be negotiable. |
| `salary_currency_conversion` | Derived | Documents any approved currency conversion, including its source and reference date. |
| `salary_disclosure_type` | Standardised | Classification of the form of remuneration disclosure. |
| `salary_extraction_confidence` | Derived / Review | Confidence in extracted remuneration information. |
| `salary_evidence_text` | Raw / Evidence | Supporting advertisement wording. |
| `salary_review_status` | Standardised | Review state. |

### 9.3 Salary disclosure categories

| Category | Definition |
|---|---|
| Exact amount | A specific remuneration amount is disclosed. |
| Range | Minimum and maximum amounts are disclosed. |
| Starting/minimum amount | Only a starting or minimum amount is disclosed. |
| Maximum amount | Only a maximum amount is disclosed. |
| Negotiable — no amount | Negotiability is stated without a numerical amount. |
| Commission | Commission-based remuneration is disclosed. |
| Stipend/allowance | A stipend or allowance is disclosed. |
| Benefits only | Benefits are disclosed without a numerical salary amount. |
| Not disclosed | No remuneration information is provided. |
| Unclear | Remuneration wording cannot be classified reliably. |

### 9.4 Operational rules

1. Preserve original salary wording.
2. Preserve original currency.
3. Preserve original remuneration period.
4. Distinguish gross and net amounts where stated.
5. Distinguish salary from commission, stipends, allowances and benefits.
6. Do not infer a salary from job title, seniority or external salary benchmarks.
7. Do not assume that "competitive salary" represents a disclosed amount.
8. Preserve ranges; do not automatically replace them with midpoints.
9. Do not convert currencies without a documented source, rate and conversion date.
10. Do not annualise remuneration unless the original period and conversion basis are sufficiently clear.
11. Do not treat missing salary information as zero remuneration.
12. Review ambiguous or conflicting salary statements manually.

### 9.5 Comparability

Salary comparisons may only be undertaken where values have a defensible common basis.

Potential comparability requirements include:

- Currency.
- Remuneration period.
- Gross or net basis.
- Employment arrangement.
- Salary versus other remuneration type.
- Sufficiently reliable extraction.

If these conditions cannot be met, report disclosure patterns separately and qualify or omit numerical remuneration comparisons.

---

## 10. Geographic and Work-Arrangement Variables

### 10.1 Purpose

These variables capture where the employer is based, where work is performed and whether the opportunity is accessible to candidates working in South Africa.

### 10.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `location_text_raw` | Raw | Original location wording. |
| `employer_country` | Standardised | Country in which the employer is based, where verified. |
| `work_country` | Standardised | Country or countries in which the work is to be performed. |
| `province` | Standardised | South African province or documented geographic classification. |
| `city` | Standardised | City or town associated with the work location. |
| `location_category` | Standardised | Normalised location category. |
| `work_arrangement` | Standardised | On-site, hybrid, fully remote, flexible, not disclosed or unclear. |
| `remote_eligibility` | Standardised | Whether remote work is permitted for the opportunity. |
| `remote_work_scope` | Standardised | Geographic scope of the remote arrangement. |
| `international_remote_flag` | Derived | Indicates a qualifying international remote opportunity. |
| `south_africa_eligibility` | Standardised | Whether the advertisement explicitly permits candidates working in South Africa. |
| `location_flexibility` | Standardised | Indicates whether location flexibility is explicitly offered. |
| `relocation_required_flag` | Standardised | Indicates whether relocation is explicitly required. |
| `travel_required_flag` | Standardised | Indicates whether travel is explicitly required. |
| `geographic_extraction_confidence` | Derived / Review | Confidence in geographic extraction. |
| `geographic_evidence_text` | Raw / Evidence | Supporting advertisement wording. |
| `geographic_review_status` | Standardised | Review state. |

### 10.3 Geographic classifications

Geographic records must support:

- All nine South African provinces.
- Multiple South African provinces.
- South Africa — location unspecified.
- Qualifying international remote.
- Other qualifying geographic arrangement.
- Unclear or unverified location.

### 10.4 Work-arrangement categories

| Category | Definition |
|---|---|
| On-site | Work is explicitly performed at a physical workplace. |
| Hybrid | A combination of on-site and remote work is stated. |
| Fully remote | Work is explicitly described as remote. |
| Flexible | Location arrangement is described as flexible but not sufficiently specified for another category. |
| Not disclosed | No work-arrangement information is provided. |
| Unclear | Available wording is ambiguous. |

### 10.5 Operational rules

- Employer location and work location must remain separate.
- Do not infer a province from an employer's registered address.
- Do not infer remote eligibility from a remote label alone.
- International remote opportunities qualify only where the advertisement explicitly allows candidates working in South Africa.
- Record domestic and qualifying international remote opportunities separately.
- Preserve multiple locations where the advertisement covers more than one location.
- Do not force a multi-location opportunity into one province without a documented analytical rule.
- Do not infer relocation or travel requirements.
- Uncertain geographic eligibility must be reviewed.

---

## 11. Employment and Working-Condition Variables

### 11.1 Purpose

These variables describe the employment arrangement and working conditions advertised.

### 11.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `employment_type_raw` | Raw | Original employment-type wording. |
| `employment_type_standardised` | Standardised | Normalised employment category. |
| `employment_duration` | Standardised | Advertised contract or programme duration, where stated. |
| `contract_renewal_possible` | Standardised | Indicates whether renewal is explicitly possible. |
| `graduate_programme_flag` | Standardised | Identifies an explicitly stated graduate programme. |
| `internship_flag` | Standardised | Identifies an internship opportunity. |
| `learnership_flag` | Standardised | Identifies a learnership opportunity. |
| `apprenticeship_flag` | Standardised | Identifies an apprenticeship opportunity. |
| `part_time_flag` | Standardised | Identifies part-time employment. |
| `freelance_flag` | Standardised | Identifies genuine paid freelance work. |
| `project_contract_flag` | Standardised | Identifies a project-based contract. |
| `working_hours` | Standardised | Advertised hours or schedule, where stated. |
| `shift_work_flag` | Standardised | Indicates whether shift work is explicitly required. |
| `working_days` | Standardised | Advertised working days, where stated. |
| `benefits_text_raw` | Raw | Original benefits wording. |
| `benefits_categories` | Standardised | Normalised benefits categories. |
| `work_authorisation_requirement` | Standardised | Explicit work-authorisation or eligibility requirement. |
| `employment_extraction_confidence` | Derived / Review | Confidence in extracted employment information. |
| `employment_evidence_text` | Raw / Evidence | Supporting advertisement wording. |
| `employment_review_status` | Standardised | Review state. |

### 11.3 Employment categories

- Permanent.
- Fixed-term.
- Temporary.
- Graduate programme.
- Graduate position.
- Internship.
- Learnership.
- Apprenticeship.
- Part-time.
- Freelance.
- Project-based contract.
- Multiple employment arrangements.
- Not disclosed.
- Unclear.

### 11.4 Operational rules

- Preserve original employment wording.
- Distinguish graduate programmes from graduate positions.
- Preserve separate internship, learnership and apprenticeship indicators.
- A role may have multiple relevant employment characteristics.
- Genuine paid freelance work may qualify.
- Volunteer and unpaid speculative projects do not qualify.
- Do not infer contract duration or renewal possibility.
- Do not infer benefits from employer reputation or industry norms.
- Keep work arrangement separate from employment type.
- Preserve working-hour and shift information only where explicitly stated.

---

## 12. Temporal Variables

### 12.1 Purpose

Temporal variables establish research-period eligibility and support monthly and quarterly analysis.

### 12.2 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `publication_date` | Raw / Standardised | Original verified date on which the advertisement was published. |
| `closing_date` | Raw / Standardised | Advertised application closing date, where available. |
| `first_seen_date` | Standardised | Date the project first identified the advertisement. |
| `collection_date` | Standardised | Date the project acquired or recorded the advertisement. |
| `last_verified_date` | Standardised | Date on which the advertisement or its details were last verified. |
| `repost_date` | Raw / Standardised | Date of a verified repost or subsequent publication instance. |
| `publication_month` | Derived | Month derived from verified publication date. |
| `publication_quarter` | Derived | Quarter derived from verified publication date. |
| `publication_year` | Derived | Year derived from verified publication date. |
| `advertisement_age_days` | Derived | Age calculated using a clearly identified reference date. |
| `days_until_closing` | Derived | Difference between closing date and a clearly identified reference date. |
| `date_confidence` | Derived / Review | Confidence in the verified date. |
| `date_evidence_text` | Raw / Evidence | Supporting date wording or evidence. |
| `date_review_status` | Standardised | Review state. |

### 12.3 Research-period rule

The approved research period is:

**1 November 2025 to 31 October 2026 inclusive.**

The publication date determines research-period eligibility.

### 12.4 Operational rules

- Preserve original date wording where permitted.
- Standardise verified dates using a consistent date representation.
- Keep publication, closing, first-seen, collection, last-verified and repost dates distinct.
- Do not substitute collection date for publication date.
- Do not substitute closing date for publication date.
- Advertisements discovered after 31 October 2026 may qualify if their original publication date is credibly verified within the research period.
- Uncertain or conflicting publication dates must be held for review.
- Confirmed out-of-period advertisements must be excluded.
- Reposts must be assessed under the approved canonical-record rules.
- Derived temporal values must identify their reference date where the result depends on one.

---

## 13. Missing Data, Conflicts and Data Quality Variables

### 13.1 Purpose

These variables document completeness, ambiguity, extraction quality and manual review requirements.

### 13.2 Approved data-status vocabulary

| Status | Definition |
|---|---|
| `observed` | Information directly observed in the source. |
| `extracted` | Information extracted from source content. |
| `standardised` | Information normalised using documented rules. |
| `derived` | Information calculated or classified from other variables. |
| `not_stated` | Source does not state the information. |
| `not_applicable` | Variable does not apply to the record. |
| `unclear` | Information exists but cannot be interpreted reliably. |
| `conflicting` | Available evidence contains inconsistent information. |
| `not_verified` | Information has not been sufficiently verified. |
| `not_processed` | Information has not yet undergone the required processing. |

### 13.3 Variables

| Variable | Layer | Definition / Operationalisation |
|---|---|---|
| `data_completeness_status` | Derived | Overall completeness classification for the record or relevant dataset scope. |
| `missing_field_count` | Derived | Number of fields missing within a clearly defined validation scope. |
| `critical_field_status` | Derived | Status of fields required for eligibility or a particular processing stage. |
| `record_validation_status` | Derived | Overall validation result. |
| `manual_review_required` | Derived | Indicates whether human review is necessary. |
| `manual_review_reason` | Standardised | Reason manual review is required. |
| `conflicting_evidence_flag` | Derived | Indicates conflicting source evidence. |
| `data_quality_issue_codes` | Standardised | One or more documented data-quality issue classifications. |
| `data_quality_notes` | Raw / Review | Supporting quality observations. |
| `last_reviewed_date` | Standardised | Date of the most recent review. |
| `reviewed_by` | Standardised | Reviewer identifier or role, where appropriate. |

### 13.4 Data-quality issue categories

Potential issue categories include:

- Missing or incomplete information.
- Ambiguous information.
- Conflicting information.
- Invalid date.
- Unclear salary.
- Uncertain geographic classification.
- Uncertain employment classification.
- Uncertain job-family assignment.
- Duplicate uncertainty.
- Extraction failure.
- Standardisation failure.
- Insufficient provenance.
- Other documented issue.

### 13.5 Operational rules

1. Missing information must not be converted into a negative value.
2. Conflicting evidence must remain identifiable.
3. Uncertain records must be flagged for review.
4. A missing non-critical field does not automatically disqualify an otherwise eligible advertisement.
5. An advertisement may be suitable for some analyses but not others.
6. Data completeness must be evaluated in relation to the intended analysis.
7. Manual corrections must be traceable.
8. Validation must distinguish eligibility failures from analytical limitations.
9. The project must not silently discard records because some optional fields are missing.

---

## 14. Logical Data Entities and Relationships

### 14.1 Purpose

The following entities describe the logical information structure required by the research.

They do not prescribe the final physical database design.

### 14.2 Approved logical entities

| Entity | Purpose | Example relationships |
|---|---|---|
| Advertisement | Represents one unique canonical opportunity. | Linked to employer, family assignments, skills and other requirements. |
| Employer | Represents an identifiable advertising or hiring organisation. | May be associated with multiple advertisements. |
| Job-family assignment | Represents an advertisement's assignment to one or more job families. | Links advertisements to job-family codes. |
| Skill relationship | Represents a skill associated with an advertisement. | Links advertisements to standardised skills. |
| Qualification relationship | Represents a qualification requirement associated with an advertisement. | Links advertisements to qualifications. |
| Certification relationship | Represents a certification requirement associated with an advertisement. | Links advertisements to certifications. |
| Experience requirement | Represents an advertised experience requirement. | Links advertisements to experience information. |
| Location relationship | Represents a work location or geographic eligibility relationship. | Links advertisements to one or more locations. |
| Employment characteristic | Represents employment type and working-condition information. | Links advertisements to employment characteristics. |

### 14.3 Logical relationship principles

- One advertisement may have multiple job-family assignments.
- One advertisement may have multiple skills.
- One advertisement may have multiple qualifications or certifications.
- One advertisement may have multiple locations.
- One advertisement may have multiple employment characteristics.
- An employer may be associated with multiple advertisements.
- A relationship must retain its association with the canonical advertisement.
- Duplicate publication instances must not inflate canonical advertisement counts.

### 14.4 Physical implementation

The final implementation may use separate tables, linked records or another appropriate structure.

Specific database design decisions remain subject to technical architecture.

---

## 15. Counting and Aggregation Rules

### 15.1 Unique advertisements

The total advertisement count must use distinct canonical `advertisement_id` values.

Duplicate source instances must not inflate the count.

### 15.2 Job-family demand

Family-level demand is calculated using unique canonical advertisements assigned to each family.

Because one advertisement may belong to multiple families:

- Family totals may exceed the total number of unique advertisements.
- Family percentages may overlap.
- Family counts must not be presented as mutually exclusive unless an explicitly approved alternative classification is used.
- Any comparison must disclose the multi-family assignment rule.

### 15.3 Skill demand

Skill frequency is based on unique advertisement-skill relationships.

Repeated mentions of the same standardised skill in one advertisement count once for advertisement-level frequency.

### 15.4 Qualification and certification demand

Qualification and certification frequency is based on unique advertisement-qualification or advertisement-certification relationships.

These must remain separate analytical measures.

### 15.5 Geographic demand

Geographic frequency is based on unique advertisements associated with the relevant location category.

Where one advertisement covers multiple locations, geographic totals may overlap.

### 15.6 Employer counts

Employer counts must use distinct reliably identified employers.

Unknown or unverified employer identities must not be treated as confirmed distinct organisations.

### 15.7 Percentage denominators

Every percentage must identify its denominator.

Examples:

\[
\text{Skill prevalence} =
\frac{\text{Unique eligible advertisements containing the skill}}
{\text{Eligible unique advertisements in the relevant group}}
\times 100
\]

\[
\text{Salary disclosure rate} =
\frac{\text{Eligible advertisements with disclosed remuneration}}
{\text{Eligible advertisements assessed for salary disclosure}}
\times 100
\]

\[
\text{Graduate accessibility proportion} =
\frac{\text{Advertisements classified as graduate-specific or entry-level accessible}}
{\text{Advertisements assessed for graduate accessibility}}
\times 100
\]

Denominators must account for missing, unclear or unassessed values where relevant.

---

## 16. Taxonomy and Standardisation Management

### 16.1 Taxonomy requirements

The following classifications require documented management:

- Job families.
- Seniority.
- Graduate accessibility.
- Skills.
- Skill categories.
- Qualifications.
- Certifications.
- Experience.
- Salary disclosure.
- Geographic categories.
- Work arrangements.
- Employment types.
- Data-quality issue codes.

### 16.2 Version control

Taxonomy changes must be documented.

A change must identify:

- Taxonomy affected.
- Previous definition.
- New definition.
- Reason for change.
- Effective version.
- Impact on previously classified records.
- Whether records require reprocessing.

### 16.3 Standardisation safeguards

- Preserve raw source values.
- Avoid unsupported equivalence assumptions.
- Maintain consistent category definitions.
- Review ambiguous mappings.
- Document transformation rules.
- Do not change historical classifications silently.
- Ensure analysis outputs identify the relevant taxonomy or data version.

---

## 17. Privacy and Disclosure Considerations

The dataset must be designed around the project's aggregate publication objective.

The following safeguards apply:

- Collect only information necessary for approved research objectives.
- Avoid unnecessary personal information about recruiters, employees or applicants.
- Apply source-specific restrictions to stored advertisement content.
- Keep restricted raw data private.
- Do not expose restricted source text or personal information in public outputs.
- Review small-cell results before publication.
- Avoid publishing combinations that could unintentionally identify individuals or confidential opportunities.
- Use aggregate results for public-facing reporting.
- Clearly label synthetic or illustrative records if used in demonstrations.
- Do not present synthetic records as collected observations.

Specific retention periods, access permissions and deletion procedures are governed by the Data Governance Plan and Data Retention and Access documentation.

---

## 18. Confirmed Decisions and Unresolved Implementation Matters

### 18.1 Confirmed decisions

The following are approved:

- Three-layer raw, standardised and derived data model.
- Raw source preservation.
- Stable canonical advertisement identifier.
- Provenance and duplicate-tracking requirements.
- Employer variables.
- Seven job-family codes.
- Multi-family assignment.
- Seniority and graduate-accessibility classifications.
- Technical and professional skill classification.
- Qualification and certification separation.
- Experience requirement variables.
- Salary disclosure and remuneration variables.
- Geographic and remote-work variables.
- Employment and working-condition variables.
- Six distinct temporal date fields.
- Missing-data and conflict statuses.
- Data-quality and manual-review requirements.
- Nine logical data entities.
- Advertisement and relationship-level counting rules.
- Taxonomy versioning and traceability.
- Aggregate publication and privacy safeguards.

### 18.2 Unresolved implementation matters

The following remain open:

- Physical database schema and data types.
- Exact database constraints and relationships.
- Final skill taxonomy contents and version.
- Final qualification and certification taxonomy.
- Exact experience-category boundaries and overlap handling.
- Detailed salary standardisation and conversion procedures.
- Final confidence scoring thresholds.
- Exact validation rules and quality thresholds.
- Extraction libraries and technical methods.
- Physical representation of multi-valued relationships.
- Final retention periods and implementation-specific access controls.

These items must be finalised through the appropriate implementation and governance decisions. They must not be presented as already approved technical choices.

---

## 19. Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| DD-AC-01 | Raw, standardised and derived data layers are distinguished. |
| DD-AC-02 | Raw source preservation requirements are documented. |
| DD-AC-03 | Advertisement identity and provenance variables are defined. |
| DD-AC-04 | Employer variables and identity safeguards are documented. |
| DD-AC-05 | All seven approved job families and codes are defined. |
| DD-AC-06 | Multi-family classification is supported. |
| DD-AC-07 | Seniority and graduate-accessibility classifications are defined. |
| DD-AC-08 | Technical and professional skills variables are documented. |
| DD-AC-09 | Skill extraction and counting rules are defined. |
| DD-AC-10 | Qualification and certification variables are distinguished. |
| DD-AC-11 | Experience variables and provisional categories are documented. |
| DD-AC-12 | Salary disclosure and remuneration variables are defined. |
| DD-AC-13 | Geographic and work-arrangement variables are defined. |
| DD-AC-14 | Employment and working-condition variables are documented. |
| DD-AC-15 | All six approved temporal date fields are included. |
| DD-AC-16 | Missing, unclear, conflicting and not-applicable states are