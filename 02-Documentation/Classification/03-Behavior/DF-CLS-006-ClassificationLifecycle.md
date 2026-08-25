# Documentation Framework

# DF-CLS-006 — Classification Lifecycle

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-006 |
| **Title** | Classification Lifecycle |
| **Family** | Classification |
| **Type** | Behavior |
| **Component** | Classification |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Classification component defines the semantic organization of documents through the elements:

- Family;
- Type;
- Class.

The Classification Schema defines their structural representation.

Classification itself is not static.

As the Documentation Framework evolves, classification definitions may be introduced, refined, superseded, or removed from active use.

This document defines the conceptual lifecycle of Classification definitions.

The lifecycle described here concerns the **evolution of the Classification system**.

It must therefore be distinguished from the lifecycle of an individual document.

The architectural model identifies Lifecycle as a separate Metadata category describing the evolutionary state of a document, including properties such as Version, Revision and Status.

---

# 2. Purpose

The purpose of this document is to define how Classification definitions evolve over time.

It establishes:

- what constitutes a Classification definition;
- the lifecycle of a classification definition;
- the distinction between definition lifecycle and document lifecycle;
- the conceptual transitions through which classification definitions may evolve;
- the effect of lifecycle changes on existing classifications;
- the preservation of historical classification meaning.

The lifecycle provides the temporal dimension necessary for controlled evolution of Classification.

---

# 3. Scope

This document applies to the lifecycle of:

- Family definitions;
- Type definitions;
- Class definitions;
- classification values;
- classification relationships;
- classification schema definitions.

It does not define:

- document Version;
- document Revision;
- document Status;
- Workflow states;
- classification validation rules;
- classification governance authorities;
- classification constraints;
- formal serialization.

Document lifecycle properties such as Version, Revision and Status belong to the document Lifecycle category and are used by Workflow.

---

# 4. Classification Lifecycle Concept

A Classification definition is a semantic definition that gives meaning to a classification element or value.

For example:

```text id="cls-lc-001"

            Family
            │
            └── META

```

or:

```text id="cls-lc-002"

            Type
            │
            └── DCL

```

The lifecycle governs the evolution of these definitions.

Conceptually:

```text id="cls-lc-003"

        Classification Definition
                    │
                    ▼

                Lifecycle
                │
                ├── Definition
                ├── Active Use
                ├── Deprecation
                └── Retirement

```

The exact normative state vocabulary is not established by the current source material; the states above therefore represent the lifecycle model proposed by this document.

---

# 5. Classification Lifecycle versus Document Lifecycle

The two concepts must remain separate.

The document lifecycle describes the evolution of a document:

```text id="cls-lc-004"

            Document
            │
            └── Lifecycle
                ├── Version
                ├── Revision
                └── Status

```

The Classification lifecycle describes the evolution of classification definitions:

```text id="cls-lc-005"

            Classification Definition
            │
            └── Lifecycle

```

Therefore:

```text id="cls-lc-006"

        Document Lifecycle

                ≠

    Classification Lifecycle

```

This distinction follows the architectural separation of responsibilities established by the framework. Metadata categories group related properties and no component replaces another.

---

# 6. Classification Definitions

A Classification definition may describe:

- a Family;
- a Type;
- a Class;
- a classification value;
- a classification relationship;
- a schema element.

Conceptually:

```text id="cls-lc-007"

            Classification Definition
            │
            ├── Element Definition
            │
            └── Value Definition

```

The lifecycle applies to the definition rather than to every document that uses the definition.

---

# 7. Lifecycle Subject

The subject of the Classification Lifecycle is therefore:

```text id="cls-lc-008"

    Classification Definition

```

and not:

```text id="cls-lc-009"

    Document

```

A document may continue to exist while the classification definition assigned to it changes lifecycle state.

---

# 8. Lifecycle Dimensions

The Classification Lifecycle can be considered along two related dimensions:

```text id="cls-lc-010"

            Definition Lifecycle
            │
            └── controls semantic availability

            Document Classification
            │
            └── records classification usage

```

