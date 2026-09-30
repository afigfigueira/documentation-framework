---

# Architectural Milestones

This section records the completion of significant architectural milestones in the evolution of the Documentation Framework.

Each milestone corresponds to one or more canonical documents that collectively establish a stable architectural capability.

Once completed, these documents become part of the official Documentation Framework specification and serve as normative references for future development.

---

| Column | Description |
|---------|-------------|
| **Status** | Current state of the record within the workflow. Indicates whether the work is pending, in progress, or completed. See **Record Status** for the list of valid values. |
| **Order Date** | Date on which the record or work order was created. This represents the official registration date of the requested work. |
| **Start Date** | Date on which work effectively began. This field remains empty until the record enters the **Started** state. |
| **Completion Date** | Date on which all planned work was completed and the record was officially closed. |
| **Document** | Identifier or name of the document associated with the record. This should uniquely identify the document being created, updated, or managed. |
| **Path** | Relative or absolute location of the document within the documentation repository. This field allows the physical file to be located independently of its document identifier. |

---

# Record Status

The **Status** field represents the current stage of the work associated with a record.

| Status | Name | Description |
|--------|------|-------------|
| **O** | Open | The record has been created but work has not yet started. It is waiting to be processed. |
| **S** | Started | Work on the document is currently in progress. The record is active and has not yet been completed. |
| **C** | Completed | All planned work has been finished successfully. The record is considered closed. |

---

## Status Lifecycle

```text

                  Open
                    │
                    ▼

                 Started
                    │
                    ▼

                Completed

```

The lifecycle is intentionally simple:

- **Open** 		→ Initial state assigned when the record is created.
- **Started** 	→ Indicates that work has begun.
- **Completed** → Final state indicating that all work has been finished.

---

# Milestone Status

The **Milestone Status** field represents the overall progress of an architectural milestone.

Only the following values are valid.

| Status | Description |
|----------|-------------|
| **Not Started** | None of the documents belonging to the milestone have entered the implementation process. All associated records remain in the **Open** state. |
| **In Progress** | One or more documents belonging to the milestone are currently being developed. At least one associated record is in the **Started** state, while the milestone is not yet complete. |
| **Completed** | Every document belonging to the milestone has been completed. All associated records are in the **Completed** state and the milestone is considered finished. |

---

## Milestone Lifecycle

```text
               Not Started
                    │
                    ▼

               In Progress
                    │
                    ▼

                Completed
```

The milestone lifecycle is intentionally simple.

- **Not Started** → No work has begun on any document belonging to the milestone.
- **In Progress** → At least one document is under development.
- **Completed** → All documents associated with the milestone have been completed.

---

## Relationship with Record Status

A milestone status is derived from the status of its associated records.

| Milestone Status | Record Status Composition |
|------------------|--------------------------|
| **Not Started** | All records are **Open**. |
| **In Progress** | At least one record is **Started** or **Completed**, but not all records are **Completed**. |
| **Completed** | All records are **Completed**. |

The **Milestone Status** is therefore not managed independently. It is a summary status derived from the collection of record statuses belonging to the milestone.

---

# Table Template

| #Status | Order Date | Start Date | Completion Date |Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| O:S:C | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | XXX-XXX-NNN — Doc. Name | XXX-XXX-NNN-Doc.Name.md |
| O:S:C | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | XXX-XXX-NNN — Doc. Name | XXX-XXX-NNN-Doc.Name.md | 

---

### Review milestone scope — M8–M14

The following milestones track this review. Completed means the stated review/documentary acceptance criteria are met; it does not admit Draft documents as official normative specifications, approve them, publish them or assign a Baseline. The earlier introduction and M0–M7 remain historical records. O/S/C and milestone states are reused for the declared review scope.

## Milestone M14 — Integrated validation and final delivery

**Milestone Status:** Not Started

### Objectives and acceptance

Verify all corrected editions, classification, dependencies, identities, paths and findings; reconcile central tracking and deliver Context-Reviewed.zip with exact manifest. Initial report creation does not complete this future result.

Dependencies: M10-M13. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| O | 2026-09-30 |  |  | DF-RVW-002 — integrated validation and final delivery | /03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md |

---

## Milestone M13 — Localized identity, planning and reference reconciliation

**Milestone Status:** Not Started

### Objectives and acceptance

Recover distinct CLS-003; reconcile DID filename/reference mappings; review all roadmaps, root functional files and register findings. Validate affected operational references and qualify historical examples. General ID migration is unnecessary; localized correction remains pending.

