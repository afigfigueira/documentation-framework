# Documentation Framework

# DF-MTD-001 — Metadata Architecture

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-001 |
| **Title** | Metadata Architecture |
| **Family** | Metadata |
| **Type** | Architecture |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Introduction

Metadata is one of the core architectural components of the Documentation Framework.

It provides the standardized descriptive information required to characterize every document independently of its content.

The Metadata component establishes the architectural foundation upon which document identification, classification, governance, discovery and automation are built.

Metadata does not describe the knowledge contained within a document.

Instead, it describes the document itself as an architectural entity.

**Current governing scope.**

Metadata describes the applicable documentary entity/edition and its context;it does not substitute for the knowledge content itself. Descriptors may be informed by content and evolve with it. Independent semantics does not require physically isolated content or forbid actual bytes/representation evidence. Current normalized-document rules apply only in their declared scope;all files named README.md,CHANGELOG.md or ArchitecturalMilestones.md remain non-normalized functional files with content/reference duties. This is not a universal mandatory header,Profile or complete Instance population claim.

Architecture defines responsibility and interfaces. Metadata has its own Concepts,Element/Value,Model,Dictionary,Schema,Profile/Instance,lifecycle,validation,governance,relationship and constraint contracts. Identity/Classification meanings,common mechanisms and actual authorized execution retain separate owners (sections6–8).

---

# 2. Purpose

The purpose of the Metadata component is to provide a standardized, technology-independent mechanism for describing documents throughout the Documentation Framework.

Metadata enables documents to become self-describing while remaining independent of their physical representation, storage mechanism or implementation technology.

**Current governing scope.**

Technology independence is independence of semantic definitions from a particular tool,storage or serialization. Actual representation,concrete document/edition bytes,Schema/effectiveProfile/Instance,physical/reference/access/history/provider conditions still have to be satisfied for real use. Supporting self-description does not prove every required descriptor is canonically defined,populated,approved or available.

---

# 3. Scope

This document defines the architecture of the Metadata component.

It specifies:

- the architectural purpose of Metadata;
- component responsibilities;
- architectural boundaries;
- architectural dependencies;
- interactions with other components;
- architectural principles governing Metadata.

It does not define:

- Metadata elements;
- Metadata fields;
- Metadata schemas;
- Metadata validation rules;
- implementation details.

These topics are specified in dedicated Metadata documents.

**Current governing scope.**

The included architectural subjects and excluded detailed definitions above remain. This document establishes domain responsibility,operative boundaries and provider contracts;the dedicated Metadata sources own their detailed concepts,fields,schemas,rules and conditions. A scope exclusion here is not a ban on the Metadata component defining those domain contracts in its own documents.

Metadata Concepts defines conceptual meanings;Model defines abstraction/composition;Element/Value distinguishes definition from an assigned documentary value;Dictionary defines authoritative Element information;Schema organizes permitted structure and references;Profile constrains declared use without silently redefining owners;Instance supplies actual values. Current Model7.6/Schema15 require exactly one Profile for an Instance;identify the actual single effective Profile and its governing editions rather than silently making the requirement optional. General cardinality/population/physical-record details and actual canonical Profile/catalog evidence remain genuine owner-source gaps. No field IDs,values or complete accepted Profile are allocated here.

---

# 4. Architectural Position

Metadata belongs to the Documentation Layer of the Documentation Framework.

```text

           Documentation Framework

                Foundation
                    │
                    │
               Architecture
                    │
                    │
           Documentation Layer
                    │
                    │
       ┌─────────────────────────┐
       │        Metadata         │
       └─────────────────────────┘
                    │
                    │
                    ▼

            Document Identity
             Classification
                Templates

```

**Current received-span relation scope.** View4 is actual support/allocation and selected descriptive-service context,not every peer in a higher Layer or a universal required-provider/execution chain.

| Received literal fragment | Actual current typed interpretation |
|---|---|
| Documentation Framework | The framework container,not an additional component or required runtime provider. Its support/allocation/source authority is not an execution stage. |
| Foundation | Common foundational support/authority area. Actual applicable source editions govern;vertical placement does not require every consumer to execute or consume every foundational document. |
| Architecture | Common architectural support/authority area. Actual allocation,ownership/support order/interfaces/cycle constraints remain;this label is not a separate runtime executor. |
| Documentation Layer | Primary allocation area containing Metadata,Document Identity,Classification andTemplates peers. Actual same-Layer required contracts are permitted with explicit scope/interfaces and no genuine required cycles. |
| Metadata | The actual Metadata component/domain definition and representation owner,not every represented semantic owner,common process/record or installed executor. Real provider scopes and unresolved reciprocal claims remain8.1. |
| Document Identity | The actual same-Layer document-key/domain/edition/reference owner. Descriptor provision does not transfer identity meaning;actual Metadata→Identity and reciprocalIdentity→Metadata required claims remain unresolved8.1. |
| Classification | The actual same-Layer category/assignment meaning owner,not a new Layer or automaticMetadata-ownedType field. Actual required representation/reverse represented-meaning scopes retain source authority and cycle assessment8.1. |
| Templates | The actual same-Layer reusable structural-definition owner. Representation can realize Metadata locations under real Schema/effectiveProfile contracts;no universal mandatoryTemplate runtime or ownership of Metadata semantics follows. |


Metadata supplies descriptive contracts to declared consumers,including same-Layer peers. Its place in a planning or allocation view neither changes primary allocation nor proves introduced/installed capabilities,a higher peer Layer or a required execution sequence.

**Current governing scope.**

The received view below is allocation/support and selected service-consumption evidence,not a current complete required-provider graph or an execution order. Metadata,Document Identity,Classification andTemplates remain Documentation peers;being supplied descriptive contracts does not place peers in a higher Layer. Foundation/Architecture support and actual required consumer→provider directions are separately stated8.1. Exact label fragments have individual scope maps;no component or Layer is created by this drawing.

---

# 5. Architectural Purpose

The Metadata component provides standardized descriptive information that characterizes documents independently of their content.

Metadata enables every document to become:

- self-describing;
- uniquely identifiable;
- semantically classifiable;
- governable;
- discoverable;
- traceable;
- automatable.

Metadata does not replace document content.

Instead, it complements document content by providing architectural information about the document itself.

**Current governing scope.**

All seven capability concerns remain intended responsibilities,not observed implementation results. Identity establishes qualified documentK/localR/exact-edition/reference meaning;Metadata represents descriptors under its actual owners. A MetadataElement permanent architectural identity underMTD00415 is not automatically a normalizedDF document key. Classification owns applicable category/assignment meaning;Metadata representation does not allocate categories or perform assignments.

Self-describing,discoverable,governable,traceable andautomatable require actual subject/source editions,applicability,authority,evidence and mandatory coverage for real claims. This source performs no registration,live lookup,evaluation,decision,condition fulfillment,adoption,operation or installed runtime.

---

# 6. Responsibilities

The Metadata component is responsible for:

- describing documents through standardized Metadata;
- providing descriptive information for architectural components;
- supporting document identification;
- supporting document classification;
- supporting governance processes;
- supporting discovery mechanisms;
- supporting architectural traceability;
- supporting automation activities.

Metadata shall not perform responsibilities assigned to other architectural components.

**Current governing scope.**

The eight support responsibilities remain. Metadata shall define its own domain concepts/model/Element-Value/Dictionary/Schema/Profile/Instance and lifecycle/validation/governance/relationship/constraint conditions. This does not duplicate common mechanisms or transfer other components' semantic authority. Operative exclusions7 distinguish actual domain rules,shared processes/records/projections/capabilities and authorized execution.

