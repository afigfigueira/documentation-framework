# Documentation Framework

# DF-DID-014 – Document Identity Specification

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-DID-014 |
| **Title** | Document Identity Specification |
| **Family** | Document Identity |
| **Type** | Reference |
| **Component** | Document Identity |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Purpose

This is the working normative specification of Document Identity for its explicitly declared documentary/domain subjects and applicable owner contracts. It consolidates scoped requirements and source roles without replacing every detailed owner definition or claiming an implemented, approved or globally reconciled component.

Two conformance subjects are distinguished. **K — assigned document key** is the governing qualified Domain+Identifier and its same-logical-document association. **R — supporting assigned identity record** represents that assigned subject with the five mandatory roles in §7, including a responsible lifecycle assertion and canonical-target descriptor. K is not a container of every mutable record or connection; R is not a new allocated document identity. Pre-allocation is a separate subject, not an assigned R whose key is absent.

This edition makes an explicit local normative decision about the previously unqualified mandatory-record and evolution clauses; the prior/new map and exact affected peer editions are retained externally and in §§7/14/20. It does not silently delete received State/Canonical Reference requirements or equate them with optional incoming relationships. Detailed serialization, canonical Metadata Element/Profile registration and complete owner/consumer propagation are not fabricated.

Normative authority follows actual applicable source declarations, subject/context and common Architecture/Policy, not Type Reference, a title, citation or received Canonical naming. DID-012 remains non-normative advice; current DID-011 architectural/evolution requirements and DID-013 qualified definitions have their own applicable roles (§§15/17). A local source correction or validation is distinct from implemented conformity, formal approval, publication and exact Baseline inclusion.

---

# 2. Scope

The ten original specification subjects remain, scoped to actual contracts and evidence:

| Received subject | Working scope |
|---|---|
| the architectural purpose of Document Identity | Document-key/domain meaning and required allocation/preservation contracts; actual operations remain separate |
| the conceptual identity model | Assigned K, supporting R and typed owner/record associations rather than every physical file/entity |
| the canonical identity structure | The §7 complete-assigned-record roles distinguished from the stable key and selected peer views |
| the architectural elements composing a Document Identity | Five received subjects retained with actual key/record/assertion/descriptor roles |
| lifecycle behaviour | Pre-allocation and assigned assertions under selected DID-006 transitions and actual decision evidence |
| validation requirements | Exact declared claims, applicable rules, performed checks, observations, coverage and limits |
| governance rules | Documentary contracts/authority and preservation requirements, not an installed engine or permission model |
| architectural relationships | Actual scoped consumer→provider requirements versus semantic ownership, references, projection and execution |
| mandatory constraints | Applicable qualified requirements; no full success from missing/conflicting mandatory evidence |
| extensibility principles | Ordinary compatible extensions versus necessary assessed normative revision under common authority |

The seven received exclusions remain implementation-design boundaries:

- implementation technologies;
- programming languages;
- storage mechanisms;
- databases;
- repository implementations;
- APIs;
- serialization formats.

They do not exempt implementations from legitimate governed logical representation, schema/interface, authorization or evidence requirements. No database/API/adapter, allocation algorithm, runtime resolver or complete DMS/CMS implementation is supplied.

Apply identity requirements to applicable assigned normalized logical documents and actual declared record/operation scopes. Every README.md, CHANGELOG.md and ArchitecturalMilestones.md remains non-normalized at every location. Files, copies, exact editions/Status, metadata/category/template entities, registrations, graph projections and pre-allocation subjects are not automatically new document allocations.

---

# 3. Architectural Overview

Document Identity is the Documentation component owning document-key/domain meaning and applicable allocation, preservation, lifecycle, validation and identity-governance contracts under common Architecture/Policy. Its supporting architectural role does not allocate it to the structural Foundation area or make every component a required consumer.

The component defines contracts; actual allocation, checking, retirement and document-management execution belong to the applicable DMS, tool or manual process, with CMS governing changes in its scope. Real operations need actual authority/decision, exact rules/source editions, subject/domain/artifacts/context, executor, observations and coverage. Naming an owner or generating a string/header is not an allocation, installed engine or permission.

Assigned K shall remain associated with the same logical document under its governing contract; actual uniqueness and preservation claims need assignment, canonicalization, population/collision/reservation/history evidence. R and other supporting records may evolve under responsible rules without reallocating K. A specification requirement is not proof that every actual document or implementation is already conformant.

---

# 4. Architectural Objectives

The six original objectives remain with declared scope and evidence limits.

| Objective | Qualified requirement / objective boundary |
|---|---|
| uniquely identify every document | Applicable assigned normalized logical-document/domain subjects; actual qualification/allocation/population/history, not every file or entity |
| preserve permanent document identity | Preserve assigned same-document association, non-reuse, reservations and intended historical recognition |
| ensure long-term traceability | Retain actual assignment/record/edition/reference/decision provenance and coverage; no perpetual content availability promise |
| provide canonical document references | Intended qualified document/exact-edition/context descriptors and actual reference observations, not a universal resolver |
| support interoperability between framework components | Actual compatible owner/provider/consumer interfaces and transition evidence; no completed global rollout inferred |
| maintain architectural independence from implementation technologies | Logical owner meaning versus actual representations/adapters/executors and applicable evidence obligations |

Objectives do not create allocation history, mandatory Metadata catalog entries, permissions, approval or Baseline selection.

---

# 5. Core Principles

All six original principle headings remain. Apply them to the stated K/R/operation subject and responsible contracts; they do not freeze every support record, allocate new AP identifiers or override common architectural evolution rules.

---

## 5.1. Permanence