The first concerns the classification system.

The second concerns documents classified using that system.

These responsibilities must not be conflated.

---

# 9. Initial Definition

A classification definition begins when its semantic meaning is established.

Conceptually:

```text id="cls-lc-011"

                Undefined
                    │
                    ▼

                 Defined

```

At this point the definition exists conceptually but is not necessarily available for normal classification use.

The distinction between defining a concept and using it is important for controlled evolution.

---

# 10. Definition State

A definition is considered **Defined** when its semantic identity and meaning have been established.

For example:

```text id="cls-lc-012"

    Family
    Name:        META
    Definition:  <authoritative definition>

```

or:

```text id="cls-lc-013"

    Type
    Name:        DCL
    Family:      META
    Definition:  <authoritative definition>

```

The Classification Dictionary is responsible for authoritative terminology and definitions.

---

# 11. Activation

A defined classification may become available for use.

Conceptually:

```text id="cls-lc-014"

                 Defined
                    │
                    ▼

                  Active

```

An **Active** classification definition is available for use in new Classification assignments.

The framework's existing material establishes the need for controlled and stable classification, but does not define a formal activation state. Therefore, `Active` is introduced here as the lifecycle concept required to distinguish a definition from one currently available for use.

---

# 12. Active Classification

An Active classification definition may be used to classify documents.

Conceptually:

```text id="cls-lc-015"

            Active Definition
                    │
                    ▼

         Document Classification

```

For example:

```text id="cls-lc-016"

    Family  =  META
    Type    =  DCL

```

The use of `META` and `DCL` follows the classification structure documented by the framework. The Document ID example `META-DCL-001` explicitly identifies `META` as Family and `DCL` as Type.

---

# 13. Modification

A classification definition may require refinement.

Conceptually:

```text id="cls-lc-017"

                  Active
                    │
                    ▼

                Modified
                    │
                    ▼

                  Active

```

Modification may affect:

- definition wording;
- documentation;
- relationships;
- constraints;
- permitted usage.

Modification must not silently change the semantic identity of an existing classification.

The architectural evolution principle establishes that new properties may be introduced provided existing meanings are not altered and compatibility is maintained.

---

# 14. Semantic Change

A change to the meaning of an existing classification is different from a documentation correction.

For example:

```text id="cls-lc-018"

    Definition Correction

```

may preserve the semantic meaning.

Whereas:

```text id="cls-lc-019"

    Semantic Redefinition

```

changes what the classification means.

A semantic redefinition must therefore be treated as a controlled lifecycle event.

---

# 15. Deprecation

A classification definition may cease to be recommended for new use.

Conceptually:

```text id="cls-lc-020"

                  Active
                    │
                    ▼

                Deprecated

```

A **Deprecated** classification remains historically meaningful but should no longer normally be selected for new classifications.

Deprecation is therefore different from deletion.

```text id="cls-lc-021"

    Deprecated  ≠  Deleted

```

The existing architectural material establishes preservation of identity and historical continuity; it does not establish a formal classification deprecation state. The state is therefore introduced here as part of the lifecycle model rather than presented as an already-established framework rule.

---

# 16. Deprecated Classifications

A deprecated classification may remain associated with existing documents.

For example:

```text id="cls-lc-022"

            Existing Document
            │
            └── Classification
                └── Deprecated Value

```

The historical classification should not automatically become invalid merely because the definition is deprecated.

This preserves the historical meaning of documents.

---

# 17. Retirement

A classification definition may eventually cease to be part of the active Classification vocabulary.

Conceptually:

```text id="cls-lc-023"

                Deprecated
                    │
                    ▼

                 Retired

```

Retirement means that the definition is no longer available for ordinary new classification.

It does not imply that historical references must be erased.

---

# 18. Retirement versus Deletion

Retirement and deletion are distinct concepts.

```text id="cls-lc-024"

            Retirement
            │
            └── definition remains historically known

            Deletion
            │
            └── definition is removed

```