Dependencies: M10-M12; impact map before migration. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| O | 2026-09-30 |  |  | DF-RDM-030 | /Roadmaps/02-Documentation/Classification/DF-RDM-030-ClassificationRoadmap.md |
| O | 2026-09-30 |  |  | DF-RDM-020 | /Roadmaps/02-Documentation/DocumentIdentity/DF-RDM-020-DocumentIdentityRoadmap.md |
| O | 2026-09-30 |  |  | DF-RDM-010 | /Roadmaps/02-Documentation/Metadata/DF-RDM-010-MetadataRoadmap.md |
| O | 2026-09-30 |  |  | DF-RDM-040 | /Roadmaps/02-Documentation/Templates/DF-RDM-040-TemplatesRoadmap.md |
| O | 2026-09-30 |  |  | DF-RDM-001 | /Roadmaps/DF-RDM-001-DocumentationFrameworkRoadmap.md |
| O | 2026-09-30 |  |  | DF-RDM-002 | /Roadmaps/DF-RDM-002-ArchitecturalImplementationStrategy.md |
| O | 2026-09-30 |  |  | README.md | /Roadmaps/README.md |
| O | 2026-09-30 |  |  | ArchitecturalMilestones.md | /ArchitecturalMilestones.md |
| O | 2026-09-30 |  |  | CHANGELOG.md | /CHANGELOG.md |
| O | 2026-09-30 |  |  | README.md | /README.md |
| O | 2026-09-30 |  |  | Nominal DF-CLS-003; wrong received declaration | /02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md |

---

## Milestone M12 — Documentation component review cycles

**Milestone Status:** Not Started

### Objectives and acceptance

Complete cycles for all 60 normalized component sources and content/reference checks for four README files; reconcile Metadata, Document Identity, Classification and Templates.