Preserve the assigned K association with the same logical document, together with allocated/retired reservations and intended historical recognition under its governing contract. Retirement ends active use in its actual scope without releasing K for another document. Permanence is not proof of complete history, validity of every connection or perpetual live retrieval.

---

## 5.2. Immutability

Assigned K and its same-document association remain unchanged through ordinary content, classification, representation, repository and documentary edition/Status evolution. State, reference/descriptor, registration and graph records can change under their own responsible contracts. Necessary governing normative/domain/representation revision first requires §14 previous/new authority, owner/consumer/interfaces, mappings/history and reference/exact-snapshot continuity; no arbitrary reassignment or historical retargeting is permitted.

---

## 5.3. Uniqueness

An applicable assigned normalized logical document has one governing identity under its declared document/domain contract. Different logical documents shall not receive a conflicting full qualified K within that governing allocation/canonicalization scope. Actual assignments, intended subjects, aliases, population and current/historical collision/reservation coverage substantiate the claim.

Copies, legitimate aliases, editions, repeated registrations/projections or equal numeric suffixes across different registered series do not alone constitute competing allocations. A gap, missing record or matching syntax establishes neither availability nor complete uniqueness.

---

## 5.4. Stability

Ordinary document evolution preserves K while actual records, exact editions, interfaces, targets and freshness can be affected and require assessment. Current Family/Type/Component/title/path/format/Version/Revision/Status does not reconstruct the stable allocated key. Stability is not a guarantee of harmless movement, unchanged every-record bytes or successful future consumers. Necessary contract revision follows §14 with explicit prior/new interpretation and transition evidence.

---

## 5.5. Canonical Representation

Each assigned K has one governing canonical identifier interpretation/representation under its domain rules, distinguished from the logical document and legitimate mapped aliases. An unqualified rendering is not universally unique across domains or a guaranteed working resolver.

For this corpus the domain is Documentation Framework, represented by DF. DF-SSS-NNN uses a registered uppercase three-letter stable allocation series and a positive three-digit 001–999 number. 000 is not allocated; allocated/retired numbers are not reused; gaps prove no availability. At 999, register a traceable unused continuation series rather than widen syntax or recycle. A recorded historical series purpose does not mandate renumbering after classification changes. Other domains need their own explicit contracts. This UPDATE allocates no key, series or alias.

---

## 5.6. Technology Independence

Document-key/domain semantics are distinct from technology choices. Actual representations, canonical formats, logical schemas/interfaces and justified integration constraints remain governed requirements, not prohibited by independence. Implementations retain actual source/input/output editions/bytes, mappings, contributors/authority, checks and observed limits; an adapter neither owns identity meaning nor proves complete interoperability.

---

# 6. Conceptual Model

The received conceptual view's five labels remain, with typed key/record/assertion/descriptor roles rather than untyped composition or runtime dependencies. Exact original text/digest is external evidence at this original section; no historical view identifier is invented.

<!-- original-section-view: 6 -->
**Previously unnamed view in §6 — Assigned subject and supporting identity-record roles.**

| Original label | Working subject / typed relation | Scope and authority |
|---|---|---|
| Document Identity | Logical assigned subject K represented by R | Not a recursively embedded key or new document allocated for the record |
| Identifier | Canonical representation/interpretation of K under its governing domain | One qualified assigned-key meaning; legitimate aliases retain responsible mappings |
| Identity Domain | Governing qualification/allocation/preservation contract for K | Domain+Identifier interprets K; domain label alone proves no actual uniqueness |
| Identity State | Mandatory R lifecycle assertion about the assigned subject in §7 | Mutable supporting assertion with actual event/decision/provenance, not a key coordinate or document Status |
| Canonical Reference | Mandatory R canonical-target descriptor in §7 | Intended qualified document/exact-edition/context; not an incoming Relationships connection or guaranteed URL |
<!-- end-original-section-view -->

Received Document Identity→Identifier/Domain/State arrows are qualified logical roles, not mandatory storage pointers, ownership transfer or required service edges. Received Identifier→Canonical Reference depicts canonical rendering/target interpretation, not a rule that a reference is part of the immutable identifier string or that every target needs an incoming edge. The exact original arrow text remains in maps; mandatory R scope is explicit in §7, not silently removed by drawing a different view.

---

# 7. Canonical Elements

The five received rows remain mandatory for a **complete supporting assigned identity record R** claimed under this V2.0 R1 working specification. This is an explicit correction of the received unqualified every-identity composition: it separates the logical assigned key K from supporting record/assertion/descriptor roles. It does not make State or Canonical Reference optional to pass a complete-R claim, nor add them as immutable coordinates of K.

| Element | Qualified description / subject | Mandatory for complete assigned R |
|---|---|---|
| Document Identity | Intended assigned logical document K and same-document association represented by this record; not a second allocated identity or required recursive object field | Yes |
| Identifier | Canonical identifier interpretation/representation qualifying the intended K under responsible rules | Yes |
| Identity Domain | Governing semantic/allocation/preservation scope qualifying K | Yes |
| Identity State | Supporting actual lifecycle assertion for the assigned subject, mapped to Lifecycle State in §8 with responsible event/decision/source evidence | Yes |
| Canonical Reference | Supporting descriptor identifying the intended canonical qualified document target, or declared exact edition with required coordinates/bytes/context; it may reuse governed key rendering without an additional runtime locator | Yes |

**State role.** Identity State and Lifecycle State are controlled names for the same R assertion role here, not universal aliases for Metadata State or document Status. In assigned-R scope, Assigned, Preserved or Retired is interpreted under actual DID-006 subject/event/decision rules and its selected eight-transition contract. Unassigned denotes pre-allocation and is not an assigned R with a nonexistent K. No global permission graph or undocumented edge is granted. Supporting assertion records can change while K remains stable.