The framework's emphasis on stable identity and preservation of knowledge favors retaining historical semantic information rather than silently removing it.

The Research Journal explicitly establishes that document identity remains permanent even when title, content or organization changes.

---

# 19. Proposed Lifecycle

The conceptual lifecycle is:

```text id="cls-lc-025"

            ┌───────────────┐
            │    Defined    │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │    Active     │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │  Deprecated   │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │    Retired    │
            └───────────────┘

```

Modification may occur while a definition is active:

```text id="cls-lc-026"

            Active
            │
            └──►  Modified  ───►  Active

```

The exact transition rules remain subject to Classification Governance.

---

# 20. Lifecycle States

The proposed states are:

| State | Meaning |
|-------|---------|
| **Defined** | Semantic definition has been established |
| **Active** | Definition is available for normal use |
| **Deprecated** | Definition remains valid historically but should not normally be used for new classifications |
| **Retired** | Definition is no longer available for normal use |

These states describe the lifecycle of the **classification definition**, not the lifecycle status of a document.

---

# 21. Defined State

A classification is in the Defined state when:

- its identity has been established;
- its semantic meaning has been documented;
- its relationship to other classification concepts has been established where required.

Conceptually:

```text id="cls-lc-027"

            Defined
            │
            ├── Identity
            ├── Meaning
            └── Definition

```

---

# 22. Active State

A classification is Active when it is authorized for ordinary classification use.

Conceptually:

```text id="cls-lc-028"

            Active
            │
            ├── Available for use
            ├── Discoverable
            └── Valid classification target

```

The specific authority responsible for activation is outside the scope of this document.

---

# 23. Deprecated State

A classification is Deprecated when it remains part of the historical classification vocabulary but is no longer recommended for new use.

Conceptually:

```text id="cls-lc-029"

            Deprecated
            │
            ├── Historically valid
            ├── Existing references preserved
            └── New use discouraged

```

A deprecated value should therefore remain interpretable.

---

# 24. Retired State

A classification is Retired when it has reached the end of its active lifecycle.

Conceptually:

```text id="cls-lc-030"

            Retired
            │
            ├── Not available for new use
            └── Historical meaning preserved

```

Retirement should not automatically imply removal from historical records.

---

# 25. Lifecycle and Existing Documents

The lifecycle of a Classification definition must not retroactively alter the identity of documents.

For example:

```text id="cls-lc-031"

            Document
            │
            ├── Document Identity
            │
            └── Classification
                │
                └── Value

```

If the classification value later becomes Deprecated:

```text id="cls-lc-032"

            Document
            │
            ├── Document Identity
            │
            └── Historical Classification
                │
                └── Deprecated Value

```

The document remains the same document.

This follows the established principle that document identity is permanent and independent of name, version, revision and location.

---

# 26. Lifecycle and Document Identity

Classification lifecycle transitions must never change Document Identity.

Therefore:

```text id="cls-lc-033"

     Classification Lifecycle Change
                    │
                    ▼

            Document Identity
            │
            └── unchanged

```

This is particularly important where classification changes occur as the framework evolves.

---

# 27. Lifecycle and Document Version

A change to a classification definition is not automatically a change to a document Version.

Document Version is part of the document Lifecycle and is separate from Classification.

Conceptually:

```text id="cls-lc-034"

         Classification Lifecycle
                    │
               independent
                    │
                    ▼

            Document Lifecycle

```

The existing architecture explicitly places Version, Revision and Status in the document Lifecycle category.

---

# 28. Lifecycle and Document Revision

Similarly, a change in Classification definition does not automatically constitute a document Revision.

Revision belongs to the document lifecycle.

The Classification lifecycle governs classification definitions.

Therefore:

```text id="cls-lc-035"

         Classification Revision

                    ≠

            Document Revision

```

Any operational rule connecting the two must be established by Workflow or Governance rather than assumed by the Classification component.

---

# 29. Lifecycle and Document Status

Document Status is also distinct from the lifecycle state of a Classification definition.

For example:

```text id="cls-lc-036"

    Classification  =  Active
    Document        =  Draft

```

