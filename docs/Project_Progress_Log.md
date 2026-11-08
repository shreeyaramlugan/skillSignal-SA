# SkillSignal SA — Project Progress Log

**Project ID:** SSA-001  
**Document ID:** SSA-DOC-003  
**Version:** 2.0  
**Status:** Active

## 1. Purpose

Records project activities, completed tasks, evidence, blockers and outstanding work.

This document provides a chronological record of SkillSignal SA's progress, including project setup, research planning, documentation approvals, technical preparation and implementation.

It distinguishes between:

- Activities completed and supported by evidence.
- Project decisions and documentation content approved.
- Approved documentation awaiting incorporation into local files.
- Activities that have not started.
- Outstanding work, dependencies and blockers.

Approval of documentation does not automatically mean that the corresponding local file has been updated, saved, committed or implemented.

The Project Progress Log must be updated as work is completed and verified.

---

## 2. Project Milestones

| ID | Milestone | Status |
|---|---|---|
| MS-001 | Project Charter | Completed |
| MS-002 | Project Workspace | Completed |
| MS-003 | GitHub Repository | Completed |
| MS-004 | Project Documentation | Completed — Initial Foundation |
| MS-005 | Research Design | Approved — File Incorporation Pending |
| MS-006 | Data Acquisition Design | Approved — File Incorporation Pending |
| MS-007 | Technical Architecture | In Progress |
| MS-008 | Data Engineering | Not Started |
| MS-009 | Analytics and NLP | Not Started |
| MS-010 | BI and Publication | Not Started |
| MS-011 | Development Schedule and Readiness Review | Completed |
| MS-012 | Section B Research Methodology Documentation | Approved — File Incorporation Pending |
| MS-013 | Section B Data Governance Documentation | Approved — File Incorporation Pending |
| MS-014 | Project Decision Log Update | Approved — File Incorporation Pending |
| MS-015 | Project Progress Log Update | Awaiting Approval |

### 2.1 Milestone Status Clarification

**MS-001 to MS-004:** The initial project charter, workspace, repository and foundational documentation have been completed.

**MS-005 and MS-006:** The research design and data acquisition methodology have progressed beyond their initial planning stage. The relevant Section B documentation has received approval, but its incorporation into the local files remains outstanding.

**MS-007:** Preliminary technical architecture documentation was created during Section A. Final physical architecture and implementation decisions remain outstanding.

**MS-008 to MS-010:** Data engineering, advanced analytics, BI and publication implementation have not started.

**MS-011:** The approved development schedule and readiness review have been completed.

**MS-012 to MS-015:** These milestones track the Section B documentation approval and incorporation process separately, so documentation approval is not confused with actual file updates.

---

## 3. Activity Log

The original activity entries from Version 1.2 are retained. Additional entries record the Section B planning and approval work.

| Date | Task ID | Activity | Status | Evidence |
|---|---|---|---|---|
| 2026-11-08 | A1 | Created project workspace and opened in VS Code | Completed | Local project folder |
| 2026-11-08 | A2 | Created GitHub repository and connected local Git | Completed | GitHub repository and initial commit |
| 2026-11-08 | A3 | Created and finalised foundational project documentation | Completed | Section A and project management documents |
| 2026-11-08 | A4 | Prepared and validated Python analytics environment | Completed | requirements.txt, package import test, pip check and Jupyter kernel |
| 2026-11-08 | A5.8 | Created and validated approved project directory structure | Completed | Project directory review |
| 2026-11-08 | A5.9 | Created and validated preliminary data governance documentation | Completed | Four files in docs/03_Data_Governance |
| 2026-11-08 | A5.10 | Created and validated preliminary research methodology documentation | Completed | Four files in docs/02_Research_Methodology |
| 2026-11-08 | A5.11 | Created and validated proposed technical architecture documentation | Completed | Four files in docs/04_Technical_Architecture |
| 2026-11-08 | A5.12 | Reviewed project structure and existing Git ignore rules | Completed | Directory listing and Git status |
| 2026-11-08 | A6 | Created and validated the approved ten-week development schedule | Completed | docs/01_Project_Management/Development_Schedule.md |
| 2026-11-08 | A7 | Completed project readiness assessment and authorised progression to Section B | Completed | docs/01_Project_Management/Project_Readiness_Review.md |
| 2026-11-08 | B1–B2 | Finalised and approved the research problem, justification, aim and objectives | Completed | Approved Section B research decisions |
| 2026-11-08 | B3 | Finalised and approved twelve research questions and seven hypotheses with H0 and H1 | Completed | Approved Research Questions and Hypotheses content |
| 2026-11-08 | B4 | Finalised and approved research scope, boundaries, inclusions and exclusions | Completed | Approved Research Design content |
| 2026-11-08 | B5 | Finalised and approved the target population, accessible population, sampling frame and sampling strategy | Completed | Approved Sampling Strategy content |
| 2026-11-08 | B6 | Approved the retrospective research period and collection framework | Completed | Approved Research Design and Sampling Strategy content |
| 2026-11-08 | B7 | Finalised and approved the data dictionary and variable operationalisation requirements | Completed | Approved Data Dictionary content |
| 2026-11-08 | B8 | Finalised and approved the statistical analysis framework | Completed | Approved Statistical Methodology content |
| 2026-11-08 | B-GOV | Finalised and approved the data governance plan | Completed | Approved Data Governance Plan content |
| 2026-11-08 | B-DEC | Revised and approved the complete Project Decision Log, retaining Section A and incorporating Section B decisions | Completed | Approved Project Decision Log content |
| 2026-11-08 | B-PROG | Revised the Project Progress Log using the existing Version 1.2 as its foundation | Awaiting Approval | Proposed Project Progress Log Version 2.0 |