**Canonical-target role.** Canonical Reference states the intended target/interpretation and applicable source/context evidence; it is not a promised permanently available URL or a new independent identity allocation. It can concern K as a logical document, or an explicitly selected edition with additional context. A complete R needs this descriptor role, but it does not require an incoming Relationships record: external incoming document-reference population remains0..N under DID-003/005. Descriptor presence, connection validity and observed retrieval are separate checks; a historical intended target can remain interpretable while live content is unavailable. Never silently create/retarget K or immutable snapshot members.

A consumer checking only K can report that narrower coverage; it cannot call a missing-State/Canonical-Reference record a fully conformant R or infer full implementation conformance. Conversely, a pre-allocation or non-document subject is not an invalid assigned R merely because it is outside that declared claim. Full conformance needs explicit applicable subject/rule inventory (§§15/18), actual checks and unresolved-authority limits.

No implementation claiming complete R may remove an applicable mandatory role. These are logical record responsibilities, not a newly registered Metadata Element/Profile, prescribed serialization, actual populated record or approved merged implementation schema. The current working contract uses existing DID-006 assertion and DID-009/013 document-target meanings; it does not manufacture missing canonical catalogs or imply peer rollout.

**Prior/new authority and affected sources.** V1.0 R0 §§6–8 declared universal composition/mandatory State/Canonical Reference without these subjects. V2.0 R1 retains all five Yes requirements but qualifies complete assigned-R scope, Identity State↔Lifecycle State and canonical descriptor versus incoming association. DID-003/004/005/006/013 and affected consumers require comparison/propagation at their exact recorded editions. DID-005§6's selected key/association view is not silently overwritten or a waiver of R obligations. Their prior references and unresolved-field notes remain historical/current source evidence until a separately traced update qualifies them. This local decision is explicit; full owner-source agreement, canonical field registration and implementation transition are not certified.

---

# 8. Canonical Schema

The second received view retains its five labels and logical organization, with explicit subjects. It does not prescribe a runtime object layout, serialization or complete Metadata schema.

<!-- original-section-view: 8 -->
**Previously unnamed view in §8 — Assigned identity-record roles versus stable key.**

| Original schema label | Typed interpretation | Working relationship / limit |
|---|---|---|
| Document Identity | Assigned logical subject K represented by supporting R | The record is about the same document, not another allocation |
| Identifier | Canonical representation role qualifying K | Interpreted with Identity Domain; not all mutable record contents |
| Identity Domain | Governing domain role qualifying K | Responsible domain/canonicalization/allocation/reservation evidence required |
| Lifecycle State | Mandatory R supporting lifecycle assertion | Controlled §7 name for Identity State in this record scope; not document Status or nonexistent assigned key in Unassigned |
| Canonical Reference | Mandatory R canonical-target descriptor | Qualified target/edition/context responsibility, not optional incoming0..N association, immutable key field or live resolver guarantee |
<!-- end-original-section-view -->

K has governing Domain+Identifier meaning; R has the five mandatory roles of §7. The received tree's parent/child lines express this qualified logical organization, not universal physical field containment, event order or required consumer edges. Complete-R mandatory roles remain; the selected DID-005 key/association schema and detailed record/field owners keep their scoped responsibilities. Actual additional representation/profile rules, field definitions/values, authority and consumer compatibility require their own evidence. No accepted complete framework-wide schema or populated record is inferred from this view.

---

# 9. Lifecycle Specification

The received four-label overview is retained as a subject/assertion view, not an exhaustive transition graph or operational permission pipeline.

<!-- original-section-view: 9 -->
**Previously unnamed view in §9 — Lifecycle subjects and actual assertion evidence.**

| Original label | Subject / meaning | Evidence / limit |
|---|---|---|
| Unassigned | Applicable documentary pre-allocation subject | No assigned K or complete assigned R is presumed; allocation needs an actual responsible decision |
| Assigned | Evidenced qualified K association with intended logical document | Actual allocation/association rules, collision/reservation/history and resulting assertion |
| Preserved | Evidenced continuing same-document association through qualifying evolution | Supporting records may change; actual event/context and selected transitions govern |
| Retired | Evidenced end of active use in its declared scope | Same-document history and reserved K retained; no reuse or perpetual content availability |
<!-- end-original-section-view -->

Compare the eight selected current DID-006§7 rows, including the five Preserved self-loops omitted from the received overview:

| Current State | Event | Next State | Actual applicability / evidence |
|---|---|---|---|
| Unassigned | Identity Assignment | Assigned | Pre-allocation subject; responsible allocation/association decision and actual collision/reservation/history checks |
| Assigned | Document Evolution | Preserved | Actual qualifying evolution with continuing same-document assignment evidence |
| Preserved | Content Revision | Preserved | Qualifying content evolution; exact edition/context and preserved K |
| Preserved | Metadata Update | Preserved | Metadata Evolution alias in its actual subject/context; descriptor owner retained |
| Preserved | Classification Update | Preserved | Classification Evolution alias; changed categories do not reconstruct allocated key |
| Preserved | Repository Migration | Preserved | Actual movement/context and preserved K; references/index freshness separately assessed |
| Preserved | Governance Transition | Preserved | Governance Evolution alias; actual process/state evidence, not automatic snapshot/key change |
| Preserved | Identity Retirement | Retired | Actual responsible retirement scope/decision, same-document history/reservation retained |

These selected rows are not proof of real permission or successful execution. No unlisted edge is granted by implication; a real case not covered, including direct Assigned retirement without qualifying prior evolution, needs an explicit responsible owner decision/change with impact/evidence assessment rather than event relabelling. Retired has no outgoing edge in this selected scope; that does not define every external contract. Maintaining an unchanged assertion without an event is not automatically a new self-loop.