For applicable normalized documents,current Family is canonical component/admitted documentary-area membership,primaryType is exactly one ofArchitecture/Structure/Behavior/Reference,andClass is optional but requires an explicit nonconflicting definition if used. Classification/common governing sources retain those meanings;Metadata owns their descriptive representation and broader unrelated concepts. This is not a new field catalog or a claim the received source defined an old Family-ownedType hierarchy.

---

# 7. Non-Responsibilities

The following operative exclusions distinguish Metadata-domain contracts from common mechanisms and actual execution. The Metadata component shall not:

- allocate or assign document identities as an operational act,or redefine Document Identity allocation/preservation contracts;
- replace Classification-owned category or assignment semantics,or perform a classification operation merely by representing descriptor values;
- take over common documentary Workflow,Policies,Reviews or Baselines responsibilities merely because it defines Metadata-domain lifecycle and governance contracts;
- take over common document registration,indexing or discovery operations through its Dictionary or descriptive records;
- take over common typed connection-record/provenance mechanisms or other domains' relationship semantics through Metadata-domain relationship definitions;
- replace the common validation capability or claim an evaluation has executed merely by declaring Metadata-domain rules;
- own operational documentation generation merely through descriptive definitions or output fields;
- stand in for an installed automation system or its authorized executor.

The excluded common mechanisms and operational responsibilities remain with their actual owners and authorized processes. Metadata shall define its own domain lifecycle,validation,governance and relationship contracts without taking over those mechanisms or claiming performed operations.

Metadata provides descriptive concepts,definitions,structure,usage/state/validation/decision conditions and represented values for its domain. It is not restricted to passive values,and it does not thereby own every consuming domain meaning,common record or executor.

**Current governing scope.**

The current operative exclusions above replace blanket bans that would deny Metadata's own Lifecycle,Validation,Governance orRelationships contracts. The following maps retain every received exclusion subject as historical evidence and explain the actual current boundary;the received wording is not a second current governing prohibition.

| Received exclusion subject (historical wording) | Actual current owner and execution boundary |
|---|---|
| assign document identities; | Metadata defines and represents descriptor requirements;Document Identity retains actual document-key/domain meaning and allocation-preservation contracts. Actual authorized processes execute allocation. Permanent Metadata Element identity is a separate domain entity,not automatically a DF document allocation. |
| classify documents; | Classification owns applicable category/assignment meaning;Metadata defines and represents descriptors under its own Schema/effective Profile. Neither a generated field nor a changed Family/Type recalculates document identity. |
| govern document lifecycles; | Metadata defines its own artifact/definition/Schema/Profile/Instance state-use and decision conditions. Common process/rule/review/snapshot mechanisms and actual authority/executor retain their contracts;document Status is not every Metadata artifact state. |
| maintain document registries; | An authoritative Metadata definition/entry catalog is not the common Registry. Registry owns registrations/indexes/projections and source-edition/freshness/access evidence;actual storage/execution remains with implementation. |
| manage relationships; | Metadata defines its own composition/specialization/association/dependency/traceability meanings and represented relations. Relationships retains common typed connections/provenance;actual typed endpoints/kind/assertion/context and required provider edges remain. |
| perform validation; | Metadata defines applicable domain criteria and source/Schema/effective-Profile requirements. The common validation capability and actual authorized tool/manual/DMS/CMS executor evaluate concrete inputs;nonmutating evaluation is distinct from correction,decision and operation. |
| generate documentation; | Metadata supplies actual descriptor/representation contracts;Templates supplies its structural contracts and registered generation capabilities/processes/executors retain operational responsibility. A generated header does not allocate identity,approval or canonical fields. |
| implement automation. | Automation is an architectural area/capability context containing registered components,not a new single Metadata runtime. Actual checking/generation/integration requires concrete source editions,inputs,authority,observations and effects;this source installs or executes none. |

Document Identity retains allocation/preservation contracts and actual authorized allocation execution;Metadata does not rekey from Family/Type/Component/version/location changes. MetadataElement identity,documentK/localR/exact edition,domain decision/record identity and common registration/connection identity remain distinct. No canonical Element/field/Profile or actual operation is generated by describing these contracts.

---

# 8. Architectural Dependencies

**Current governing scope.**

An architectural relation shall identify its kind and actual source/definition edition. Required dependency means indispensable consumer→provider contract in a declared scope;documentary authority,semantic association,data flow,allocation,projection,navigation and execution are separate. A different name cannot remove a real required edge. Exact area allocations and actual cycle rules remain authoritative;the complete accepted graph and detailed provider interfaces are not supplied by this local source.

---

## 8.1. Depends On

Metadata uses Foundation and Architecture as common documentary and structural authorities. Its actual required provider contracts also include the stated same-Layer identity/representation and classification-meaning scopes below;the previous only-Foundation-and-Architecture restriction is replaced by this scoped contract.

Required cross-Layer provider contracts shall respect the actual support order in ARC-004 sections12–13 and ARC-005 section12:Foundation,Architecture,Documentation,Governance,Discovery,Automation,Integration. Same-Layer required contracts shall have explicit owners,scope,source editions and interfaces and shall satisfy the prohibition of genuine required cycles. Representing upper-area meanings or citing authority is not by itself a runtime edge;an indispensable provider shall not be hidden by relabelling it as a reference. Changing a structural constraint requires its own assessed responsible-source revision,not an arbitrary upward exception.

**Current governing scope.**

The following actual current declarations specify their source authority,scope and unresolved interface conditions. They are not complete implementation records.

| Actual consumer → provider | Required contract / actual source | Scope,interface and unresolved condition |
|---|---|---|
| Metadata → Foundation / Architecture; Documentation → earlier support authorities | Actual common concepts,allocation,structural support order and owner/dependency constraints. Documentary authority is not automatically a runtime dependency on every foundational document. DF-ARC-004 V2.0 R2 §12; DF-ARC-005 V2.0 R2 §12 | Identify applicable source/definition editions and real required contract. No universal adjacent Layer chain or all-earlier-provider requirement. |
| Metadata → Document Identity; Documentation → Documentation | Actual document-key/domain/edition/reference meaning for the applicable assigned normalized document being described;DID0095.1.1 explicitly declares Metadata→Document Identity. DF-DID-009 V2.0 R1 §5.1.1; DF-DID-001 V2.0 R2 §9.1; DF-DID-005 V2.0 R1 §9 | Typed documentK/localR/exact edition and intended reference subject;Metadata owns descriptors,not identity meaning. Exact field/record/consumer interfaces and general representation details need actual owner evidence. The reverse claim below remains unresolved. |
| Document Identity → Metadata; Documentation → Documentation | Actual functionalDIDREADME declaration requires canonical Metadata concepts used to describe document identity;DID0019.1 andDID0095.1.1/10 explicitly retain this reciprocal required claim. DF-DID-001 V2.0 R2 §9.1; DF-DID-009 V2.0 R1 §5.1.1; DF-DID-009 V2.0 R1 §10 | Identify indispensable concepts/interfaces for identity core versus descriptive records and actual use. Different scope names alone do not prove independence or dissolve a genuine required cycle. No current accepted cycle-free integration is claimed. |
| Metadata → Classification; Documentation → Documentation | Classification-owned category/assignment/normalized-role meaning where Metadata represents those actual values;ARC0055.1/5.3 and adoptedPolicy3 retain those domain responsibilities. DF-ARC-005 V2.0 R2 §5.1; DF-ARC-005 V2.0 R2 §5.3; DF-RVW-001 V1.0 R2 §3; DF-CLS-001 V2.0 R1 §12 | Applicable Family membership,one uniform Architecture/Structure/Behavior/Reference Type and optional defined nonconflicting Class;not every unrelated field namedType. Exact definition/source edition and assignment context needed,no fabricated field catalog. |
| Classification → Metadata; Documentation → Documentation | Actual CLS00112 required provider declaration where governed Metadata representation is indispensable for document classification in scope. DF-CLS-001 V2.0 R1 §12; DF-CLS-001 V2.0 R1 §20; DF-CLS-001 V2.0 R1 §21 | Category/assignment semantics remain with Classification;Metadata owns Dictionary/Schema/effectiveProfile/Instance representation. Assess actual reciprocal required scopes/interfaces/cycles,not semantic relabelling as an exemption. |
| Templates → Metadata / Document Identity / Classification; Documentation → Documentation | Actual receivedTPL0019.1 consumes established concepts when representing standardized structures. The actual peer declaration is retained;this source does not certify every blanket peer dependency scope. DF-TPL-001 V1.0 R0 §5; DF-TPL-001 V1.0 R0 §7; DF-TPL-001 V1.0 R0 §9.1 | Template entity/instance/output and applicable normalized Template document differ. Metadata→Templates is not asserted as a universal core runtime dependency;any actual use requiring a Template structural contract needs its own real scope/authority/interface and cycle assessment. |
| Registry / Workflow / Baselines / Knowledge Graph → Metadata and other actual scoped owners; Higher support areas → Documentation;other selected same-area contracts retained | Actual ARC00412/ARC00512 include Registry→Metadata descriptors,Workflow→Metadata state/edition,Baselines→Metadata exact-edition context;Graph document nodes needIdentity and typed connections needRelationships. DF-ARC-004 V2.0 R2 §12; DF-ARC-005 V2.0 R2 §12 | Registration/decision/exact-snapshot/projection owners retain source-edition/provenance/freshness/access and real typed endpoint duties. These are selected current declarations,not a complete graph,operational inventory or all-document one-to-one mapping. |

