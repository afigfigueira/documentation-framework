# Documentation Framework

# DF-DID-001 — Document Identity Architecture

| Metadata | Value |
|---|---|
| **Document ID** | DF-DID-001 |
| **Title** | Document Identity Architecture |
| **Family** | Document Identity |
| **Type** | Architecture |
| **Component** | Document Identity |
| **Author** | Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

Received V1.0 R0 declares Family Documentation, Component Document Identity, Type Architecture, Author Arnaldo Figueira, Status Canonical and Baseline1.0. Those facts remain history in §12.2; no approval, publication or snapshot-selection event is inferred. This successor records actual assistant contribution and ten corrections pending VALIDATE DOCUMENT, independently of authorization or approval.

---

# 1. Purpose

This source defines the architectural responsibility, boundaries, allocation and applicable contract interpretation of the **Document Identity** component. It owns logical document identity semantics and their allocation, preservation, reference, validation and identity-governance requirements within a declared domain.

Logical identity identifies a document under its Domain+Identifier contract; exact editions, mutable classification, physical representations and identity-record state are distinct. This source defines contracts rather than an implemented assigning or managing service. DMS, tools or an applicable manual process execute operations; CMS governs changes in its own scope. Architectural requirements and source presence do not establish deployed uniqueness, resolution, storage, approval or implementation conformance.

Every file named **README.md**, **CHANGELOG.md** or **ArchitecturalMilestones.md**, at every location, is a non-normalized functional file. Normalization requires no Document ID, Family, Type, Component, Version, Revision, Status or Baseline for these names. Applicable content, organization, references, history, inventory and hash checks remain. Legitimate existing information is not automatically removed; no document/Metadata Element IDs are assigned by this scope statement.

---

# 2. Architectural Context

Document Identity has one primary allocation in the **Documentation structural area**, alongside Metadata, Classification and Templates. Family identifies actual component membership, so this document uses Family=Document Identity and matching Component; Type=Architecture follows its primary architectural responsibility. Documentation is an area, not this source's component Family.

<!-- original-section-view: 2 -->
**Previously unnamed view in §2 — Documentation primary capability allocation.**

| Capability | Primary structural area | Role |
|---|---|---|
| Metadata | Documentation | Descriptive definitions/represented values under their domain owners |
| Document Identity | Documentation | Qualified logical document identity and preservation contracts |
| Classification | Documentation | Mutable semantic categories and classification contracts |
| Templates | Documentation | Reusable representation structures and constraints |
<!-- end-original-section-view -->

This allocation view preserves the four received names and carries no required-dependency direction or execution sequence. Primary ownership permits explicit cooperation and cross-cutting support without competing identity semantics. Seven structural areas and five conceptual concerns remain distinct under ARC-004/005; this component introduces neither another Layer nor a new capability.

---

# 3. Architectural Responsibility

The component defines:

- logical document identity, its domain qualification and canonical representation contracts;
- allocation scope, uniqueness, permanence, preservation and non-reuse requirements;
- valid identity association with the same logical document across normal evolution;
- reference/alias interpretation and exact-edition reference boundaries;
- identity-specific validation, lifecycle/governance and evolution obligations;
- applicable consumer/provider interfaces and evidence requirements.

**The component does not assign identifiers.** It defines assignment/allocation contracts; DMS/tool/manual executors perform actual allocation, persistence, lookup and transition actions with identified rules, inputs, observations and responsibility evidence. README and DID-014's assigning wording remains a pending peer discrepancy in §12.3, not proof of an implemented DF service.

Under the adopted corpus convention, the identity domain is Documentation Framework, represented by DF. A normalized document ID uses **DF-SSS-NNN**, with a registered three-letter uppercase stable allocation series SSS and positive three-digit number NNN (001–999). Full identifiers are unique within the domain; equal numeric suffixes across different series are not collisions. Current Family, Type, Component, path, Version, Revision and Status do not reconstruct or recalculate an assigned valid ID. 000 is not allocated; gaps do not prove availability and allocated/retired numbers are not reused. New allocation or series continuation requires explicit records and collision/history checks under Review Policy §4; reaching 999 does not permit silent widening or recycling.

