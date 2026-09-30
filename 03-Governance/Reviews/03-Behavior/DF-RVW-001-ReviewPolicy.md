# Documentation Framework

# DF-RVW-001 — Review Policy

| Metadata | Value |
|---|---|
| **Document ID** | DF-RVW-001 |
| **Title** | Review Policy |
| **Family** | Reviews |
| **Type** | Behavior |
| **Component** | Reviews |
| **Author** | Codex — AI assistant |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

## 1. Purpose, authority and scope

This document defines the working contracts for the review initiated on 2026-09-30 from the supplied Context.zip. Its authority for conducting this review derives from the user's explicit instructions in Load-Review-Context.md, edition 4, and the subsequent CONTINUAR command for Step 3. It does not evidence publication, framework-wide release approval, or operational implementation of Reviews.

Reviews is an existing architectural component: DF-ARC-005 §6.3 assigns technical reviews, architectural reviews and consistency verification to it. This policy and DF-RVW-002 belong to that component; their location does not create a new Layer or component. Review artifacts are maintained under the existing 03-Governance/Reviews area, with Behavior and Reference documentation categories.

The rules below govern working editions and this review's tracking. They are the responsible process source for these review conventions. Identity semantics remain owned by Document Identity; classification semantics by Classification; descriptive schemas/profiles by Metadata; framework architecture by Architecture. Those sources must incorporate the applicable decisions through their scheduled REVIEW/UPDATE/VALIDATE cycles. Their remaining discrepancies are recorded in DF-RVW-002, rather than reported as integrated consistency.

Where received documents conflict with the user's adopted rules, the adopted rules govern the working review. The received rule remains preserved as input/historical evidence and is pending reconciliation; it is not a second governing rule for the same working operation. No completed rollout across existing sources is claimed by creating this policy.

## 2. Normalized documents and functional files

Every file named README.md, CHANGELOG.md or ArchitecturalMilestones.md in this corpus is a non-normalized functional file. It retains its name and does not require Document ID, Family, Type, Component, Version, Revision, Status or Baseline by virtue of document normalization. Do not infer a finding from absence of those fields. Do not automatically delete legitimate existing information.

These files remain in inventories, SHA-256 manifests, content reviews and applicable structural, terminology, reference and consistency checks. CHANGELOG.md and ArchitecturalMilestones.md retain their own entry/milestone IDs, states, dates and historical conventions. Their maintenance is not conditional on normalized document metadata.

The input corpus comprises 79 documents within normalization scope and 8 non-normalized files. Two normalized review documents are introduced by Step 3. Machine-readable exports attached to DF-RVW-002 are representations of its inventories and matrices, not independent normalized documents or new authorities. Each export identifies its parent document and edition in its manifest or accompanying report.

## 3. Classification contract

### 3.1. Uniform Type

Type identifies the primary responsibility of every normalized document and uses exactly one value from {Architecture, Structure, Behavior, Reference}. There are no special Type values for Foundation, Architecture, global roadmaps or review artifacts.

| Type | Primary responsibility |
|---|---|
| Architecture | Foundations, principles, concepts, conceptual models/elements and architectural decisions. |
| Structure | Organization, composition, schemas, structural relationships, restrictions and element catalogs. |
| Behavior | Processes, lifecycle, validation, governance, extensibility and planned evolution. |
| Reference | Consultation, terminology, consolidated specifications, examples, recommendations and historical records. |

Use the spelling Behavior. Base, Core, Schema, Dictionary and Lifecycle are not additional Type values. A historical evolution account is Reference; a process or evolution plan is Behavior. Assess content and primary responsibility rather than filename or directory alone. Normative or informative authority is established by explicit statements/references, never by Type=Reference alone. Validation is not approval.

### 3.2. Family and Component

| Document category | Family | Component |
|---|---|---|
| Belongs to a component | Canonical component name | Same canonical name, when the field is used. |
| Foundation without a component | Foundation | Absent/not applicable. |
| Architecture without a component | Architecture | Absent/not applicable. |
| Global roadmap or global implementation strategy | Roadmap | Absent/not applicable. |
| This review's policy/report | Reviews | Reviews. |

