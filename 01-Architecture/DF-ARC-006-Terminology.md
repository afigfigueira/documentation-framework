# Documentation Framework

# Terminology

| Metadata | Value |
|---|---|
| **Document ID** | DF-ARC-006 |
| **Title** | Terminology |
| **Family** | Architecture |
| **Type** | Reference |
| **Author** | Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Introduction

This glossary provides the common consultation and convergence vocabulary for the Documentation Framework. Entries identify subjects, contexts, controlled aliases and responsible source meanings; they do not transfer every domain’s semantic authority to Terminology.

Architectural sources use applicable canonical meanings and identify qualified contexts or deviations. Existing conflicts and incomplete owner contracts remain recorded for reconciliation. Consistent communication is an assessed objective, not a guarantee established by a glossary’s presence.

---

# 2. Purpose

The primary responsibility is terminology consultation: identify meanings and distinctions, reference responsible contracts, and support traceable architectural usage and evolution. Therefore Type is Reference; Family Architecture denotes the common documentary area, not an invented component or special Type.

The glossary preserves its original 39 term anchors, provides missing owner-linked model distinctions and separates normative authority, classification, operational implementation and evidence. It owns its common vocabulary organization/usage within the declared scope, without replacing detailed domain definitions or declaring all consuming sources consistent.

---

# 3. Scope

Applicable vocabulary concerns Foundation, Architecture, component specifications, Governance, reference material, roadmaps and Templates. Terms identify their subjects/contexts; domain-specific interpretation follows responsible owners and the adopted working rules. Detailed component and external DMS/CMS specifications are not supplied by this reference.

Every README.md, CHANGELOG.md and ArchitecturalMilestones.md at every location is a non-normalized functional file. Such names require no normalized Document ID, Family, Type, Component, Version, Revision, Status or Baseline by normalization. Their content, structure, references, inventory and hash evidence remain reviewable; the exclusion creates no exceptions to the four Types for normalized documents.

DF defines documentary contracts; DMS, tools or applicable manual processes execute management/checking operations. CMS governs changes in its own scope. A definition, normative statement, Type Reference or resolving reference proves neither approval, publication, snapshot inclusion nor implemented conformance.

---

# 4. Terminology Principles

Common terms preserve responsible owner meanings in a declared scope. Summaries and qualified usage do not become competing semantic authorities; unresolved conflicts remain explicit.

## 4.1. Canonical

Each concept/record has an identified responsible owner and authoritative contract within its semantic domain/scope. The glossary references those meanings; it does not make every copied definition canonical merely by restating it. Derived representations retain source/edition provenance.

---

## 4.2. Unambiguous

State the subject, domain and qualified context of a term. Formal contextual aliases map to one meaning; shared words across domains require qualification. Ambiguity and competing definitions are assessed from actual usage rather than prohibited by an unqualified one-word/one-concept claim.

---

## 4.3. Consistent

Preserve applicable meaning across consuming sources and traceable projections. Record owner conflicts, stale usage and incomplete propagation. An edited glossary alone proves neither integrated consistency nor conformity of unseen sources.

---

## 4.4. Stable

Definitions evolve through controlled, justified owner/consumer changes. Preserve compatible meaning where feasible; necessary incompatibility requires explicit impact, edition transition and verification. Stability does not forbid every justified revision or guarantee harmless extension.

---

## 4.5. Technology Independent

Architectural definitions avoid prescribing technology unless an integration constraint explicitly requires it. Actual representations, formats, storage adapters and executors still need applicable contracts and evidence; conceptual independence does not prove universal interoperability.

---

# 5. Core Terminology

Each entry supplies a concise consultation meaning and identifies the responsible role/source. Section 9 resolves supplied references and their limits. An owner reference is not automatically a required runtime-service edge or completed peer review.

## 5.1. Architecture

The common arrangement of principles, concepts, capability boundaries, structural allocations and typed contracts in DF. Architecture includes definitions and constraints; it is not evidence that an operational system exists.

**Responsible role/source:** Common Architecture; Architectural Concepts, Layers and Components (§9).

---

## 5.2. Architectural Component

A contextual synonym for Component (§5.7): a capability boundary with a defined responsibility and owner contracts. This entry introduces no second component meaning or registration.

**Responsible role/source:** Common Architecture; Architectural Components (§9); controlled alias in §6.

---

## 5.3. Architectural Layer

A contextual synonym for structural Layer (§5.21). Structural areas, conceptual concerns and physical directories remain distinct; the term does not make every grouping a capability component.

**Responsible role/source:** Common Architecture; Architectural Layers (§9); controlled alias in §6.

---

## 5.4. Architectural Principle

An explicit design/evolution rule within its stated architectural scope. Its applicability and responsible source determine the requirement; a principle alone proves neither implementation nor conformity.

**Responsible role/source:** Common Architecture; Architectural Principles, with scheduled reconciliation, and applicable owner contracts (§9).