These are qualified corpus requirements, not syntax imposed on every external domain. Other entity/domain contracts need their own explicit registration and responsibility decisions. This UPDATE allocates no identity or series and performs no ID/path migration. Detailed integration into DID schema/constraints/specification owners remains scheduled.

---

# 4. Scope

The component's scope includes identity concepts, models, elements/schema, constraints, identity lifecycle, validation, governance, typed relationships, assessed extensibility, specifications and examples. Detailed sources retain their responsibilities; this architecture does not invent a canonical merged field catalog or certify all peer requirements.

For applicable normalized documents, logical identity remains associated with the same document across ordinary content/descriptor, classification, representation, repository and document-edition changes. Exact edition coordinates, document Status, identity-record assignment/preservation/retirement evidence, maturity and Baseline membership are separate facts. A mutable state record is not a replacement for the stable identity key.

Unassigned concerns a pre-allocation subject, not an already assigned Domain+Identifier key. Retirement preserves allocated-number reservation, document association/history and reference interpretation; it does not guarantee a running resolver or retrievable content. Document lifecycle and identity-record lifecycle can have distinct subjects/contracts. The source does not prescribe a universal transition or permission graph.

DID-003/004/005/006/010/014 currently disagree on reference cardinality, mandatory State/Canonical Reference fields and identity state terminology. Those actual claims are preserved in §12.3 for full owner cycles. The architectural distinctions here neither merge incompatible schemas nor silently remove/add their mandatory fields. No Metadata Dictionary Element, Profile or canonical state record is fabricated.

---

# 5. Out of Scope

The following roles are separate from document identity semantic ownership. Area labels, registered capability contracts and operational executors are identified separately; naming an owner proves no implemented service.

| Received responsibility | Responsible contract/role | Operational or semantic boundary |
|---|---|---|
| Document metadata | Metadata plus applicable semantic domain owners | Dictionary defines, Schema organizes, Profile constrains and Instance supplies values under one effective Profile; descriptive representation does not replace identity |
| Document classification | Classification | Family/Type and other category meanings remain mutable and separately owned |
| Registry management | Registry | Catalog/lookup contracts and provenance; actual registration/lookup executed by an applicable system/process |
| Discovery services | Discovery area: Registry, Relationships, Knowledge Graph, Navigation, Search | Area groups capabilities; it is not another component or mandatory routing intermediary |
| Workflow management | Workflow and applicable Policies | Subject-specific transitions/rules; DMS/tool/manual operation, not an implemented DF workflow engine |
| Version control | Documentary edition contracts versus source-control systems/adapters | Version/Revision/Status semantics follow applicable governance/edition contracts; repository commits and Source Control Integration adapters do not define them |
| Repository management | DMS or other applicable external system | Organization, storage, permissions and physical-location execution |
| Storage technologies | Applicable implementations/external systems | Persistence mechanisms preserve applicable representation/provenance requirements |
| Identifier generation algorithms | Applicable allocation executor | Generate/allocate under identity-domain rules and collision/reservation evidence; no algorithm supplied here |
| Persistence mechanisms | Applicable implementation/external system | Store identity/edition/context records without acquiring identity semantics |

Governance is an area grouping Workflow, Policies, Reviews and Baselines; it is not a single invented component owning all operational management. Reviews records examined scope/results; Baselines defines immutable selected exact approved editions and context. CMS change evidence does not substitute for documentary approval or snapshot inclusion.

---

# 6. Architectural Principles

Applicable common principles remain owned by ARC-002. The eight received labels below are retained with their actual owner/application role rather than fabricated AP IDs or an unqualified conformance declaration.