Roadmap is an explicitly scoped documentary planning area for global, non-component plans. It reuses the received Family value in DF-RDM-001/002, not an invented component or Layer. These two documents use Type=Behavior. The existing Component=Documentation Framework in DF-RDM-002 must be assessed and removed from its working header in the scheduled UPDATE: the framework is the container, not a component of itself.

Component roadmaps belong to the component they plan and therefore use Family=component, Type=Behavior and matching Component, regardless of central storage under Roadmaps. Current component names are Metadata, Document Identity, Classification and Templates. DocumentIdentity is a directory alias, not a competing canonical component name.

Do not remove Component indiscriminately. The global roadmap decision is localized and does not remove it from component documents. Family/Type changes do not determine document identity or structural Layer allocation.

### 3.3. Class

Class remains a separate, optional semantic dimension. This policy does not create a complete Class vocabulary or make it mandatory. Retain received values as evidence, then assess each use in its document cycle. A value that merely repeats Type or misstates authority must be reconciled with evidence. New review artifacts omit Class because no additional distinction is needed. Optional does not mean unrestricted: any value used must have an explicit, non-conflicting definition.

## 4. Identity convention for this corpus and review artifacts

### 4.1. Representation and uniqueness

The identity domain is Documentation Framework. Its representation prefix is DF. A working normalized document identifier follows DF-SSS-NNN, where SSS is a registered three-letter uppercase allocation-series code and NNN is a three-digit positive allocation number, 001–999. The full identifier is unique within the domain. Numbers are allocated within a series; equal numeric suffixes across different series are not collisions.

Series codes are stable allocation namespaces, not the document's current Family, Type, component, location, version or revision. Preserve existing valid identifiers when those characteristics change. A series' original purpose is recorded for traceability, but it does not recalculate an existing document ID after reassignment/reclassification.

| Series | Received origin/purpose | Step 3 action |
|---|---|---|
| FND | Foundation documents | Preserve existing allocations. |
| ARC | Framework Architecture documents | Preserve existing allocations. |
| MTD | Metadata documents | Preserve existing allocations. |
| DID | Document Identity documents | Preserve existing allocations. |
| CLS | Classification documents | Preserve unambiguous allocations; resolve the nominal CLS-003 collision. |
| TPL | Templates documents | Preserve existing allocations. |
| RDM | Planning documents | Preserve allocations even when Family becomes a component name. |
| RVW | Review policy and consolidated review report | Allocate 001 to this policy and 002 to DF-RVW-002 after collision checks. |

This is a corpus convention, not a format imposed on identities in other domains or an identifier-generation implementation. Scheduled reconciliation of DF-DID-005/010/014 owns its integration into the identity contract. Foundation and Classification must qualify the earlier Family/Type-based convention accordingly.

### 4.2. Allocation, reservations and retirement

New allocation requires an explicit series record and collision scan of headers, filenames, references, historical/reserved records and this review's allocation register. Do not reuse allocated/retired numbers. A gap does not prove availability; when allocation history is unavailable, record that limitation and use a documented allocation decision rather than infer a historical reservation. Missing IDs are not assigned to the eight functional files excluded in §2.

000 is not allocated under this working convention; it is not implicitly a README code. RVW-001/002 are the only new allocations at Step 3; no future numbers are reserved. At 999, do not widen the syntax or silently recycle: register another unused three-letter series with traceable continuation and preserve all old IDs. A new domain is a separate semantic decision, not a shortcut for renumbering this corpus.

Maintain an allocation register in DF-RVW-002's exports, including series, number, identifier, path, allocation status and evidence. Retired IDs remain reserved. The source archive and the input manifest preserve received declarations, including invalid ones; preservation is evidence, not acceptance of a collision.

### 4.3. Localized correction and historical syntax

No general ID migration is required by the adopted classification change. The nominal DF-CLS-003-ClassificationModel.md wrongly declares DF-CLS-001 and repeats the Architecture prose. Its correction is pending a distinct document recovery/update and path-scoped map. It is not a global DF-CLS-001→DF-CLS-003 replacement or an alias that makes one identifier resolve to two documents.

Operational references must resolve to the intended final identity/path after a coordinated correction. Historical examples such as META-DCL-001, or earlier roadmap forms containing RDM as an extra segment, must be explicitly qualified where historical or revised where they purport to prescribe the current working convention. Do not rewrite history as if the new convention had always existed.