is conceptually possible.

Likewise:

```text id="cls-lc-037"

    Classification  =  Deprecated
    Document        =  Approved

```

may be historically valid.

The framework's source material identifies Status as a document lifecycle property, not a Classification property.

---

# 30. Classification Lifecycle and Workflow

The architectural model states that Lifecycle properties of documents are used directly by Workflow.

The Classification Lifecycle should similarly remain conceptually independent from Workflow.

Workflow may operationally support lifecycle transitions, but Workflow does not define the semantic meaning of Classification states.

Conceptually:

```text id="cls-lc-038"

         Classification Lifecycle
                    │
                    ▼

            Defines lifecycle
                    │
                    ▼

    Workflow
        may operationalize transitions

```

---

# 31. Lifecycle and Governance

Classification lifecycle transitions require governance.

For example:

```text id="cls-lc-039"

                 Defined
                    │
            governed decision
                    │
                    ▼

                  Active

```

and:

```text id="cls-lc-040"

                  Active
                    │
            governed decision
                    │
                    ▼

                Deprecated

```

The detailed authorities, approval mechanisms and responsibilities belong to **DF-CLS-008 — Classification Governance**.

---

# 32. Lifecycle and Validation

Validation must recognize lifecycle state when determining whether a classification may be used.

Conceptually:

```text id="cls-lc-041"

          Classification Value
                    │
                    ▼

             Lifecycle State
                    │
                    ▼

                Validation

```

For example, a Deprecated value may remain valid for historical documents while being invalid for new classification assignments.

The exact validation rules belong to **DF-CLS-007 — Classification Validation**.

---

# 33. Lifecycle and Constraints

Lifecycle states may impose constraints on classification use.

Conceptually:

```text id="cls-lc-042"

             Lifecycle State
                    │
                    ▼

            Usage Constraints

```

The formal constraints belong to **DF-CLS-010 — Classification Constraints**.

This document defines the lifecycle semantics, not the complete constraint system.

---

# 34. Lifecycle and Dictionary

The Classification Dictionary is expected to provide authoritative definitions for Classification terminology.

The lifecycle therefore affects the dictionary's entries.

Conceptually:

```text id="cls-lc-043"

            Classification Dictionary
            │
            └── Definition
                │
                └── Lifecycle State

```

A deprecated or retired definition should remain identifiable in historical documentation where necessary.

---

# 35. Lifecycle and Schema

The Classification Schema defines the structure:

```text id="cls-lc-044"

            Classification
            ├── Family
            ├── Type
            └── Class

```

The lifecycle defines how definitions associated with that schema evolve.

Therefore:

```text id="cls-lc-045"

            Schema
            │
            └── structure

            Lifecycle
            │
            └── evolution

```

Neither replaces the other.

---

# 36. Lifecycle of Family

A Family follows the general Classification Lifecycle.

Conceptually:

```text id="cls-lc-046"

            Family Definition
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active
                    │
                    ▼

               Deprecated
                    │
                    ▼

                 Retired

```

Because a Family provides a broad documentary domain, changes to its meaning may affect multiple Types.

Such changes therefore require particular care.

---

# 37. Lifecycle of Type

A Type follows the same general lifecycle.

Conceptually:

```text id="cls-lc-047"

             Type Definition
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

Because Type specializes Family, changes to a Family may affect the interpretation of associated Types.

---

# 38. Lifecycle of Class

A Class also follows the general lifecycle.

Conceptually:

```text id="cls-lc-048"

             Class Definition
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

The current framework material establishes Class as representing the nature of a document but does not define a complete Class vocabulary.

---

# 39. Lifecycle of Classification Values

A Classification value has a lifecycle independently of the documents that use it.

For example:

```text id="cls-lc-049"

            META
            │
            ├── Definition
            ├── Active Use
            ├── Deprecation
            └── Retirement

```

The value's lifecycle determines whether it remains available for new classifications.

---

# 40. Historical Preservation

Historical classification information should remain interpretable after a definition becomes Deprecated or Retired.