| Received label | Actual owner/application | Scope/limit |
|---|---|---|
| Single Responsibility | AP-006 — Separation of Responsibilities | Primary identity semantic owner permits explicit cooperation |
| Separation of Concerns | AP-006 — Separation of Responsibilities | Identity, description, classification and execution retain distinct responsibilities |
| Technology Independence | AP-003 — Technology Independence | Conceptual definition independence with actual representation requirements |
| Repository Independence | AP-003 — Technology Independence | Location/adapter changes preserve applicable identity; not guaranteed resolver availability |
| Format Independence | AP-003 — Technology Independence | Representations preserve canonical semantics under explicit constraints |
| Implementation Independence | AP-003 — Technology Independence | Contract owner differs from executor; no universal interoperability guarantee |
| Stability of Identity | AP-010 — Stable Identity | Qualified normalized logical identity and assessed necessary migration boundaries |
| Canonical Representation | DID-003 §9.5 / DID-005 §7.3 / DID-010 §5.1 | Domain representation requirements; not a newly registered framework AP |

Consult actual AP clauses/evidence boundaries and domain contracts. This selected mapping is neither the full 24-principle catalog nor an implemented conformance matrix. Canonical Representation remains an identity-specific contract role with peer schema integration pending.

---

# 7. Core Architectural Characteristics

Within its declared allocation/preservation contract, an assigned logical identity shall be unique for the document in its domain, stable through normal evolution, and never reassigned to a different document. Domain qualification is required to interpret uniqueness; an identifier string alone is not universally unique across unregistered domains.

Immutability concerns the assigned Domain+Identifier key under its applicable contract, not every mutable record about that identity. Identity-state evidence, references, location, descriptors and exact-edition coordinates can evolve under their own owner rules without automatically replacing the key. References and aliases interpret an existing logical document; they do not license another document to reuse its identity. Allocated and retired identities remain reserved.

Preserve valid assigned identity during ordinary classification, repository, format, lifecycle and edition changes. If a necessary authorized schema/ID migration would change an otherwise immutable representation/allocation contract, first assess and explicitly reconcile the governing previous/new rules with responsible identity/domain sources. Record old→new mappings, same-document continuity, aliases/reservations, collisions, historical/reference/context effects, exact source editions, affected consumers and transition verification before coordinated application. Preserve original representations and historical immutable snapshot selections; never retarget old members or reassign retired allocations to another document. No blanket permission for arbitrary identity changes or two contradictory governing rules for one operation is introduced. This localized UPDATE performs no migration.

Long-term understandable/referenceable identity is a requirement and design objective supported by qualified domain/canonicalization and actual preservation/resolution evidence. It guarantees neither universally understood bare strings nor future content availability. Exact-edition references additionally identify the intended Version/Revision and relevant bytes/context; logical identity alone selects neither an exact edition nor Baseline membership.

---

# 8. Dependencies

The following supplied sources provide documentary architecture/process authority and orientation. These links are not themselves required runtime service edges; actual required contract consumption is typed in §9. Each source retains its own applicable clauses and exact examined-edition scope.

- [DF-FND-001 — Framework Manifest](../../../00-Foundation/DF-FND-001-FrameworkManifest.md) — Framework interpretation and responsibility boundaries.
- [DF-FND-004 — Architectural Blueprint](../../../00-Foundation/DF-FND-004-ArchitecturalBlueprint.md) — Foundational contracts and selected required pairs.
- [DF-ARC-001 — Architecture Overview](../../../01-Architecture/DF-ARC-001-ArchitectureOverview.md) — Common model, allocation and actual evidence limits.
- [DF-ARC-002 — Architectural Principles](../../../01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md) — Applicable AP clauses, evolution and evidence boundaries.
- [DF-ARC-003 — Architectural Concepts](../../../01-Architecture/DF-ARC-003-ArchitecturalConcepts.md) — Entity/edition/relationship interpretation.
- [DF-ARC-004 — Architectural Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md) — Support order, same-Layer interfaces and prohibited-cycle assessment.
- [DF-ARC-005 — Architectural Components](../../../01-Architecture/DF-ARC-005-ArchitecturalComponents.md) — Registered identity capability, allocation and owner roles.
- [DF-ARC-006 — Terminology](../../../01-Architecture/DF-ARC-006-Terminology.md) — Qualified identity, domain, identifier, edition and state meanings.
- [DF-FND-006 — Design Rationale](../../../00-Foundation/DF-FND-006-DesignRationale.md) — Rationale for identity/description/governance boundaries.
- [DF-ARC-007 — Component Documentation Structure](../../../01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md) — Source-role organization and scoped conformance requirements.
- [DF-RVW-001 — Review Policy](../../../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md) — Adopted corpus allocation/classification/edition/tracking rules.
- [DF-RVW-002 — Review Report](../../../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md) — Actual examined hashes, corrections and pending peer/global reconciliation.