Document-edition Draft/Review/Approved/Published/Archived/Obsolete/Deleted statuses and identity assertions are different subjects. Status, file/edition/index deletion, archiving or unavailable content does not by itself allocate or retire K, grant a missing edge or select a Baseline. Actual State/Canonical Reference record semantics are §7's local working decision with remaining owner/consumer propagation, not a claim of complete implementation/lifecycle authority across all sources. Preserve immutable historical exact editions and selected relationship context; Draft successors inherit no approval/membership.

---

# 10. Validation Requirements

The six received validation subjects remain. For any claim, identify K/R/operation/domain scope, exact artifacts/editions/bytes/context, actual applicable mandatory rules/source editions/interfaces, executor/method, performed/unperformed checks, observations, population/coverage and limits. Requirements are not evidence that checks ran.

| Validation subject | Qualified requirement / evidence |
|---|---|
| structural validity | Applicable K representation or complete R roles, actual governing rules and subject; no universal record format assumed |
| uniqueness | Full qualified assignments/canonicalization/population/collision/reservation/history coverage, not syntax or partial index alone |
| completeness | Every applicable mandatory role for the declared R/other claim; selected K-only success does not waive State/Canonical Reference |
| integrity | Actual responsible association/provenance/authenticity rules and observations; no invented security mechanism or automatic guarantee |
| consistency | Exact subject/source/context meanings and records; legitimate edition/history differences distinguished from actual conflicts |
| reference validity | Actual typed intended qualified document/exact-edition/context, canonical descriptor and connection/resolution observations; no perpetual live guarantee |

DID-007 distinguishes Valid, Invalid, Inconsistent and Unresolvable observations. An actual violation requires applicable rule/context and observed nonconformance. Missing/unperformed/conflicting mandatory evidence withholds broader success without fabricating Invalid/Unresolvable. Preserve all supported negative observations and coverage limits rather than suppressing them through a silent precedence rule. A successful subset is narrower evidence, not full R, component or framework Valid.

Actual §7 working requirements do not complete every peer field/profile/interface decision or implementation rollout. Where applicable responsible authority remains conflicting, retain it and withhold the broader claim until reconciliation; do not silently waive mandatory roles or invent accepted field instances. Evaluation, writing a result record and separately authorized remediation are distinct. A result grants no mutation/allocation/approval/publication/Baseline selection; changed artifacts/rules/context need their own assessment.

---

# 11. Governance Requirements

All six original governance subjects remain under common governing architecture and actual domain contracts.

| Governance subject | Qualified obligation / authority boundary |
|---|---|
| permanence | Preserve assigned same-document association, reservations/history and intended recognition; not perpetual retrieval |
| uniqueness | Actual governing qualification, allocation/canonical interpretation, collision/reservation/history evidence |
| immutability | Stable K through ordinary evolution versus mutable supporting records; necessary governing change follows §14 |
| traceability | Actual assignment/decision/change/reference/edition provenance, observations, coverage and limits |
| canonical ownership | Document-key meaning with Document Identity; other descriptor/category/connection/registration/projection owners remain |
| architectural consistency | Applicable exact common/owner contracts and scoped observed checks, with unresolved authority/interfaces visible |

Governance is Workflow, Policies, Reviews and Baselines documentary contracts, not one operational owner/engine. Actual DMS/tool/manual execution and CMS change scope require real authority/rules, exact subject/edition/context, decision/executor and observations. Authorship, custody, a normative statement or local PASS alone grants no operational permission.

Ordinary governance operations do not silently redefine identity meaning. Necessary assessed normative revision under common AP-015–018 is distinct from arbitrary override; §14 specifies prior/new authority, owner/consumer/interface, compatibility/version and continuity evidence. Baselines requires exact eligible approved-edition selection and relevant pinned relationship context or traceable verification evidence. Logical identity, R completeness, review or validation alone neither approves/publishes a Draft successor nor selects its membership or retargets historical snapshots.

---

# 12. Relationship Specification

All nine received subjects remain with actual semantic/record and area/component roles. Required dependencies mean consumer→provider with explicit contract/scope, source editions and interfaces; documentary authority reference, semantic association, projection, navigation and execution are different relations.

| Original subject | Kind | Qualified relationship / owner boundary |
|---|---|---|
| Metadata | Component | Descriptor/model/schema/profile/instance owner; Metadata→Document Identity for identity of the applicable normalized document described; reciprocal requirement below remains |
| Classification | Component | Category/assignment owner; applicable classified-document key consumption does not allocate DF IDs to every category/entity |
| Templates | Component | Template definition/instance contracts; applicable normalized Template-document key consumption differs from every template entity/output |
| Registry | Component | Registration/index owner; intended qualified key/edition/context and source/freshness evidence; registration is not allocation or a mandatory intermediary |
| Relationships | Component | Typed connection/endpoint/provenance owner; document endpoints consume identity meanings, other endpoint kinds retain theirs |
| Knowledge Graph | Component | Logical node/edge projection/properties with authoritative identity/connection source/context and refresh limits; no competing authority or complete graph proof |
| Governance | Area | Workflow, Policies, Reviews and Baselines documentary contracts; actual management/decision executor and CMS scope separate |
| Automation | Area | Validation, Metadata Generator, Registry Generator, Documentation Generator and Consistency Verification capabilities; actual input/output/rule/observation/executor evidence |
| Integration | Area | Source Control Integration, CI/CD Integration, IDE Integration, Documentation Platform Integration and AI Integration optional adapters; actual authorization/mappings/contributors/checks required |

