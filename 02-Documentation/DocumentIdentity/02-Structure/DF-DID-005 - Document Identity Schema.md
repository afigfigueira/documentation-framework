# Documentation Framework

# DF-DID-005 – Document Identity Schema

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-DID-005 |
| **Title** | Document Identity Schema |
| **Family** | Document Identity |
| **Type** | Structure |
| **Component** | Document Identity |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Purpose

This document defines a logical schema view for **applicable assigned normalized document identities** under an explicit identity-domain contract. It specifies domain qualification, canonical identifier representation and optional incoming document-targeting references. The assigned key, mutable records about that key, reference associations and exact document editions are distinct subjects.

Every file named README.md, CHANGELOG.md or ArchitecturalMilestones.md is a non-normalized functional file at every location. These names require no normalized identity/header solely because they are files; applicable content, references, history and hash checks remain. A pre-allocation subject does not yet possess an assigned key. Other entity kinds and external identity domains need their own explicit owner contracts, not automatic allocation of DF document IDs.

This working schema defines requirements, not an implemented assigning, registering or resolving service. DF owns documentary semantics; DMS, tools or an applicable manual process execute operations under those contracts, while CMS governs changes in its scope. Received Canonical naming and a local validation do not establish approval, publication, Baseline membership or whole-framework implementation conformity.

---

# 2. Introduction

The three original schema-element roles are retained with explicit subject and responsibility boundaries:

- **Identity Domain:** governing scope for the assigned key and allocation/preservation requirements.
- **Identifier:** canonical representation of the qualified logical identity.
- **Identity References:** optional incoming logical associations, external to the identifier and owned as connection records by their applicable relationship contract.

Cardinality describes an applicable assigned subject or reference population, not a database layout. Logical identity is interpreted as **Domain+Identifier**, distinct from a rendered string, alias, physical file, exact Version/Revision, state record or snapshot selection. Exact-edition references additionally pin the intended edition/bytes and relevant context. Identity alone neither selects an approved Baseline member nor retargets an older immutable snapshot.

This schema does not choose physical storage, XML/JSON/YAML, database tables, classes or generation algorithms. It can impose logical representation and interface requirements that implementations must preserve. The three-role view is not a declaration that State or Canonical Reference requirements from other responsible sources have been removed; §6 records the actual peer differences.

---

# 3. Canonical Schema

The first view preserves the original Domain/Identifier/Identity References subjects while distinguishing key composition from an incoming association population. It is a logical contract view, not mandatory physical containment, a complete merged identity record or an execution/dependency graph.

<!-- original-section-view: 3 -->
**Previously unnamed view in §3 — Schema subjects.**

| Subject | Relation kind | Related subject | Scope/cardinality |
|---|---|---|---|
| Assigned Document Identity | governing domain qualification | Identity Domain | Exactly1 domain per assigned key |
| Assigned Document Identity | canonical representation | Identifier | Exactly1 canonical identifier under that domain's rules |
| Identity References | typed incoming document-targeting associations | Intended Document Identity or exact edition | Incoming population0..N; each valid reference identifies its intended qualified target/context |
<!-- end-original-section-view -->

The first two rows describe the qualified key and its interpretation. The third is not an identifier segment or a required contained connection store. Original view text/digest is preserved in external UPDATE evidence under its original section; no historical diagram ID is invented. Selected peer requirements in §6 remain explicit.

---

# 4. Schema Elements

The three received labels and their Purpose/Cardinality/Characteristics headings are retained. Logical role and subject are distinguished from mandatory fields in a particular complete record. State/Canonical Reference differences remain declared in §6 rather than guessed away here.

---

## 4.1. Identity Domain



### 4.1.1. Purpose

Identity Domain establishes the declared qualification, owner and scope within which an assigned document key shall be unique. Defining a domain imposes a requirement; actual allocation/collision/reservation evidence establishes observations within a stated population and history scope. An unqualified string is not universally unique across other domains.

---

### 4.1.2. Cardinality