---

## 5.5. Baseline

A separately identified immutable, explicitly selected set of exact approved document editions with relevant pinned relationship context or traceable verification evidence. Snapshot identity, member logical identity, edition coordinates, approval eligibility, consistency and actual inclusion are separate facts. A time label or current path is insufficient to select members; a snapshot need not contain every current source or a complete live graph.

**Responsible role/source:** Governance/Baselines contracts summarized by Concepts §5.13 and Components §6.4 (§9).

---

## 5.6. Classification

The domain contract for meaningful documentary categories and assignments. Metadata represents values; Classification owns their semantic meaning. Family, document Type and optional Class are complementary distinctions under the adopted rules (§§5.43–5.45), independent of permanent document identity, current path, edition Status and primary component allocation.

**Responsible role/source:** Classification; Classification Concepts and the adopted Review Policy §3 (§9), pending full domain-source reconciliation.

---

## 5.7. Component

A capability building block with a defined primary responsibility and explicit owner/consumer boundaries. The supplied register contains 23 capabilities, allocated 4/4/5/5/5 across Documentation/Governance/Discovery/Automation/Integration. Registration is distinct from logical entities, files, concerns, implemented services and complete documentation. One primary allocation allows explicit cross-cutting participation without competing semantic ownership.

**Responsible role/source:** Common Architecture; Architectural Components and Layers (§9). Architectural Component (§5.2) is the controlled contextual synonym.

---

## 5.8. Concept

A defined abstraction with an identified subject/domain and responsible contract. Concepts may concern knowledge, entities, descriptors, states or capabilities; not every concept is a registered component or structural Layer. Shared words require explicit contextual qualification rather than an invented universal meaning.

**Responsible role/source:** Common Architecture; Architectural Concepts (§9), with domain-specific meanings retained by their owners.

---

## 5.9. Dependency

Required consumption: a consumer needs a provider contract in a declared scope. Direction is consumer→provider; record consumer, provider, contract, scope and responsible source editions. Documentary authority reference, semantic association, projection, navigation and execution are separately typed. Applicable structural/cycle rules remain with Layers/owners; genuine indispensable edges or cycles must remain visible and cannot be hidden by relabelling.

**Responsible role/source:** Common Architecture and applicable owner/consumer contracts; Concepts §8, Layers §§12–13 and Components §12 (§9).

---

## 5.10. Discovery

Capabilities for locating, navigating and consulting identified entities/editions through declared information sources/views. State, provenance and freshness limits remain explicit; discoverability grants no approval or complete coverage. Discovery as a structural area differs from a single operational service.

**Responsible role/source:** Discovery capability boundaries in Components §7 (§9); actual implementations require their own evidence.

---

## 5.11. Document

A logical documentary entity with a purpose and a coherent unit of represented knowledge. File and physical location are representations, not its logical key. Applicable normalized identity, Metadata, classification and edition-governance contracts apply only within normalization scope (§§3/5.56/5.57). An exact edition (§5.40) differs from the enduring logical document.

**Responsible role/source:** Document Identity for logical identity; Metadata/Classification/Governance for their respective meanings, as summarized by Concepts §5.3 (§9).

---

## 5.12. Document Identity

Permanent logical identity under the applicable Domain+Identifier allocation/preservation contract. Its identifier representation (§5.52) is not the entity itself. Filename, repository, title, classification, Version/Revision and Status do not automatically recalculate a valid identity. The adopted corpus representation DF-SSS-NNN uses a stable allocation series independent of current Family/Type; full DID source integration remains pending.

**Responsible role/source:** Document Identity; Document Identity Concepts, with working corpus syntax in Review Policy §4 (§9). No new allocation or migration is performed here.

---

## 5.13. Documentation

Organized representation of knowledge through documentary entities and applicable architectural/domain contracts. It includes normalized sources and functional files in their respective scopes, not only a directory tree. DF defines those contracts; actual producing/managing processes are separately identified.

**Responsible role/source:** Common Architecture; Architectural Concepts and Framework Manifest (§9).

---

## 5.14. Documentation Framework

The architectural framework of documentary definitions, representation/organization rules and applicable governance/discovery/evolution contracts. DF defines what those contracts require; DMS, tools or manual processes execute document-management operations, while CMS governs changes in its own scope. This term proves no users, permissions, storage engine or deployed workflow.

**Responsible role/source:** Common Architecture and Foundation; Framework Manifest, Blueprint and Concepts (§9).

---

## 5.15. Framework

In this glossary’s declared DF context, a controlled short form of Documentation Framework (§5.14). It does not mean that every framework in another domain has the same contracts or that DF is an implemented management system.

**Responsible role/source:** Common Architecture; context mapping in §6, not a second definition owner.

---

## 5.16. Governance

