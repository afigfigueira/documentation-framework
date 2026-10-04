# Documentation Framework

# Architectural Layers

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-ARC-004 |
| **Title** | Architectural Layers |
| **Family** | Architecture |
| **Type** | Structure |
| **Author** | Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Introduction

The Documentation Framework organizes structural responsibilities into seven architectural areas, called Layers in this document. A Layer groups related primary responsibilities; it is not automatically a runtime tier, directory, service or registered component.

Primary allocation, cross-cutting participation, documentary authority and required consumer/provider contracts are distinct. Modularity, maintainability, scalability and controlled evolution are intended properties assessed against actual contracts and evidence, rather than guaranteed outcomes of a seven-area diagram.

---

# 2. Purpose

This structural specification organizes responsibilities and component allocation, defines scoped dependency constraints and explicit interfaces, separates conceptual concerns from structural areas, and supports assessed incremental evolution.

Its primary responsibility is organization, composition and structural restrictions; therefore its Type is Structure. Family Architecture identifies the documentary area, not a component or a special Type. Independent development is an objective subject to provider/consumer compatibility, not unconditional edition independence.

---

# 3. Scope

This document defines structural Layers, their responsibilities, primary component allocation and the rules for interpreting required dependencies. It summarizes owner contracts without replacing their detailed definitions.

It does not establish an implemented DMS, operational permissions, users, storage architecture or a complete executable workflow. DF defines documentary contracts; a DMS, tool or applicable manual process executes them. A CMS governs changes in its own scope. Source presence and architectural capability descriptions do not establish implemented services.

Every README.md, CHANGELOG.md and ArchitecturalMilestones.md is a non-normalized functional file at every corpus location. These files remain subject to applicable content, reference and integrity checks, without normalized header, Family/Type or identity requirements. The exclusion creates no exceptions to the four Types for normalized documents.

---

# 4. Layered Architecture

The Documentation Framework is organized into **seven structural Layers**. The following view records allocation and responsibility; its row order does not declare a dependency edge or execution sequence.

<!-- original-section-view: 4 -->
**Previously unnamed view in §4 — Structural areas and primary allocation.**

| Structural area | Primary structural responsibility | Registered component allocation in this working view |
|---|---|---|
| Foundation | Framework identity, vision, rationale and historical basis | Supporting definition documents; no component invented |
| Architecture | Common concepts, principles, structural rules and vocabulary | Supporting definition documents; no component invented |
| Documentation | Documentary representation, identity, classification and templates | Metadata; Document Identity; Classification; Templates |
| Governance | Documentary lifecycle, policy, review and snapshot contracts | Workflow; Policies; Reviews; Baselines |
| Discovery | Typed connections and traceable catalog/network/discovery views | Registry; Relationships; Knowledge Graph; Navigation; Search |
| Automation | Repeatable checks and generation under owner contracts | Validation; Metadata Generator; Registry Generator; Consistency Verification; Documentation Generator |
| Integration | Scoped adapters to external environments | Source Control Integration; CI/CD Integration; IDE Integration; Documentation Platform Integration; AI Integration |
<!-- end-original-section-view -->

The five conceptual concerns are Knowledge, Documentation, Governance, Discovery and Preservation. They are a different view from these seven structural areas. Knowledge is the subject matter represented by documents; Preservation participates across documentary history, exact editions, governance and immutable snapshots. Neither creates an additional structural Layer or component by implication.

Foundation and Architecture organize supporting definitions. A folder or definition document is not registered as a capability component merely by appearing in this view. The 23 capability entries are allocated 4/4/5/5/5 across Documentation/Governance/Discovery/Automation/Integration. Section 12 separately types selected required contracts; §13 constrains their interpretation.

---

# 5. Foundation Layer

## 5.1. Purpose

Foundation provides the framework's conceptual basis: identity, architectural vision, rationale, historical evolution and foundational interpretation. Its documents explain why the framework exists and establish common foundations; they do not duplicate detailed component ownership.

---

## 5.2. Responsibilities

Foundation records framework philosophy, foundational assumptions, architectural motivations and the provenance of historical evolution. Architectural Blueprint provides the foundation architectural comparison basis; Manifest states orientation, Rationale explains decisions, and historical documents record when/how evolution occurred.