Dependencies: M10/M11; typed domain dependencies recorded per cycle. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| O | 2026-09-30 |  |  | DF-CLS-001 | /02-Documentation/Classification/01-Architecture/DF-CLS-001-ClassificationArchitecture.md |
| O | 2026-09-30 |  |  | DF-CLS-002 | /02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md |
| O | 2026-09-30 |  |  | DF-CLS-001 | /02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md |
| O | 2026-09-30 |  |  | DF-CLS-004 | /02-Documentation/Classification/02-Structure/DF-CLS-004-ClassificationElements.md |
| O | 2026-09-30 |  |  | DF-CLS-005 | /02-Documentation/Classification/02-Structure/DF-CLS-005-ClassificationSchema.md |
| O | 2026-09-30 |  |  | DF-CLS-009 | /02-Documentation/Classification/02-Structure/DF-CLS-009-ClassificationRelationships.md |
| O | 2026-09-30 |  |  | DF-CLS-006 | /02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md |
| O | 2026-09-30 |  |  | DF-CLS-007 | /02-Documentation/Classification/03-Behavior/DF-CLS-007-ClassificationValidation.md |
| O | 2026-09-30 |  |  | DF-CLS-008 | /02-Documentation/Classification/03-Behavior/DF-CLS-008-ClassificationGovernance.md |
| O | 2026-09-30 |  |  | DF-CLS-010 | /02-Documentation/Classification/03-Behavior/DF-CLS-010-ClassificationConstraints.md |
| O | 2026-09-30 |  |  | DF-CLS-011 | /02-Documentation/Classification/03-Behavior/DF-CLS-011-ClassificationExtensibility.md |
| O | 2026-09-30 |  |  | DF-CLS-012 | /02-Documentation/Classification/04-Reference/DF-CLS-012-ClassificationBestPractices.md |
| O | 2026-09-30 |  |  | DF-CLS-013 | /02-Documentation/Classification/04-Reference/DF-CLS-013-ClassificationDictionary.md |
| O | 2026-09-30 |  |  | DF-CLS-014 | /02-Documentation/Classification/04-Reference/DF-CLS-014-ClassificationSpecification.md |
| O | 2026-09-30 |  |  | DF-CLS-015 | /02-Documentation/Classification/04-Reference/DF-CLS-015-ClassificationExamples.md |
| O | 2026-09-30 |  |  | README.md | /02-Documentation/Classification/README.md |
| O | 2026-09-30 |  |  | DF-DID-001 | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md |
| O | 2026-09-30 |  |  | DF-DID-002 | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-002 - Document Identity Concepts.md |
| O | 2026-09-30 |  |  | DF-DID-003 | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-003 - Document Identity Model.md |
| O | 2026-09-30 |  |  | DF-DID-004 | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-004 - Document Identity Elements.md |
| O | 2026-09-30 |  |  | DF-DID-005 | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-005 - Document Identity Schema.md |
| O | 2026-09-30 |  |  | DF-DID-009 | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-009 - Document Identity Relationships.md |
| O | 2026-09-30 |  |  | DF-DID-010 | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-010 - Document Identity Constraints.md |
| O | 2026-09-30 |  |  | DF-DID-006 | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-006 - Document Identity Lifecycle.md |
| O | 2026-09-30 |  |  | DF-DID-007 | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-007 - Document Identity Validation.md |
| O | 2026-09-30 |  |  | DF-DID-008 | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-008 - Document Identity Governance.md |
| O | 2026-09-30 |  |  | DF-DID-011 | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-011 - Document Identity Extensibility.md |
| O | 2026-09-30 |  |  | DF-DID-012 | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-012 - Document Identity Best Practices.md |
| O | 2026-09-30 |  |  | DF-DID-013 | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-013 - Document Identity Dictionary.md |
| O | 2026-09-30 |  |  | DF-DID-014 | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-014 - Document Identity Specification.md |
| O | 2026-09-30 |  |  | DF-DID-015 | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-015 - Document Identity Examples.md |
| O | 2026-09-30 |  |  | README.md | /02-Documentation/DocumentIdentity/README.md |
| O | 2026-09-30 |  |  | DF-MTD-001 | /02-Documentation/Metadata/01-Architecture/DF-MTD-001-MetadataArchitecture.md |
| O | 2026-09-30 |  |  | DF-MTD-002 | /02-Documentation/Metadata/01-Architecture/DF-MTD-002-MetadataConcepts.md |
| O | 2026-09-30 |  |  | DF-MTD-003 | /02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md |
| O | 2026-09-30 |  |  | DF-MTD-004 | /02-Documentation/Metadata/01-Architecture/DF-MTD-004-MetadataElements.md |
| O | 2026-09-30 |  |  | DF-MTD-005 | /02-Documentation/Metadata/02-Structure/DF-MTD-005-MetadataSchema.md |
| O | 2026-09-30 |  |  | DF-MTD-009 | /02-Documentation/Metadata/02-Structure/DF-MTD-009-MetadataRelationships.md |
| O | 2026-09-30 |  |  | DF-MTD-010 | /02-Documentation/Metadata/02-Structure/DF-MTD-010-MetadataConstraints.md |
| O | 2026-09-30 |  |  | DF-MTD-013 | /02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md |
| O | 2026-09-30 |  |  | DF-MTD-006 | /02-Documentation/Metadata/03-Behavior/DF-MTD-006-MetadataLifecycle.md |
| O | 2026-09-30 |  |  | DF-MTD-007 | /02-Documentation/Metadata/03-Behavior/DF-MTD-007-MetadataValidation.md |
| O | 2026-09-30 |  |  | DF-MTD-008 | /02-Documentation/Metadata/03-Behavior/DF-MTD-008-MetadataGovernance.md |
| O | 2026-09-30 |  |  | DF-MTD-011 | /02-Documentation/Metadata/03-Behavior/DF-MTD-011-MetadataExtensibility.md |
| O | 2026-09-30 |  |  | DF-MTD-012 | /02-Documentation/Metadata/04-Reference/DF-MTD-012-MetadataBestPractices.md |
| O | 2026-09-30 |  |  | DF-MTD-014 | /02-Documentation/Metadata/04-Reference/DF-MTD-014-MetadataSpecification.md |
| O | 2026-09-30 |  |  | DF-MTD-015 | /02-Documentation/Metadata/04-Reference/DF-MTD-015-MetadataExamples.md |
| O | 2026-09-30 |  |  | README.md | /02-Documentation/Metadata/README.md |
| O | 2026-09-30 |  |  | DF-TPL-001 | /02-Documentation/Templates/01-Architecture/DF-TPL-001-TemplatesArchitecture.md |
| O | 2026-09-30 |  |  | DF-TPL-002 | /02-Documentation/Templates/01-Architecture/DF-TPL-002-TemplatesConcepts.md |
| O | 2026-09-30 |  |  | DF-TPL-003 | /02-Documentation/Templates/01-Architecture/DF-TPL-003-TemplatesModel.md |
| O | 2026-09-30 |  |  | DF-TPL-004 | /02-Documentation/Templates/02-Structure/DF-TPL-004-TemplateElements.md |
| O | 2026-09-30 |  |  | DF-TPL-005 | /02-Documentation/Templates/02-Structure/DF-TPL-005-TemplatesSchema.md |
| O | 2026-09-30 |  |  | DF-TPL-009 | /02-Documentation/Templates/02-Structure/DF-TPL-009-TemplatesRelationships.md |
| O | 2026-09-30 |  |  | DF-TPL-006 | /02-Documentation/Templates/03-Behavior/DF-TPL-006-TemplatesLifecycle.md |
| O | 2026-09-30 |  |  | DF-TPL-007 | /02-Documentation/Templates/03-Behavior/DF-TPL-007-TemplatesValidation.md |
| O | 2026-09-30 |  |  | DF-TPL-008 | /02-Documentation/Templates/03-Behavior/DF-TPL-008-TemplatesGovernance.md |
| O | 2026-09-30 |  |  | DF-TPL-010 | /02-Documentation/Templates/03-Behavior/DF-TPL-010-TemplatesConstraints.md |
| O | 2026-09-30 |  |  | DF-TPL-011 | /02-Documentation/Templates/03-Behavior/DF-TPL-011-TemplatesExtensibility.md |
| O | 2026-09-30 |  |  | DF-TPL-012 | /02-Documentation/Templates/04-Reference/DF-TPL-012-TemplatesBestPractices.md |
| O | 2026-09-30 |  |  | DF-TPL-013 | /02-Documentation/Templates/04-Reference/DF-TPL-013-TemplatesDictionary.md |
| O | 2026-09-30 |  |  | DF-TPL-014 | /02-Documentation/Templates/04-Reference/DF-TPL-014-TemplatesSpecification.md |
| O | 2026-09-30 |  |  | DF-TPL-015 | /02-Documentation/Templates/04-Reference/DF-TPL-015-TemplatesExamples.md |
| O | 2026-09-30 |  |  | README.md | /02-Documentation/Templates/README.md |