```text
Exactly one
```

One governing domain per applicable assigned identity. This is membership cardinality; a domain's population may be0..N unless a separately applicable domain-owner contract sets another minimum. Pre-allocation subjects do not yet have an assigned key. No external-domain registry or live allocation is created by this rule.

---

### 4.1.3. Characteristics

- **Mandatory:** governing domain qualification is required for the applicable assigned key.
- **Immutable:** ordinary changes preserve domain/key association under the governing contract; a necessary governed migration first requires §11 reconciliation.
- **Permanent:** domain/assignment history and non-reuse reservations remain traceable; this does not guarantee future content retrieval.

Namespace/non-overlap claims require explicit domain rules, owners, cross-domain qualification and checked allocation coverage, not presumed global separation.

---

## 4.2. Identifier



### 4.2.1. Purpose

Identifier is the canonical representation of assigned identity under its governing domain/canonicalization rules. The logical document, qualified key, rendered string and any permitted alias are distinct. Alternative representations must identify the intended existing key; they do not license another document to reuse it.

For this corpus, the domain is **Documentation Framework**, represented by **DF**. The adopted identifier convention is **DF-SSS-NNN**, where SSS is a registered uppercase three-letter stable allocation series and NNN is a positive three-digit allocation001–999. Full qualified identifiers, not numeric suffixes alone, determine collisions. The series records its allocation origin; current Family, Type, Component, path, Version/Revision and Status do not regenerate an assigned ID.

000 is not allocated and is not a README code. Gaps do not prove availability; allocated and retired numbers remain reserved. Allocation requires explicit series records and checks of relevant current/historical/reserved identities and references. At999, register an unused three-letter continuation series with traceability; do not widen syntax or recycle silently. Policy§4 and DID-001/003/004 establish these corpus rules. This schema integrates their scoped representation; other domains require explicit rules and no new allocation or migration occurs here.

Canonical interpretation states the responsible domain/rules and intended existing target. Alias/canonicalization handling must be explicit and preserve historical interpretation. Neither this format nor a syntax match proves allocation, uniqueness, a running resolver or retrieval availability.

---

### 4.2.2. Cardinality

```text
Exactly one
```

One canonical identifier representation per applicable assigned identity. Domain qualification remains required. Multiple aliases or physical representations do not create multiple logical document identities or erase the canonical interpretation requirement.

---

### 4.2.3. Characteristics

- **Mandatory:** a canonical identifier represents the applicable assigned identity.
- **Unique:** the qualified Domain+Identifier shall identify the intended document; actual collision/reservation coverage is recorded separately.
- **Immutable:** ordinary content/classification/status/edition/repository changes preserve the assigned key under its governing contract.
- **Permanent:** preserve same-document association and allocated/retired reservations; never reassign to another document.

Deterministic interpretation is a governed representation requirement, not proof of an implemented generator/resolver. Necessary contract/migration changes require the prior/new assessment in §11 rather than silent reallocation.

---

## 4.3. Identity References



### 4.3.1. Purpose

Identity References is the population of typed incoming associations targeting an intended qualified document identity or exact edition. They are logical associations, external to the identifier; they need not be physically stored within an identity record.

Document Identity owns document endpoint meaning; Relationships owns connection semantics/records and provenance. Registry owns registration/index records; graph projections do not create alternative identity authority. Other endpoint kinds use their own applicable identity contracts rather than automatically receiving normalized DF document IDs. Exact-edition targeting additionally identifies intended coordinates/bytes and context; logical identity alone is insufficient.

---

### 4.3.2. Cardinality

```text
Zero or more
```

An assigned identity can exist without any incoming reference. This preserves the received0..N and agrees with DID-003 §6 and DID-004 §§4.5/7.5. Incoming population cardinality differs from each reference's valid target: a valid document-targeting association must identify its intended qualified document/edition under its relation contract. This schema does not define every possible multi-endpoint relationship format.

---

### 4.3.3. Characteristics