The Metadata↔Document Identity reciprocal required declarations remain unresolved. The Metadata↔Classification represented-meaning and required-representation scopes likewise require actual owner/interface/cycle assessment. Separating core from descriptor use,receiving data through a projection,or calling an edge semantic does not establish independence or acyclicity. Genuine required cycles remain prohibited and must be reconciled by actual responsible contract/allocation revisions;recording a conflict is not permission to operate a prohibited cycle.

Metadata-domain Governance/Lifecycle/Validation/Relationships documents remain Metadata contracts in Documentation,not automatically upper-area runtime components. Documentary process authority and represented state values alone create no required upper-area runtime service. If an actual indispensable upper provider is found,retain the edge and assess the responsible structural/source change;do not evade the support constraint through relabelling. No global DAG certification or integrated rollout follows from this table.

---

## 8.2. Required By

Metadata provides architectural support for:

- Document Identity;
- Classification;
- Workflow;
- Policies;
- Baselines;
- Registry;
- Relationships;
- Knowledge Graph;
- Validation;
- Automation;
- AI Integration.

These components consume Metadata but do not own it.

**Current governing scope.**

All eleven consumer subjects remain. Their actual interface scope is typed below;the list does not make every consumer mandatory for every Instance or transfer its domain authority to Metadata.

| Original consumer | Actual current scope / interface |
|---|---|
| Document Identity | Actual identity-descriptor consumption and reciprocalMetadata→Identity declaration8.1;exact core-versus-record interfaces remain pending. LogicalK/localR/exact edition differs from MetadataElement identity. |
| Classification | Actual Metadata representation provider where indispensable,with Classification-owned meanings and reverse represented-meaning scope8.1. No Family-ownedType tree or owner transfer. |
| Workflow | Common documentary process/transition owner uses represented state/edition values;Metadata own lifecycle conditions and real authority/evidence/operation remain separate. |
| Policies | Common decision/rule mechanism uses descriptors;Metadata owns domain decision conditions,not actual organizational authority or performed approval. |
| Baselines | Exact edition-reference/selection/pinned context provider for actual snapshot duties;no inclusion of a changed Draft from its header or presence. |
| Registry | Descriptor index/registration/projection with actual source-edition/provenance/freshness/access requirements;definition records are not registrations. |
| Relationships | Typed connection/provenance mechanism uses Metadata descriptors;domain relation semantics/endpoints and required providers retain actual owners. |
| Knowledge Graph | Typed entity/connection projections use descriptors and other actual identity/relationship contracts;no full live graph or all-document endpoint assumption. |
| Validation | Common capability and real executor consume actual domain rules/Schema/effectiveProfile/definitions/observations/bytes with coverage/nonmutation duties;not installed by this source. |
| Automation | Area/capability context with actual registered checking/generation/verification owners and authorized executor/effects,not one newly allocated Metadata engine. |
| AI Integration | Actual registered Integration capability may consume Metadata under scoped exchange/reference/authority contracts;no inferred universal final runtime stage or performed reasoning. |

The consumer list includes AI Integration while the original relationship table12 containsTemplates instead;neither list claims a complete one-to-one registry. Their distinct original subjects are preserved rather than inventing a missing-table defect or new component.

---

# 9. Component Interactions

Metadata shall distinguish explicit typed architectural relations from actual required dependencies. A required dependency is a consumer→provider contract needed in its declared scope;allocation,documentary authority,semantic association,representation,projection,navigation and execution are separate meanings. Actual required edges and their unresolved reciprocal claims are retained in section8.1,not inferred or erased from the drawing.

```text

            ┌──────────────────────────────────────────────────────┐
            │                       Metadata                       │
            │                          │                           │
            │       ┌──────────────────┼──────────────────┐        │
            │       │                  │                  │        │
            │       ▼                  ▼                  ▼        │
            │    Document        Classification       Templates    │
            │    Identity                                          │
            │                                                      │
            └──────────────────────────────────────────────────────┘
                                       │
                                       ▼

                             Governance Components
                                       │
                                       ▼

                              Discovery Components
                                       │
                                       ▼

                             Automation Components
                                       │
                                       ▼

                            Integration Components

```

**Current received-span relation scope.** View9 keeps parallel Classification/Templates and split Document Identity as peers;higher-area groups show consumer context,not a complete graph,priority or installed runtime pipeline. Actual required directions/interfaces/reciprocal cycles remain8.1.

| Received literal fragment | Actual current typed interpretation |
|---|---|
| Metadata | The actual Metadata component/domain definition and representation owner,not every represented semantic owner,common process/record or installed executor. Real provider scopes and unresolved reciprocal claims remain8.1. |
| Document | First raw fragment of the split name Document Identity in the received view9. With the next Identity fragment it denotes one registered component,not a separate Document component or every physical/entity endpoint. |
| Classification | The actual same-Layer category/assignment meaning owner,not a new Layer or automaticMetadata-ownedType field. Actual required representation/reverse represented-meaning scopes retain source authority and cycle assessment8.1. |
| Templates | The actual same-Layer reusable structural-definition owner. Representation can realize Metadata locations under real Schema/effectiveProfile contracts;no universal mandatoryTemplate runtime or ownership of Metadata semantics follows. |
| Identity | Second raw fragment of the split name Document Identity in view9,not a distinct component or an automatically allocated MetadataElement. Keep actual identity/descriptor/edition/reference/provider boundaries8.1. |
| Governance Components | Higher support-area consumer group containing actual Workflow,Policies,Reviews,Baselines contracts,not one component or a compelled next runtime stage. DomainMetadata governance is not automatically an upper-area execution dependency. |
| Discovery Components | Higher support-area consumer group including actual Registry,Relationships,Knowledge Graph,Navigation,Search owners. Projection/index/connection source-edition/provenance/freshness/access and required-provider duties remain;not complete live graph or mandatory serial pipeline. |
| Automation Components | Higher support-area capability group containing registered Validation,Metadata Generator,Registry Generator,Documentation Generator,Consistency Verification. Actual authorized executor,input bytes/source editions/authority/observations/effects remain separate;no installed run from this drawing. |
| Integration Components | Higher support-area consumer/adapter context containing actual registered integration capabilities,includingAI Integration. Actual scoped exchange/source-edition/reference/authority conditions remain;not an obligatory final execution stage or global architecture approval. |