---

## Milestone M11 — Architecture review cycles

**Milestone Status:** Not Started

### Objectives and acceptance

Execute full document cycles for all seven architecture sources; reconcile views, responsibilities, dependencies and conventions.

Dependencies: M10; reconcile owner definitions before consumers. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| O | 2026-09-30 |  |  | DF-ARC-001 | /01-Architecture/DF-ARC-001-ArchitectureOverview.md |
| O | 2026-09-30 |  |  | DF-ARC-002 | /01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md |
| O | 2026-09-30 |  |  | DF-ARC-003 | /01-Architecture/DF-ARC-003-ArchitecturalConcepts.md |
| O | 2026-09-30 |  |  | DF-ARC-004 | /01-Architecture/DF-ARC-004-ArchitecturalLayers.md |
| O | 2026-09-30 |  |  | DF-ARC-005 | /01-Architecture/DF-ARC-005-ArchitecturalComponents.md |
| O | 2026-09-30 |  |  | DF-ARC-006 | /01-Architecture/DF-ARC-006-Terminology.md |
| O | 2026-09-30 |  |  | DF-ARC-007 | /01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md |

---

## Milestone M10 — Foundation review cycles

**Milestone Status:** In Progress

Step 4.01 (2026-09-30): Blueprint REVIEW completed with findings; its complete REVIEW/UPDATE/VALIDATE cycle remains Started. Source V1.0, Revision absent, Approved, Baseline 1.0 is unchanged; report DF-RVW-002 V1.0 R3, section 9; CHANGELOG #207-210. No completion date.

Step 4.01 UPDATE (2026-09-30): current Blueprint V2.0 R1, Draft, Baseline Not assigned; corrected pending VALIDATE DOCUMENT. Prior REVIEW edition/history remains preserved. Report DF-RVW-002 V1.0 R4, section 10; CHANGELOG #211-213. Cycle remains Started, no completion date.

Step 4.01 VALIDATE (2026-09-30): local Blueprint correction scope PASS on unchanged V2.0 R1; eleven local findings Closed-verified. Record C, completion 2026-09-30; five records O. M10 remains In Progress under record composition. Draft/unassigned; no approval or integrated conformity. Report V1.0 R5 section 11; CHANGELOG #214-216.

### Objectives and acceptance

Execute complete REVIEW/UPDATE/VALIDATE cycles for the six sources; reconcile responsible definitions, record actual editions and verification evidence. Partial Step 2 readings do not complete these cycles.

Dependencies: M9. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| O | 2026-09-30 |  |  | DF-FND-001 | /00-Foundation/DF-FND-001-FrameworkManifest.md |
| O | 2026-09-30 |  |  | DF-FND-002 | /00-Foundation/DF-FND-002-ResearchJournal.md |
| O | 2026-09-30 |  |  | DF-FND-003 | /00-Foundation/DF-FND-003-EvolutionTimeline.md |
| C | 2026-09-30 | 2026-09-30 | 2026-09-30 | DF-FND-004 — V2.0 R1 Draft, scoped validation PASS | /00-Foundation/DF-FND-004-ArchitecturalBlueprint.md |
| O | 2026-09-30 |  |  | DF-FND-005 | /00-Foundation/DF-FND-005-FrameworkEvolution.md |
| O | 2026-09-30 |  |  | DF-FND-006 | /00-Foundation/DF-FND-006-DesignRationale.md |