- **Optional:** incoming reference population0..N; absence does not invalidate an assigned identity.
- **Extensible:** additional governed associations or endpoint types preserve existing meaning/ownership; a new reference does not redefine its target.
- **Implementation independent:** semantic target/owner/provenance rules do not prescribe a storage layout or require every consumer to route through Registry/Knowledge Graph.

Reference records can evolve under their owner rules without reallocating the target identity. Dangling, ambiguous, stale or unavailable targets are observations requiring evidence and correction, not permission to create or silently retarget an identity. Historical interpretation differs from current retrieval.

---

# 5. Cardinality

| Element | Cardinality | Actual subject and interpretation |
|---|---|---|
| Identity Domain | 1 | One governing domain per applicable assigned key; domain population is a different subject |
| Identifier | 1 | One canonical representation under governing domain rules; aliases do not allocate another document |
| Identity References | 0..N | Optional incoming document-targeting association population; each valid association identifies its intended qualified target/context |

These three original rows are retained. The first two concern the assigned key; the last concerns external associations, not a mandatory identifier segment or schema-owned record collection. They do not settle complete-record State/Canonical Reference obligations in §6 or create cardinalities for every other endpoint kind.

---

# 6. Logical Relationships

The second view preserves the same three subjects as the received relationship diagram. It qualifies direction, authority and subject; it is not a mandatory object layout, operational call chain or required-dependency graph.

<!-- original-section-view: 6 -->
**Previously unnamed view in §6 — Logical relationships and owner boundaries.**

| From | Relation kind | To | Meaning / boundary |
|---|---|---|---|
| Assigned Document Identity | belongs within | Identity Domain | One governing allocation/preservation scope |
| Assigned Document Identity | is represented through | Identifier | One canonical interpretation under domain rules |
| Identity Reference | targets | Intended Document Identity / exact edition | Incoming0..N population; connection records remain with their relationship owner |
<!-- end-original-section-view -->

Minimal key/association scope is distinct from the complete subject claimed by other specifications. The following records actual peer requirements; it neither deletes mandatory peer fields nor invents an accepted merged record/state machine.

| Subject | This source's retained view | Actual responsible peer clauses | Remaining integration obligation |
|---|---|---|---|
| Domain / Identifier | Assigned governing qualification and canonical representation | DID-003 §§4–6; DID-004 §§4/7; DID-014 §§7–8 mandatory Domain/Identifier | Preserve qualified key and explicitly governed corpus representation/other domains |
| Identity References | Optional incoming associations0..N | DID-003 §§5.4/6; DID-004 §§4.5/7.5 | Connection ownership,typed target and exact-edition evidence; not a mandatory key field |
| Identity State / Lifecycle State | Not introduced as a merged key field by this source | DID-014 §§7–8 mandates State/Lifecycle State; DID-006 §§4–8 defines Unassigned/Assigned/Preserved/Retired for its lifecycle subject | Reconcile field/record subject,authority,vocabulary and transitions with owners; no implicit removal or universal-state approval |
| Canonical Reference | Not equated with optional plural Identity References | DID-014 §§7–8 makes Canonical Reference mandatory | Reconcile representation/field versus association meaning and mandatory scope; omission from this selected view does not waive the peer requirement |

DID-004 retains Active/Archived/Deprecated as historical candidate terminology; these are not automatically equivalent to DID-006 lifecycle states or document-edition Draft/Review/Approved/Published/Archived status. Unassigned concerns pre-allocation, not an already assigned key. State,Status,exact edition,maturity,approval and Baseline membership require their proper subject/owner evidence. This source-local schema correction does not complete DID-006/014 cycles,authorize disregarding mandatory claims or certify integrated conformity. Contradictory complete-record claims require a coordinated owner decision before claiming a fully reconciled implementation contract.

---

# 7. Schema Principles

The four original principles are retained as bounded requirements. Their headings are not invented framework AP identifiers or proof of implemented outcomes.

---

## 7.1. Single Responsibility