Metadata remains the authoritative source of descriptive information regardless of the number of consuming components.

**Current governing scope.**

Metadata is authoritative for its own descriptive definitions/representation,not every represented identity,classification,state,decision or operation. Actual current ClassificationArchitecture12 preserves the functionalClassificationREADME10 statement that Type meaning remains with Metadata as a pending owner-source discrepancy. For normalized documentary classification,current ARC0055.1/5.3 andPolicy3 retain Classification/common meaning ownership. This does not transfer every unrelated Metadata field calledType or silently rewrite that unchanged README.

The view's Document andIdentity fragments form the split name DocumentIdentity;Classification andTemplates are parallel peers. Higher-area consumer groups are not single new components or a compulsory runtime pipeline. Required provider directions/interfaces/cycles remain those actually evidenced8.1,even when the exact received drawing is retained as historical/conceptual evidence.

---

# 10. Architectural Principles

The Metadata component shall conform to the following principles.

**Current governing scope.**

All nine principles retain actual mandatory force in their responsible source/definition edition and applicable scope. The current operative10.6–10.9 clauses distinguish ordinary meaning stability from necessary actual mandate revision;earlier received wording is preserved in the before/diff evidence,not treated as a simultaneous conflicting current rule. Technology/content/repository/storage/format independence does not remove actual representation/reference/physical/history/provider obligations.

---

## 10.1. Technology Independence

Metadata shall not depend on implementation technologies.

**Current governing scope.**

Definitions do not depend semantically on a particular implementation technology. Real implementations still require concrete subjects/bytes,source editions,representation/interfaces,authority and evidence for their claims. No installed technology or executor is allocated by this principle.

---

## 10.2. Content Independence

Metadata shall remain independent of document content.

**Current governing scope.**

Metadata describes the document/entity/edition rather than replacing its knowledge content. Values can legitimately reflect actual content and change in coordinated document evolution. This principle does not ban content-informed descriptors or concrete bytes in validation,or prove physically separate storage/access/compliance.

---

## 10.3. Repository Independence

Metadata shall not depend on repository organization.

**Current governing scope.**

Repository location does not define Metadata semantics or logical document identity. Actual representation,index/reference/access/freshness/history and authorized migration/provider conditions remain;neutrality is not a live retrieval guarantee or permission to move files.

---

## 10.4. Storage Independence

Metadata shall not depend on storage technologies.

**Current governing scope.**

Storage neutrality preserves meaning across legitimate realizations;it does not prove an actual stored Instance meets its Schema/effectiveProfile/reference/history contract or supply a concrete backend/record. Actual data and provider effects need evidence.

---

## 10.5. Format Independence

Metadata shall not depend on document formats.

**Current governing scope.**

A format does not redefine owner meanings. A real conversion still needs actual content/edition/representation/effectiveProfile/reference/history/interface equivalence and authorized effects;no conversion or universal serialization/field schema is implemented here.

---

## 10.6. Explicit Semantics

Every Metadata Element shall possess a single,well-defined authoritative meaning for its identified definition/source edition and applicable context. Ordinary use or representation shall not silently redefine it;necessary revision shall follow the actual governing-change conditions in section16.

**Current governing scope.**

Element definition/source edition,documentary value,record representation and actual use differ. A well-defined meaning is not proof a complete canonical Element population exists. Context does not authorize arbitrary semantic variation;necessary actual changed meaning needs the prior/new governing revision16,not a tag hiding simultaneous contradictory mandates.

---

## 10.7. Single Source of Truth

Each Metadata concept shall possess one authoritative definition for its identified source edition and applicable scope. Labels,synonyms,copies and representations do not alone establish different concepts,identity equivalence or competing canonical authority. Required earlier definitions remain historical evidence;an actual necessary successor shall be assessed under section16,not made a second contradictory current rule.

**Current governing scope.**

One authoritative definition does not prohibit legitimate labels/synonyms or preserved historical copies. Equivalence/duplication and identity require actual definition/source-edition/context/authority evidence;names alone authorize no merge,deletion,rekey or canonical adoption. Working documentDraft,term/Element state and actual accepted definition are distinct claims.

---

## 10.8. Extensibility

Ordinary additive Metadata extension shall preserve established applicable meanings and owner responsibilities. A necessary architectural,semantic,role or interface mandate revision is a distinct governed change and shall actually identify and revise the responsible prior/new contract under section16,with authority,need/alternatives,affected batch/interfaces,honest compatibility,mappings/history/pinned continuity,authorized transition and later checks. Unchanged peer restrictions are not waived by this sentence.

**Current governing scope.**

This clause actually changes the unqualified received preservation contract;it is not a generic disclaimer beside an unchanged restriction. Actual MTD00311.5/12,MTD00513/14,MTD0119/11 andMTD01412 restrictions remain real unchanged peer obligations pending their own source-specific cycles. This target successor does not repeal them or grant arbitrary semantic/role transfer. Current necessary revision16 must establish actual prior/new owner authority before coordinated adoption.

---

## 10.9. Backward Compatibility

Metadata evolution shall preserve compatibility with previously established Metadata whenever possible. Where necessary actual revision is incompatible,it shall be declared and assessed honestly under section16;required historical meaning and continuity evidence shall not be dropped merely because current-use compatibility cannot be retained.

**Current governing scope.**

Compatibility concerns actual meaning,use,structure/representation,consumers and source editions,not only readable names or unchanged IDs. Necessary incompatibility shall retain required older meaning,observations and pinned context,with actual mappings/conditions/effects and later checks. Historical interpretation,original conformity,current allowed use and live access are separate,no blanket grandfathering or automatic older invalidity.

---

# 11. Architectural Constraints

The Metadata component shall satisfy the following architectural constraints.

- Metadata shall remain independent of implementation.
- Metadata shall remain independent of programming languages.
- Metadata shall remain independent of tooling.
- Metadata shall remain independent of repositories.
- Metadata shall remain independent of storage mechanisms.
- Metadata shall remain independent of serialization formats.
- Metadata shall not duplicate responsibilities belonging to other architectural components.

**Current governing scope.**

All seven original constraints remain. Metadata-domain definitions/conditions are not duplication of common mechanisms or other domains' meanings. Actual required owner boundaries,Schema/effectiveProfile/Instance,physical/reference/index/access/retrieval/freshness/history/provider interfaces still apply despite implementation/language/tool/repository/storage/format neutrality. A necessary change to a real boundary or foundational mandate needs the actual responsible revision16,not an unrecorded exception.

---

# 12. Relationship with Other Components

Metadata collaborates with other components while preserving strict responsibility boundaries.

