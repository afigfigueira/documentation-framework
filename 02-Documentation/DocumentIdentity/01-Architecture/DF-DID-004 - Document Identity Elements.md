# Documentation Framework

# DF-DID-004 – Document Identity Elements

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-DID-004 |
| **Title** | Document Identity Elements |
| **Family** | Document Identity |
| **Type** | Architecture |
| **Component** | Document Identity |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Purpose

This document defines the architectural roles, constraints, associations and responsibility boundaries of the five named Document Identity elements. It addresses assigned **in-scope normalized logical documents** under a declared identity-domain contract, rather than prescribing serialization, storage, identifier generation or a running resolver.

All files named README.md, CHANGELOG.md or ArchitecturalMilestones.md are non-normalized functional files at every location. Their applicable content, reference, history and hash checks remain; they need no normalized ID/header solely because they are files. Pre-allocation subjects, physical files, representations, logical documents and exact editions are distinct. A document's logical identity alone selects neither Version/Revision nor exact Baseline membership.

Requirements here are architectural contracts, not evidence of actual allocation, uniqueness, implementation, approval or publication. DMS, tools or an applicable manual process execute operations under those contracts; CMS governs changes in its scope. The peer-reconciliation limits in §13.3 remain visible.

---

# 2. Introduction

The five retained element concepts distinguish the assigned identity, canonical identifier representation, domain, state-related facts and references. They are not automatically five mandatory schema fields or a complete implementation model.

An assigned key is interpreted as **Domain+Identifier**. Stability concerns its association with the same logical document under the governing allocation/preservation contract; identity-record states, reference records, classification, locations and edition coordinates can change under their respective owners. Permanence requires reservation/non-reuse and traceability; it does not promise future content retrieval.

Definitions, requirements and observed outcomes shall be distinguished. Evaluation records the responsible source/edition, actual artifacts and domain/context, check or executor, coverage, observations and unresolved conditions. Source presence, title or a local PASS does not prove global conformity.

---

# 3. Architectural View

The following selected conceptual view retains the five original concepts. It depicts roles, not mandatory field composition, ownership transfer, operational calls or required-dependency direction.

<!-- original-section-view: 3 -->
**Previously unnamed view in §3 — Element roles.**

| Subject | Relation | Related concept | Qualification |
|---|---|---|---|
| Document Identity | has canonical representation | Identifier | One canonical representation under the governing domain rules |
| Document Identity | is qualified by | Identity Domain | One governing domain per assigned key |
| Identity Status | describes state-related facts about | Document Identity | Separately owned state/edition/lifecycle subjects; no merged mandatory field is implied |
| Identity Reference | targets | Document Identity or intended exact edition | Typed document endpoint; incoming population0..N; additional exact-edition coordinates/context required |
<!-- end-original-section-view -->

The original diagram's Identity References label is the plural population of Identity Reference. DID-003 §§4–6 supplies the selected conceptual model/cardinality interpretation. Schema/Specification mandatory fields and lifecycle vocabularies still require their own reconciliation; see §§4.4/13.3. Full received/written view texts and hashes are attached to the review report UPDATE evidence; this original-section anchor does not invent a historical diagram ID.

---

# 4. Architectural Elements

The five original element titles and subordinate headings are retained. Conceptual element responsibility does not by itself create a Metadata Element, mandatory schema field, interface or runtime component.

---

## 4.1. Document Identity



### 4.1.1. Description

**Document Identity** is the stable same-document logical identity under a declared allocation/preservation contract. An assigned key differs from the file containing the document, its edition coordinates, descriptive records and reference associations. An unassigned documentary subject does not yet possess that assigned key.

---

### 4.1.2. Responsibility

- Identify the applicable assigned logical document within its domain.
- Preserve the same-document association across ordinary lifecycle, classification, content, edition, format and repository changes.
- Provide document endpoint meaning for qualified references without claiming a live resolution service.

Allocation, collision/reservation and preservation checks require actual records and responsible executors; registration alone proves no approval or successful allocation.

---

### 4.1.3. Characteristics

- **Unique:** a requirement within the qualified domain and examined allocation scope, not globally unique unqualified strings.
- **Immutable:** the assigned key/association under its governing contract, not every state/reference record.
- **Permanent:** allocated/retired keys are not reassigned; historical interpretation is preserved without a retrieval guarantee.
- **Canonical:** an explicitly governed interpretation/representation, not document Status, approval or automatic Baseline inclusion.