The functional DID README states: “The Document Identity component depends on the Metadata component for the canonical definition of metadata concepts used to describe document identity.” Current DID-009§5.1.1/§10 retains Document Identity→Metadata alongside Metadata→Document Identity. Preserve both actual required declarations pending responsible core-versus-descriptor/interface/source-edition reconciliation. Different scope names, projection or navigation relabelling do not dissolve a genuine required cycle.

The received all-relationships-unidirectional-towards-Identity claim is replaced, not accepted as the current general rule. Ownership/authority and typed association are not required edges; actual indispensable providers remain required even through projections. Apply ARC-004/005 support order and same-Layer explicit-interface/cycle rules; these do not require every earlier provider or a serial pipeline. No complete globally acyclic graph or integrated consumer compatibility is certified. Repeated descriptors, aliases, copies/editions and projection records are not alone duplicate allocations or semantic ownership transfer.

---

# 13. Constraint Specification

The eight original constraint subjects remain with explicit K/R/operation applicability and actual responsible rules.

| Constraint subject | Qualified requirement |
|---|---|
| exactly one identity per document | One governing assigned identity for the applicable normalized logical document/domain contract; functional/pre-allocation/other entity scope differs |
| exactly one canonical identifier | One responsible canonical interpretation for assigned K under its domain, with legitimate traceable aliases distinguished |
| immutable identity | Assigned K/same-document association stable through ordinary evolution; supporting records can change; necessary governing revision follows §14 |
| permanent identity | Preserve historical same-document association/reservations; no perpetual content-retrieval guarantee |
| unique identity | Actual qualified assignments/canonicalization and collision/reservation/population/history coverage, not syntax/index-only success |
| non-reusable identity | No allocated/retired K assigned to another logical document; gaps or unavailable content do not establish availability |
| technology independence | Logical semantic separation with legitimate representation/interface/integration and evidence obligations |
| repository independence | Location/custody/index changes do not reconstruct K; actual target/freshness/consumer/history effects assessed |

DID-010 owns the detailed applicable constraint subjects; this consolidation does not silently rewrite all peers or turn a missing record into an observed violation. Establish actual mandatory rule/subject/context and observed nonconformance before claiming failure. Full success needs all applicable mandatory requirements/authority/evidence for its declared scope; narrower observations retain their limits. No automatic repair, allocation or permission is supplied.

---

# 14. Extensibility Specification

**Current V2.0 R1 decision.** Ordinary compatible implementation extensions preserve applicable owner meanings, mandatory requirements and assigned same-document continuity. Necessary normative/foundational/responsibility/interface revision is permitted only through actual assessed common Architecture AP-015–018 and responsible change authority; it is not falsely labelled compatible merely because it is called an extension.

All five received extension subjects remain:

| Original condition | Current qualified application |
|---|---|
| preserve backward compatibility | Preserve compatible meaning where feasible for ordinary extension; necessary incompatibility requires explicit actual prior/new authority/rationale/consumer and transition evidence |
| preserve canonical identity semantics | Ordinary implementations do not silently replace owner meaning; necessary normative revision is separately assessed, not an arbitrary key reassignment |
| preserve interoperability | Evaluate actual provider/consumer/adapter/source editions and transition checks; no completed global rollout inferred |
| preserve mandatory constraints | Ordinary additions do not waive applicable requirements; necessary normative changes explicitly identify old/new mandates, authority, compatibility and affected exact sources before propagation |
| remain additive | Prefer additive compatible change when it meets the actual need; not an absolute prohibition on necessary justified normative revision |

**Received restriction and affected sources.** V1.0 R0 required every extension to be additive/backward-compatible and stated “Core identity semantics are not extensible.” That exact prior claim remains in original/map/diff/history evidence. This V2.0 R1 replaces this specification's absolute extension-only prohibition with the scoped ordinary-extension/necessary-revision contract above under common architecture. It does not leave the old absolute clause simultaneously governing the same current operation, silently rewrite the past or grant arbitrary mutation of an assigned K.

DID-005§11, DID-010§12, DID-011§§4.2/9 and DID-013§9 currently cite that received restrictive claim or its unresolved authority. Their exact current bytes/editions/hashes are in the affected-source map. They are not edited or automatically revalidated here; their prior-source references and pending notes must be qualified through a separately traced propagation step before claiming integrated agreement. Other K/R field/interface and consumer decisions likewise need actual reconciliation. The current local decision and remaining propagation are separate facts.

For any necessary term/mandate/owner/normative/domain/path/representation transition:

1. Preserve original exact artifacts, rules/editions, actual observations and failed checks. Identify prior/new meaning or mandate, actual responsible authority, intended subject/domain/context, need, alternatives and rationale.
2. Assess exact semantic/record owners, consumers and indispensable consumer→provider interfaces, mandatory field/state/reference/lifecycle effects and actual reciprocal/cycle claims. Resolve governing authority for the actual operation before asserting broader conformity; do not rename away a real required edge.
3. Record compatibility and exact old→new role/term/key/alias mappings, domain qualification, collisions/reservations/history, same-document continuity and intended reference/exact-edition/pinned-snapshot effects. Never reassign allocated/retired K to another document or silently retarget immutable historical members.
4. Apply only the separately authorized scoped change with actual contributor/event provenance, coordinated transition evidence and working edition/history. Compatible correction retains Version; compatible additive capability increments minor; incompatible contract/convention change increments major and resets minor to0. Every persisted changed document edition increments Revision monotonically across Versions; other entity allocation/lifecycle contracts remain separate.
5. Validate resulting exact artifacts/editions in the subsequent appropriate operation, recording actual checks/executor/observations/coverage/remaining peer work. Unchanged-source validation increments neither source coordinate; later changed bytes need their own assessment. Preserve earlier pending/failed events rather than rewriting them as historical success.

This UPDATE changes documentary requirements only. It executes no identity/domain migration, owner transfer, allocation, retirement, implementation rollout, formal approval, publication or Baseline selection.