| Component | Received relationship summary | Actual current interface and evidence boundary |
|---|---|---|
| Document Identity | Consumes Metadata to describe document identity.  | Document Identity owns document-key/domain/allocation-preservation/reference meaning;Metadata owns descriptor definitions/Schema/effectiveProfile/Instance. Actual reciprocal required contracts8.1 remain unresolved,no rekey,automatic allocation or complete merged record. |
| Classification | Consumes Metadata to organize documents.  | Classification owns applicable category/assignment semantics,including normalized Family/primaryType/optionalClass meaning;Metadata owns broader representation. Actual required reciprocal scopes8.1 and functionalREADME Type-meaning discrepancy remain pending,no accepted assignment/owner takeover. |
| Templates | Define how Metadata is represented in documents.  | Templates defines reusable structural organization and may realize Metadata locations/representation under actual Schema/effectiveProfile contracts. It does not own Metadata semantics/Schema or make every Metadata use require an installed Template runtime. ActualTPL0019.1 declarations remain source-qualified. |
| Workflow | Consumes Metadata during lifecycle management.  | Workflow owns common document-process/transition mechanisms;Metadata defines its own artifact/definition/Schema/Profile/Instance state-use contracts and represents descriptors. Actual subject/edition/authority/conditions/evidence and authorized execution differ from documentStatus or source presence. |
| Policies | Uses Metadata for governance decisions.  | Policies owns common applicable decision/rule mechanisms;Metadata Governance defines domain change conditions. Actual authority/evidence/rationale/conditions/fulfillment/adoption/effects are needed;phase authorization is not canonical or operational approval. |
| Baselines | Preserve Metadata across framework evolution.  | Baselines owns exact selected-edition membership and immutable snapshot evidence. Required prior Metadata meaning/Schema/Profile/Instances/decisions/pinned context remain separately preserved;source presence,prior approval or receivedBaseline1.0 does not select this changed Draft. |
| Registry | Indexes Metadata for document discovery.  | Registry owns registrations/indexes/projections and source-edition provenance/freshness/access obligations. A descriptor or authoritative Metadata Dictionary is not a registration,complete populated index or live retrieval guarantee. |
| Relationships | Connect Metadata across architectural entities.  | Relationships owns common typed connection records/provenance;Metadata owns domain composition/association/dependency meanings. Real kind/definition/assertion/typed endpoints/properties/count/source editions and required provider edges remain,no universal all-document tuple/inverse registry. |
| Knowledge Graph | Uses Metadata as semantic nodes and properties.  | Knowledge Graph owns logical projections of typed entities/relations/provenance. Metadata can supply node/property descriptors;not every node is a document and a projection is not semantic ownership,current assignment validity or complete live accepted provider graph. |
| Validation | Verifies Metadata compliance.  | Common Validation capability and actual authorized executor evaluate concrete Metadata against responsible source-rule-definition-set/Schema-effectiveProfile editions,scope/authority/observations/coverage. Metadata owns domain criteria;nonmutating evaluation is not correction,approval,operation or a deployed checker from this statement. |
| Automation | Produces and consumes Metadata during automated processes.  | Automation area/capabilities include registered Validation,Metadata Generator,Registry Generator,Documentation Generator andConsistency Verification owners. Actual DMS/CMS/tool/manual executor,inputs/source bytes/authority/observations/effects remain separate. Producing fields gives no canonical allocation,approval,adoption or permission. |

**Current governing scope.**

All eleven original component/relationship pairs are preserved beside their actual current interface/evidence scope. Some received summaries are shorthand,not complete allocated records or observed operations. Metadata domain relationship definition/association/assertion and common typed connection/projection mechanisms differ;endpoints need actual domain/identity/source-edition/context evidence,not automatic all-document keys or a universal physical tuple.

Registry andGraph outputs require actual source-edition/provenance/snapshot/freshness/access evidence;reading or producing descriptors alone proves no current assignment validity,canonical adoption or complete populated runtime graph. Required provider relationships8.1 remain,including unresolved reciprocal requirements. Actual Templates andAutomation source declarations are retained with their own scope and pending detail,not silently accepted or rewritten.

---

# 13. Architectural Evolution

The Metadata component evolves incrementally according to the Metadata Roadmap.

Its evolution follows the progression:

1. Core Metadata
2. Structural Metadata
3. Lifecycle Metadata
4. Governance Metadata
5. Traceability Metadata
6. Discovery Metadata
7. Automation Metadata

Each ordinary additive stage shall preserve previously established applicable concepts. A stage that necessarily changes a governing concept,role or interface shall be treated as an actual assessed prior/new mandate revision under sections10.8 and16,not silently called a compatible extension. The seven stages are planning concerns,not new components,performed capability milestones or a universal required-provider/execution order.

**Current governing scope.**

All seven stages preserve their exact order and distinct concerns. They are the received MetadataRoadmap planning progression,not seven new architectural components or proof current capabilities have been implemented/published. The actual Roadmap6.1 initial-field list and11 success criteria remain received source-specific plans;they allocate no canonical Metadata Elements/Profiles/Instances or completed milestones.

Metadata definition/Schema/Profile/Instance evolution,documentaryVersion/Revision and actual domain artifact/source editions are different subjects. A stage/Version label does not propagate consumer successors,state changes,approval or Baseline inclusion. Required history and actual adoption/effects remain under responsible owners16.

---

# 14. Conformance

The following six concerns summarize local architectural conformance;they are not an exhaustive or sufficient full-implementation test:

- Metadata is maintained independently of document content;
- Metadata responsibilities remain isolated from other components;
- Metadata follows the Documentation Framework terminology;
- Metadata respects the Documentation Layer boundaries;
- Metadata remains technology independent;
- Metadata is extensible without architectural disruption.

**Current governing scope.**

For a declared MetadataArchitecture conformance claim,the implementation shall satisfy every actual applicable requirement of this Architecture,including the nine principles,seven constraints and the operative responsibility/provider/evolution rules,with independently applicable owner contracts retained. Real source/definition/rule-set/Schema-effectiveProfile/subject editions,scope/applicability/authority,observations/executor and mandatory coverage shall support the claim. An untested subset or absent evidence does not justify broader success or fabricate a violation/default outcome.

MetadataSpecification15.1 Core means every actual mandatory requirement,including unnumbered/incorporated duties andR005 Profile compliance. Its Extended15.2 states Core plus extensibility/governance/lifecycle concerns that overlap already mandatory duties;retain actual capability evidence and genuine additional-differentiation limits,not a new disjoint optional package. The Dictionary's16 recommended attributes7 andSpecification14 six required entry subjects remain distinct actual contracts. IllustrativeDictionary13 MTD-001/Published values are not allocated canonical Element or lifecycle records. No mandatory information is waived or missing ID/state/Version/Revision/relationship/constraint/field/Profile population invented.

MetadataValidation7/10/11/13/14 andSpecification10 retain actual structural/profile/semantic/consistency/referential evaluation,criterion/severity versus Valid/Valid with Warnings/Invalid aggregate scope,determinism/repeatability/coverage/nonmutation. Missing evidence is not by itself an observed violation,warning severity or operational permission. Evaluation does not silently modify Metadata;recording,correction,decision and authorized operation are separate. Source-local documentary checks do not certify a complete implementation,performed evaluation,canonical adoption,global architecture or actual availability.

---

# 15. Related Documents

**Current governing scope.**

All eighteen received related-document subjects retain their intended unique ID/title/path and order through explicit relative links. Source authority comes from actual declaration/incorporation and applicable owner editions,not Type,title,link success or list order. MetadataBestPractices remains explicitly informative;omission alone is no nonconformance and advice waives no independent mandate. Current peers' actual invalidType/header details and wider content work remain pending their own scheduled cycles,not normalized by this source.

---

## 15.1. Architecture

- [DF-ARC-004 — Architectural Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md)
- [DF-ARC-005 — Architectural Components](../../../01-Architecture/DF-ARC-005-ArchitecturalComponents.md)
- [DF-ARC-006 — Terminology](../../../01-Architecture/DF-ARC-006-Terminology.md)

**Current governing scope.**

These three actual Architecture sources retain owner/allocation/support-order/terminology contracts and genuine integration limits. A local source correction does not accept unresolved provider cycles or actual physical-placement deviations.

---

## 15.2. Roadmaps