Required dependencies are consumer→provider contracts with scope, exact responsible editions and interfaces. Cross-Layer provider precedence and same-Layer ownership/cycle assessment follow ARC-004 §§12–13. Circular required dependencies are prohibited in the governed scope and actual conflicts remain visible. Documentary authority, allocation, semantic association, projection, navigation and execution are distinct; no label change hides an indispensable requirement. The UPDATE map pins compared editions/scopes; this source claims no complete globally acyclic graph or deployed interface inventory.

---

# 9. Component Relationships

The following are scoped architectural contract declarations for documentary uses. They do not establish an operational service call, every-component routing requirement or complete dependency graph.

| Consumer | Provider | Required contract/use | Source/scope boundary |
|---|---|---|---|
| Metadata | Document Identity | Identity of the normalized document described | DID-009 §5.1 declaration; descriptive values retain their own semantic owners |
| Classification | Document Identity | Identity of the normalized document being classified | DID-009 §5.2; category/definition entity identity is a separate qualified contract |
| Templates | Document Identity | Identity of normalized Template documentation/document instances | DID-009 §5.3; Template definition/instance keys are not automatically DF document IDs |
| Registry | Document Identity | Logical document identity for a document catalog entry | DID-001 §9.4; source-edition provenance and exact lookup context required |
| Relationships | Document Identity | Identity of document endpoints | DID-001 §9.5; other endpoint kinds use their own domain contracts |
| Knowledge Graph | Document Identity | Logical document node identity | ARC-005 §12; typed edges remain Relationships records, not document identities |
| Baselines | Document Identity | Logical member identity | ARC-005 §12; exact edition/descriptive/context evidence additionally required |
| Workflow | Document Identity | Identified normalized document subject | DID-009 §6.1; applicable transition execution remains with the actual process |

## 9.1. Metadata

Identity identifies the logical document; Metadata defines/represents descriptors and owner meanings. Dictionary/Schema/Profile/Instance roles remain separate under one effective Profile. Identity data can be represented descriptively without transferring identity semantics or creating missing Metadata Element/catalog records.

**Unresolved reciprocal declarations:** supplied README states Document Identity→Metadata for descriptive concepts, while DID-009 §§5/10 states Metadata→Document Identity and no dependency on consuming components. Both source claims remain visible as required-dependency evidence pending owner/context/interface reconciliation. Distinguish core identity meaning from identity-record descriptor use, but do not silently downgrade a genuinely required contract into navigation or declare the apparent cycle resolved. Different stated uses alone do not prove operational independence or global acyclicity. Full Metadata/DID source cycles must establish the actual required scopes and cycle treatment under ARC-004.

## 9.2. Classification

Classification owns category meanings and uses identity when categorizing a normalized document. Current Family/Type/Component labels are independent from stable allocation series and do not automatically reconstruct an assigned valid ID. Classification definitions and their own lifecycle/keys are different subjects from document editions; their actual identity contracts need qualification. Nominal CLS-003/CLS-001 collision reconciliation remains scheduled, not corrected by this source.

## 9.3. Templates

Templates owns reusable documentary structures and definition/instance contracts. A normalized document describing or applying a Template can require document identity; Template entities and graph/relationship identifiers are not thereby allocated normalized document IDs. Templates consumes appropriate owner meanings without redefining document identity, Metadata or Classification. Source presence and using a Template prove neither consistency nor approved publication.

## 9.4. Registry