---

# 15. Compliance Requirements

Conformance is a declared actual claim, not a property inferred from specification presence or a list of citations. Identify implementation/record/population scope, K/R/operation subjects/domain, exact artifacts/editions/bytes/context, applicable responsible mandatory clauses/source editions/interfaces, authority/executor, performed/unperformed checks, observations, coverage and limits before deciding the result.

The ten original owner-source subjects remain, with applicability governed by their exact responsible clauses (§17). Their requirements are not all interchangeable universal rules for every entity/context. A complete supporting-R claim retains all five §7 roles; K-only or pre-allocation observations do not imply full R/implementation conformity. Implementation conformance here includes every applicable current specification requirement and actual applicable independent owner requirements, not just a convenient subset.

- [DF-DID-001 — Document Identity Architecture](../01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md)
- [DF-DID-002 — Document Identity Concepts](../01-Architecture/DF-DID-002%20-%20Document%20Identity%20Concepts.md)
- [DF-DID-003 — Document Identity Model](../01-Architecture/DF-DID-003%20-%20Document%20Identity%20Model.md)
- [DF-DID-004 — Document Identity Elements](../01-Architecture/DF-DID-004%20-%20Document%20Identity%20Elements.md)
- [DF-DID-005 — Document Identity Schema](../02-Structure/DF-DID-005%20-%20Document%20Identity%20Schema.md)
- [DF-DID-006 — Document Identity Lifecycle](../03-Behavior/DF-DID-006%20-%20Document%20Identity%20Lifecycle.md)
- [DF-DID-007 — Document Identity Validation](../03-Behavior/DF-DID-007%20-%20Document%20Identity%20Validation.md)
- [DF-DID-008 — Document Identity Governance](../03-Behavior/DF-DID-008%20-%20Document%20Identity%20Governance.md)
- [DF-DID-009 — Document Identity Relationships](../02-Structure/DF-DID-009%20-%20Document%20Identity%20Relationships.md)
- [DF-DID-010 — Document Identity Constraints.](../02-Structure/DF-DID-010%20-%20Document%20Identity%20Constraints.md)

The two received recommended source subjects also remain, with their actual current roles made explicit:

| Received subject | Current authority / limit |
|---|---|
| DF-DID-011 — Document Identity Extensibility | Current architectural/evolution requirements and ordinary-extension/necessary-revision protocol apply in their declared scope; not merely recommendations because received §15 grouped it there |
| DF-DID-012 — Document Identity Best Practices | Explicit non-normative recommendations; this citation does not promote the whole advice document into mandatory implementation requirements or waive independent owner rules |

DF-DID-013 supplies explicit scoped component-normative vocabulary, and common Foundation/Architecture sources retain their applicable roles in §17. An authority/reference list is not a new claim that every historical rationale sentence or recommended practice is mandatory. Specific adopted requirements need their own actual applicable declaration and subject, not implicit promotion by title/Type.

Use DID-007 outcome/coverage meanings. Actual negative observations require actual responsible rules/subjects/context; missing/unperformed/conflicting mandatory authority or evidence withholds broader success without fabricated failure. Preserve all supported negatives, omissions and narrower observations. §7/§14 make current local subject/mandate/evolution decisions, but full peer/source agreement, missing canonical catalog/interface decisions and actual implementation transition are not certified; resolve applicable conflicts before a broader conformance claim.

Neither exact logical identity, working Version/Status, a normative declaration nor local document PASS establishes operational permission, formal architecture/document approval, publication or exact eligible approved-edition/pinned-context Baseline selection. Prior results stay with their exact bytes/editions/coverage. Initial REV2-09/10 and other global findings keep independent closure criteria; this source-local correction closes none automatically.

---

# 16. Architectural Conformance

All ten original characteristic subjects and received Mandatory designation remain for actual applicable conformance claims, with explicit subject/evidence boundaries rather than implemented guarantees.

| Characteristic | Requirement | Applicable subject / evidence boundary |
|---|---|---|
| Uniqueness | Mandatory | Actual qualified K assignments/canonicalization/population/collision/reservation/history coverage |
| Permanence | Mandatory | Same-document association, non-reuse/reservations and intended historical recognition |
| Immutability | Mandatory | Ordinary assigned K preservation distinguished from mutable supporting records and necessary assessed normative change |
| Stability | Mandatory | Actual prior/current meaning, consumer/reference effects and continuity evidence; no harmless-change promise |
| Canonical Representation | Mandatory | Responsible domain interpretation/rendering/alias rules, exact source/context and actual mappings |
| Validation | Mandatory | Applicable actual checks, outcomes/coverage and unresolved conditions; not automatic full Valid or permission |
| Governance | Mandatory | Applicable owner/common requirements, real decision/authority/executor evidence and separate selection/approval facts |
| Technology Independence | Mandatory | Owner meaning distinct from implementation choices, legitimate interfaces/representations and observed adapter compatibility |
| Repository Independence | Mandatory | K not reconstructed from location/custody, actual movement/target/index/freshness/history assessment |
| Implementation Independence | Mandatory | Definitions do not choose a runtime or excuse actual executor/rule/source/input-output/contributor/evidence obligations |

Justify applicability/inapplicability responsibly; do not omit a mandatory requirement to manufacture success. A characteristic label alone proves neither observed compliance nor all-peer authority reconciliation. Actual conformance, implementation evidence, formal approval and Baseline selection remain distinct.

---

# 17. Normative References

The received Normative References heading and all twenty-one source subjects remain. Actual authority is clause/subject/context/edition-specific: the heading does not make every sentence of every listed document mandatory, approve Draft sources or convert recommendations into normative requirements.