### 3.1 Section B Approval Record

The following eight documents have received explicit approval of their proposed contents:

| No. | Document | Content Approval | Local File Update |
|---|---|---|---|
| 1 | `docs/02_Research_Methodology/Research_Design.md` | Approved | Pending |
| 2 | `docs/02_Research_Methodology/Research_Questions_and_Hypotheses.md` | Approved | Pending |
| 3 | `docs/02_Research_Methodology/Sampling_Strategy.md` | Approved | Pending |
| 4 | `docs/03_Data_Governance/Data_Dictionary.md` | Approved | Pending |
| 5 | `docs/02_Research_Methodology/Statistical_Methodology.md` | Approved | Pending |
| 6 | `docs/03_Data_Governance/Data_Governance_Plan.md` | Approved | Pending |
| 7 | `docs/Project_Decision_Log.md` | Approved | Pending |
| 8 | `docs/Project_Progress_Log.md` | Awaiting Approval | Pending |

**Important:** The approval statuses above refer to the proposed document contents. No local file updates, Git commits or pushes have been performed as part of this documentation approval process.

---

## 4. Outstanding Tasks

### 4.1 Section A Close-out

- Review the A6/A7 planning documentation and updated progress log.
- Obtain authorisation to incorporate the approved updates.
- Verify the resulting documentation.
- Commit and push the authorised changes after verification.

### 4.2 Section B Documentation

- Obtain approval of Project Progress Log Version 2.0.
- Obtain explicit authorisation to update the eight approved local files.
- Review existing local file contents before replacing or updating them.
- Reconcile approved content with useful existing documentation.
- Incorporate the approved contents into the relevant files.
- Verify file paths, headings, cross-references and consistency.
- Confirm that all eight files reflect their approved versions.
- Review Git status and confirm that only authorised files have changed.
- Commit and push the verified documentation updates when authorised.

### 4.3 Section C — Data Source Research

- Identify candidate recruitment platforms and employer career pages.
- Assess source relevance, accessibility, reliability and coverage.
- Review source-specific terms and permitted use.
- Investigate historical advertisement availability for the approved research period.
- Evaluate zero-budget acquisition feasibility.
- Populate the Data Source Register with actual source assessments.
- Approve suitable sources and acquisition methods.
- Conduct a source and collection feasibility assessment.
- Establish the dataset target after the source pilot.

### 4.4 Section D — Data Architecture

- Finalise the physical data architecture.
- Translate the approved logical entities into a physical data model.
- Define canonical advertisement and duplicate relationships.
- Define employer, skills, qualifications, certifications and location relationships.
- Establish schema validation and data integrity requirements.
- Record database implementation decisions.

### 4.5 Section E — Technical Implementation

- Finalise the technical stack and versions.
- Establish reproducible dependency management.
- Implement project configuration and processing components.
- Establish logging, validation and testing procedures.
- Integrate the approved physical data model.
- Document development and execution procedures.

### 4.6 Sections F–J — Implementation and Delivery

- Acquire and validate the eligible advertisement dataset.
- Implement cleaning, standardisation and deduplication.
- Implement job-family classification and information extraction.
- Produce reproducible analytical datasets.
- Implement descriptive, comparative and suitable inferential analysis.
- Evaluate optional NLP and advanced analytical methods.
- Develop and validate BI outputs.
- Complete technical and analytical testing.
- Review publication permissions and disclosure risks.
- Prepare the final research and portfolio deliverables.