---

## Milestone M9 — Review conventions and tracking

**Milestone Status:** Completed

Translation follow-up 3.2.1 (2026-09-30): DF-RVW-002 V1.0 R2, English, Draft, Baseline Not assigned; CHANGELOG #205/#206; scoped translation evidence in report assets. Original acceptance scope and milestone state retained.

Current supporting report edition: DF-RVW-002 V1.0 R5 includes the Step 4.01 review, update and scoped validation; the original M9 criteria remain completed. Foundation source work is tracked separately in M10.

### Objectives and acceptance

Establish review policy, two artifact identities, stable plan, central records and scoped checks. Completion excludes downstream source propagation, integrated consistency and approval. Completed on 2026-09-30.

Dependencies: M8. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| C | 2026-09-30 | 2026-09-30 | 2026-09-30 | DF-RVW-001 | /03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md |
| C | 2026-09-30 | 2026-09-30 | 2026-09-30 | DF-RVW-002 — conventions and tracking | /03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md |

---

## Milestone M8 — Received corpus established

**Milestone Status:** Completed

### Objectives and acceptance

Inventory all 87 input Markdown files, record editions/hashes, collisions and evidence limits. Acceptance excludes correction of input findings; completed on 2026-09-30.

Dependencies: supplied Context.zip. Evidence: DF-RVW-002 and its attached manifests/matrices. Source editions: received V1.0 (declared Revision or absent), except new review documents V1.0 R1. No estimated completion dates.

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | -------- | ---- |
| C | 2026-09-30 | 2026-09-30 | 2026-09-30 | DF-RVW-002 — input inventory | /03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md |

---

## Milestone M7 — Templates Component

**Milestone Status:** Completed

### Objectives

Define the complete architectural specification of the Templates component.

## Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
| ------: | :--------- | :--------- | :-------------- | ------------------------------------- | -------------------------------------------------------------------------- |
| C | 2026-09-11 | 2026-09-11 | 2026-09-11 | README | /02-Documentation/Templates/README.md |
| C | 2026-09-13 | 2026-09-13 | 2026-09-13 | DF-TPL-001 — Templates Architecture | /02-Documentation/Templates/01-Architecture/DF-TPL-001-TemplatesArchitecture.md |
| C | 2026-09-13 | 2026-09-13 | 2026-09-13 | DF-TPL-002 — Templates Concepts | /02-Documentation/Templates/01-Architecture/DF-TPL-002-TemplatesConcepts.md |
| C | 2026-09-13 | 2026-09-13 | 2026-09-13 | DF-TPL-003 — Templates Model | /02-Documentation/Templates/01-Architecture/DF-TPL-003-TemplatesModel.md |
| C | 2026-09-18 | 2026-09-18 | 2026-09-18 | DF-TPL-004 — Template Elements | /02-Documentation/Templates/02-Structure/DF-TPL-004-TemplateElements.md |
| C | 2026-09-18 | 2026-09-18 | 2026-09-18 | DF-TPL-005 — Templates Schema | /02-Documentation/Templates/02-Structure/DF-TPL-005-TemplatesSchema.md |
| C | 2026-09-18 | 2026-09-18 | 2026-09-19 | DF-TPL-006 — Templates Lifecycle | /02-Documentation/Templates/03-Behavior/DF-TPL-006-TemplatesLifecycle.md |
| C | 2026-09-19 | 2026-09-19 | 2026-09-19 | DF-TPL-007 — Templates Validation | /02-Documentation/Templates/03-Behavior/DF-TPL-007-TemplatesValidation.md |
| C | 2026-09-19 | 2026-09-19 | 2026-09-22 | DF-TPL-008 — Templates Governance | /02-Documentation/Templates/03-Behavior/DF-TPL-008-TemplatesGovernance.md |
| C | 2026-09-22 | 2026-09-22 | 2026-09-22 | DF-TPL-009 — Templates Relationships | /02-Documentation/Templates/02-Structure/DF-TPL-009-TemplatesRelationships.md |
| C | 2026-09-22 | 2026-09-22 | 2026-09-22 | DF-TPL-010 — Templates Constraints | /02-Documentation/Templates/03-Behavior/DF-TPL-010-TemplatesConstraints.md |
| C | 2026-09-22 | 2026-09-22 | 2026-09-22 | DF-TPL-011 — Templates Extensibility | /02-Documentation/Templates/03-Behavior/DF-TPL-011-TemplatesExtensibility.md |
| C | 2026-09-22 | 2026-09-22 | 2026-09-23 | DF-TPL-012 — Templates Best Practices | /02-Documentation/Templates/04-Reference/DF-TPL-012-TemplatesBestPractices.md |
| C | 2026-09-23 | 2026-09-23 | 2026-09-23 | DF-TPL-013 — Templates Dictionary | /02-Documentation/Templates/04-Reference/DF-TPL-013-TemplatesDictionary.md |
| C | 2026-09-23 | 2026-09-23 | 2026-09-23 | DF-TPL-014 — Templates Specification | /02-Documentation/Templates/04-Reference/DF-TPL-014-TemplatesSpecification.md |
| C | 2026-09-23 | 2026-09-23 | 2026-09-23 | DF-TPL-015 — Templates Examples | /02-Documentation/Templates/04-Reference/DF-TPL-015-TemplatesExamples.md |