---

## 4.2. Identifier



### 4.2.1. Description

The **Identifier** represents a document identity under its domain's canonicalization/allocation rules. The logical entity, qualified key and rendered string are related but distinct. Aliases and other representations shall identify the intended existing key under explicit rules; they do not allocate another interchangeable document identity.

---

### 4.2.2. Responsibility

- Represent the assigned qualified identity under responsible domain rules.
- Support unambiguous human/machine interpretation with the necessary domain/context.
- Preserve valid allocations when Family, Type, Component, path or edition changes.

For this corpus, Documentation Framework is the domain, represented by DF. The adopted convention is **DF-SSS-NNN**: registered uppercase three-letter stable allocation series and positive three-digit allocation001–999. Current classification does not regenerate assigned IDs. Equal numeric suffixes across different series are not collisions when the full qualified IDs differ. 000 is not allocated; a gap proves no availability; allocated/retired numbers are not reused. At999, register an unused series with traceable continuation rather than widen or recycle silently. This restates DID-001/Review Policy; detailed DID-005/010/014 integration remains pending. No new allocation occurs here.

---

### 4.2.3. Characteristics

Unique within the governed domain, stable for its assigned document, deterministically interpretable under explicit representation/canonicalization rules, and semantically independent of implementation technology. Deterministic interpretation does not demonstrate an implemented generator/resolver or actual uniqueness. Logical requirements can constrain adapters and representations without choosing a storage format.

---

## 4.3. Identity Domain



### 4.3.1. Description

**Identity Domain** defines the qualified scope, responsible allocation rules and uniqueness boundary. Domain definition imposes a requirement; actual population and collision/reservation checks establish observations within a stated scope.

---

### 4.3.2. Responsibility

- Establish domain qualification, namespace and responsible allocation/preservation authority.
- Require collision and reservation checks across applicable current/historical records.
- Make non-overlap and cross-domain interpretation explicit rather than assume every bare string is globally unique.

One assigned key has one governing domain. A domain may contain0..N assigned identities unless an applicable owner contract establishes another minimum. Other domains require explicit owners/rules and qualification; this document does not create a universal external-domain registry.

---

### 4.3.3. Characteristics

Stable governing meaning, explicit architectural qualification, and implementation-independent semantics. Domain stability does not prove operational namespace separation; declared owners, actual allocations and context must support that assessment.

---

## 4.4. Identity Status



### 4.4.1. Description

**Identity Status** retains the original architectural element name for state-related facts about identity records. It is not defined here as one universal validity enum. Separate assigned-key existence/preservation/retirement, state assertions, document-edition Draft/Review/Approved/Published/Archived status, maturity and Baseline membership.

DID-003 does not make Identity Status a sixth core entity; DID-005 omits a State field; DID-014 makes Identity State mandatory. Those are real peer-contract differences, not permission to silently add or remove mandatory fields. Metadata can describe a domain-owned state without redefining its semantics; independence does not mean that no descriptive representation or required consumer contract can exist.

---

### 4.4.2. Possible States

The received labels **Active**, **Archived** and **Deprecated** are retained as historical candidate terminology, not an authoritative current state machine or proof of architectural validity. DID-006 §§4–8 and DID-014 §9 instead use Unassigned, Assigned, Preserved and Retired for their stated lifecycle subject. Unassigned is pre-allocation; it does not mean an assigned key already exists.

Do not equate Archived document status with retired identity or derive identity validity from a state word alone. Final state vocabulary, transition permissions, subject and authority require explicit DID-006/014 and Schema/Model reconciliation. This architectural clarification neither approves their complete lifecycle nor invents a merged transition graph.

---

## 4.5. Identity Reference



### 4.5.1. Description

An **Identity Reference** is a typed association whose document endpoint identifies an intended qualified logical document or exact edition. Other endpoint kinds use their own applicable identity contracts. Document Identity owns document endpoint meaning; Relationships owns connection semantics/records, and Registry owns registration/index records in their scopes. An association does not transfer those responsibilities.

---

### 4.5.2. Responsibility