Responsibility for maintaining these definitions differs from operational execution and domain ownership. Knowledge and Preservation participation does not allocate every concerned component to Foundation or make these six documents registered components.

---

## 5.3. Primary Documents

| Source | Role and current comparison limit |
|---|---|
| [DF-FND-001 — Framework Manifest](../00-Foundation/DF-FND-001-FrameworkManifest.md) | Framework orientation and classification; earlier scoped validation only |
| [DF-FND-002 — Research Journal](../00-Foundation/DF-FND-002-ResearchJournal.md) | Research history and original rationale provenance; earlier scoped validation only |
| [DF-FND-003 — Evolution Timeline](../00-Foundation/DF-FND-003-EvolutionTimeline.md) | Evolution events and dated chronology; earlier scoped validation only |
| [DF-FND-004 — Architectural Blueprint](../00-Foundation/DF-FND-004-ArchitecturalBlueprint.md) | Foundational architectural definitions/comparison basis; earlier scoped validation only |
| [DF-FND-005 — Framework Evolution](../00-Foundation/DF-FND-005-FrameworkEvolution.md) | Framework evolution account and historical scope; earlier scoped validation only |
| [DF-FND-006 — Design Rationale](../00-Foundation/DF-FND-006-DesignRationale.md) | Reasons for architectural decisions; earlier scoped validation only |

These are supplied sources with earlier scoped documentary validation, Draft/unassigned working editions and their own historical evidence. Their presence grants no release approval, implemented service or whole-framework conformity.

---

# 6. Architecture Layer

## 6.1. Purpose

Architecture defines common principles, concepts, structural allocation, component boundaries and terminology. Concepts establishes the conceptual model; Layers establishes structural organization; Components records capability responsibilities; Terminology provides consultation against responsible definitions.

---

## 6.2. Responsibilities

Architecture maintains the common model, structural rules, responsibility boundaries and shared vocabulary. It references detailed owner contracts instead of redefining their semantics.

Foundation/Architecture documentary authority references are not automatically runtime dependencies on an upper-area implementation. Common definitions and domain specifications may cross-reference each other without proving a service cycle; actual required contracts must still be assessed explicitly under §§12–13.

---

# 7. Documentation Layer

## 7.1. Purpose

Documentation defines documentary representation, logical identity, mutable classification and reusable structures. It represents Knowledge while contributing to Discovery, Governance and Preservation under applicable contracts; this participation does not change primary allocation.

---

## 7.2. Components

- Metadata
- Document Identity
- Classification
- Templates

---

## 7.3. Responsibilities

Metadata describes identified editions through applicable descriptors. Document Identity owns logical identity semantics; Classification owns category semantics; Templates defines reusable structural representations. Governance owns lifecycle and approval meaning even when Metadata represents those values.

Within Metadata, Dictionary defines descriptors and meaning, Schema organizes references to definitions, Profile constrains applicable usage, and Instance supplies values under one effective Profile. This summary creates neither catalog records nor a canonical Profile and does not replace the scheduled owner specifications.

Document identity, exact edition, Version/Revision, edition Status and Baseline membership remain distinct. Stable corpus allocations do not change merely because Family, Type or location changes. Conceptual separation of content and descriptors allows coordinated evolution; it does not guarantee automatic consistency or independent revisions.

---

# 8. Governance Layer

## 8.1. Purpose

Governance defines contracts for documentary evolution: lifecycle states, transition conditions, review evidence, approval decisions, publication eligibility and snapshot selection. DF defines those rules; a DMS, tool or applicable manual process executes them. A CMS may initiate/govern change within its own scope.

---

## 8.2. Components

- Workflow
- Policies
- Reviews
- Baselines

---

## 8.3. Responsibilities

Workflow applies documentary state/transition contracts to identified editions; Policies defines applicable rules; Reviews records examined scope and findings; Baselines defines exact snapshot membership. These are capability responsibilities, not proof of an implemented lifecycle engine.

Review, validation, approval, publication and membership are separate events. A check result identifies exact bytes/edition, rules, coverage and limits; it does not grant approval or publication. Status belongs to the identified edition, not every past/future representation of its logical document.