- [DF-RDM-010 — Metadata Roadmap](../../../Roadmaps/02-Documentation/Metadata/DF-RDM-010-MetadataRoadmap.md)

**Current governing scope.**

The actual componentMetadataRoadmap remains a planning/evolution source with its received constraints/fields/stage/success criteria and pending own normalization/content cycle. It is not a newly allocated Metadata component or evidence its planned deliverables were executed.

---

## 15.3. Metadata Specifications

- [DF-MTD-002 — Metadata Concepts](DF-MTD-002-MetadataConcepts.md)
- [DF-MTD-003 — Metadata Model](DF-MTD-003-MetadataModel.md)
- [DF-MTD-004 — Metadata Elements](DF-MTD-004-MetadataElements.md)
- [DF-MTD-005 — Metadata Schema](../02-Structure/DF-MTD-005-MetadataSchema.md)
- [DF-MTD-006 — Metadata Lifecycle](../03-Behavior/DF-MTD-006-MetadataLifecycle.md)
- [DF-MTD-007 — Metadata Validation](../03-Behavior/DF-MTD-007-MetadataValidation.md)
- [DF-MTD-008 — Metadata Governance](../03-Behavior/DF-MTD-008-MetadataGovernance.md)
- [DF-MTD-009 — Metadata Relationships](../02-Structure/DF-MTD-009-MetadataRelationships.md)
- [DF-MTD-010 — Metadata Constraints](../02-Structure/DF-MTD-010-MetadataConstraints.md)
- [DF-MTD-011 — Metadata Extensibility](../03-Behavior/DF-MTD-011-MetadataExtensibility.md)
- [DF-MTD-012 — Metadata Best Practices](../04-Reference/DF-MTD-012-MetadataBestPractices.md)
- [DF-MTD-013 — Metadata Dictionary](../02-Structure/DF-MTD-013-MetadataDictionary.md)
- [DF-MTD-014 — Metadata Specification](../04-Reference/DF-MTD-014-MetadataSpecification.md)
- [DF-MTD-015 — Metadata Examples](../04-Reference/DF-MTD-015-MetadataExamples.md)

**Current governing scope.**

All fourteen Metadata peers retain actual source-local authority and receivedV1R0 duties pending their cycles. Their Model/Schema/Profile/Instance,required validation/governance/history and no-redefinition/ownership restrictions are not silently waived. This architecture does not create missing canonical fields/Profiles or restart any completed Identity/Classification cycle. There was no initial ChangeHistory in the received source;only the actual later contribution below is dated.

---

# 16. Actual Working Decisions,Coordination and Provenance

This is an actual authorized working architectural successor under Review Policy,not canonical approval,condition fulfillment,effective adoption,publication,Baseline selection or complete implementation/global architectural acceptance. The operative responsibility/dependency/preservation clauses in7/8.1/10.6–10.9/13 are actually changed;the received source remains exact historical evidence,not a second contradictory current governing rule.

| Actual decision established before mutation | Received contract / risk | Current choice | Actual authority and need / alternatives |
|---|---|---|---|
| Actual domain-contract versus common mechanism and execution responsibility | Section7 bans governing lifecycles/managing relationships/performing validation and says Metadata only provides descriptive information,without distinguishing its actual own family contracts. | Metadata defines its domain conceptual/representation/state-use/validation/governance/relationship contracts;common mechanisms/records and authorized operational executor retain ownership. All eight exclusions are actually rewritten in that scope. | Actual ARC0055.1/6/7/8,MTD006/007/008/009 and adopted Policy3/5/6;Metadata stays in Documentation. A generic disclaimer beside unchanged operative bans leaves conflicting rules. Moving Metadata to Governance/Automation or transferring all common mechanisms fabricates architecture. Selected actual operative replacement preserves subjects and real owner/executor boundaries. |
| Actual required provider declarations and unresolved reciprocal interfaces | Section8.1 permits only Foundation/Architecture dependencies despite source-declared Metadata→Identity and reciprocal Identity→Metadata,plus actual Classification representation requirements. | Replace blanket restriction with actual consumer→provider/source-edition/scope/interface map;retain support-order/same-Layer rules and required-cycle prohibition. Preserve reciprocal declarations as unresolved,not waived by semantic/reference naming. | Actual ARC00412/13,ARC00512,DID0019.1,DID0095.1.1/10,functionalDIDREADME,CLS00112/20 and Policy6. Deleting required edges,calling every dependency a reference,or declaring complete acyclicity is unsupported. An arbitrary upper-area exception violates current structural constraints. Selected actual scoped provider declarations expose conflicts for responsible coordinated reconciliation. |
| Broader Metadata representation and independent meaning/state/evidence owners | Passive descriptor/service summaries and representation table can be overread as complete accepted fields/Profiles,identity/classification ownership,executed validation or sufficient approval. | State actual Concepts/Element/Value/Model/Dictionary/Schema/effectiveProfile/Instance responsibilities,known one-Profile duty and genuine detail/population gaps. Identity/classification meanings,typed states,authority/conditions/evidence/history and concrete execution remain separate. | Actual ARC0055.1–5.4,MTD0037/10/12,MTD00511/12/14/15,MTD014R005/7/10/14/15,DID014 and currentCLS contracts. Inventing canonical field IDs/values/Profiles,waiving missing information,or imposing a universal Template runtime would exceed evidence. Selected broad interface map retains mandatory duties and real limits without allocating records or weakening owners. |
| Actual ordinary preservation and necessary governing mandate revision | Sections10.8/13 unqualified preservation/no-redefinition and actual peer MTD003/005/011/014 restrictions can prohibit necessary semantic/role/interface revision. | Actually revise target clauses:ordinary extension preserves meanings;necessary actual prior/new mandate revision requires authority,need/alternatives,batch/interfaces,honest incompatibility,mappings/history/pinned continuity,authorized transition/effects and later checks. Unchanged peer restrictions remain real pending source-specific work. | Actual adopted Policy5.2/6,ARC00413/17,ARC00515,target architectural authority and current responsible Metadata owner clauses. A permanent freeze prevents required correction;arbitrary mutation or claiming Governance alone overrides unchanged contracts is false. Selected real target-rule replacement honestly changes contract permission and warrants majorV2.0 R1,not a cosmetic compatible label. |
| Complete preservation,physical/consumer/stage/conformance scope and traceable edition | Two unnamed CRLF views,29 bodies,all original consumer/exclusion/evolution subjects and no initial Change History must remain;capability/stage/local conformance summaries are not implemented or globally accepted architecture. | Preserve full before/current evidence,all original subjects/two exact spans17 fragments/11 pairs/18 target references. Retain physical/provider/authority/history duties,stage planning and full mandatory breadth;new actual contribution only,no invented initial event. | Actual Policy2/3/5/6/7,ARC0075/14,MTD014Core and all50-path prospective/current-source interfaces. Replacing the source with a summary loses work;fabricating initial history or source authorship is false. Selected cumulative actual author/Draft/unassigned successor and exact maps preserve qualified/reconstructed/failed-corrected history without global closure or completed-cycle restart. |

## 16.1. Necessary actual mandate revision and honest compatibility

Actual section7 blanket domain-responsibility exclusions and Metadata-only-description rule are replaced by domain-contract/common-mechanism/executor boundaries. Actual8.1 onlyFoundation/Architecture dependency restriction is replaced by scoped required-provider/same-Layer/structural-constraint rules,with real reciprocal requirements exposed rather than hidden. Actual10.6–10.9/13 preserve ordinary meanings while permitting necessary explicitly assessed governing revisions. These changes alter what the architectural contract permits/requires;they justify an incompatible major successor V1.0 R0→V2.0 R1 under Policy5.2. Revision remains monotonic0→1;the major is not due to Type,label,path,format,links or peer numbering. TypeArchitecture/current01-Architecture and actual ID/title/Family/Component/English remain.