- Identify an intended existing qualified target without creating/redefining its identity.
- Distinguish document-level targeting from exact-edition targeting, which additionally pins coordinates/bytes and relevant context.
- Support cross-component references with declared owner, relation kind, source/target and provenance.

An identity can exist without incoming references: document-targeting incoming population is0..N under DID-003 §6 and DID-005 §§4.3/5. A dangling or ambiguous reference is an unresolved validity observation; it does not authorize creating or silently retargeting an identity. Historical target interpretation is distinct from current retrieval.

---

# 5. Element Relationships

The second selected conceptual view preserves Document and the five original element concepts while clarifying relationship direction and subject. It is not a mandatory object layout or required-service graph.

<!-- original-section-view: 5 -->
**Previously unnamed view in §5 — Document and element associations.**

| From | Relation kind | To | Bounds / interpretation |
|---|---|---|---|
| Applicable assigned normalized Document | assigned identity association | Document Identity | One governing key for that logical document under its declared contract |
| Document Identity | canonical representation | Identifier | One canonical representation; aliases do not allocate a different document |
| Document Identity | domain membership | Identity Domain | One governing domain; domain population0..N absent another applicable owner minimum |
| Identity Status | state-related description | Document Identity record | Separate record/subject; mandatory field and state vocabulary remain peer work |
| Identity Reference | document targeting | Document Identity / exact edition | Incoming reference population0..N; qualified target/context required |
<!-- end-original-section-view -->

The original outbound arrows did not prove semantic ownership of every related record or universal one-way dependency. Preserve definition ownership while recording actual required consumer→provider contracts, associations, projections, navigation and execution separately under ARC-004 §§12–13. No mandatory dependency is concealed by a different arrow/relationship label, and no global acyclicity is claimed.

---

# 6. Element Responsibilities

| Element | Responsibility | Boundary |
|---|---|---|
| Document Identity | Same-document logical identity under its domain contract | Assigned key differs from file, edition and state records |
| Identifier | Canonical representation of qualified identity | Allocation/canonicalization rules and observed checks required |
| Identity Domain | Governing qualification and uniqueness scope | Declared boundary is not proof of population uniqueness |
| Identity Status | Distinguishes state-related assertions about the proper subject | State vocabulary/mandatory-field authority remains pending peer reconciliation |
| Identity Reference | Typed targeting of an intended existing document/edition | Connection ownership and0..N incoming population remain separate from key ownership |

These five retained rows describe architectural responsibility, not five mandatory persisted schema fields.

---

# 7. Element Constraints

The following requirements apply within the stated normalization, assignment and domain scope. A requirement is not evidence of its own execution. Actual checks identify responsible contracts/editions, artifacts, executor, coverage, observations and unresolved conditions.

---

## 7.1. Document Identity

- One assigned identity for an applicable assigned normalized logical document under its declared contract; pre-allocation subjects and functional files differ.
- Preserve the key's association with the same document; never reuse allocated or retired identities for another document.
- Ordinary content, classification, edition, format, repository and status changes do not reallocate the key.

If a necessary authorized migration would change the otherwise immutable representation/allocation contract, first reconcile previous/new owner rules, affected sources/consumers, mappings, collision/reservation history, aliases, transition checks and historical reference/snapshot continuity. Preserve old evidence and do not retarget immutable snapshot members. No migration is performed here.

---

## 7.2. Identifier

- One canonical identifier representation per assigned identity under explicit domain rules.
- Uniqueness assessed over the full qualified key, with current/historical allocation and reservation coverage stated.
- Stable assigned representation under the governing contract; mutable classification and edition coordinates are not identifier segments recalculated by this UPDATE.
- Canonical interpretation and any aliases require explicit target rules; no runtime resolution guarantee is inferred.

---

## 7.3. Identity Domain

- Each assigned identity belongs to one governing domain.
- Namespace/non-overlap requirements require explicit qualification, owners and checked scope; coincident numeric suffixes across different series do not alone collide.
- A domain's existence does not require a currently allocated member absent another contract.
- Domain change affecting assigned identity requires the prior/new contract and continuity assessment in §7.1, not silent reassignment.

---

## 7.4. Identity Status

