# SkillSignal SA — Database Design

**Project ID:** SSA-001
**Document ID:** SSA-DOC-014
**Version:** 0.1
**Status:** Conceptual design — implementation pending

---

## 1. Purpose

This document proposes the conceptual database structure
for SkillSignal SA.

The design supports traceable job advertisement records,
skills analysis, classification and research reporting.

## 2. Proposed Design Principles

- Avoid unnecessary duplication.
- Preserve original source information where permitted.
- Separate advertisements from extracted skills.
- Support multiple skills per advertisement.
- Preserve classification and taxonomy provenance.
- Use consistent identifiers.
- Enforce data integrity.
- Support analytical queries.

## 3. Proposed Conceptual Entities

| Entity | Purpose |
|---|---|
| DataSource | Records approved source information |
| JobAdvertisement | Stores structured advertisement records |
| JobFamily | Stores the seven project job families |
| Skill | Stores standardised skill definitions |
| AdvertisementSkill | Connects advertisements to extracted skills |
| Qualification | Stores qualification information |
| AdvertisementQualification | Connects advertisements to qualifications |
| Location | Stores standardised geographic information |
| ClassificationResult | Records classification outcomes |
| AcquisitionRun | Records acquisition activity |
| ProcessingRun | Records processing activity |
| DataQualityIssue | Records quality findings and exceptions |

These are conceptual entities, not approved database tables.

## 4. Proposed Relationships

- One DataSource may have many JobAdvertisements.
- One JobAdvertisement belongs to a source.
- One JobFamily may classify many JobAdvertisements.
- One JobAdvertisement may contain many Skills.
- One Skill may appear in many JobAdvertisements.
- AdvertisementSkill resolves the many-to-many skill relationship.
- One JobAdvertisement may reference multiple qualifications.
- One Location may be associated with multiple advertisements.
- One AcquisitionRun may acquire multiple records.
- One ProcessingRun may process multiple records.
- One record may have multiple DataQualityIssues.

## 5. Identifier Strategy

Potential identifiers include:
- Internal primary keys.
- Source-specific record identifiers.
- Stable skill identifiers.
- Classification identifiers.
- Processing run identifiers.

The final choice of UUIDs, integer keys or other identifiers
remains pending.

## 6. Integrity Requirements

The final implementation should consider:
- Primary key constraints.
- Foreign key constraints.
- Appropriate uniqueness rules.
- Nullability.
- Valid date ranges.
- Controlled classification values.
- Referential integrity.
- Duplicate detection.

## 7. Historical Traceability

The database design should support:
- Source attribution.
- Acquisition timestamps.
- Processing timestamps.
- Taxonomy versions.
- Classification methods.
- Relevant transformation history.

The degree of historical versioning remains to be determined.

## 8. Proposed Analytical Access

The database should support queries involving:
- Job-family demand.
- Skill frequencies.
- Skill co-occurrence.
- Seniority and experience requirements.
- Qualification requirements.
- Geographic distributions.
- Temporal distributions.
- Salary disclosure.

## 9. Outstanding Decisions

- Final entity and table list.
- Physical schema.
- Column names and data types.
- Key strategy.
- Indexing strategy.
- Normalisation decisions.
- Database migration tooling.
- Connection and access configuration.
- Backup and recovery arrangements.

---
**Status note:** No database schema or SQL migration
is approved by this conceptual design.