A Baseline is a separately identified immutable, explicitly selected set of exact approved editions, with relevant pinned relationship context or traceable verification evidence. Approval eligibility, consistency and actual inclusion are separate checks. A Draft successor does not retarget earlier members or inherit membership. The working header's Not assigned marker evidences no selection.

Preservation includes history, exact editions and snapshot provenance across areas. Integration may execute an authorized publication operation; it does not acquire independent approval authority or replace Governance contracts.

---

# 9. Discovery Layer

## 9.1. Purpose

Discovery defines semantic access to identified entities, editions and relationships. Directories remain physical locations; they do not provide semantic identity or authority by themselves. Discovery can expose Draft, historical or snapshot-specific editions when their state and scope are explicit; discoverability does not establish approval.

---

## 9.2. Components

- Registry
- Relationships
- Knowledge Graph
- Navigation
- Search

---

## 9.3. Responsibilities

Relationships owns typed connection records with identified endpoints and provenance. Relation kinds distinguish semantic reference, association, replacement, navigation and required dependency. A semantic connection does not automatically impose a provider service requirement.

Registry supplies catalog/lookup projections and Knowledge Graph supplies network projections from identified authoritative records/editions. Catalog or projection authority does not replace Identity, Classification, Governance or relationship-record ownership. Derived copies are allowed with source-edition provenance, refresh rules and current/stale/historical/snapshot status.

Navigation and Search consume declared information sources to support access and knowledge organization. A particular Registry-to-Graph or search pipeline requires its own scoped contract/evidence; no universal intermediate service is inferred from the list. Dependency analysis must retain genuine required edges and distinguish them from other relation kinds; this source certifies neither a complete network nor a globally acyclic graph.

---

# 10. Automation Layer

## 10.1. Purpose

Automation defines repeatable documentary capabilities under applicable owner contracts. Actual implementations operate on identified representations and inputs. The architectural model provides definitions and constraints; it does not prove deployed tools or eliminate files, formats and storage adapters.

---

## 10.2. Components

- Validation
- Metadata Generator
- Registry Generator
- Consistency Verification
- Documentation Generator

The received activity labels Metadata Generation, Registry Generation and Documentation Generators correspond here to the named component entries Metadata Generator, Registry Generator and Documentation Generator in ARC-005. This is label reconciliation, not new component registration or completed reconciliation of that peer source.

---

## 10.3. Responsibilities

Validation and Consistency Verification consume identified requirements from responsible owners. A result records exact input editions/bytes, applicable rules, checks, observations, coverage, executor and limits. Successful checks do not approve artifacts, select a Baseline, guarantee product consequences or establish integrated conformity.

Generators produce documentary artifacts or projections under explicit input/output contracts and provenance. They do not redefine descriptor, identity, classification, lifecycle or relationship meaning. Generated values require assessment and refresh/freshness evidence where applicable. Reducing manual maintenance is an intended benefit, not a measured or guaranteed outcome asserted by this specification.

---

# 11. Integration Layer

## 11.1. Purpose

Integration defines adapters connecting documentary contracts to supported external environments. It consumes the relevant domain interfaces and authorization contracts; adapters are selected according to the use case, not a mandatory product ecosystem or a newly inferred Layer. Intended integration does not establish an installed or implemented tool.

---

## 11.2. Components

- Source Control Integration
- CI/CD Integration
- IDE Integration
- Documentation Platform Integration
- AI Integration

Received Source Control, CI/CD, IDE Extensions and Documentation Platforms are reconciled with the ARC-005 integration component names above. An IDE extension is a possible implementation of IDE Integration, not its exhaustive definition. All five entries retain Integration as their primary area.

---

## 11.3. Responsibilities

Integrations can support source-control provenance, checks in delivery pipelines, authoring environments, authorized documentary publication and AI assistance. The applicable executor implements the operation using identified inputs and owner contracts; an external platform does not become a new documentary semantic authority.

Publishing follows Governance authorization for the exact edition. AI-assisted contributions record actual authorship/contribution and examined evidence separately from user authorization, review, validation and approval. Subsequent human or tool edits require assessment of the resulting bytes; a previous check result does not transfer automatically or assign responsibility for product consequences.

Integration existence, completeness, performance and outcomes need implementation evidence beyond this structural specification.

---

# 12. Layer Dependencies