- Changing a state description does not automatically change the assigned identity key.
- State assertions identify their subject, owner and governing vocabulary; document-edition status, identity lifecycle and approval/Baseline evidence differ.
- A Metadata representation does not redefine the state domain. Do not assert total independence where actual consuming contracts exist.
- Preserve the DID-004/006/014 and DID-003/005 differences in §4.4 until the responsible peer cycles reconcile them. No new universal valid-state or transition enum is imposed.

---

## 7.5. Identity Reference

- A valid document-targeting reference identifies its intended existing qualified target, and exact-edition references additionally pin the intended edition/context.
- An identity requires no incoming reference merely to exist; applicable incoming population0..N is separate from per-reference target validity.
- A reference neither allocates nor redefines the target. Other endpoint kinds follow their own contracts.
- Mutable connection records retain their owners/provenance; identity stability does not guarantee all references remain valid or retrievable after arbitrary change.

---

# 8. Ownership

| Element | Definition responsibility | Related record/execution boundary |
|---|---|---|
| Document Identity | Document Identity | Actual allocation/preservation executor and evidence are separately identified |
| Identifier | Document Identity under domain rules | Generator/adapter/resolver implements applicable rules; no service supplied here |
| Identity Domain | Document Identity and declared domain authority | Namespace/registration/allocation decisions need actual records |
| Identity Status | Applicable identity-state/lifecycle owner; detailed peer reconciliation pending | Metadata may describe states; document status/approval/Baselines retain their own subjects |
| Identity Reference | Document Identity for document endpoint semantics | Relationships owns connections, Registry registration; other endpoint kinds retain domain ownership |

Consumers shall not silently redefine document identity. Exclusive identity meaning does not give Document Identity ownership of all metadata, classifications, connections, indexes or governance operations. Definition, required consumption, data projection and execution differ.

---

# 9. Relationships with Other Components

| Component / retained area label | Interaction | Responsibility / evidence limit |
|---|---|---|
| Metadata | Describes identified documents and represented state/edition facts | Metadata owns descriptors; domain owners retain identity/status meanings; Schema/Profile/Instance rules still apply |
| Classification | Associates categories with identified documents | Mutable classification does not recalculate assigned IDs |
| Registry | Registers/indexes qualified identities | Registry owns registration records; registration alone proves no allocation, approval or resolution |
| Relationships | Connects qualified endpoints using typed associations | Owns relation semantics/records; Document Identity owns document endpoint meaning |
| Knowledge Graph | Projects identities and typed relationships | Projection does not create identity authority or require every consumer to route through a graph |
| Governance (area label retained) | Workflow, Policies, Reviews and Baselines act within their scopes | Governance is an area, not a new component; logical identity alone does not select an approved exact-edition Baseline member |

The six original rows remain, with Governance explicitly qualified. Actual required consumer→provider edges identify contract, scope, responsible sources and interfaces under ARC-004. The supplied DID README declares identity consumption of Metadata descriptive concepts, while DID-009 §§5/10 declares Metadata→Document Identity and no consuming-component dependency. These claims need actual core/descriptor/interface scope assessment; different names alone prove no independence or acyclicity. Do not conceal a required cycle through projection or semantic relabelling. No universal Registry/Graph routing path is imposed.

---

# 10. Architectural Characteristics

The eight received characteristics are retained with bounded meanings.

| Characteristic | Qualified requirement / observation boundary |
|---|---|
| Canonical | Governed identity interpretation/representation; not lifecycle Canonical status, approval or publication |
| Uniquely identifiable | Qualified domain/key with stated collision/allocation evidence; no global bare-string guarantee |
| Immutable | Assigned key/same-document association under governing contract; state/reference records may change |
| Permanent | Reservation/non-reuse and historical target continuity; no future content-availability guarantee |
| Implementation independent | Conceptual semantics do not choose a runtime; legitimate logical/interface/representation requirements still apply |
| Repository independent | Ordinary repository movement preserves identity; actual references/bytes/adapters still need checks |
| Technology independent | Domain meaning is not redefined by storage/serialization; actual integrations must preserve it |
| Reusable across the Documentation Framework | Applicable consumers reuse responsible meanings under explicit compatible contracts; no evidence of complete rollout |

Conformance assessment requires actual artifacts/editions/context, applicable rules, checks/executor, observations, coverage and unresolved conditions. This draft UPDATE supplies no implemented allocation, resolver, global proof, approval, publication or Baseline membership.

