# SkillSignal SA — Data Dictionary

**Project ID:** SSA-001
**Document ID:** SSA-DOC-007
**Version:** 0.1
**Status:** Preliminary field proposal — not a final database schema

---

## 1. Purpose

This document proposes a common vocabulary for describing
South African technology job advertisements.

The final dataset schema will be confirmed after research design,
source assessment and acquisition planning.

Field availability will vary by source. Missing information
must not be fabricated or silently inferred.

## 2. Proposed Advertisement Fields

| Field | Description | Proposed type | Notes |
|---|---|---|---|
| record_id | Internal unique record identifier | String | Generated internally |
| source_id | Reference to source register | String | Required for provenance |
| source_record_id | Identifier assigned by original source | String | Nullable |
| source_url | Original advertisement URL | String | Subject to retention and access rules |
| job_title | Advertised position title | String | Preserve original title |
| employer_name | Advertised employer | String | Nullable where unavailable |
| location_text | Original advertised location | String | Preserve original wording |
| province | Standardised South African province | String | Derived where supportable |
| city | Standardised city or locality | String | Derived where supportable |
| country | Country associated with advertisement | String | Expected to be South Africa |
| publication_date | Original publication date | Date | Nullable |
| closing_date | Application closing date | Date | Nullable |
| employment_type | Employment arrangement | String | Requires classification rules |
| workplace_type | On-site, hybrid or remote | String | Requires classification rules |
| job_family | Classified project job family | String | Seven-family taxonomy |
| seniority_level | Classified seniority | String | Requires approved rules |
| experience_requirement | Advertised experience requirement | String | Preserve original wording |
| minimum_experience_years | Extracted minimum years | Decimal | Nullable; extraction must be traceable |
| qualification_requirement | Advertised qualification requirement | String | Preserve original wording |
| salary_text | Original advertised salary wording | String | Nullable |
| salary_min | Extracted lower salary bound | Decimal | Nullable; retain currency context |
| salary_max | Extracted upper salary bound | Decimal | Nullable; retain currency context |
| salary_currency | Currency of advertised salary | String | Do not assume if unclear |
| description_text | Advertisement description | Text | Subject to source restrictions |
| skills_extracted | Extracted skills | Structured data | Requires taxonomy and extraction method |
| acquisition_timestamp | Date and time record was acquired | Timestamp | Include timezone |
| processing_timestamp | Date and time record was processed | Timestamp | Include timezone |
| record_status | Processing or quality status | String | Controlled values to be defined |

## 3. Proposed Skill Extraction Structure

Skills should ultimately be represented in a separate related
structure rather than relying exclusively on a single text field.

Potential fields:

| Field | Description |
|---|---|
| skill_id | Internal skill identifier |
| skill_name | Standardised skill name |
| skill_category | Skill classification |
| original_term | Wording found in advertisement |
| record_id | Related advertisement |
| extraction_method | Method used to identify the skill |
| confidence | Extraction confidence, if supported |
| taxonomy_version | Version of the skills taxonomy |

## 4. Data Type and Missing-Value Rules

- Dates must use a consistent date representation.
- Timestamps must retain timezone information.
- Monetary values must retain currency and salary-period context.
- Missing values must be represented consistently.
- Unknown values must not be replaced with fabricated values.
- Original source wording should be preserved where useful and permitted.
- Derived values must be distinguishable from original source values.

## 5. Classification and Derived Fields

Fields such as job family, seniority, province, employment type
and extracted skills may be derived from source content.

Each derived field must have a documented rule or method.

Classification decisions must be reproducible and reviewable.

## 6. Outstanding Decisions

The following require later approval:
- Final field list and mandatory fields.
- Database data types and constraints.
- Normalisation and relational design.
- Controlled vocabularies.
- Job-family and seniority classification rules.
- Skills taxonomy structure.
- NLP extraction output and confidence handling.
- Source-specific field availability.

---
**Status note:** This is a planning dictionary, not an approved
PostgreSQL schema or a guarantee that every source provides
these fields.