An actual necessary architectural,semantic,role,interface or foundational mandate revision shall identify the responsible prior/new source and exact applicable meaning,need/rationale/alternatives,authority and decision conditions,the concrete affected owner/consumer/interface batch,and honest compatibility. It shall provide actual old/new mappings/nonreuse,required earlier meaning/rules/definitions/Schema/Profile/Instance/assignments/states/decisions/results/source editions and pinned continuity,authorized coordinated transition/effects and later checks. A governing contract that truly changes shall actually be revised;adding a scope label or Governance paragraph does not remove contradictory current duties. Required history is not optional because a new consumer contract is incompatible.

This working phase authorization permits this Draft source correction. It is not an organizational actor assignment,canonical/operational decision,fulfillment of required adoption/activation/publication conditions,permission for all operations or exact Baseline inclusion. Actual responsible scope/authority/evidence/rationale/conditions/fulfillment/effect/source-edition records remain needed;genuine actor/guard/route/general-record/interface gaps are not invented. Necessary approval is not proof of sufficient effective adoption. Metadata Element/definition/Schema/Profile/Instance,document Status/Workflow,identity/reference record,decision/outcome,validation result/finding and Milestone states are distinct. No universal state aliases/machine or consumer transition is inferred.

Actual unchanged MetadataModel11.5/12,MetadataSchema13/14,MetadataExtensibility9/11 andMetadataSpecification12 retain received no-redefinition/ownership/preservation constraints in their own scopes. Current MetadataLifecycle/Elements deprecation/older-validity claims andDictionary history duties likewise remain actual peer statements requiring source-specific reconciliation. This local target revision does not repeal them or certify integrated compatibility;where a real necessary peer mandate must change,it needs its own actual responsible prior/new revision,authority,compatibility/history/interfaces and separate checks. Existing scoped duties are not ignored merely because this target now distinguishes ordinary addition from necessary revision.

## 16.2. Required history,physical representation and conformance limits

Required earlier meaning and source/definition/Schema/Profile/rule-set/assignment/state/decision/result editions and needed pinned references shall remain interpretable under actual owners. Historical interpretation,original conformity,current allowed use/compliance and live retrieval/access/freshness are different claims. A later traced reassessment under the actual earlier contract may use new evidence while retaining previous observations;new rules shall not be backdated. Retirement/replacement/approval does not automatically delete records,migrate assignments,rekey documents,propagate consumer successors,guarantee every older assignment valid/invalid or select a Baseline.

DocumentVersion/Revision,this sourceV2R1,MetadataElement/definition architectural editions,Profile/Instance context and identity localR/record/effective-state coordinates shall not be silently conflated. No numbering/reset/default per-Element value,canonical field or new metadata definition is fabricated. Cumulative authorship records actual contributions,not approval or blanket responsibility for every later product.

Semantic technology/content/repository/storage/format independence preserves meaning while actual descriptor/Schema/effectiveProfile/Instance,physical/reference/index/access/retrieval/freshness/use/history/provider duties remain. Actual concrete subject/bytes/source editions/authority,observations/executor and mandatory coverage are needed for evaluated claims. Missing evidence withholds unsupported breadth without inventing a violation/default aggregate/severity/waiver/permission;known supported violations remain. Nonmutating evaluation is separate from recording/correction/decision/authorized operation. This source supplies no installed engine,complete canonical Element/Profile population,performed examples/full Core-Extended implementation or globally accepted runtime.

Both actual ClassificationElementsArchitecture at02-Structure and ClassificationConstraintsStructure at03-Behavior remain unmet ARC007 placement requirements pendingM13,not compliant,waived or mere missing-evidence gaps. MetadataArchitecture itself remains correctly placedArchitecture/current01-Architecture. Metadata↔Identity and actual Metadata/Classification provider scope/cycle questions remain visible and must be reconciled under the actual no-required-cycle rule;recording them does not waive it. Global19/M14 and actual owner/general-detail/population/count/precedence/authority/guard/record/representation/provider/interface/cycle/implementation/permission/architectural acceptance criteria remain independent.

## 16.3. Actual prospective owner and consumer coordination

These50 concrete current owner/consumer/reference paths were identified with raw hashes,coordinates,literal clauses,path-specific prior/proposed need/authority/interfaces/compatibility-history before source mutation. Full evidence is attached to the Review Report;the paths remain unchanged here. This is a prospective coordinated batch,not completed propagation or every external consumer known. Functional files remain non-normalized.