---

# 11. Dependencies

The three original dependencies remain:

- [DF-DID-001 — Document Identity Architecture](DF-DID-001-DocumentIdentityArchitecture.md): component role, normalized scope, qualified assignment/preservation and ownership.
- [DF-DID-002 — Document Identity Concepts](DF-DID-002%20-%20Document%20Identity%20Concepts.md): conceptual identity/domain/reference distinctions.
- [DF-DID-003 — Document Identity Model](DF-DID-003%20-%20Document%20Identity%20Model.md): conceptual entities and selected cardinalities, including0..N incoming references.

These are source-contract dependencies, not a running call chain. Also consult [Schema](../02-Structure/DF-DID-005%20-%20Document%20Identity%20Schema.md), [Lifecycle](../03-Behavior/DF-DID-006%20-%20Document%20Identity%20Lifecycle.md), [Relationships](../02-Structure/DF-DID-009%20-%20Document%20Identity%20Relationships.md), [Constraints](../02-Structure/DF-DID-010%20-%20Document%20Identity%20Constraints.md) and [Specification](../04-Reference/DF-DID-014%20-%20Document%20Identity%20Specification.md) for their actual owner clauses and unresolved field/state/representation integration; links do not claim finished peer cycles.

Architectural boundaries follow [Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md) and [Components](../../../01-Architecture/DF-ARC-005-ArchitecturalComponents.md). Metadata description uses [Model](../../Metadata/01-Architecture/DF-MTD-003-MetadataModel.md) and [Dictionary](../../Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md) without fabricating new fields/profiles. Working identity, edition, authorship and evidence rules follow [Review Policy](../../../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md); current operations are in [Review Report](../../../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md).

Before cross-document normative propagation or migration, identify the responsible batch, rationale, old/new meaning and affected owners/consumers. Partial rollout does not establish integrated consistency.

---

# 12. Summary

The five original architectural element concepts remain traceable while assigned key/representation, domain, mutable state-related facts and typed references are distinguished. The document defines bounded responsibilities and requirements rather than universal operational guarantees.

Detailed schema/state/mandatory-field, ownership/required-dependency and representation integration remains scheduled with the responsible peers. A local correction or validation does not approve those peers, the whole component or the framework. Exact validation of this successor remains pending.

---

# 13. Edition History and Reconciliation

## 13.1. Received edition

Received V1.0 R0: Family Documentation, Type Architecture, Component Document Identity, Author Arnaldo Figueira, Status Canonical, Baseline1.0, English; original date not supplied. Preserve these as input declarations, not proof of actual approval/publication or an assigned successor Baseline. The exact original bytes/hash remain in external review/update evidence.

## 13.2. Working successor and compatibility

| Date | Version | Revision | Author contribution | Change / lifecycle |
|---|---|---|---|---|
| 2026-10-14 | 2.0 | 1 | Codex — AI assistant; original Arnaldo Figueira contribution retained | Step4.17 UPDATE after recovered REVIEW; incompatible applicability, state/field authority, ownership and guarantee clarification. Draft; Baseline Not assigned; ten corrections pending VALIDATE DOCUMENT. |

The incompatible change narrows previous universal identity/guarantee assertions and corrects state authority, reference ownership/cardinality and field interpretation. This is more than relabelling Family: increment major1→2, minor0, Revision0→1 under Review Policy§5. Cumulative Author does not attribute every event or approval to every listed person. No source ID/path migration is needed.

## 13.3. Pending integration and validation

DID-003 conceptual entities, DID-005 optional references/no State, DID-006 lifecycle and DID-014 mandatory State/Canonical Reference remain separate actual contracts; no merged schema or universal transition graph is certified. Detailed DID-005/010/014 corpus syntax, state authority, Metadata representation, Registry/Relationships ownership, reciprocal required dependencies and implementation outcomes require owner/consumer reconciliation and scoped evidence. The actual UPDATE map records source/peer hashes, changes and original view provenance.

This edition has not undergone VALIDATE DOCUMENT. Prior exact-edition and attribution-only results retain their original scopes; no approval, publication, Baseline, allocation, migration or global architectural validation is inferred.

---

**End of Document**