Each schema role has one stated responsibility and subject. Domain/key meanings,reference association records,Metadata descriptions,registration and execution are separately owned. A logical view may reference related records without transferring their ownership or declaring every concept a mandatory stored field.

---

## 7.2. Stability

Preserve assigned same-document identity and compatible consumer meaning during ordinary evolution. Schema stability is a design objective with controlled contract evolution, not a claim that all future editions are compatible by definition.

Prefer compatible/additive extensions where they preserve the governing contract. A necessary incompatible change first identifies previous/new meaning,affected owners/consumers,dependencies,exact editions and transition/migration evidence under §11. It does not silently override still-applicable peer constraints. Working document Version/Revision successors follow Policy§5; entity allocation and lifecycle are distinct.

---

## 7.3. Canonical Representation

Applicable assigned identities conform to the declared governing domain/representation contract, not an unqualified universal format for all external domains. In this corpus, DF-SSS-NNN and Domain+Identifier rules in §4.2 apply independently of current classification.

Alternative implementations preserve intended target interpretation,qualified key/association meaning,cardinality and responsible provenance under explicit mappings. Syntax validity differs from actual allocation/uniqueness,record completeness,reference validity and exact-edition/Baseline selection. The partial view here does not silently replace DID-014's mandatory complete-record claims; §6 records pending reconciliation.

---

## 7.4. Technology Independence

The logical schema does not choose programming languages,databases,serialization formats,repositories or storage mechanisms. Implementations and adapters still need to satisfy applicable logical domain/representation/interface,record and evidence requirements. Technology independence is not evidence that every implementation already interoperates.

Assess actual artifacts/editions/context against applicable owner rules,with checks,observations,executor,coverage and unresolved conditions. DMS/tool/manual execution and CMS change evidence do not replace DF domain semantics,formal approval or actual Baseline inclusion.

---

# 8. Schema Constraints

The following requirements concern the stated assigned key and incoming-association subjects. Requirement text is not execution evidence. Record responsible contracts/editions,artifacts/domain/context,executor,coverage,observations and unresolved conditions for any claimed check.

---

## 8.1. Identity Domain

- A governing domain shall qualify every applicable assigned key; pre-allocation subjects and excluded functional files differ.
- Ordinary evolution preserves the assigned domain/key association under its governing contract.
- Domain qualification,owner,rules and namespace/collision/reservation coverage shall be explicit; a domain declaration does not prove actual uniqueness.
- A necessary migration affecting the governing contract requires §11 prior/new reconciliation and continuity checks before application; no silent domain reassignment is authorized.

---

## 8.2. Identifier

- Each applicable assigned identity has one canonical identifier representation under its domain rules.
- Full qualified key uniqueness requires actual allocation/collision/reservation evidence; matching syntax alone does not prove it.
- Assigned identifiers remain stable across ordinary classification,content,edition,location and document-status changes; current Family/Type does not reconstruct allocation series.
- Allocated and retired identifiers shall never be reassigned to another document. Preserve old representations,reservations and historical references/snapshot selections through any necessary governed transition.
- Apply §4.2 corpus syntax and canonicalization scope; no new series,identifier,alias or migration is created by this UPDATE.

---

## 8.3. Identity References

- A valid document-targeting reference identifies its intended existing qualified document or exact edition/context; other endpoint kinds follow their own contracts.
- Incoming population remains optional0..N; an identity does not need an incoming reference merely to exist.
- References never allocate or redefine their target and remain external to the identifier.
- Connection records retain their relationship owner and provenance; mutations do not automatically change the target key.
- Record dangling,ambiguous,stale or unavailable references as actual observations; preserve historical interpretation and never silently retarget. Identity stability alone guarantees no live-content retrieval or universal future reference validity.

---

# 9. Ownership

| Schema Element | Definition responsibility | Related record/execution boundary |
|---|---|---|
| Identity Domain | Document Identity and declared domain authority | Namespace/allocation rules and actual records/registrations need scoped evidence |
| Identifier | Document Identity under governing domain rules | Actual generator/adapter/resolver executes applicable contracts; no service supplied here |
| Identity References | Document Identity for document endpoint meaning | Relationships owns typed connections/provenance; Registry registration and other endpoint kinds retain their owners |