This is especially important because the framework is intended to preserve knowledge over time.

Conceptually:

```text id="cls-lc-050"

    Current Classification Vocabulary
                    │
                 evolves
                    │
                    ▼

    Historical Classification Vocabulary
    │
    └── preserved

```

This principle is consistent with the framework's treatment of permanent document identity and controlled evolution.

---

# 41. Replacement of Classifications

When a classification is Deprecated, a replacement may be introduced.

Conceptually:

```text id="cls-lc-051"

           Old Classification
                    │
                deprecated
                    │
                    ▼

            New Classification

```

However, this does not mean that the new classification automatically replaces every historical occurrence.

Replacement rules depend on:

- semantic compatibility;
- document context;
- migration requirements;
- governance decisions.

Those rules are outside the scope of this document.

---

# 42. Classification Migration

Migration may be required when an existing classification is replaced.

Conceptually:

```text id="cls-lc-052"

           Existing Documents
                    │
                    ▼

           Migration Analysis
                    │
                    ▼

           New Classification

```

Migration must preserve the original document identity.

The framework establishes that the identifier remains stable even when the content evolves or the document is reorganized.

---

# 43. Automatic Migration

This document does not establish that classification migration should be automatic.

An automatic migration mechanism would require:

- explicit mapping rules;
- semantic equivalence;
- validation;
- governance approval.

These subjects belong to subsequent Classification documents.

---

# 44. Lifecycle History

A classification definition should have an evolution history when lifecycle transitions occur.

Conceptually:

```text id="cls-lc-053"

            Classification Definition
            │
            ├── Defined
            ├── Activated
            ├── Modified
            ├── Deprecated
            └── Retired

```

The history allows the framework to understand not only the current meaning but also how that meaning evolved.

---

# 45. Immutable Historical Meaning

Once a classification value has been used in an authoritative document context, its historical meaning should not be silently rewritten.

Instead:

```text id="cls-lc-054"

            Historical Definition
            │
            └── preserved

```

and:

```text id="cls-lc-055"

            New Meaning
            │
            └── new definition or controlled evolution

```

This protects the interpretability of historical documentation.

---

# 46. Lifecycle and Compatibility

Classification evolution should preserve compatibility whenever possible.

The framework's architectural evolution explicitly favors incremental growth while preserving existing meanings and compatibility.

Therefore:

- additive changes are preferred where possible;
- semantic changes require control;
- deprecated definitions should remain interpretable;
- historical references should not become ambiguous.

---

# 47. Lifecycle Invariants

The following invariants apply conceptually:

1. Classification lifecycle is distinct from document lifecycle.
2. Classification lifecycle does not modify Document Identity.
3. Family, Type and Class retain their established semantic responsibilities.
4. A deprecated classification remains historically identifiable.
5. Retirement does not imply automatic historical deletion.
6. Lifecycle transitions require controlled governance.
7. Classification lifecycle state does not replace document Status.
8. Classification lifecycle does not replace document Version or Revision.
9. Historical classification meaning should remain interpretable.
10. Changes to classification meaning must not occur silently.

---

# 48. Proposed State Model

The complete proposed state model is:

```text id="cls-lc-056"

             ┌──────────────┐
             │    Defined   │
             └──────┬───────┘
                    │
                    ▼
             ┌──────────────┐
             │    Active    │
             └──────┬───────┘
                    │
                    ▼
             ┌──────────────┐
             │  Deprecated  │
             └──────┬───────┘
                    │
                    ▼
             ┌──────────────┐
             │   Retired    │
             └──────────────┘

    Active  ───►  Modified  ───►  Active

```

This is the conceptual lifecycle proposed by this document.

The exact transition rules remain to be established by Classification Governance.

---

# 49. Lifecycle Model

The relationship between Classification and its lifecycle can therefore be summarized as:

```text id="cls-lc-057"

              Classification
                    │
                    ▼

        Classification Definition
                    │
                    ▼

                Lifecycle
                │
                ├── Defined
                ├── Active
                ├── Deprecated
                └── Retired

```