Applicable contracts for responsibilities, controlled evolution, decisions and required evidence. Workflow, Policies, Reviews and Baselines define distinct capability roles; an applicable DMS/tool/manual process executes operations, and CMS supplies change evidence within its own scope. Domain governance, document-edition Status, validation, approval, publication and Baseline membership remain separate.

**Responsible role/source:** Responsible domain Governance contracts and common Architecture summaries in Components §6 (§9).

---

## 5.17. Identity

The persistent characteristic/key by which an entity is recognized within its declared identity domain, independent of mutable properties. Identity is represented through an identifier but is not synonymous with the string representation. Document Identity (§5.12) is a qualified identity domain role; other endpoints use their own appropriate contracts and do not automatically receive normalized document IDs.

**Responsible role/source:** Relevant entity-domain owner; Document Identity Concepts §§3.3–3.5 for documentary identity (§9).

---

## 5.18. Integration

Optional, use-case-specific adapters to supported external environments/interfaces. They consume applicable owner and authorization contracts; descriptions establish neither installed tools nor successful execution. Publication requires Governance authorization for the exact edition, and an adapter gains no new semantic or approval authority.

**Responsible role/source:** Integration capability definitions in Components §9 (§9); actual executor/implementation evidence remains separate.

---

## 5.19. Knowledge

Subject matter represented, organized, preserved and communicated by documentation; it can exist independently of documentary representations. Knowledge is a conceptual concern, not a new registered DF component or structural area. DF defines representation contracts rather than becoming the operational manager of every knowledge asset.

**Responsible role/source:** Knowledge-producing domain for subject meaning; common Architecture representation role in Concepts §5.1 (§9).

---

## 5.20. Knowledge Graph

A semantic-network projection of identified entities and typed Relationships records, with authoritative source/edition provenance. Views distinguish current, stale, historical and snapshot context and refresh rules. Derived values gain no competing semantic authority; a graph capability proves neither a complete network nor global required-dependency acyclicity.

**Responsible role/source:** Discovery/Knowledge Graph projection role; Relationships and endpoint domains retain record/identity meanings, as summarized by Components §7.3 (§9).

---

## 5.21. Layer

In the structural context, a grouping/allocation boundary governed by Architectural Layers. Seven structural areas are Foundation, Architecture, Documentation, Governance, Discovery, Automation and Integration; Foundation/Architecture supply support definitions. Five conceptual concerns—Knowledge, Documentation, Governance, Discovery and Preservation—are a different view. Knowledge is subject matter and Preservation is cross-cutting; neither implies another registered component or structural Layer. Required boundaries follow explicit contracts, not visual order or directory nesting.

**Responsible role/source:** Common Architecture; Architectural Layers (§9). Architectural Layer (§5.3) is a controlled contextual synonym; other uses require qualification.

---

## 5.22. Lifecycle

The subject-specific states, transitions and evolution contracts of an identified entity or definition. Document editions, Metadata Elements, Classification definitions and Template entities can have distinct lifecycles with their own owners. A state list does not establish a universal Workflow graph, operational permission model or implementation maturity.

**Responsible role/source:** Relevant entity/domain lifecycle owner; Classification Lifecycle and common Workflow summaries provide explicit distinctions (§9).

---

## 5.23. Metadata

Definitions and represented descriptor values for documentary entities/editions. Dictionary defines descriptors, Schema organizes references/structural constraints, Profile restricts usage and Instance supplies values under one effective Profile (§§5.46–5.51). Identity, Classification and Governance retain their meanings even when Metadata represents their values. Conceptual separation from content guarantees neither independent editions nor content-free verification; coordinated changes can be necessary.

**Responsible role/source:** Metadata, referencing responsible domain semantic owners; Metadata Model/Dictionary and Concepts §5.4 (§9). Received owner discrepancies remain pending.

---

## 5.24. Navigation

Logical access through declared entity/edition and relationship views, with identified targets, relevant provenance, state and freshness. Navigation associations neither approve targets nor automatically declare required provider services or storage contracts.

**Responsible role/source:** Discovery/Navigation capability role in Components §7.4 (§9), consuming identified sources rather than replacing their owners.

---

## 5.25. Policy

An explicit applicable rule within a declared governance scope, with a responsible source and required evidence. Naming a policy establishes no automatic compliance or permission; execution and decisions are separately evidenced.

**Responsible role/source:** Applicable Governance/domain policy owner; working review conventions in Review Policy (§9).

---

## 5.26. Registry

Authoritative catalog/lookup capability within its declared catalog scope, referencing logical entities, exact editions and traceable records/projections. Catalog authority does not replace Identity, Classification, Governance or Relationships semantics. Derived copies retain provenance and current/stale/historical/snapshot context; no indispensable Registry intermediary or physical single-copy storage is inferred for every consumer.

**Responsible role/source:** Discovery/Registry catalog role in Components §7.1 (§9); source-domain owners retain meaning.

---

## 5.27. Relationship