Metadata Element IDs, document IDs, finding IDs, CHANGELOG numbers and Milestone IDs are separate entities. Creating this policy does not assign Metadata Element IDs or create element lifecycle/publication records.

## 5. Version, Revision, Status and Baseline

### 5.1. Received evidence

The 79 in-scope input documents declare Version 1.0 and Baseline 1.0; 73 declare Revision 0 and six Foundation documents do not declare Revision. Historical sources distinguish significant Version evolution from backward-compatible Revision changes: DF-FND-002 §6.6 and DF-FND-004 §§4.10/6.8. Neither establishes a complete numerical successor contract for this review. The following working rule formalizes that gap while preserving input evidence.

### 5.2. Edition successors

Version uses the observed major.minor numeric form. Revision is a monotonic integer per document across version changes during this review.

| Change | Version action | Revision action |
|---|---|---|
| Compatible correction/clarification/reclassification preserving contractual meaning | Keep Version. | Increment declared Revision by one; use 1 when absent. |
| Compatible additive contract capability | Increment minor by one. | Increment declared Revision by one; use 1 when absent. |
| Incompatible contract/convention change | Increment major by one and set minor to 0. | Increment declared Revision by one; use 1 when absent. |
| Validation/reporting with no source content change | Keep Version. | Keep Revision; track the event centrally. |
| New normalized review document | Initial Version 1.0. | Initial Revision 1; no invented Revision 0 history. |

Explain compatibility per UPDATE. Changing a classification label does not automatically change Version; replacing what a classification/schema contract permits may be incompatible even if no IDs change. Assess changes to identity syntax/resolution separately from a filename correction. Do not reset an existing Revision counter on Version changes during this review. Future alternative numbering requires a traceable policy change, not an implied reset.

Each completed persisted working edition with changed content receives its successor. Draft editing before an edition is finalized is preparation, not evidence of completed intermediate editions. If a validated/finalized edition needs a correction, create another successor and retain the failed validation event. No source revision is incremented merely to record this policy's adoption.

### 5.3. Working lifecycle and Baseline

Edited working documents start at Status=Draft, including successors of received Approved/Canonical documents. A subsequent explicit submission may use Review; formal approval/publication requires its own decision/evidence. Leave untouched source statuses unchanged. Canonical in a received header is preserved as historical evidence, not automatically granted to a successor or silently converted into Approved.

A newly created or modified working edition has Baseline=Not assigned unless its exact inclusion is evidenced. Record original Status and Baseline in the edition history and input manifest. Do not change the original Baseline snapshot. Draft is a lifecycle state; Not assigned is an explicit absence marker in the human-readable working header, not a new Baseline identifier.

This policy and DF-RVW-002 are Draft, Version 1.0, Revision 1, Baseline Not assigned. Passing their scoped checks does not approve/publish them or place them in a Baseline. The conventions for these working headers do not populate the canonical Metadata Dictionary or create a Metadata Profile lifecycle event by implication.

## 6. REVIEW, UPDATE, VALIDATE and evidence

Keep Step 1–7 and document substep numbers 4.01–4.87 stable. Step 3.1 identifies this policy; Step 3.2 identifies the consolidated report. The eight functional files keep their scheduled content/reference substeps but have no normalization requirement.

REVIEW reports findings, sections, severity, proposed correction and closure evidence without modifying the reviewed source. UPDATE shows exact material before/after, compatibility assessment, full updated source, diff, edition history, central CHANGELOG entry and Milestone. Mark source corrections pending validation. VALIDATE compares the exact updated edition with its input and affected sources, checks related occurrences and records outcome/limits with SHA-256 evidence. A failure creates a traceable corrective step.

Before any cross-document normative change or path/ID migration, identify the batch, rationale, affected documents and previous/new mapping. Do not claim integrated consistency during partial rollout. Resolve semantic references and actual dependencies separately; do not use a renamed relationship type to conceal a mandatory dependency cycle.

Finding states used for this review are Open, Corrected—pending validation, Closed—verified and Not applicable—scope decision. These tracking states are not document Status, element lifecycle or Milestone Status. Closure requires evidence; scope exclusion requires the specific decision. INV-02 is Not applicable because the user excluded the eight functional files, not because IDs were assigned or validation passed.