A required dependency is directed **consumer→provider**: the consumer needs the stated provider contract in the declared scope. Allocation, documentary authority reference, semantic association, data projection, navigation and execution order are separately typed and must not be inferred solely from row order or arrows.

For cross-Layer required contracts governed here, the support order is Foundation, Architecture, Documentation, Governance, Discovery, Automation, Integration. Lower means an earlier support area in this declared order, not a lower visual row. A consumer's cross-Layer required provider belongs to an earlier support area. This does not require every consumer to depend on every earlier Layer or form an adjacent serial chain. Same-Layer required contracts are permitted under explicit ownership/interfaces and the cycle rule. Changing this structural constraint requires assessed architectural revision under §17, not an unrecorded upward-dependency exception.

<!-- original-section-view: 12 -->
**Previously unnamed view in §12 — Selected required contracts; consumer→provider.**

| Consumer | Consumer area | Provider | Provider area | Required contract | Scope/justification |
|---|---|---|---|---|---|
| Registry | Discovery | Metadata | Documentation | Descriptive values with source-edition provenance | When indexing edition descriptors; refresh or identify stale values |
| Knowledge Graph | Discovery | Document Identity | Documentation | Entity identity for logical document nodes | When keying document nodes; other entity kinds use their own endpoint identity contracts |
| Knowledge Graph | Discovery | Relationships | Discovery | Typed connection records and provenance | When projecting the semantic network and interpreting dependency kinds |
| Workflow | Governance | Metadata | Documentation | Represented state/edition descriptors | When interpreting documentary state values for a governance transition |
| Workflow | Governance | Policies | Governance | Applicable transition and evidence rules | When deciding permitted governance operations; execution remains with the applicable process |
| Baselines | Governance | Document Identity | Documentation | Logical member identity | When selecting/preserving document-edition members |
| Baselines | Governance | Metadata | Documentation | Exact edition-reference/descriptive contract | When selecting/preserving exact editions; relevant relationship context must also be pinned or evidenced |
<!-- end-original-section-view -->

These seven intended contracts reproduce the selected comparison basis in Concepts V2.0 R1 §8/Blueprint V2.0 R1 §8.11 with primary areas added. Knowledge Graph→Relationships and Workflow→Policies are legitimate same-Layer pairs. The rows are architectural declarations for their stated scopes, not a verified complete graph or implementation inventory.

The received seven-box dependency chain is preserved in input/diff/view provenance, not accepted as a mandatory service or execution sequence. Its allocation meaning belongs to §4. Foundation documents referencing component sources, or Metadata representing Governance/Identity/Classification meanings, do not automatically create runtime dependencies. Conversely, an indispensable provider contract remains required even if its data arrives through a projection or an interface is labelled a reference.

The complete graph requires owner/consumer reconciliation, explicit context-specific edges and cycle/compatibility assessment beyond these rows. Unresolved peer claims remain recorded; no global acyclicity or integrated conformity is asserted.

---

# 13. Dependency Rules

The following rules govern declared structural allocation and required consumption. Their applicability is explicit; documentary navigation and semantic associations are not a substitute for evidence of actual required dependencies.

---

## 13.1. Rule 1 — Downward Dependencies

Apply the support order defined in §12 to required cross-Layer provider contracts. Record the consumer, provider, primary areas, contract, scope and responsible source edition. Same-Layer consumption is assessed through the component interface and ownership contracts.

No required edge is inferred from vertical position or an illustrative execution arrow. No arbitrary required higher-area dependency is accepted by relabelling it as reference/navigation; a changed allocation or support constraint requires a traceable compatibility/impact decision under §17.

---

## 13.2. Rule 2 — No Circular Dependencies

Circular required dependencies are prohibited in the governed contract scope, including cycles among components within an area and across areas. Assess actual required edges and source evidence, not just the area ordering. A missing edge or a different relationship label cannot establish acyclicity.

Where an actual required cycle or conflicting provider declaration is found, retain it visibly in the evidence and reconcile the responsible contracts/allocations. This working source does not certify a complete cycle-free framework graph.

---

## 13.3. Rule 3 — Independent Evolution

Preserve separation and compatible provider contracts where feasible. Independent component/Layer development remains subject to consumer constraints, coordinated descriptive/content changes and exact-edition compatibility assessment. Shared concerns do not require independent releases, and separate areas do not guarantee them.