An explicitly typed connection record between identified endpoints with appropriate entity-domain identity and provenance. Kinds can include semantic reference, association, replacement, navigation and required dependency. Endpoint/cardinality rules belong to applicable owners; not every endpoint is a normalized document. Record presence, not a word or arrow alone, supports traceability; no complete relation catalog or cycle-free graph is implied.

**Responsible role/source:** Relationships owns typed records; endpoint domains own their identities/meaning, as summarized by Concepts §5.7 and Components §7.2 (§9).

---

## 5.28. Repository

A physical storage organization for documentary representations/artifacts. It is an implementation concern distinct from logical identity, classification and primary semantic authority. Actual formats, locations, adapters and access contracts still need implementation evidence; conceptual independence does not eliminate physical constraints or prove automatic interoperability.

**Responsible role/source:** Applicable DMS/storage implementation contract; DF supplies documentary representation rules rather than a complete repository specification (§§3/5.58).

---

## 5.29. Review

An evaluation that records identified requirements, exact examined sources/editions, findings, coverage, evidence and limits. It may use Validation/Consistency Verification results without taking over domain rule ownership. Review, successful checking, approval, publication and snapshot inclusion are distinct events.

**Responsible role/source:** Reviews capability and applicable process contracts; Review Policy §§6–7 and Components §6.3 (§9).

---

## 5.30. Roadmap

A plan for progressive documentary/architectural and, where applicable, implementation evolution of DF or a component. Central Roadmaps/ storage is a planning organization, not a structural Layer or an automatic component/Family assignment. Component plans use canonical component Family and Type Behavior under the adopted rules; global admitted plans use Family Roadmap. A plan proves no implemented maturity or completed work.

**Responsible role/source:** Applicable planning source and domain owners; Framework Roadmap and Review Policy §3.2 (§9).

---

## 5.31. Semantic

Pertaining to meaning/interpretation within a defined subject/domain, as distinct from physical representation. The same word in different domains requires qualification; represented values and projections preserve owner meaning rather than introducing competing definitions.

**Responsible role/source:** Responsible subject/domain owner; common vocabulary role summarized here without replacing that owner.

---

## 5.32. Single Source of Truth

One identified authoritative definition or record owner for a stated semantic domain/scope. Summaries, catalogs and projections may repeat derived values with source/edition provenance and refresh limits; logical authority does not mandate one physical copy or universal routing. Unresolved conflicting definitions remain recorded and reconciled with responsible owners rather than hidden by a glossary claim.

**Responsible role/source:** Applicable semantic/record domain owner; common Architecture ownership principles in Concepts/Components (§9).

---

## 5.33. Specification

A consolidated source of identified applicable requirements, domain responsibilities, constraints, references and conformance obligations. It states normative/informative scope explicitly; supporting sources can also carry normative requirements. A title, Type Reference or directory grants no approval, publication or implemented conformance. A specification does not substitute for another domain’s semantics merely by referencing them.

**Responsible role/source:** Relevant domain specification owner; Component Documentation Structure §10 and actual supplied specifications (§9).

---

## 5.34. Template

A reusable structural definition for organizing/representing documentation under applicable constraints. It is distinct from its applied Template Instance (§5.55) and does not guarantee consistency merely by existing. Templates may define structural locations/compatibility requirements, but do not redefine Metadata, Identity, Classification, Workflow, Registry or storage semantics. Template Type (§5.54) is distinct from document Type (§5.44).

**Responsible role/source:** Templates; Template Concepts and Template Specification (§9).

---

## 5.35. Terminology

The common consultation/convergence vocabulary for architectural terms, with identified subjects, contexts, controlled aliases and responsible source meanings. This glossary owns its organization and common vocabulary usage within the declared scope; it does not become a competing owner of every component definition or certify semantic consistency throughout all sources.

**Responsible role/source:** Common Architecture vocabulary role; domain semantic owners remain those identified in individual entries and §9.

---

## 5.36. Traceability

The evidenced ability to follow identified entities, source editions, typed relationships, decisions and changes over time. It requires actual records, resolvable targets and preserved provenance; a glossary, relationship concept or directory alone does not establish complete traceability.

**Responsible role/source:** Applicable record/domain/process owners; Relationships/Reviews and owner-source evidence supply the examined scope (§9).

---

## 5.37. Validation

Scoped assessment of identified requirements against exact artifacts/editions and relevant context, with rules, checks, observations, coverage, executor and limits. Rules belong to responsible owners; an implementation/process executes/evidences checks. A local PASS neither proves unexamined conformity nor approves, publishes, selects a Baseline or transfers to later changed bytes.

**Responsible role/source:** Relevant domain validation contract and Automation/Validation capability; Concepts §5.15, Components §8.1 and Review Policy §6 (§9).

---

## 5.38. Version