---

## Milestone M6 — Classification Component

**Milestone Status:** Completed

### Objectives

Define the complete architectural specification of the Classification component.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|:-----------|:-----------|------------------------------|--------------------------------------------------------------------------------------------------------------|
| C | 2026-08-09 | 2026-08-09 | 2026-08-09 | README | /02-Documentation/Classification/README.md |
| C | 2026-08-09 | 2026-08-09 | 2026-08-09 | DF-CLS-001 — Classification Architecture | /02-Documentation/Classification/01-Architecture/DF-CLS-001-ClassificationArchitecture.md |
| C | 2026-08-09 | 2026-08-09 | 2026-08-09 | DF-CLS-002 — Classification Concepts | /02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md |
| C | 2026-08-20 | 2026-08-20 | 2026-08-20 | DF-CLS-003 — Classification Model | /02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md |
| C | 2026-08-20 | 2026-08-20 | 2026-08-20 | DF-CLS-004 — Classification Elements | /02-Documentation/Classification/02-Structure/DF-CLS-004-ClassificationElements.md |
| C | 2026-08-25 | 2026-08-25 | 2026-08-25 | DF-CLS-005 — Classification Schema | /02-Documentation/Classification/02-Structure/DF-CLS-005-ClassificationSchema.md |
| C | 2026-08-25 | 2026-08-25 | 2026-08-25 | DF-CLS-006 — Classification Lifecycle | /02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md |
| C | 2026-08-25 | 2026-08-25 | 2026-08-27 | DF-CLS-007 — Classification Validation | /02-Documentation/Classification/03-Behavior/DF-CLS-007-ClassificationValidation.md |
| C | 2026-08-27 | 2026-08-27 | 2026-08-27 | DF-CLS-008 — Classification Governance | /02-Documentation/Classification/03-Behavior/DF-CLS-008-ClassificationGovernance.md |
| C | 2026-08-27 | 2026-08-27 | 2026-08-28 | DF-CLS-009 — Classification Relationships | /02-Documentation/Classification/02-Structure/DF-CLS-009-ClassificationRelationships.md |
| C | 2026-08-28 | 2026-08-28 | 2026-08-29 | DF-CLS-010 — Classification Constraints | /02-Documentation/Classification/03-Behavior/DF-CLS-010-ClassificationConstraints.md |
| C | 2026-08-29 | 2026-08-29 | 2026-09-06 | DF-CLS-011 — Classification Extensibility | /02-Documentation/Classification/03-Behavior/DF-CLS-011-ClassificationExtensibility.md |
| C | 2026-09-06 | 2026-09-06 | 2026-09-06 | DF-CLS-012 — Classification Best Practices | /02-Documentation/Classification/04-Reference/DF-CLS-012-ClassificationBestPractices.md |
| C | 2026-09-06 | 2026-09-06 | 2026-09-06 | DF-CLS-013 — Classification Dictionary | /02-Documentation/Classification/04-Reference/DF-CLS-013-ClassificationDictionary.md |
| C | 2026-09-06 | 2026-09-06 | 2026-09-07 | DF-CLS-014 — Classification Specification | /02-Documentation/Classification/04-Reference/DF-CLS-014-ClassificationSpecification.md |
| C | 2026-09-07 | 2026-09-07 | 2026-09-07 | DF-CLS-015 — Classification Examples | /02-Documentation/Classification/04-Reference/DF-CLS-015-ClassificationExamples.md |