The input/final/validated manifests record paths, identity and edition where applicable, SHA-256 and scope. Evidence exports are attached to DF-RVW-002. A manifest's own hash belongs in its delivery receipt/enclosing package, not recursively inside its own contents. A document's hash is recorded outside the document itself. Validation logs do not force recursive revisions of themselves.

## 7. Central CHANGELOG and Milestones

Reuse CHANGELOG.md and ArchitecturalMilestones.md, retaining their historical content. They remain non-normalized. Keep the CHANGELOG's sequential #, reverse chronology, Author, Type, Document, Impact and Description columns. Add Reviewed and Validated event types to distinguish executed reviews/checks from document content updates; these event Types are not document Type values. Existing Created/Updated/etc. and impact values remain in force.

Use Author=Codex — AI assistant for entries executed by this assistant. Do not attribute the edit to the user merely because the user authorized it. For each update, record source path/ID, old/new edition, material change, finding, validation state, report/diff link and Milestone in the Description. Append a later validation event rather than rewriting a pending-validation update into a historical success. Do not log future intentions as completed changes.

Preserve M0–M7. Create M8–M14 for the review's verifiable results, with the existing Not Started/In Progress/Completed milestone states and O/S/C record states. A milestone's state derives from its own records for its declared work scope. Completion of a historical implementation milestone is not closure of a new review milestone.

M8 establishes the received corpus, including explicit limitations. M9 establishes this review's policy, artifact identities, central tracking and scoped checks. M10 covers Foundation cycles; M11 Architecture cycles; M12 the four input Documentation components; M13 localized identity/path/reference reconciliation; M14 integrated validation and final delivery. M9 excludes propagation into all domain sources, which is assigned to M10–M13.

No estimated completion date is invented. Completion dates are actual dates when criteria are satisfied. No new Blocked/Not applicable milestone state is introduced; describe blockers or non-applicable migration scope in the relevant milestone's evidence. A review Milestone=Completed means its documentary criteria were met, not approval, publication, release or Baseline membership.

## 8. Downstream reconciliation and limits

The policy becomes the operating convention for the review under the user's instructions. Framework source reconciliation remains pending in the stable plan: FND-004/FND-001/FND-006 for foundations and historical qualification; ARC-003/004/005/007/006 for concepts, allocation and documentation conventions; DID-005/010/014 for identity; CLS-002/003/004/005/007/013/014 for classification; MTD-003/004/005/013/014 for definitions, schemas and profiles; RDM-001/002 and component roadmaps for planning. Other affected consumers are included in their document cycles.

This policy establishes process rules and the scoped use of current field names without declaring that their Metadata Element definitions/profile contracts already exist canonically. Dictionary/profile gaps, the CLS collision, DID schema differences, dependency ambiguity and other input findings remain Open. DF-RVW-002 provides evidence, mapping and progress; this policy does not replace any domain specification or perform its full validation.

## 9. Sources

- Load-Review-Context.md, edition 4: user-adopted rules, normalized-file exclusion, stepwise review, artifact and central tracking requirements. The instruction file remains a session input outside the Framework corpus.
- DF-FND-002 §6.6: Version versus compatible Revision evolution.
- DF-FND-004 §§4.5–4.11 and 6.3–6.8: working state, versioning and Baseline distinctions.
- DF-FND-006 §6.8: document Revision versus collective Baseline.
- DF-ARC-005 §6.3: existing Reviews component and responsibilities.
- DF-ARC-007 §§5–10/14: documentation categories by responsibility; adoption here does not prove complete Reviews component specification.
- DF-DID-005 §§3–9 and DF-DID-010 §§4–9: identity, domain, uniqueness and references; corpus representation contract pending source reconciliation.
- DF-RDM-001 §§1–4 and DF-RDM-002 §§1–4: global planning area and evolution strategy.
- Received CHANGELOG.md and ArchitecturalMilestones.md: historical formats, entry and milestone conventions, preserved in the input manifest.

## 10. Edition history

| Date | Version | Revision | Event | Scope and lifecycle |
|---|---|---|---|---|
| 2026-09-30 | 1.0 | 1 | Created at Step 3.1 | Initial working review policy; no previous edition; Draft; Baseline Not assigned. Scoped validation is logged centrally without changing this edition. |