Foundation, Architecture and detailed component roles are qualified below. Exact compared paths/metadata/Status/Baseline and SHA-256 at the REVIEW checkpoint are retained externally. Prior semantic versus attribution-only results keep their original scope; a resolved link or current header audit is not a full new peer validation. Working scope, classification, identity, edition, authorship and evidence follow [Review Policy](../../../03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md); actual operations/remaining scope are in [Review Report](../../../03-Governance/Reviews/04-Reference/DF-RVW-002-ReviewReport.md).

The functional DID README retains the actual reciprocal Metadata required declaration as comparison evidence, not a normalized source allocation. Detailed source facts and previous/current authority changes in §§7/14 require separately traced consumer propagation; no full required graph or global integration is inferred.

---

## 17.1. Foundation

All received source subjects remain with their actual scoped role.

| Received source | Actual authority / consultation and evidence role |
|---|---|
| [DF-FND-001 — Framework Manifest](../../../00-Foundation/DF-FND-001-FrameworkManifest.md) | Applicable common framework scope, document/functional distinctions and interpretation contracts; explicit authority rather than approved implementation |
| [DF-FND-004 — Architectural Blueprint](../../../00-Foundation/DF-FND-004-ArchitecturalBlueprint.md) | Applicable common Blueprint owner, identity/edition/governance/Baseline and required-contract basis; exact claims and selected editions govern |
| [DF-FND-006 — Design Rationale](../../../00-Foundation/DF-FND-006-DesignRationale.md) | Historical explanatory design rationale and contextual decisions; not blanket normative force for every historical sentence or a substitute for current responsible contracts |

---

## 17.2. Architecture

All received source subjects remain with their actual scoped role.

| Received source | Actual authority / consultation and evidence role |
|---|---|
| [DF-ARC-002 — Architectural Principles](../../../01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md) | Applicable architectural principle/evolution requirements including necessary assessed incompatible revision under AP-015–018 |
| [DF-ARC-003 — Architectural Concepts](../../../01-Architecture/DF-ARC-003-ArchitecturalConcepts.md) | Common qualified conceptual distinctions and owner summaries; detailed domain meanings retain responsible sources |
| [DF-ARC-004 — Architectural Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md) | Applicable structural allocation, support order, consumer→provider/same-Layer/interface/cycle constraints; no complete graph certification |
| [DF-ARC-005 — Architectural Components](../../../01-Architecture/DF-ARC-005-ArchitecturalComponents.md) | Applicable registered capability/area, owner/executor and selected required-contract boundaries; definitions do not install services |
| [DF-ARC-006 — Terminology](../../../01-Architecture/DF-ARC-006-Terminology.md) | Owner-linked common vocabulary, qualified usage and controlled aliases; no blanket takeover of every domain or new full R2 semantic validation |

---

## 17.3. Document Identity

All received source subjects remain with their actual scoped role.

| Received source | Actual authority / consultation and evidence role |
|---|---|
| [DF-DID-001 — Document Identity Architecture](../01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md) | Applicable assigned document/domain scope, document-key owner and actual consumer/operational boundaries |
| [DF-DID-002 — Document Identity Concepts](../01-Architecture/DF-DID-002%20-%20Document%20Identity%20Concepts.md) | Applicable identity/domain/representation/reference conceptual meanings and assessed evolution boundaries |
| [DF-DID-003 — Document Identity Model](../01-Architecture/DF-DID-003%20-%20Document%20Identity%20Model.md) | Applicable qualified entity/association and reference-cardinality model contracts; selected views not every implementation record |
| [DF-DID-004 — Document Identity Elements](../01-Architecture/DF-DID-004%20-%20Document%20Identity%20Elements.md) | Applicable key/supporting state/reference element and ownership meanings; historical candidate labels are not silently new states |
| [DF-DID-005 — Document Identity Schema](../02-Structure/DF-DID-005%20-%20Document%20Identity%20Schema.md) | Applicable assigned-key/association/corpus representation and evolution contracts; selected view does not waive complete-R roles or imply accepted merged Metadata fields |
| [DF-DID-006 — Document Identity Lifecycle](../03-Behavior/DF-DID-006%20-%20Document%20Identity%20Lifecycle.md) | Applicable pre-allocation/assignment/preservation/retirement subjects, selected eight transitions and actual event/decision limits, not universal permissions |
| [DF-DID-007 — Document Identity Validation](../03-Behavior/DF-DID-007%20-%20Document%20Identity%20Validation.md) | Applicable scoped checks, owner-defined outcome/coverage/reference/nonmutation requirements; not implemented checker success or approval |
| [DF-DID-008 — Document Identity Governance](../03-Behavior/DF-DID-008%20-%20Document%20Identity%20Governance.md) | Applicable identity-governance, operational exclusions, compliance/violation/authority and separately assessed change requirements |
| [DF-DID-009 — Document Identity Relationships](../02-Structure/DF-DID-009%20-%20Document%20Identity%20Relationships.md) | Applicable typed owners/records/endpoints/required consumption and actual reciprocal interface claims, not globally reconciled DAG |
| [DF-DID-010 — Document Identity Constraints](../02-Structure/DF-DID-010%20-%20Document%20Identity%20Constraints.md) | Applicable qualified mandatory constraint and conformance/authority/evolution requirements; actual observations remain separate |
| [DF-DID-011 — Document Identity Extensibility](../03-Behavior/DF-DID-011%20-%20Document%20Identity%20Extensibility.md) | Current applicable architectural/evolution requirements and proposal/evidence/decision protocol; not merely advisory because received §15 called it recommendations |
| [DF-DID-012 — Document Identity Best Practices](DF-DID-012%20-%20Document%20Identity%20Best%20Practices.md) | Explicit non-normative best-practice guidance; no universal mandatory requirement imported by this listing; independent owner rules remain applicable |
| [DF-DID-013 — Document Identity Dictionary](DF-DID-013%20-%20Document%20Identity%20Dictionary.md) | Explicit component-normative vocabulary in qualified owner/domain contexts, aliases/field usage and actual evidence limits; not global glossary authority |