---

## Milestone M5 — Document Identity Component

**Milestone Status:** Completed

### Objectives

Define the complete architectural specification of the Document Identity component.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|:-----------|:-----------|------------------------------|--------------------------------------------------------------------------------------------------------------|
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | README | /02-Documentation/DocumentIdentity/README.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-DID-001 — Document Identity Architecture | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-DID-002 — Document Identity Concepts | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-002-DocumentIdentityConcepts.md |
| C | 2026-08-07 | 2026-08-07 | 2026-08-07 | DF-DID-003 — Document Identity Model | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-003-DocumentIdentityModel.md |
| C | 2026-08-07 | 2026-08-07 | 2026-08-07 | DF-DID-004 — Document Identity Elements | /02-Documentation/DocumentIdentity/01-Architecture/DF-DID-004-DocumentIdentityElements.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-005 — Document Identity Schema | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-005-DocumentIdentitySchema.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-006 — Document Identity Lifecycle | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-006-DocumentIdentityLifecycle.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-007 — Document Identity Validation | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-007-DocumentIdentityValidation.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-008 — Document Identity Governance | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-008-DocumentIdentityGovernance.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-009 — Document Identity Relationships | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-009-DocumentIdentityRelationships.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-010 — Document Identity Constraints | /02-Documentation/DocumentIdentity/02-Structure/DF-DID-010-DocumentIdentityConstraints.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-011 — Document Identity Extensibility | /02-Documentation/DocumentIdentity/03-Behavior/DF-DID-011-DocumentIdentityExtensibility.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-012 — Document Identity Best Practices | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-012-DocumentIdentityBestPractices.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-013 — Document Identity Dictionary | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-013-DocumentIdentityDictionary.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-014 — Document Identity Specification | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-014-DocumentIdentitySpecification.md |
| C | 2026-08-08 | 2026-08-08 | 2026-08-08 | DF-DID-015 — Document Identity Examples | /02-Documentation/DocumentIdentity/04-Reference/DF-DID-015-DocumentIdentityExamples.md |

---

## Milestone M4 — Metadata Component

**Milestone Status:** Completed

### Objectives

Define the architectural model governing metadata within the Documentation Framework.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|:-----------|:-----------|------------------------------|-----------------------------------------------------------------------------------------------|
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | README | /02-Documentation/Metadata/README.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-MTD-001 — Metadata Architecture | /02-Documentation/Metadata/01-Architecture/DF-MTD-001-MetadataArchitecture.md |
| C | 2026-08-04 | 2026-08-04 | 2026-08-04 | DF-MTD-002 — Metadata Concepts | /02-Documentation/Metadata/01-Architecture/DF-MTD-002-MetadataConcepts.md |
| C | 2026-08-04 | 2026-08-04 | 2026-08-05 | DF-MTD-003 — Metadata Model | /02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-004 — Metadata Elements | /02-Documentation/Metadata/01-Architecture/DF-MTD-004-MetadataElements.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-005 — Metadata Schema | /02-Documentation/Metadata/02-Structure/DF-MTD-005-MetadataSchema.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-006 — Metadata Lifecycle | /02-Documentation/Metadata/03-Behavior/DF-MTD-006-MetadataLifecycle.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-007 — Metadata Validation | /02-Documentation/Metadata/03-Behavior/DF-MTD-007-MetadataValidation.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-008 — Metadata Governance | /02-Documentation/Metadata/03-Behavior/DF-MTD-008-MetadataGovernance.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-009 — Metadata Relationships | /02-Documentation/Metadata/02-Structure/DF-MTD-009-MetadataRelationships.md |
| C | 2026-08-05 | 2026-08-05 | 2026-08-05 | DF-MTD-010 — Metadata Constraints | /02-Documentation/Metadata/02-Structure/DF-MTD-010-MetadataConstraints.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-MTD-011 — Metadata Extensibility | /02-Documentation/Metadata/03-Behavior/DF-MTD-011-MetadataExtensibility.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-MTD-012 — Metadata Best Practices | /02-Documentation/Metadata/04-Reference/DF-MTD-012-MetadataBestPractices.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-MTD-013 — Metadata Dictionary | /02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-MTD-014 — Metadata Specification | /02-Documentation/Metadata/04-Reference/DF-MTD-014-MetadataSpecification.md |
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-MTD-015 — Metadata Examples | /02-Documentation/Metadata/04-Reference/DF-MTD-015-MetadataExamples.md |

---

## Milestone M3 — Core Architecture

**Milestone Status:** Completed

### Objectives