Registry catalogs/looks up identified documentary entities or editions under declared provenance and freshness/current-historical-snapshot context. It does not redefine identity. A document lookup needs its domain/canonical key; an exact-edition lookup additionally needs edition/context evidence. No universal Registry intermediary, implemented resolver or persistent content availability is implied.

## 9.5. Relationships

Relationships owns typed connection records and provenance; Document Identity owns the contract for document endpoints. Other endpoint kinds use their own qualified identity domains. Canonical document reference validity requires the intended document/edition context and actual evidence; logical reference preservation does not imply live-content retrieval. Required edges remain required even when their data comes through a projection; a reference label cannot conceal a genuine cycle.

## 9.6. Knowledge Graph

Knowledge Graph projects identified entities and Relationships records with source/edition provenance and refresh limits. Document nodes use document identity; graph edges or non-document entities need appropriate other contracts. Projections do not create competing identity/relationship authority or certify complete network correctness. No Registry→Graph→Baseline execution chain is prescribed.

## 9.7. Governance

Workflow, Policies, Reviews and Baselines define documentary transition, decision, review and snapshot requirements; actual operation remains with DMS/tool/manual processes and CMS change scope. Identity-record lifecycle, document Status/Version/Revision, maturity, review, validation, approval, publication and membership are distinct. A state list alone is neither a universal permission graph nor an implemented workflow.

Baselines selects an explicitly identified immutable set of exact approved document editions with relevant pinned relationship context or traceable verification evidence. Identity alone cannot select an exact member; eligibility, consistency and actual inclusion remain separate checks. Draft successors neither inherit membership nor retarget older snapshots. Retired identities preserve reservations/history without implying current document publication or resolver availability.

---

# 10. Architectural Constraints

Architectural definitions remain independent of unnecessary programming language, repository, storage or serialization prescriptions. Explicit logical domain, syntax, allocation, canonicalization, reference and integration requirements are architectural contracts, not implementations of generation/storage algorithms. Actual representations and adapters must preserve applicable meaning and supply examined-input/output and executor evidence; concept independence proves neither universal-format compatibility nor tool availability.

Keep one responsible identity semantic owner while permitting explicit cooperation and supporting projections. Preserve compatible meaning where feasible; necessary contract or representation/allocation changes require justified previous/new mapping, exact affected editions, dependencies, consumers and transition checks. Valid identity continuity, non-reuse and historical snapshot evidence remain obligations; an extension is not automatically harmless.

For working document editions, compatible correction retains Version; compatible additive capability increments minor; incompatible contract change increments major and resets minor to 0. Every changed persisted edition increments Revision monotonically across Version changes. Validation of unchanged source changes neither coordinate and is tracked centrally. Other entity-domain lifecycle/numbering requires its own qualified owner, not an implied copy of document edition rules.

---

# 11. Future Architectural Documents

The received heading is retained for numbered-section provenance; the following **fifteen DID documents are actually supplied**, not automatically complete future implementation deliverables. Actual title/path/edition/role coverage is recorded in the UPDATE map. Required responsibility completeness and organization conformance follow applicable domain sources and ARC-007, not a universal filename count or source presence alone.