A document-edition coordinate describing compatible/incompatible contract evolution under an identified numbering policy, not the entire edition, logical identity, Status or Baseline. In this working review, major.minor is used: compatible correction retains Version, compatible additive capability increments minor, and incompatible contract change increments major/reset minor 0. Document Revision (§5.41) increments monotonically for changed persisted editions, including across Version changes. Other entity version policies require their own qualified owners.

**Responsible role/source:** Documentary numbering/governance contract in Review Policy §5 (§9), pending applicable domain-source integration.

---

## 5.39. Workflow

Documentary governance contracts for exact-edition states, permitted transitions, responsibilities and required evidence. DMS/tool/manual processes execute operations; Workflow definition is not an installed lifecycle engine or unconditional permission graph. Version/Revision, Status, maturity, review, validation, approval, publication and membership remain distinct, and Draft successors inherit neither approval nor earlier snapshot membership.

**Responsible role/source:** Governance/Workflow and Policies roles in Components §6 and Concepts §5.11 (§9).

---

## 5.40. Document Edition

An exact recorded state of a logical document, including represented content/descriptors and relevant context. Logical identity persists across editions; coordinates, Status and actual snapshot membership remain separate facts.

**Responsible role/source:** Document Identity for logical entity; documentary governance/Metadata for edition facts; Concepts §5.3 and Review Policy §5 (§9).

---

## 5.41. Revision

Within the document-edition policy, a monotonic coordinate for each changed persisted edition. Declared Revision 0 increments to 1 for the current successor; no absent historical Revision 0 is invented elsewhere. Validation of unchanged bytes increments neither Revision nor Version; further edits need their own assessed successor.

**Responsible role/source:** Documentary numbering contract in Review Policy §5 (§9); other entity revisions require qualification.

---

## 5.42. Status

Governance state of the exact identified document edition, not general product maturity, approval of every successor or automatic Baseline inclusion. An older Approved edition can coexist with a current Draft successor.

**Responsible role/source:** Applicable documentary governance/Workflow contracts; Review Policy §5 and Concepts §5.3 (§9).

---

## 5.43. Family

For a normalized component document, the canonical component name; for admitted non-component areas, the explicitly scoped documentary area such as Foundation, Architecture or global Roadmap. Central path, topic, title or stable ID series alone does not determine Family.

**Responsible role/source:** Classification; adopted working rule in Review Policy §3.2 (§9), pending complete domain integration.

---

## 5.44. Document Type

Primary responsibility of a normalized document: exactly Architecture, Structure, Behavior or Reference in this working review. Historical consultation is Reference; a process or planned evolution is Behavior. No Base/Core/Foundation exception or Schema/Dictionary/Lifecycle fifth Type is introduced. This is distinct from Template Type and Metadata value type.

**Responsible role/source:** Classification; adopted four-value contract in Review Policy §3.1 (§9).

---

## 5.45. Class

An optional additional semantic dimension of a document, requiring an explicit non-conflicting definition. It is separate from Family/document Type, component allocation, Status and implementation maturity. Optional does not mean mandatory, unrestricted or inferred from a filename.

**Responsible role/source:** Classification; Classification Concepts §14 and adopted Review Policy §3.3 (§9).

---

## 5.46. Metadata Element

A defined descriptor/property with identified semantics, characteristics and applicable constraints. Canonical definitions belong to the Metadata Dictionary, referencing other semantic domain owners where appropriate; element identity/lifecycle is distinct from document identity/edition. This glossary allocates no Element ID or catalog record.

**Responsible role/source:** Metadata; Metadata Model §7.2 and Dictionary (§9), with received Schema/Dictionary disagreements still pending reconciliation.

---

## 5.47. Metadata Value

A represented value assigned to an applicable Metadata Element for an identified documentary context/edition. Abstract value type is not document Type. Applicable owner/Profile constraints govern values; absence is not permission to invent identity, classification, lifecycle or approval facts.

**Responsible role/source:** Metadata representation contracts and corresponding domain meaning owners (§§5.23/5.50).

---

## 5.48. Metadata Dictionary

The authoritative domain-definition/entry catalog for Metadata Elements, including semantics and references to responsible subject owners. A terminology consultation role differs from element-catalog composition; title alone forces neither document Type nor path. This synopsis does not certify that every required entry exists.

**Responsible role/source:** Metadata; Metadata Dictionary §§1–3/6–7 (§9).

---

## 5.49. Metadata Schema

Organization/references and structural constraints over applicable Metadata definitions. Schema does not independently redefine Dictionary/domain semantics. The received Model’s Schema-defines-Elements/complete-vocabulary wording remains pending owner reconciliation rather than a second governing meaning for this synopsis.

**Responsible role/source:** Metadata structural contract; Model/Dictionary comparison and adopted owner distinctions in Concepts §5.4 (§9).

---

## 5.50. Metadata Profile

Contextual restriction/specialization of applicable Schema usage, values and cardinality without semantic redefinition. Effective requirements depend on the declared owner contract; this glossary creates no missing canonical Profile or lifecycle event.