These three original rows remain. Other components shall not silently redefine document identity,but exclusive identity meaning does not transfer all Metadata values,registrations,connections or governance operations to Document Identity. Descriptors can represent identity/state under their semantic owners without fabricating a Metadata Element,Profile or merged schema catalog.

---

# 10. Relationship with Other Components

| Component / retained area label | Usage | Contract / evidence boundary |
|---|---|---|
| Metadata | Associates descriptors with identified documents | Domain meanings remain with identity/state owners;Schema/Profile/Instance/Dictionary roles need their own applicable contracts |
| Classification | Classifies identified documents | Mutable Family/Type/Component labels do not recalculate stable allocation series |
| Registry | Registers/indexes qualified identities or editions | Owns registration records;exact-edition context and freshness evidence needed;registration alone proves no allocation/approval |
| Relationships | Creates typed semantic connections between qualified endpoints | Owns connection semantics/records;Document Identity owns document endpoint meaning;other endpoints use applicable contracts |
| Knowledge Graph | Projects identified entities and typed connections | Projection is not a new identity authority or universal routing intermediary |
| Governance (area label retained) | Workflow,Policies,Reviews and Baselines govern their stated subjects | Area,not a new component;identity alone selects no approved exact-edition Baseline member |

Six original interaction labels are preserved with qualified roles. Actual required dependencies use consumer→provider direction and state the contract,scope,provider/consumer/source editions and interfaces under ARC-004 §§12–13. Semantic association,documentary reference,projection,navigation and execution are distinct,not ways to hide a required cycle.

DID-009 §§5/10 declares Metadata→Document Identity/no consuming-component dependency,while the functional DID README Component Dependencies/Metadata declares identity consumption of Metadata descriptive concepts. These actual claims remain pending owner/core-versus-descriptor/interface reconciliation;different names alone prove neither independence nor acyclicity. No universal Registry/Graph service chain or complete graph proof is supplied.

---

# 11. Extensibility

Schema evolution shall preserve same-document assignment,non-reuse and compatible meaning where feasible. Additional roles may be introduced only through an explicit responsible contract and impact assessment,not by treating a picture or Metadata representation as an automatically registered field.

Before a necessary normative change or path/identity migration:

1. Identify the prior/new governing rules,source editions,rationale,affected owners/consumers and actual required dependencies.
2. Assess compatibility,mandatory-field/State/Canonical Reference effects,record populations,canonical representation/aliases and reference targets; retain unresolved peer claims visibly.
3. Record exact old→new mappings,collision/reservation/history checks,same-document continuity and relevant exact-edition/snapshot contexts. Preserve old evidence and never retarget immutable historical snapshot members or reassign retired IDs.
4. Establish transition verification and coordinated propagation before claiming integrated conformance. A local source update does not approve peers or execute migration.

For changed working document editions,compatible correction retains Version,compatible additive capability increments minor,incompatible contract change increments major and resets minor to0. Each persisted changed edition increments Revision monotonically across Versions. Unchanged-source validation changes neither coordinate and is recorded centrally. Those documentary coordinates do not define all other entities' allocation/lifecycle.

DID-014 §14's received additive/backward-compatible-only extension rule remains a real peer contract requiring scheduled reconciliation with the controlled-evolution approach;it is not silently waived by this source. No blanket permission to mutate assigned identity is introduced. This UPDATE executes no allocation,series registration,alias or migration.

---

# 12. Dependencies

The four original documentary dependencies remain:

- [DF-DID-001 — Document Identity Architecture](../01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md): scoped domain/assignment,preservation and component boundaries.
- [DF-DID-002 — Document Identity Concepts](../01-Architecture/DF-DID-002%20-%20Document%20Identity%20Concepts.md): logical document,key,representation,reference and descriptor distinctions.
- [DF-DID-003 — Document Identity Model](../01-Architecture/DF-DID-003%20-%20Document%20Identity%20Model.md): qualified entities and selected cardinality0..N.
- [DF-DID-004 — Document Identity Elements](../01-Architecture/DF-DID-004%20-%20Document%20Identity%20Elements.md): elements,state/reference roles,constraints and ownership boundaries.

Consult [Lifecycle](../03-Behavior/DF-DID-006%20-%20Document%20Identity%20Lifecycle.md),[Relationships](DF-DID-009%20-%20Document%20Identity%20Relationships.md),[Constraints](DF-DID-010%20-%20Document%20Identity%20Constraints.md) and [Specification](../04-Reference/DF-DID-014%20-%20Document%20Identity%20Specification.md) for actual responsible peer requirements and unresolved integration. Those links are source-contract references,not a runtime call order or completed peer approval. The [functional DID README](../README.md) retains the actual Metadata dependency declaration for comparison,not a normalized ID allocation.

Required contract interpretation and allocations follow [Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md) and [Components](../../../01-Architecture/DF-ARC-005-ArchitecturalComponents.md);descriptive roles are compared with [Metadata Model](../../Metadata/01-Architecture/DF-MTD-003-MetadataModel.md),without claiming complete Metadata owner consistency. Working classification,identity,edition,authorship and evidence follow [Review Policy](../../../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md);actual operations and limits are in [Review Report](../../../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md).

---

# 13. Summary

The schema retains the three original logical roles and their1/1/0..N cardinalities with explicit assigned-subject,qualified-key and connection-ownership boundaries. The two selected views organize meaning without imposing physical storage or claiming a fully reconciled identity record.

Requirements support scoped checks;they do not by themselves establish implementation,universal uniqueness/resolution,complete peer consistency or approval. State/Canonical Reference,extension and reciprocal required-contract integration remain explicit owner work. Exact-source VALIDATE DOCUMENT of this successor is pending.

---

# 14. Edition History and Integration Limits

## 14.1. Received provenance

Received V1.0 R0:Family Documentation,Type Structure,Component Document Identity,Author Arnaldo Figueira,Status Canonical,Baseline1.0,English;original date absent. These are received declarations,not evidence of formal approval,publication or actual successor Baseline inclusion. Exact original header,all numbered bodies and five fenced blocks remain in external REVIEW/UPDATE evidence.

## 14.2. Working successor and compatibility

| Date | Version | Revision | Contribution | Change / lifecycle |
|---|---|---|---|---|
| 2026-10-15 | 2.0 | 1 | Codex — AI assistant;original Arnaldo Figueira contribution retained | Step4.18 UPDATE;incompatible applicability,representation/record scope,reference ownership,evolution and guarantee correction. Draft;Baseline Not assigned;10 corrections pending VALIDATE DOCUMENT. |

This is not merely a Family relabelling. The successor narrows formerly universal schema/uniqueness claims,distinguishes selected key/association view from mandatory peer records,and replaces unconditional future compatibility with assessed controlled change. It integrates the adopted corpus representation while retaining other-domain qualification. Version1.0→2.0 and Revision0→1 follow Policy§5;Revision is not reset across Version changes. Source ID/path and received1/1/0..N cardinalities remain. Cumulative Author is provenance,not approval or attribution of every event/later-product consequence to every author.

## 14.3. Validation and pending propagation

Ten local corrections remain Corrected—pending validation. No VALIDATE DOCUMENT has yet examined this exact successor. Prior source-local semantic or attribution-only results retain their original edition/hash/coverage;they do not silently validate changed content.

The §6 field matrix and §§10–11 required-dependency/evolution conflicts remain actual peer work,not accepted integrated reconciliation. Full DID-006/009/010/014 and Metadata owner cycles,canonical state/record/representation contracts,reciprocal required-scope/cycle checks and actual executor observations remain pending. No allocation,migration,operational resolver,global conformity,approval,publication or Baseline is created by this UPDATE.

---

**End of Document**
