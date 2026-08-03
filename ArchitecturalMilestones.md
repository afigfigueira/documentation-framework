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

# Table Template

| #Status | Order Date | Start Date | Completion Date |Document | Path |
|--:|:-----------|-----------|-----------|-------------------|-------------------|
| O:S:C | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | XXX-XXX-NNN — Doc. Name | XXX-XXX-NNN-Doc.Name.md |
| O:S:C | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | XXX-XXX-NNN — Doc. Name | XXX-XXX-NNN-Doc.Name.md | 

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
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-010 - Metadata Roadmap | /Roadmaps/02-Documentation/Metadata/DF-RDM-010-MetadataRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-020 - Document Identity Roadmap | /Roadmaps/02-Documentation/DocumentIdentity/DF-RDM-020-DocumentIdentityRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-030 - Templates Roadmap | /Roadmaps/02-Documentation/Templates/DF-RDM-030-TemplatesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-040 - Registry Roadmap | /Roadmaps/04-Discovery/Registry/DF-RDM-040-RegistryRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-050 - Workflow Roadmap | /Roadmaps/03-Governance/Workflow/DF-RDM-050-WorkflowRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-060 - Policies Roadmap | /Roadmaps/03-Governance/Policies/DF-RDM-060-PoliciesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-070 - Baselines Roadmap | /Roadmaps/03-Governance/Baselines/DF-RDM-070-BaselinesRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-080 - Relationships Roadmap | /Roadmaps/04-Discovery/Relationships/DF-RDM-080-RelationshipsRoadmap.md | 
| O | yyyy-mm-dd | yyyy-mm-dd | yyyy-mm-dd | DF-RDM-090 - Knowledge Graph Roadmap | /Roadmaps/04-Discovery/KnowledgeGraph/DF-RDM-090-KnowledgeGraphRoadmap.md | 

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