**Responsible role/source:** Metadata; Metadata Model §7.5 and adopted Concepts §5.4 (§9), pending full Profile reconciliation.

---

## 5.51. Metadata Instance

Represented Metadata values for one identified documentary edition under exactly one effective Profile. Representation/content may require coordinated evolution; this definition guarantees no automatic completeness, synchronization or independent revisions.

**Responsible role/source:** Metadata; Metadata Model §7.6 and adopted Concepts §5.4 (§9).

---

## 5.52. Identifier

Canonical representation used to reference an identity within its declared domain. A document’s DF-SSS-NNN representation uses stable allocation namespaces and a positive allocated number; its string is not the logical entity or current classification. Detailed syntax/allocation remains with the qualified identity contract.

**Responsible role/source:** Relevant identity-domain owner; Document Identity Concepts §3.4 and working Review Policy §4 (§9).

---

## 5.53. Identity Domain

Scope in which the applicable identity contract establishes uniqueness and allocation/preservation rules. Documentation Framework is the adopted documentary domain; other architectural entity kinds can use different qualified domain contracts. Domain+Identifier and exact-edition references are distinct.

**Responsible role/source:** Relevant entity-domain owner; Document Identity Concepts §3.5 and Review Policy §4 (§9).

---

## 5.54. Template Type

Conceptual category of a Template by the kind of reusable structure/purpose it defines. This does not add a value to the four normalized-document Types or transfer document Classification authority to Templates.

**Responsible role/source:** Templates; Template Concepts §3 (§9).

---

## 5.55. Template Instance

Traceable application of an identified Template definition/version to a specific documentary context. It remains distinct from the reusable definition; changing a Template does not silently replace the definition used by an existing instance.

**Responsible role/source:** Templates; Template Concepts §8 (§9).

---

## 5.56. Functional File

Within this corpus, every README.md, CHANGELOG.md or ArchitecturalMilestones.md at any location. Such files are not normalized and require no normalized identity/header/classification by that exclusion; legitimate existing information is not automatically deleted. Content, organization, references, inventory and hashes remain reviewable.

**Responsible role/source:** User-adopted scope and Review Policy §2 (§9); central logs retain their own record conventions.

---

## 5.57. Normalized Document

A documentary source within the applicable normalization scope, with the adopted identity, classification and edition/Metadata contracts. Functional names in §5.56 are excluded before applying those obligations; missing canonical Element/Profile records are not manufactured by declaring a source normalized.

**Responsible role/source:** Applicable document/Metadata/Identity/Classification contracts and Review Policy §§2–5 (§9).

---

## 5.58. Documentation Management System (DMS)

An executing management-system role that consumes DF definitions for repositories, storage, operations, permissions, publication and related management concerns. The definition is contextual and does not supply a complete external DMS specification or register DMS as another DF capability component. Tools/manual processes can execute applicable operations where supported.

**Responsible role/source:** Relevant external management-system/process contract; common boundary in Concepts §3, Components §3 and Review Policy §1 (§9).

---

## 5.59. Change Management System (CMS)

A system/process role governing changes in its own scope and providing relevant decision/provenance evidence. CMS records do not substitute for exact documentary approval, publication or Baseline selection and do not redefine DF document semantics. This is a contextual boundary, not a supplied complete external specification or new DF component.

**Responsible role/source:** Relevant external change-management contract; common boundary in Concepts/Components and Review Policy (§9).

---

# 6. Naming Conventions

Use canonical natural-language component names in prose, including their spaces and spelling (Document Identity, Knowledge Graph, Metadata Generator). Directory aliases, identifier syntax and programming PascalCase are separate representation conventions; this glossary mandates no concatenated prose names or filename/ID migration.

Use singular entity terms where appropriate without renaming plural capability owners: Baseline is an entity term, Baselines is the registered capability name. Define abbreviations before use. Preserve context-qualified terms, documented controlled alias mappings and legitimate historical vocabulary rather than rewriting past meaning.

| Contextual expression | Canonical target/meaning | Scope/limit |
|---|---|---|
| Architectural Component | Component (§5.7) | Same capability concept in common DF Architecture; original §5.2 anchor retained |
| Architectural Layer | Structural Layer (§5.21) | Same structural grouping; conceptual concerns remain a distinct view; original §5.3 retained |
| Framework | Documentation Framework (§5.14) | Short form only in declared DF context; original §5.15 retained |
| DocumentIdentity | Document Identity | Received directory alias, not a competing component name or recalculated ID |
| DMS / CMS | Qualified system-role terms in §§5.58/5.59 | External/contextual roles, not new registered DF components or complete specifications |

Aliases have explicit targets and contexts; historic or external spelling requires a map/qualification when relevant. New terms and changed meanings follow §§8/10 and their domain owners. No taxonomy, catalog record or identity allocation is performed by naming a term.