Define the architectural model governing the Documentation Framework.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| C | 2026-08-02 | 2026-08-02 | 2026-08-03 | DF-ARC-001 — Architecture Overview | /01-Architecture/DF-ARC-001-ArchitectureOverview.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-002 — Architectural Principles | /01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-003 — Architectural Concepts | /01-Architecture/DF-ARC-003-ArchitecturalConcepts.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-004 — Architectural Layers | /01-Architecture/DF-ARC-004-ArchitecturalLayers.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-005 — Architectural Components | /01-Architecture/DF-ARC-005-ArchitecturalComponents.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-006 — Terminology | /01-Architecture/DF-ARC-006-Terminology.md |
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-ARC-007 — Component Documentation Structure | /01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md |

---

## Milestone M2 — Roadamaps

**Milestone Status:** In Progress

### Objectives

Establish a compromises that defines the long-term implementation strategy for the Documentation Framework.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | README | /Roadmaps/README.md | 
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | DF-RDM-001 — Documentation Framework Roadmap | /Roadmaps/DF-RDM-001-DocumentationFrameworkRoadmap.md | 
| C | 2026-08-03 | 2026-08-03 | 2026-08-03 | DF-RDM-010 - Metadata Roadmap | /Roadmaps/02-Documentation/Metadata/DF-RDM-010-MetadataRoadmap.md | 
| C | 2026-08-06 | 2026-08-06 | 2026-08-06 | DF-RDM-020 - Document Identity Roadmap | /Roadmaps/02-Documentation/DocumentIdentity/DF-RDM-020-DocumentIdentityRoadmap.md | 
| C | 2026-08-09 | 2026-08-09 | 2026-08-09 | DF-RDM-030 - Classification Roadmap | /Roadmaps/02-Documentation/Classification/DF-RDM-030-ClassificationRoadmap.md | 
| C | 2026-09-09 | 2026-09-09 | 2026-09-10 | DF-RDM-040 - Templates Roadmap | /Roadmaps/02-Documentation/Templates/DF-RDM-040-TemplatesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-050 - Registry Roadmap | /Roadmaps/04-Discovery/Registry/DF-RDM-050-RegistryRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-060 - Workflow Roadmap | /Roadmaps/03-Governance/Workflow/DF-RDM-060-WorkflowRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-070 - Policies Roadmap | /Roadmaps/03-Governance/Policies/DF-RDM-070-PoliciesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-080 - Baselines Roadmap | /Roadmaps/03-Governance/Baselines/DF-RDM-080-BaselinesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-090 - Relationships Roadmap | /Roadmaps/04-Discovery/Relationships/DF-RDM-090-RelationshipsRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-100 - Knowledge Graph Roadmap | /Roadmaps/04-Discovery/KnowledgeGraph/DF-RDM-100-KnowledgeGraphRoadmap.md | 

---

## Milestone M1 — Foundation

**Milestone Status:** Completed

### Objectives

Establish the conceptual and architectural foundations of the Documentation Framework.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | DF-FND-001 — Framework Manifest | /00-Foundation/DF-FND-001-FrameworkManifest.md | 
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | DF-FND-002 — Research Journal | /00-Foundation/DF-FND-002-ResearchJournal.md | 
| C | 2026-07-30 | 2026-07-30 | 2026-08-01 | DF-FND-003 — Evolution Timeline | /00-Foundation/DF-FND-003-EvolutionTimeline.md | 
| C | 2026-08-30 | 2026-08-01 | 2026-08-01 | DF-FND-004 — Architectural Blueprint | /00-Foundation/DF-FND-004-ArchitecturalBlueprint.md | 
| C | 2026-07-30 | 2026-08-01 | 2026-08-02 | DF-FND-005 — Framework Evolution | /00-Foundation/DF-FND-005-FrameworkEvolution.md |  
| C | 2026-07-30 | 2026-08-02 | 2026-08-02 | DF-FND-006 — Design Rationale | /00-Foundation/DF-FND-006-DesignRationale.md | 

---

## Milestone M0 — Repository Initialization

**Milestone Status:** Completed

### Objectives

- Establish the Documentation Framework repository.
- Define the initial repository structure.
- Define the initial license rules.
- Establish the project documentation.

### Documents

| #Status | Order Date | Start Date | Completion Date | Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | CHANGELOG | /CHANGELOG.md |
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | Architectural Milestones | /ArchitecturalMilestones.md | 
| C | 2026-07-30 | 2026-07-30 | 2026-07-30 | LICENSE | /LICENSE.md | 
| C | 2026-07-30 | 2026-07-30 | 2026-08-02 | README | /README.md | 

---

**End of Document**

---