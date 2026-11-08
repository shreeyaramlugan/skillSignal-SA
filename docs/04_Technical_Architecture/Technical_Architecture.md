# SkillSignal SA — Technical Architecture

**Project ID:** SSA-001
**Document ID:** SSA-DOC-013
**Version:** 0.1
**Status:** Proposed architecture — technical decisions pending

---

## 1. Purpose

This document describes the proposed technical architecture
for SkillSignal SA.

The architecture supports a reproducible data analytics
pipeline investigating South African technology employment demand.

## 2. Architecture Principles

- Modular and maintainable components.
- Reproducible data processing.
- Separation of raw, interim and processed data.
- Traceable data transformations.
- Automated data-quality checks.
- Zero-budget implementation.
- Appropriate technical complexity.
- Secure handling of restricted data.
- Clear separation between experimentation and reusable code.

## 3. Proposed Technology Stack

| Component | Proposed technology | Decision status |
|---|---|---|
| Programming language | Python | Proposed |
| Data manipulation | Pandas | Proposed |
| Scientific computing | NumPy and SciPy | Proposed |
| Statistical modelling | Statsmodels | Proposed |
| NLP | spaCy | Proposed |
| Database | PostgreSQL | Proposed |
| Database access | To be evaluated | Pending |
| Development environment | Jupyter | Proposed |
| Business intelligence | Power BI | Proposed |
| Version control | Git and GitHub | Existing project tooling |
| Testing | Python testing framework | Pending |
| Configuration | Structured configuration files | Proposed |

The final technology versions and implementation choices
must be recorded in the decision log.

## 4. Logical Architecture

The proposed system consists of these layers:

1. Source layer
   - Approved job advertisement sources.
   - Source-specific acquisition procedures.

2. Acquisition layer
   - Retrieval of permitted records.
   - Acquisition metadata.
   - Source provenance.

3. Raw data layer
   - Original acquired records.
   - Restricted storage where required.
   - No uncontrolled overwriting.

4. Processing layer
   - Extraction and parsing.
   - Cleaning and standardisation.
   - Deduplication.
   - Classification.
   - Skills extraction.

5. Quality layer
   - Schema validation.
   - Missing-value checks.
   - Duplicate checks.
   - Classification validation.
   - Processing logs.

6. Storage layer
   - Structured analytical records.
   - Relational database.
   - Controlled processed datasets.

7. Analysis layer
   - Exploratory analysis.
   - Statistical analysis.
   - Skills relationship analysis.
   - Geographic and temporal analysis.

8. Presentation layer
   - Power BI intelligence report.
   - Research figures and tables.
   - Research publication.

## 5. Proposed Data Flow

Approved sources
    -> Acquisition
    -> Raw records
    -> Extraction and cleaning
    -> Validation
    -> Classification and skills extraction
    -> Processed records
    -> Database and analytical datasets
    -> Statistical analysis
    -> BI reporting and research publication

Every stage should preserve relevant provenance and
document failures or exclusions.

## 6. Python Project Responsibilities

The proposed src modules are:

| Module | Responsibility |
|---|---|
| acquisition | Source-specific data retrieval and ingestion |
| cleaning | Parsing, standardisation and deduplication |
| classification | Job-family and seniority classification |
| extraction | Skills, qualifications and requirement extraction |
| analysis | Statistical and analytical procedures |
| visualisation | Reusable charts and analytical figures |

Modules should perform focused responsibilities and avoid
unnecessary dependencies between components.

## 7. Database Responsibilities

The proposed PostgreSQL database will support:
- Structured advertisement records.
- Source provenance.
- Skills and taxonomy relationships.
- Classification results.
- Quality and processing information.
- Analytical querying.

The final schema and database implementation remain pending.

## 8. Security and Data Protection

- Credentials must not be committed.
- Restricted raw records must remain private.
- Public outputs require review.
- Database access must be appropriately restricted.
- Source-specific retention requirements must be respected.

## 9. Error Handling and Observability

The pipeline should record:
- Acquisition failures.
- Parsing failures.
- Invalid records.
- Excluded records and reasons.
- Validation failures.
- Transformation errors.
- Processing timestamps.

Errors must not silently disappear or produce misleading
analytical outputs.

## 10. Outstanding Decisions

- Final technology versions.
- Database implementation.
- Database connectivity and migration tooling.
- ETL orchestration.
- NLP implementation.
- BI integration.
- Testing framework.
- Backup and deployment arrangements.

---
**Status note:** This is a proposed logical architecture,
not a final implementation specification.