---

# 7. Forbidden Terminology

Avoid undefined abbreviations, unqualified domain overloads, competing definitions, unsupported semantic authority and technology-specific implementation labels presented as universal architectural concepts. Do not use a directory, classification label, projection or terminology entry to conceal actual required dependencies or an unresolved owner conflict.

Controlled aliases, canonical plural component names, qualified contexts and documented historical vocabulary are permitted under §6; they do not license arbitrary interchangeable meanings. Distinguish Template Type, Metadata value type and document Type explicitly. A semantic owner cannot be reassigned merely to make a dependency graph look acyclic.

---

# 8. Terminology Governance

New or changed terms identify the responsible domain/source, subject/context, previous/new meaning, rationale, affected consuming editions and applicable evidence. Working review rules derive from the user-adopted policy; received incompatible wording remains preserved as input/history rather than a second governing rule for the same operation.

Assess actual consumer propagation, compatibility and required contracts. Deprecated/historical meanings retain their mappings and source editions; formal removal or replacement does not erase prior records. Canonical authority follows responsible applicable contracts, not an informal glossary claim or approval inferred from Type Reference.

Actual contribution, user authorization, review, validation, ownership and approval are separate facts. Later human/tool edits require resulting-edition/byte assessment; a previous local PASS does not transfer automatically or assign responsibility for consequences of a changed final product.

---

# 9. Relationship with Other Architecture Documents

Supplied source roles and current comparison limits are recorded below. Resolving an ID/path does not approve a source, complete its review cycle or establish a complete implementation. This glossary summarizes meanings and adopted boundaries without replacing domain semantic owners.

| Supplied source | Responsible role and comparison limit |
|---|---|
| [DF-ARC-001 — Architecture Overview](DF-ARC-001-ArchitectureOverview.md) | Overall context; remaining received count/direction reconciliation pending |
| [DF-ARC-002 — Architectural Principles](DF-ARC-002-ArchitecturalPrinciples.md) | Design principles; scheduled independent-evolution/extension reconciliation |
| [DF-ARC-003 — Architectural Concepts](DF-ARC-003-ArchitecturalConcepts.md) | Common conceptual distinctions and owner summaries; earlier exact-source validation retains scope |
| [DF-ARC-004 — Architectural Layers](DF-ARC-004-ArchitecturalLayers.md) | Structural areas, primary allocation and scoped required-dependency constraints |
| [DF-ARC-005 — Architectural Components](DF-ARC-005-ArchitecturalComponents.md) | 23 capability register, owner/executor and interaction boundaries |
| [DF-ARC-007 — Component Documentation Structure](DF-ARC-007-ComponentDocumentationStructure.md) | Responsibility-based organization, functional exclusion, explicit authority and partial-set evidence |
| [DF-FND-001 — Framework Manifest](../00-Foundation/DF-FND-001-FrameworkManifest.md) | Framework identity and documentary scope/classification distinctions |
| [DF-FND-004 — Architectural Blueprint](../00-Foundation/DF-FND-004-ArchitecturalBlueprint.md) | Common architectural ownership, edition and required-contract basis |
| [DF-MTD-003 — Metadata Model](../02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md) | Descriptor abstractions/one effective Profile; received Schema-defines-Elements/vocabulary wording remains pending reconciliation |
| [DF-MTD-013 — Metadata Dictionary](../02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md) | Metadata Element definition/entry-catalog owner; complete catalog/Profile reconciliation pending |
| [DF-DID-002 — Document Identity Concepts](../02-Documentation/DocumentIdentity/01-Architecture/DF-DID-002%20-%20Document%20Identity%20Concepts.md) | Identity/domain/identifier distinction; full syntax/applicability integration pending |
| [DF-CLS-002 — Classification Concepts](../02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md) | Classification/identity/representation distinctions; historical Family→Type hierarchy needs adopted-rule convergence |
| [DF-CLS-006 — Classification Lifecycle](../02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md) | Subject-specific definition lifecycle, distinct from document-edition governance |
| [DF-TPL-002 — Template Concepts](../02-Documentation/Templates/01-Architecture/DF-TPL-002-TemplatesConcepts.md) | Reusable definition/instance and Template Type distinction |
| [DF-TPL-014 — Template Specification](../02-Documentation/Templates/04-Reference/DF-TPL-014-TemplatesSpecification.md) | Templates domain contracts and explicit exclusions; source presence grants no implementation evidence |
| [DF-RDM-001 — Documentation Framework Roadmap](../Roadmaps/DF-RDM-001-DocumentationFrameworkRoadmap.md) | Central planning area separate from structural Layers; received header convergence pending |
| [DF-RVW-001 — Review Policy](../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md) | Adopted working classification, identity, numbering, scope and review/evidence contracts |
| [DF-RVW-002 — Review Report](../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md) | Actual correction/validation states and exact input/output/comparison evidence; no domain-semantic takeover |

