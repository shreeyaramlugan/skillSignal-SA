# SkillSignal SA — ETL Design

**Project ID:** SSA-001
**Document ID:** SSA-DOC-015
**Version:** 0.1
**Status:** Proposed pipeline — implementation pending

---

## 1. Purpose

This document describes the proposed Extract, Transform
and Load pipeline for SkillSignal SA.

The pipeline must produce traceable, validated and
reproducible analytical data.

## 2. Pipeline Stages

### Stage 1 — Source Assessment

- Confirm that the source is approved.
- Review access conditions and restrictions.
- Record source information.
- Define permitted acquisition procedures.

### Stage 2 — Extraction

- Retrieve permitted advertisement records.
- Capture source identifiers where available.
- Record acquisition timestamps.
- Record acquisition failures.
- Preserve original content where retention is permitted.

### Stage 3 — Raw Data Storage

- Store acquired records separately.
- Preserve source provenance.
- Prevent uncontrolled overwriting.
- Apply access restrictions.

### Stage 4 — Parsing and Standardisation

- Parse source formats.
- Standardise dates and text.
- Normalise relevant fields.
- Preserve original values where useful.
- Identify missing or malformed fields.

### Stage 5 — Cleaning and Deduplication

- Identify duplicate records.
- Apply documented matching rules.
- Record exclusions.
- Avoid deleting records without traceability.
- Distinguish exact duplicates from possible duplicates.

### Stage 6 — Classification

- Classify advertisements into approved job families.
- Apply seniority classification rules.
- Standardise geographic information.
- Record uncertain or ambiguous classifications.

### Stage 7 — Skills and Requirement Extraction

- Extract skills from permitted advertisement text.
- Identify qualifications and experience requirements.
- Map original terms to standardised taxonomy entries.
- Preserve extraction method and relevant confidence information.
- Flag uncertain extraction results for review.

### Stage 8 — Data Quality Validation

Check:
- Required fields.
- Data types and formats.
- Date validity.
- Duplicate status.
- Classification validity.
- Missing values.
- Referential integrity.
- Extraction consistency.

### Stage 9 — Loading

- Load validated records into the approved storage destination.
- Preserve relationships and identifiers.
- Record processing results.
- Prevent invalid records from silently entering analytical outputs.

### Stage 10 — Analytical Preparation

- Prepare datasets for statistical analysis.
- Generate approved aggregates.
- Produce analytical tables.
- Record dataset versions and preparation steps.

## 3. Proposed Data Lifecycle

data/raw/
    -> data/interim/
    -> data/processed/
    -> Database
    -> Analytical outputs

Each stage must have documented entry and exit conditions.

## 4. Failure Handling

The pipeline should distinguish:
- Source unavailable.
- Access denied.
- Extraction failure.
- Parsing failure.
- Invalid record.
- Duplicate record.
- Classification failure.
- Validation failure.
- Database loading failure.

Failures should be logged with sufficient context for
investigation without exposing credentials or restricted data.

## 5. Idempotency and Reprocessing

The implementation should aim to:
- Avoid creating duplicate records when a stage is rerun.
- Use stable identifiers where available.
- Record processing versions.
- Make transformations reproducible.
- Support controlled reprocessing.

Final idempotency rules remain pending implementation design.

## 6. Pipeline Testing

Potential tests include:
- Valid and invalid source records.
- Missing mandatory fields.
- Malformed dates.
- Duplicate advertisements.
- Ambiguous job titles.
- Unknown skills.
- Missing geographic information.
- Invalid relationships.
- Failed database operations.

## 7. Logging and Metrics

The pipeline should record:
- Records acquired.
- Records parsed.
- Records rejected.
- Duplicates identified.
- Records classified.
- Skills extracted.
- Validation failures.
- Records loaded.
- Processing duration.

Metrics must be clearly defined and consistently calculated.

## 8. Outstanding Decisions

- Source-specific acquisition implementation.
- Extraction libraries.
- Transformation framework.
- Deduplication algorithms.
- Classification methods.
- NLP implementation.
- Database loading method.
- Logging implementation.
- Scheduling and orchestration.

---
**Status note:** This is a proposed ETL workflow.
No specific extraction or transformation technology is finalised.