---

# 50. Separation of Concerns

The Classification architecture now has a clear separation:

```text id="cls-lc-058"

                DF-CLS-003
           Classification Model
                    │
                    ▼

                DF-CLS-004
         Classification Elements
                    │
                    ▼

                DF-CLS-005
          Classification Schema
                    │
                    ▼

                DF-CLS-006
         Classification Lifecycle

```

Each document addresses a different concern.

---

# 51. Relationship with Subsequent Documents

The lifecycle defined here provides the foundation for:

- **DF-CLS-007 — Classification Validation**;
- **DF-CLS-008 — Classification Governance**;
- **DF-CLS-010 — Classification Constraints**;
- **DF-CLS-011 — Classification Extensibility**;
- **DF-CLS-013 — Classification Dictionary**;
- **DF-CLS-014 — Classification Specification**;
- **DF-CLS-015 — Classification Examples**.

In particular:

```text id="cls-lc-059"

            Lifecycle
            │
            ├── Validation
            ├── Governance
            ├── Constraints
            └── Dictionary

```

---

# 52. What This Document Does Not Establish

The following are intentionally not defined here:

- authoritative lifecycle state names beyond the conceptual proposal;
- transition authorization;
- approval roles;
- mandatory lifecycle metadata;
- automatic migration;
- replacement mappings;
- exact validation rules;
- exact persistence representation;
- complete Classification vocabulary.

These subjects belong to subsequent Classification documents or to the appropriate architectural components.

---

# 53. Conformance

A Classification lifecycle implementation conforms conceptually to this document when it:

- distinguishes Classification lifecycle from Document lifecycle;
- supports controlled evolution of classification definitions;
- recognizes the distinction between active, deprecated and retired definitions;
- preserves historical classification meaning;
- does not alter Document Identity as a consequence of Classification lifecycle changes;
- does not confuse classification lifecycle state with document Status;
- supports controlled evolution of Family, Type and Class definitions.

---

# 54. Summary

Classification is not only a static structure.

Its definitions evolve as the Documentation Framework evolves.

The conceptual lifecycle is:

```text id="cls-lc-060"

                 Defined
                    │
                    ▼

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

with controlled modification possible while active:

```text id="cls-lc-061"

                  Active
                    │
                    ▼

                 Modified
                    │
                    ▼

                  Active

```

The lifecycle applies to Classification definitions rather than to documents themselves.

The distinction is fundamental:

```text id="cls-lc-062"

            Classification Lifecycle
            │
            └── evolves classification definitions

            Document Lifecycle
            │
            ├── Version
            ├── Revision
            └── Status

```

The architectural sources explicitly establish Version, Revision and Status as document lifecycle properties used by Workflow.

Classification lifecycle must also preserve historical meaning and must never alter Document Identity.

This establishes the temporal foundation required by the remaining Classification documents.

---

# 55. Related Documents

## 55.1. Foundation

- DF-FND-001 — Framework Manifest
- DF-FND-002 — Research Journal
- DF-FND-003 — Evolution Timeline
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

## 55.2. Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-004 — Architectural Layers
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology
- DF-ARC-007 — Component Documentation Structure

## 55.3. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema

## 55.4. Classification

- DF-CLS-001 — Classification Architecture
- DF-CLS-002 — Classification Concepts
- DF-CLS-003 — Classification Model
- DF-CLS-004 — Classification Elements
- DF-CLS-005 — Classification Schema
- **DF-CLS-006 — Classification Lifecycle**
- DF-CLS-007 — Classification Validation
- DF-CLS-008 — Classification Governance
- DF-CLS-009 — Classification Relationships
- DF-CLS-010 — Classification Constraints
- DF-CLS-011 — Classification Extensibility
- DF-CLS-012 — Classification Best Practices
- DF-CLS-013 — Classification Dictionary
- DF-CLS-014 — Classification Specification
- DF-CLS-015 — Classification Examples

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of the Classification Lifecycle. |

---

**End of Document**