Listed comparisons are partial and do not complete detailed owner cycles. The glossary does not resolve the nominal CLS-003/CLS-001 collision, missing canonical Metadata records, all consumer maps or a complete required graph. Earlier owner remarks about received Terminology remain exact-edition historical evidence, not validation or propagation of this successor.

---

# 10. Evolution Guidelines

Introduce a term only for a justified distinction not adequately represented by an existing qualified term or controlled alias. Record owner/subject/context, previous/new meaning, affected source editions, references and transition evidence before propagation. Avoid duplicate semantic authorities and title-derived classification.

Preserve compatible meaning where feasible. Necessary incompatible changes require explicit justification, consumer compatibility/required-contract assessment, versioned transition and verification. A new term or supplemental definition is not presumed harmless to every consumer.

For document editions in this working review, compatible correction retains Version, compatible additive capability increments minor, and incompatible contract change increments major/reset minor 0. Each changed persisted edition increments Revision monotonically across Version changes; unchanged-source validation increments neither coordinate and is tracked centrally. Domain-specific entity lifecycle/version rules remain separately qualified.

Local glossary correction does not certify complete terminology rollout, global acyclicity, owner catalog completeness or operational outcomes. Actual integrated checks remain separate work.

---

# 11. Conclusion

Terminology provides concise owner-linked consultation meanings, qualified contexts and traceable aliases. It supports assessed communication and convergence without claiming to eliminate all ambiguity, replace detailed domain semantics or certify every document’s consistency.

This edition applies eight findings and two warnings as **Corrected—pending validation**. Exact-source validation, owner-source integration and consuming/global reconciliation remain pending. Architecture/Reference V2.0 R1 is Draft, with Baseline Not assigned; source presence or construction checks confer no approval, publication or snapshot selection.

## 11.1. Compatibility assessment

Received §§1/2/5.35/9 claim glossary-wide semantic authority; §5.11 universally requires normalized identity/Metadata; §§5.5/5.22/5.38/5.39 conflate snapshot, subject lifecycle and edition facts; §§6/7 prohibit synonyms while existing paired entries and canonical prose names require contextual mappings. Operational and relationship definitions also lack domain/executor/evidence boundaries.

V2.0 introduces owner-linked scope/authority, normalized/functional applicability, exact-edition/required-contract distinctions and controlled alias/representation rules. Earlier universal interpretations are no longer permitted. This is an **incompatible normative contract reconciliation**, not merely Type reclassification or additional consultation links. Version 1.0 increments major to 2.0; declared Revision 0 increments to 1 without reset. DF-ARC-006/path remain stable; no ID/file migration, new component or Metadata Element allocation is performed.

## 11.2. Local edition history

| Date | Version | Revision | Contribution/event | State/evidence |
|---|---|---|---|---|
| Not supplied | 1.0 | 0 | Received Terminology source; Author absent | Architecture/Terminology; Draft/Baseline1.0 declarations preserved; no historic approval/selection inferred |
| 2026-10-14 | 2.0 | 1 | Codex — AI assistant: owner-linked scope/definitions,39 preserved terms,20 supplemental distinctions, controlled aliases,18 source links and compatibility/history | Architecture/Reference; Draft; Baseline Not assigned; ten corrections pending VALIDATE DOCUMENT; CHANGELOG #311; Review Report §40 |

Input SHA-256: `c99cc06206cbd1382529c295ea72e0177325202fc039d2bc48b2181cc41d90eb`. Original source bytes, all 55 numbered sections and 39 term labels remain in input/map/diff evidence. Actual contribution differs from authorization, review, validation, ownership and approval; mixed contributions retain their attribution. Later changed bytes need their own assessment without inherited result or final-product consequence responsibility. No original author, date or absent historic event is invented.

## 11.3. Propagation and verification limits

This UPDATE modifies Terminology and central report/tracking/evidence only. Ten earlier exact-source validations retain their scopes; owner summaries and past notes do not validate this successor or complete its consumer rollout. Detailed Metadata, Identity, Classification, Templates and planning sources retain their scheduled cycles.

Metadata Model’s Schema-defines-Elements/vocabulary wording, Dictionary/Profile completeness, received Classification Family→Type interpretation, identity syntax/applicability and nominal CLS collision remain pending owner reconciliation. The glossary adds no canonical catalog/Profile/lifecycle record or external DMS/CMS specification. Registry/Graph projections and record meanings remain scoped; no universal intermediary or complete globally acyclic graph is certified.

M11 remains In Progress: Concepts/Layers/Components/ARC-007 C, Terminology S, two peers O; no Terminology completion date. All 19 global records remain Open and 97 earlier localized closures retain their scopes. No implementation maturity, integrated conformity, approval, publication, Baseline or final Context-Reviewed.zip is claimed.

---

**End of Document**

---