| ID | Actual declared title / supplied source | Evidence/role boundary |
|---|---|---|
| DF-DID-001 | Document Identity Architecture | This working architecture; ten local corrections pending validation |
| DF-DID-002 | [DF-DID-002 — Document Identity Concepts](DF-DID-002%20-%20Document%20Identity%20Concepts.md) | Concept definitions; full source cycle pending |
| DF-DID-003 | [DF-DID-003 — Document Identity Model](DF-DID-003%20-%20Document%20Identity%20Model.md) | Model/cardinality and canonical representation; conflicts pending |
| DF-DID-004 | [DF-DID-004 — Document Identity Elements](DF-DID-004%20-%20Document%20Identity%20Elements.md) | Element/identity-status meanings; full source cycle pending |
| DF-DID-005 | [DF-DID-005 — Document Identity Schema](../02-Structure/DF-DID-005%20-%20Document%20Identity%20Schema.md) | Schema; references/state/mandatory-field reconciliation pending |
| DF-DID-006 | [DF-DID-006 — Document Identity Lifecycle](../03-Behavior/DF-DID-006%20-%20Document%20Identity%20Lifecycle.md) | Identity-record lifecycle; state-subject reconciliation pending |
| DF-DID-007 | [DF-DID-007 — Document Identity Validation](../03-Behavior/DF-DID-007%20-%20Document%20Identity%20Validation.md) | Validation requirements; full source cycle pending |
| DF-DID-008 | [DF-DID-008 — Document Identity Governance](../03-Behavior/DF-DID-008%20-%20Document%20Identity%20Governance.md) | Identity-governance contracts; full source cycle pending |
| DF-DID-009 | [DF-DID-009 — Document Identity Relationships](../02-Structure/DF-DID-009%20-%20Document%20Identity%20Relationships.md) | Typed consumer relationships/reciprocal dependency reconciliation pending |
| DF-DID-010 | [DF-DID-010 — Document Identity Constraints](../02-Structure/DF-DID-010%20-%20Document%20Identity%20Constraints.md) | Identity/domain/identifier/reference constraints; full cycle pending |
| DF-DID-011 | [DF-DID-011 — Document Identity Extensibility](../03-Behavior/DF-DID-011%20-%20Document%20Identity%20Extensibility.md) | Controlled identity extensibility; full source cycle pending |
| DF-DID-012 | [DF-DID-012 — Document Identity Best Practices](../04-Reference/DF-DID-012%20-%20Document%20Identity%20Best%20Practices.md) | Best-practice recommendations; full source cycle pending |
| DF-DID-013 | [DF-DID-013 — Document Identity Dictionary](../04-Reference/DF-DID-013%20-%20Document%20Identity%20Dictionary.md) | Domain Dictionary consultation; full source cycle pending |
| DF-DID-014 | [DF-DID-014 — Document Identity Specification](../04-Reference/DF-DID-014%20-%20Document%20Identity%20Specification.md) | Consolidated specification; assignment/schema/conformance reconciliation pending |
| DF-DID-015 | [DF-DID-015 — Document Identity Examples](../04-Reference/DF-DID-015%20-%20Document%20Identity%20Examples.md) | Illustrative examples; not implemented conformance |

Received DID-005 title Document Identity Structure maps to actual **Document Identity Schema**; received DID-013 Document Identity Reference maps to actual **Document Identity Dictionary**. All fifteen IDs remain unchanged. Physical names containing spaces and the directory alias DocumentIdentity remain actual supplied paths; this UPDATE renames/moves no source. Classification, placement, content and mandatory role coverage for every peer remain scheduled rather than certified from this map.

Explicit applicable declarations/incorporation establish normative requirements. Architecture, Structure, Behavior or Reference can contain such requirements; Type, title, directory or received Canonical status alone confers no approval, publication or Baseline membership. This source retains architectural identity ownership without asserting all supplied peer contracts are already mutually coherent.

---

# 12. Summary

Document Identity owns qualified logical document identity and its applicable allocation, preservation, reference and validation/governance contracts. Normalized document applicability, Domain+Identifier boundaries, stable series independent of classification and actual executor/evidence requirements prevent unqualified identity/service guarantees. Supporting state/reference records and exact editions remain separate subjects.

The ten local corrections are **Corrected—pending validation**. Full peer schema/lifecycle/assignment/reciprocal required-contract reconciliation and global identity/classification/collision, source maps, Metadata catalog/Profile, planning and implementation work remain pending. No approval, publication, Baseline selection, complete graph or deployed assignment/resolution is established.

A result applies only to exact examined bytes/editions and declared checks. Actual contribution, authorization, review, validation, ownership and approval remain separate. Later human/tool disk edits require assessment of their resulting bytes and do not inherit earlier outcomes or assign the previous contributor responsibility for consequences of a changed final product.

## 12.1. Compatibility assessment