---

## 13.4. Rule 4 — Explicit Interfaces

Required interactions name the actual provider contract, consumer use, scope and authoritative source edition. Registered components provide capability boundaries; Foundation/Architecture sources provide applicable definitions. Distinguish a definition reference from an operational interface requirement.

Implementations must identify actual input/output representations and executor evidence within their scope. This structural summary does not fabricate a missing detailed interface specification or implementation.

---

## 13.5. Rule 5 — Responsibility Isolation

Each registered component has exactly one primary structural allocation in this working model. Primary ownership does not confine all participation to one concern or forbid explicit consumer/provider collaboration. Preserve authoritative domain semantics while recording cross-cutting participation and traceable projections.

Metadata remains in Documentation; Workflow and Baselines remain in Governance. Knowledge/Preservation participation creates neither a competing owner nor an additional structural allocation. Primary reallocation requires the assessed architectural change process in §17.

---

# 14. Layer Characteristics

The following are intended architectural characteristics with contract and evidence limits. They guide design and assessment; allocation alone does not guarantee operating quality.

---

## 14.1. Cohesion

Components grouped in an area have related primary responsibilities. Assess cohesion against the component definitions and explicit boundaries; do not invent an extra component merely to make a directory layout uniform.

---

## 14.2. Independence

Conceptual separation avoids unnecessary coupling and preserves domain ownership. It permits explicit required contracts, cross-cutting participation and coordinated edition evolution. It is not unconditional independence of provider/consumer meaning or releases.

---

## 14.3. Stability

Foundation and common architectural contracts aim for stable meaning, with justified evolution and assessed consumer effects. No relative change frequency is mandated: an earlier support area may require urgent or incompatible correction when evidence warrants it.

---

## 14.4. Extensibility

Additional capabilities, Layers or allocation changes require a demonstrated need, owner/consumer impact assessment, explicit contract/dependency mapping and transition evidence. Extension is preferred where it preserves meaning; it is not guaranteed to leave existing areas unaffected.

---

## 14.5. Technology Independence

Layer definitions avoid prescribing a particular implementation technology unless it is an explicit integration constraint. Actual tools still need formats, adapters and execution evidence. Technology independence does not certify implementation availability or universal suitability.

---

# 15. Relationship with Architectural Components

Layers organize primary component responsibilities; components identify capability boundaries. Each registered component has exactly one primary area while contributing across concerns through declared contracts. The 23 entries in §§7–11 retain their 4/4/5/5/5 allocation.

Detailed component registration/responsibilities are supplied by ARC-005, linked in §16. This source uses its named counterparts for seven received activity/environment labels and makes that mapping explicit in §§10.2/11.2. It creates no new components and does not certify unreconciled peer dependencies or implemented services.

Foundation/Architecture supporting documents, the five conceptual concerns, documentary Family/Type and physical directories are separate classifications. Reallocating a capability requires impact/transition assessment, not a document rename or Family/Type edit alone.

---

# 16. Relationship with Other Architecture Documents

The following documentary references identify supplied roles and current comparison limits. They are not automatic required runtime edges or completed peer cycles.

| Source | Relationship and comparison limit |
|---|---|
| [DF-ARC-001 — Architecture Overview](DF-ARC-001-ArchitectureOverview.md) | Overall architecture; received count/direction/independence remains scheduled reconciliation |
| [DF-ARC-002 — Architectural Principles](DF-ARC-002-ArchitecturalPrinciples.md) | Governing principles; §8.2 permits justified breaking changes; full cycle pending |
| [DF-ARC-003 — Architectural Concepts](DF-ARC-003-ArchitecturalConcepts.md) | Conceptual model and selected scoped required contracts; V2.0 R1 with earlier exact-source local validation |
| [DF-ARC-005 — Architectural Components](DF-ARC-005-ArchitecturalComponents.md) | Component registration/responsibilities; matching names do not complete its owner/dependency reconciliation |
| [DF-ARC-006 — Terminology](DF-ARC-006-Terminology.md) | Terminology consultation; abbreviated/duplicated received definitions remain scheduled reconciliation |

---

# 17. Evolution Guidelines