| Actual affected path | Actual input edition / scope | Actual proposed coordination |
|---|---|---|
| 00-Foundation/DF-FND-004-ArchitecturalBlueprint.md | V2.0 R1 | Retain actual foundational/current owner mandate and received source-qualified Metadata dependency/responsibility context;actual meaning changes need prior/new source authority and compatibility/history evidence. |
| 00-Foundation/DF-FND-006-DesignRationale.md | V2.0 R1 | Retain actual foundational/current owner mandate and received source-qualified Metadata dependency/responsibility context;actual meaning changes need prior/new source authority and compatibility/history evidence. |
| 01-Architecture/DF-ARC-003-ArchitecturalConcepts.md | V2.0 R2 | Retain actual component allocation/support-order/same-Layer interfaces/no required cycles and genuine placement obligations;assess actual Metadata domain-versus-executor responsibility revision without inventing component/Layer or globally accepted DAG. |
| 01-Architecture/DF-ARC-004-ArchitecturalLayers.md | V2.0 R2 | Retain actual component allocation/support-order/same-Layer interfaces/no required cycles and genuine placement obligations;assess actual Metadata domain-versus-executor responsibility revision without inventing component/Layer or globally accepted DAG. |
| 01-Architecture/DF-ARC-005-ArchitecturalComponents.md | V2.0 R2 | Retain actual component allocation/support-order/same-Layer interfaces/no required cycles and genuine placement obligations;assess actual Metadata domain-versus-executor responsibility revision without inventing component/Layer or globally accepted DAG. |
| 01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md | V2.0 R2 | Retain actual component allocation/support-order/same-Layer interfaces/no required cycles and genuine placement obligations;assess actual Metadata domain-versus-executor responsibility revision without inventing component/Layer or globally accepted DAG. |
| 02-Documentation/Classification/01-Architecture/DF-CLS-001-ClassificationArchitecture.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/02-Structure/DF-CLS-004-ClassificationElements.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/02-Structure/DF-CLS-005-ClassificationSchema.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/02-Structure/DF-CLS-009-ClassificationRelationships.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/03-Behavior/DF-CLS-007-ClassificationValidation.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/03-Behavior/DF-CLS-008-ClassificationGovernance.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/03-Behavior/DF-CLS-010-ClassificationConstraints.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/03-Behavior/DF-CLS-011-ClassificationExtensibility.md | V2.0 R2 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/04-Reference/DF-CLS-012-ClassificationBestPractices.md | V1.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/04-Reference/DF-CLS-013-ClassificationDictionary.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/04-Reference/DF-CLS-014-ClassificationSpecification.md | V2.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/04-Reference/DF-CLS-015-ClassificationExamples.md | V1.0 R1 | Retain actual Family membership/uniform primaryType/optionalClass/domain definition-assignment semantics,Metadata broader representation and actual required provider/history/Core obligations. Source-local Classification closures do not settle Metadata owner integration. |
| 02-Documentation/Classification/README.md | Functional file;non-normalized,no edition assigned | Keep non-normalized README navigation/owner/provider assertions and source-qualified historical context;no normalized ID/header requirement or silently edited consumer/Metadata Type meaning. |
| 02-Documentation/DocumentIdentity/01-Architecture/DF-DID-001-DocumentIdentityArchitecture.md | V2.0 R2 | Retain actual identity domain/documentK/localR/exact edition,Metadata descriptor/Schema/Profile/Instance and actual reciprocal provider declarations;identify actual scope/contract/interfaces without renaming away indispensable Metadata↔Identity cycle. |
| 02-Documentation/DocumentIdentity/02-Structure/DF-DID-005 - Document Identity Schema.md | V2.0 R1 | Retain actual identity domain/documentK/localR/exact edition,Metadata descriptor/Schema/Profile/Instance and actual reciprocal provider declarations;identify actual scope/contract/interfaces without renaming away indispensable Metadata↔Identity cycle. |
| 02-Documentation/DocumentIdentity/02-Structure/DF-DID-009 - Document Identity Relationships.md | V2.0 R1 | Retain actual identity domain/documentK/localR/exact edition,Metadata descriptor/Schema/Profile/Instance and actual reciprocal provider declarations;identify actual scope/contract/interfaces without renaming away indispensable Metadata↔Identity cycle. |
| 02-Documentation/DocumentIdentity/04-Reference/DF-DID-014 - Document Identity Specification.md | V2.0 R1 | Retain actual identity domain/documentK/localR/exact edition,Metadata descriptor/Schema/Profile/Instance and actual reciprocal provider declarations;identify actual scope/contract/interfaces without renaming away indispensable Metadata↔Identity cycle. |
| 02-Documentation/DocumentIdentity/README.md | Functional file;non-normalized,no edition assigned | Keep non-normalized README navigation/owner/provider assertions and source-qualified historical context;no normalized ID/header requirement or silently edited consumer/Metadata Type meaning. |
| 02-Documentation/Metadata/01-Architecture/DF-MTD-002-MetadataConcepts.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/01-Architecture/DF-MTD-004-MetadataElements.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/02-Structure/DF-MTD-005-MetadataSchema.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/02-Structure/DF-MTD-009-MetadataRelationships.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/02-Structure/DF-MTD-010-MetadataConstraints.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/03-Behavior/DF-MTD-006-MetadataLifecycle.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/03-Behavior/DF-MTD-007-MetadataValidation.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/03-Behavior/DF-MTD-008-MetadataGovernance.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/03-Behavior/DF-MTD-011-MetadataExtensibility.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/04-Reference/DF-MTD-012-MetadataBestPractices.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/04-Reference/DF-MTD-014-MetadataSpecification.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/04-Reference/DF-MTD-015-MetadataExamples.md | V1.0 R0 | Retain actual received owner contract for concepts/model/elements/schema/lifecycle/validation/governance/relations/constraints/extensibility/dictionary/specification/examples. Architecture replacement must name actual prior/new mandates,need/authority/interfaces and honest compatibility/history;unchanged current restrictions are not silently waived. |
| 02-Documentation/Metadata/README.md | Functional file;non-normalized,no edition assigned | Keep non-normalized README navigation/owner/provider assertions and source-qualified historical context;no normalized ID/header requirement or silently edited consumer/Metadata Type meaning. |
| 02-Documentation/Templates/01-Architecture/DF-TPL-001-TemplatesArchitecture.md | V1.0 R0 | Retain actual Templates definition/representation responsibilities and conditional template use versus Metadata Schema/effectiveProfile/Instance authority. No mandatory template-runtime dependency,complete merged field catalog or Profile population inferred. |
| 02-Documentation/Templates/02-Structure/DF-TPL-005-TemplatesSchema.md | V1.0 R0 | Retain actual Templates definition/representation responsibilities and conditional template use versus Metadata Schema/effectiveProfile/Instance authority. No mandatory template-runtime dependency,complete merged field catalog or Profile population inferred. |
| 02-Documentation/Templates/02-Structure/DF-TPL-009-TemplatesRelationships.md | V1.0 R0 | Retain actual Templates definition/representation responsibilities and conditional template use versus Metadata Schema/effectiveProfile/Instance authority. No mandatory template-runtime dependency,complete merged field catalog or Profile population inferred. |
| 02-Documentation/Templates/03-Behavior/DF-TPL-010-TemplatesConstraints.md | V1.0 R0 | Retain actual Templates definition/representation responsibilities and conditional template use versus Metadata Schema/effectiveProfile/Instance authority. No mandatory template-runtime dependency,complete merged field catalog or Profile population inferred. |
| 02-Documentation/Templates/04-Reference/DF-TPL-014-TemplatesSpecification.md | V1.0 R0 | Retain actual Templates definition/representation responsibilities and conditional template use versus Metadata Schema/effectiveProfile/Instance authority. No mandatory template-runtime dependency,complete merged field catalog or Profile population inferred. |
| 02-Documentation/Templates/README.md | Functional file;non-normalized,no edition assigned | Keep non-normalized README navigation/owner/provider assertions and source-qualified historical context;no normalized ID/header requirement or silently edited consumer/Metadata Type meaning. |
| 03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md | V1.0 R2 | Apply adopted exact phase/effect-based edition/cumulative and event-specific author/functional exclusion/stable plan/central evidence rules. Prior global criteria and completed/failed/corrected history remain independent. |
| Roadmaps/02-Documentation/Metadata/DF-RDM-010-MetadataRoadmap.md | V1.0 R1 | Keep actual seven Metadata stages/initial-field plan/integration consumers/success criteria as received planned evolution,not performed capabilities,new components or mandatory provider/execution graph. Component roadmap remains pending own normalization/content cycle. |

68 REVIEW-time current source snapshots remain source-qualified:targetV1R0 is exact historical input,current working successorV2R1;other67 selected sources retain exact bytes,not full peer revalidation.54 input-of4.44 REVIEW literal occurrences across41 sources and22 current prior-note contexts retain actual source/time bases. Actual source/central successors are separately diffed rather than pretending those old literals are total current occurrences. Current Identity/Classification source-local results,explicit Model reconstruction/prior factual qualifications,CLS011 failedV2R1/later correctedV2R2 and report129 later history reconciliation remain intact. No earlier completed cycle is restarted or source-qualified global criterion narrowed.

All29 original numbered bodies/15 chapters/31 raw headings,twelve listgroups83 subjects,nine principles,seven constraints,seven stages,eighteen intended related subjects and eleven full component-relation pairs are mapped before/current. The eight actual exclusion bullet replacements retain their original subjects in explicit historical/current maps. Both exact unnamed CRLF spans/17 raw-line fragments remain with typed scope and final section hashes;no diagram IDs are allocated. Proper separate table headers/delimiters/data arities are checked. Received source has no ChangeHistory;the actual later contribution below does not invent an original date/event.

All16 local corrections remain Corrected—pending validation. Construction checks establish preparation/preservation/traceability,not the separate VALIDATE phase. Pause after UPDATE. CONTINUAR starts4.44 VALIDATE of this exactV2.0 R1 only.

---

# Actual Later Contribution

The received V1.0 R0 source has no Change History section. Its exact raw bytes,header and Arnaldo Figueira authorship are retained in the input/before evidence;no original date or initial contribution event is invented here.

| Date | Version | Revision | Contributor | Actual contribution / status |
|---|---|---|---|---|
| 2026-10-16 | 2.0 | 1 | Codex — AI assistant | Step4.44 UPDATE:actual incompatible responsibility/dependency/preservation mandate correction with typed owner/provider/state/authority/evidence/history/representation/conformance boundaries and complete original subject maps. Cumulative original author retained;16 corrections pending separate VALIDATE. Draft;Baseline Not assigned;no canonical/operational/global approval. |

**End of Document**

---