---

# 18. Conformance Statement

An implementation claiming this working specification's conformance shall identify its actual applicable K/R/operation subjects, mandatory clauses/owner authority, exact artifacts/editions/context and complete performed check/observation/coverage evidence as in §§10/15/16. Full claimed implementation conformance includes every applicable current requirement and independently applicable responsible normative owner clause; a narrower K-only or partial check is not a full supporting-R or whole-component result.

No implementation-specific optimization, extension or integration may silently redefine governing meaning, waive applicable mandatory roles, reassign allocated/retired K to another document, fabricate allocation/state/approval facts or retarget immutable historical members. Necessary explicit normative revision follows §14 rather than an absolute ban on all future responsible architecture change.

Where mandatory authority, field/profile/interface meanings, actual required scopes or evidence remain unresolved for the broader claim, retain narrower unambiguous observations and withhold broader conformity pending responsible reconciliation. This working document's local validation would cover its exact corrected bytes/scope, not every implementation, peer rollout, global acyclic graph or formal architecture approval. Approval, publication and Baseline inclusion require separate actual decisions/evidence.

---

# 19. Summary

This working specification retains the original architectural subjects, five mandatory record roles, lifecycle labels, requirements, relationships, characteristic/reference subjects and three views with explicit key/record/authority/evidence boundaries. It defines a current scoped normative contract; it does not claim a complete already-approved merged record catalog, complete owner-source agreement or implemented global conformance.

§7 explicitly distinguishes immutable assigned K from complete supporting assigned R, retaining State and canonical-target descriptor obligations without requiring an incoming relationship. §14 explicitly supersedes this source's received absolute extension-only restriction with ordinary compatible addition versus necessary assessed normative revision. Exact prior/new decisions, affected peer editions and remaining propagation are preserved; old source references are not silently rewritten or treated as already migrated.

Actual reciprocal Metadata/Identity required interfaces, complete owner/consumer graph, canonical field/profile/interface registrations, source propagation and implementation transition remain responsible work with their exact scope. Initial global REV2-09/10 and nineteen global Open findings retain independent criteria; no local operation closes them automatically. Source remains Draft/Baseline Not assigned; its own VALIDATE DOCUMENT has not yet occurred. No allocation, migration, ownership transfer, retirement, runtime service, operational permission, approval, publication or Baseline selection is performed.

---

# 20. Edition History and Pending Integration

## 20.1. Received provenance

Received V1.0 R0: Family Documentation, Type Reference, Component Document Identity, Author Arnaldo Figueira, Status Canonical, Baseline1.0, English; original date absent. Received declarations are evidence, not approval or successor inclusion. All28 original headings/19 chapters, lists/table/source subjects and three original views/text digests are preserved externally with exact before/after maps. No historical view ID, date, source ID or Metadata allocation is invented.

## 20.2. Working successor and compatibility

| Date | Version | Revision | Contribution | Change / lifecycle |
|---|---|---|---|---|
| 2026-10-15 | 2.0 | 1 | Codex — AI assistant; original Arnaldo Figueira contribution retained | Step4.27 UPDATE: incompatible applicability/authority, key-versus-complete-assigned-record mandatory scope, state/reference/lifecycle, extension and conformance correction. Draft; Baseline Not assigned;15 corrections pending VALIDATE DOCUMENT. |

This is an explicit incompatible normative contract/convention correction, not merely Family or reference-link repair. Universal composition becomes assigned K versus complete supporting R with all five mandatory roles retained, State/Lifecycle State contextual equivalence and canonical-target descriptor distinct from incoming0..N. This source's absolute extension-only prohibition is replaced by ordinary compatible extension versus necessary assessed normative revision under common authority, with actual prior/new affected-source propagation. Blanket all-citation authority, one-way relationships and global conformance meanings are scoped to actual owner clauses, typed required edges and observed evidence.

Version1.0→2.0 and Revision0→1 follow Policy§5; Revision remains monotonic across Versions. Type Reference, ID/path, all original heading numbers/titles, mandatory/relationship/characteristic/source subjects and view labels remain. Original constraints/restrictions remain exact historical evidence, not simultaneous contradictory current rules. Cumulative Author records actual contributions, not approval or authorship of every later event by every listed person.

## 20.3. Pending validation, affected peers and limits

Fifteen corrections remain Corrected—pending validation. No VALIDATE DOCUMENT has examined this exact successor. Earlier exact semantic/attribution-only results retain actual source bytes, editions and coverage; changed content inherits no result.

Section7's local K/R mandate decision requires actual field/profile/interface and source/consumer propagation with DID-003/004/005/006/013. Section14's local replacement of the V1.0 R0 restriction requires exact-source qualification in DID-005§11, DID-010§12, DID-011§§4.2/9, DID-013§9 and affected consumers. Those peers retain their current bytes/editions; no unexecuted propagation is logged as complete. Actual reciprocal Metadata/Identity required scopes/interfaces, the full owner/consumer graph and implemented conformity remain pending. Global REV2-09/10 and all nineteen global Open findings keep independent closure evidence.

This UPDATE changes DID-014 and central tracking/evidence only. No source ID/path migration, canonical Metadata Element/Profile population, ownership transfer, actual assignment, retirement, domain/series registration, runtime service, operational permission, formal approval, publication or Baseline selection is performed. Working Draft/unassigned is not architectural acceptance of all remaining integration decisions.

---

**End of Document**