Preserve conceptual integrity, explicit domain ownership, dependency constraints and compatible meaning where feasible. A new Layer, component reallocation, changed responsibility or revised required contract must identify the previous/new mapping, rationale, affected owners/consumers and source editions before propagation.

Assess whether extension preserves existing contracts; a new capability can affect structure and cannot be assumed harmless. Necessary incompatible changes require explicit justification, transition plan and verification. Under the adopted review policy, compatible correction retains Version; compatible additive capability increments minor; incompatible contract change increments major and resets minor to 0. Each changed persisted edition increments Revision monotonically, including across Version changes. Validation without source change retains both coordinates and is recorded centrally.

A complete propagation and integrated dependency/compatibility check is a separate result. Earlier scoped local validation does not establish every consumer's conformity; source identities and historical evidence remain preserved unless a necessary mapped migration is explicitly justified.

---

# 18. Conclusion

The structural model distinguishes seven areas, one primary allocation per capability, cross-cutting concerns, semantic ownership and scoped required consumption. It supports assessed maintainability and evolution without guaranteeing those outcomes or implemented operational capability.

This working edition applies eight findings and two warnings as **Corrected—pending validation**. Exact-source VALIDATE DOCUMENT, peer propagation and integrated checks remain pending. Draft/unassigned confers no approval, publication or Baseline membership.

## 18.1. Compatibility assessment

V1.0 asserted unscoped only-lower/no-higher dependencies in §§12/13.1, confined responsibilities in §13.5 and mandatory backward compatibility in §17. V2.0 replaces ambiguous serial/visual dependency interpretation with explicit support order, scoped consumer→provider contracts and same-Layer requirements; distinguishes primary ownership from cross-cutting participation; and permits justified incompatible evolution under an assessed transition.

This is an **incompatible normative contract reconciliation**. Type/count/name corrections alone would be compatible; the changed constraints justify Version 1.0→2.0. Declared Revision 0 increments to 1 without reset. DF-ARC-004 and its path remain stable; no Component/Class or identity allocation is invented. The operating review conventions are defined by [DF-RVW-001 — Review Policy](../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md).

## 18.2. Local edition history

| Date | Version | Revision | Contribution/event | State/evidence |
|---|---|---|---|---|
| Not supplied | 1.0 | 0 | Received Layers source; Author absent | Family Architecture/Type Layers; Draft/Baseline1.0 declarations preserved; approval/selection evidence not supplied |
| 2026-10-05 | 2.0 | 1 | Codex — AI assistant: seven areas, scoped required contracts, primary/cross-cutting ownership, component label reconciliation, execution/evidence boundaries and references | Family Architecture/Type Structure; Draft; Baseline Not assigned; ten corrections pending VALIDATE DOCUMENT; CHANGELOG #281; Review Report §31 |

Input SHA-256: `086e0280fea3a95e42cc452e88fd68f5a0ef6f7f21680ef183d367090a8947ab`. Actual content contribution differs from user authorization, review, validation, ownership and approval. Mixed human/assistant contributions retain their attribution. Later disk edits need assessment of the resulting edition/bytes; previous evidence does not transfer automatically or assign responsibility for consequences of the final product. No original author is invented and no historic approval is inherited.

## 18.3. Propagation and verification limits

This UPDATE changes Layers and central report/tracking/evidence only. Concepts and the six Foundation sources retain their prior exact-source validation scopes. Concepts' earlier note about received Layers discrepancies remains event-time evidence and does not certify this successor. Overview, Principles, Components, Terminology and detailed owner sources retain their scheduled cycles and remaining discrepancies.

The [DF-RVW-002 — Review Report](../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md) §31 records the actual before/after map, source/view hashes, affected comparison sections and construction checks. The complete received source and two originally unnamed views remain in the input/diff/map; replacement views use original-section provenance rather than invented historic IDs.

M11 remains In Progress: Concepts C, Layers S, five peers O; no Layers completion date. All 19 prior global records remain Open; INV-04/REV2-01/02 still require remaining source reconciliation. Earlier 67 local closures retain their exact-source scopes. Owner catalog/Profile, identity/classification and full required-graph/compatibility reconciliation remain pending. No final integrated conformity, release, selected snapshot or final Context-Reviewed.zip is asserted.

---

**End of Document**

---