Received identity guarantees/applicability, immutable representation and governance-independent meanings are unqualified; §10 excludes all implementation detail without separating logical representation/allocation requirements, while §12 claims guaranteed permanent identities. V2.0 replaces universal interpretations with explicit normalized/domain/edition/key-record distinctions, actual contract/executor and reference evidence, visible pending reciprocal requirements, and assessed necessary representation/allocation contract migration rather than an unconditional prohibition or arbitrary reassignment permission.

This is **incompatible normative contract reconciliation**. Version 1.0 increments major to 2.0/minor 0; declared Revision 0 increments monotonically to 1. Family correction alone is compatible; Type remains Architecture. Links, title/catalog/editorial corrections alone would also be compatible. Original twelve chapters and 19 numbered sections remain traceable; added §§12.1–12.3 record compatibility, history and propagation. The sole original unnamed allocation view retains provenance externally; no historic view ID is invented. DF-DID-001/path and all fifteen catalog IDs remain unchanged.

## 12.2. Edition history

| Date/event | Version | Revision | Actual contribution and event | Status/Baseline/evidence |
|---|---|---|---|---|
| Original date not supplied; received 2026-09-30 | 1.0 | 0 | Arnaldo Figueira; received Family Documentation, Component Document Identity, Type Architecture, English | Canonical; Baseline1.0 declared; no supplied approval/publication/selection event inferred |
| 2026-10-14 | 2.0 | 1 | Codex — AI assistant; localized scope/identity contract/executor/relationship/evidence reconciliation | Draft; Baseline Not assigned; ten corrections pending VALIDATE DOCUMENT; CHANGELOG #341; Review Report §49 |

Exact input SHA-256: `fda8e8684e464d0c0042850e4b5eaaed5eaefc5e409135274255ce9de8180624`. Complete received/written header and numbered-body maps, one original/written view text/digest, fifteen catalog mappings, eight principle roles, ten boundary rows, required/peer claims and full source/central diff are external evidence. The current source hash is external to avoid recursive revision. Original authorship is preserved; user authorization alone does not attribute this assistant's contribution to the user. Original date and historical approval/selection remain unknown.

## 12.3. Propagation and validation limits

Only DF-DID-001 and central report/tracking/evidence change in this UPDATE. Exact comparison editions/scopes and actual catalog metadata are pinned in the UPDATE map. No allocation, ID/path migration, peer source correction, Metadata Element/Profile creation or external system implementation is performed. Thirteen earlier exact-source Foundation/Architecture validations retain their recorded scopes; their historical pending statements do not certify this successor or completed peer rollout.

| Examined peer discrepancy | Actual source claims | Scheduled reconciliation boundary |
|---|---|---|
| Assignment | DID-001 contract owner does not assign; README/DID-014 §3 says assigning | Contract/executor wording in README and DID-014 still pending |
| Identity-record State/Status | DID-004 Active/Archived/Deprecated; DID-006/DID-014 Unassigned/Assigned/Preserved/Retired | Actual subjects, states and transitions need full owner decisions; no merged graph fabricated |
| Reference cardinality/schema | DID-005 Domain1/Identifier1/Identity References0..N; DID-003 Document Identity→Identity Reference1:N | Full cardinality/schema reconciliation in DID-003/005/010/014 pending |
| Mandatory representation fields | DID-014 adds mandatory Identity State/Canonical Reference and a different schema from DID-005 | No silent mandatory-field removal/addition or guessed unified schema here |
| Reciprocal required consumption | README DID→Metadata descriptive concepts; DID-009 Metadata→DID/no consumer dependency | Both required claims visible; actual owner/context/interface/cycle reconciliation pending |

All nineteen global records remain Open, including REV2-09; INV-02 retains the functional-file exclusion. Ten local corrections await exact-source VALIDATE DOCUMENT. M12 remains In Progress; M10/M11 retain documentary-cycle completion, not integrated conformance. No final Context-Reviewed.zip or whole-component/framework PASS is delivered. Working Draft/Baseline Not assigned requires independent approval, publication and exact membership evidence.

---

**End of Document**

---