---

## 5. Blockers

**Current status: No confirmed blockers recorded.**

There are outstanding dependencies and unresolved decisions, but these are not automatically classified as blockers.

| ID | Dependency / Potential Blocker | Current Position | Required Action |
|---|---|---|---|
| BLK-001 | Section B local file incorporation | Approved content awaiting explicit authorisation | Obtain authorisation and update files |
| BLK-002 | Data source availability | Individual source assessments not completed | Conduct Section C source research |
| BLK-003 | Source permissions | Source-specific permissions not yet confirmed | Review applicable source restrictions |
| BLK-004 | Historical advertisement coverage | Availability not yet established | Evaluate permitted historical sources |
| BLK-005 | Dataset size | No fixed target approved before pilot | Establish feasibility-based target |
| BLK-006 | Physical database design | Logical model approved; physical implementation pending | Complete Section D |
| BLK-007 | Experience category boundaries | Exact implementation boundaries remain open | Finalise before implementation |
| BLK-008 | Salary comparability | Standardisation depends on available data | Assess during source and data evaluation |
| BLK-009 | Technical implementation choices | Some technology decisions remain unresolved | Complete technical assessment |
| BLK-010 | NLP implementation | Methods remain proposals | Assess feasibility and research value |

No item above should be marked as an active blocker unless it actually prevents progress on a planned activity.

---

## 6. Activity Entry Template

Use this template when recording new project activities.

| Field | Details |
|---|---|
| Date | YYYY-MM-DD |
| Task ID | |
| Activity | |
| Status | Not Started / In Progress / Completed / Blocked |
| Evidence | |
| Issues | |
| Next Action | |

---

## 7. Progress Recording Rules

1. Record completed activities only when the work has actually been performed.
2. Identify evidence supporting completed activities.
3. Distinguish approval of documentation content from local file incorporation.
4. Do not mark a document update as completed until the local file has been updated and verified.
5. Do not mark a Git commit or push as completed without evidence.
6. Keep unresolved decisions and dependencies visible.
7. Do not report data acquisition, statistical analysis or research findings before those activities have occurred.
8. Update the milestone table when project stages change.
9. Retain historical activity entries when revising this document.
10. Record significant project decisions in the Project Decision Log.

---

## 8. Current Project Position

### 8.1 Completed

- Project charter and initial planning.
- Workspace and repository setup.
- Initial project documentation.
- Python analytics environment preparation and validation.
- Project directory structure and preliminary governance documentation.
- Preliminary research methodology documentation.
- Proposed technical architecture documentation.
- Existing Git ignore rules review.
- Ten-week development schedule.
- Project readiness assessment.
- Section B research design and methodology decisions.
- Section B sampling strategy.
- Section B data dictionary and variable operationalisation.
- Section B statistical methodology.
- Section B data governance plan.
- Revised Project Decision Log content.

### 8.2 Approved but Not Yet Incorporated

- Research Design.
- Research Questions and Hypotheses.
- Sampling Strategy.
- Data Dictionary.
- Statistical Methodology.
- Data Governance Plan.
- Project Decision Log.

Project Progress Log Version 2.0 is awaiting approval.

### 8.3 Not Yet Completed

- Section B local file incorporation and verification.
- Individual data source assessments and approvals.
- Final source-specific acquisition procedures.
- Physical database architecture.
- Final technical implementation decisions.
- Data acquisition and engineering.
- Statistical analysis and NLP implementation.
- BI dashboard implementation.
- Testing and validation.
- Publication and final portfolio delivery.

---

## 9. Next Project Milestone

The immediate next milestone is:

**Complete and incorporate the approved Section B documentation.**

The work will proceed as follows:

1. Approve this revised Project Progress Log.
2. Obtain explicit authorisation for local file changes.
3. Inspect and reconcile the existing eight files.
4. Incorporate the approved contents without changing unrelated files.
5. Verify the resulting documents and cross-references.
6. Review the final Git status.
7. Commit and push only when explicitly authorised.
8. Begin Section C data source research.

No local file changes, Git commits or pushes are authorised by this progress log.

---

## 10. Document Maintenance

This document must be updated throughout the project lifecycle.

The project owner is responsible for ensuring that the progress log accurately reflects completed work, evidence, blockers, approvals, outstanding tasks and project milestones.

**Current version:** 2.0  
**Current status:** Active  
**Section A:** Completed  
**Section B:** Documentation content approved; local file incorporation pending  
**Next milestone:** Incorporation and verification of approved Section B documentation