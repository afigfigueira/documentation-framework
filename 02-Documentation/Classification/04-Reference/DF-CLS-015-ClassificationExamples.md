# Documentation Framework

# DF-CLS-015 — Classification Examples

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-015 |
| **Title** | Classification Examples |
| **Family** | Classification |
| **Type** | Reference |
| **Component** | Classification |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

This document provides examples illustrating the application of the Classification component of the Documentation Framework.

The examples demonstrate how the concepts, elements, schema, lifecycle, validation, governance, relationships, constraints and extensibility mechanisms defined by the Classification documentation family may be applied.

The examples are intentionally illustrative.

They do not define additional Classification requirements.

Where an example appears to conflict with a normative requirement, the applicable normative document takes precedence.

---

# 2. Purpose

The purpose of this document is to provide concrete examples of Classification usage.

The examples support:

- understanding the Classification model;
- understanding Classification terminology;
- illustrating Classification structures;
- demonstrating Classification assignments;
- demonstrating relationships;
- demonstrating validation;
- demonstrating lifecycle transitions;
- demonstrating governance;
- demonstrating extensibility;
- illustrating correct and incorrect Classification practices.

---

# 3. Scope

This document covers examples of:

- Classification Elements;
- Classification hierarchies;
- Classification assignments;
- Classification relationships;
- Classification schemas;
- Classification constraints;
- lifecycle states;
- validation;
- governance;
- extensions;
- terminology;
- historical Classification.

The examples are technology independent.

No particular implementation mechanism is assumed.

---

# 4. Example Conventions

The examples use a fictional documentation environment.

The fictional environment contains documentation concerning:

- architecture;
- development;
- testing;
- deployment;
- governance.

The names used in the examples are illustrative and shall not be interpreted as canonical Classification Elements of the Documentation Framework unless they are explicitly defined by the normative Classification documentation.

---

# 5. Example 1 — Basic Classification

Consider a document describing the architectural structure of a software system.

The document may be assigned to a Classification Element representing architecture.

Conceptually:

```text

                 Document
                    │
                    ▼

        Classification Assignment
                    │
                    ▼

               Architecture

```

The Classification assignment establishes that the document belongs to the semantic category represented by `Architecture`.

The document's physical location does not determine this Classification.

For example, the document could be stored at:

```text

    /docs/architecture.md

```

or:

```text

    /project/design/system-architecture.md

```

without changing its Classification.

---

# 6. Example 2 — Hierarchical Classification

A Classification hierarchy may be represented as:

```text

            Documentation
            │
            ├── Architecture
            │   ├── Principles
            │   ├── Concepts
            │   └── Design
            │
            ├── Development
            │   ├── Coding
            │   ├── Testing
            │   └── Build
            │
            └── Operations
                ├── Deployment
                ├── Monitoring
                └── Maintenance

```

In this example:

- `Documentation` is a broader Classification Element;
- `Architecture` is a specialization;
- `Principles` is a further specialization of `Architecture`;
- `Concepts` is a further specialization of `Architecture`.

The hierarchy expresses semantic specialization.

It is not merely a directory structure.

---

# 7. Example 3 — Parent and Child Elements

Consider:

```text

            Architecture
            │
            └── Architectural Principles

```

Here:

```text

    Parent =  Architecture
    Child  =  Architectural Principles

```

The child represents a more specific semantic concept than the parent.

A valid hierarchical relationship therefore expresses:

```text

            Architectural Principles

             IS A SPECIALIZATION OF

                  Architecture

```

It would not be appropriate to create the relationship merely because the two documents happen to be stored in the same directory.

---

# 8. Example 4 — Classification Elements

A fictional Classification model may contain:

| Identifier | Name | Parent |
|------------|------|--------|
| CLS-ARCH | Architecture | — |
| CLS-ARCH-PRN | Architectural Principles | CLS-ARCH |
| CLS-ARCH-CON | Architectural Concepts | CLS-ARCH |
| CLS-DEV | Development | — |
| CLS-DEV-TST | Testing | CLS-DEV |

The identifiers provide stable identity.

The names provide human-readable terminology.

The parent relationship provides semantic structure.

---

# 9. Example 5 — Classification Assignment

Suppose the following document exists:

```text

    Document ID: DOC-001
    Title: Architectural Principles

```

The document may receive:

```text

    Classification:
        Architecture

```

The assignment can conceptually be represented as:

```text

            DOC-001
            │
            └── classified-as ──► Architecture

```

The Classification assignment does not change the identity of `DOC-001`.

It provides semantic categorization.

---

# 10. Example 6 — Multiple Classification Assignments

A document may legitimately participate in more than one Classification context when the Classification Schema permits multiple assignments.

For example:

```text

    Document: Testing Strategy

```

may be associated with:

```text

    Development
    Testing
    Quality

```

Conceptually:

```text

                             ┌─────►  Development
                             │
            Testing Strategy ├─────►  Testing
                             │
                             └─────►  Quality

```

Whether multiple assignments are permitted is determined by the applicable Classification Schema and Constraints.

This example therefore demonstrates a possible use, not a universal rule.

---

# 11. Example 7 — Classification and Document Identity

Consider:

```text

    Document ID: DF-CLS-015
    Title: Classification Examples
    Classification: Classification

```

The two concepts have different responsibilities.

```text

            Document Identity
            │
            └── identifies the document

            Classification
            │
            └── categorizes the document

```

Changing the Classification does not create a different document identity.

Likewise, changing the document identity does not automatically redefine its Classification.

---

# 12. Example 8 — Classification and Metadata

Consider a document with the following metadata:

```text

    Document ID: DOC-017
    Title: Deployment Architecture
    Author: Example Author
    Status: Approved
    Classification: Architecture

```

The fields have different responsibilities.

```text

    Document ID
        ─────►  identifies the document

    Title
        ─────►  names the document

    Author
        ─────►  provides descriptive information

    Status
        ─────►  represents lifecycle information

    Classification
        ─────►  provides semantic categorization

```

Classification should not be used as a replacement for general Metadata.

---

# 13. Example 9 — Classification Schema

A simplified Classification Schema might specify:

```text

    ClassificationElement
        Identifier
        Name
        Definition
        Parent
        LifecycleState

```

A document assignment may then be represented conceptually as:

```text

    ClassificationAssignment
        Document
        ClassificationElement

```

The schema defines the permitted structure.

It does not define the meaning of every individual Classification Element.

That meaning is provided by the applicable definitions.

---

# 14. Example 10 — Cardinality Constraint

Suppose a Classification Schema specifies:

```text

    Document
        ClassificationElement
            Cardinality:  1..*

```

This means that every classified document must have at least one Classification assignment.

For example:

```text

            Document A
            ├── Architecture
            └── Design

```

satisfies the example cardinality.

A document with:

```text

            Document B
            └── no Classification

```

does not satisfy it.

The actual cardinality applicable to a Classification implementation is determined by its normative Schema and Constraints.

---

# 15. Example 11 — Invalid Classification Reference

Suppose a document contains:

```text

    Classification: UnknownCategory

```

but `UnknownCategory` is not defined by the Classification Schema.

The assignment is invalid.

Conceptually:

```text

                 Document
                    │
                    ▼

             UnknownCategory
                    │
                    X

               Not defined

```

Validation should detect the invalid reference.

---

# 16. Example 12 — Invalid Hierarchy

Consider:

```text

            Architecture
            │
            └── Testing

```

If the Classification Model defines `Testing` as belonging to `Development`, then assigning it directly beneath `Architecture` may violate the applicable structural or semantic constraints.

The problem is not necessarily the names.

The problem is that the relationship does not conform to the defined Classification Model.

---

# 17. Example 13 — Semantic Duplication

Consider two Classification Elements:

```text

    CLS-001 — Architecture
    CLS-002 — System Architecture

```

Suppose both are defined as:

> Documentation describing the architectural structure of a system.

If no meaningful semantic distinction exists, the model contains potential semantic duplication.

The preferred approach is to determine whether:

- the concepts are genuinely different;
- one should be a specialization of the other;
- one is a synonym;
- one should be removed.

The Classification Dictionary should record the resulting canonical terminology.

---

# 18. Example 14 — Meaningful Specialization

Consider:

```text

            Architecture
            │
            ├── Software Architecture
            │
            └── Deployment Architecture

```

This can be a meaningful hierarchy because the concepts have distinguishable semantic scopes.

The parent expresses a broader concept.

The children express specific architectural domains.

---

# 19. Example 15 — Non-Hierarchical Relationship

Not every relationship between Classification Elements is hierarchical.

Consider:

```text

            Security
            │
            └── related-to ──► Compliance

```

The relationship indicates semantic association.

It does not imply:

```text

    Security IS A Compliance

```

or:

```text

    Compliance IS A Security

```

The relationship type therefore matters.

---

# 20. Example 16 — Relationship Definition

A relationship may be defined conceptually as:

```text

    Relationship Type:
        related-to

    Source:
        Security

    Target:
        Compliance

    Meaning:
        Security and Compliance are semantically associated.

```

This is an explicit relationship.

Its semantics do not need to be inferred from document location or naming conventions.

---

# 21. Example 17 — Lifecycle

A Classification Element may progress through a controlled lifecycle:

```text

                 Proposed
                    │
                    ▼

                 Defined
                    │
                    ▼

                 Approved
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

For example:

```text

    Architecture
        State: Active

```

Later:

```text

    Architecture
        State: Deprecated

```

Eventually:

```text

    Architecture
        State: Retired

```

The exact lifecycle and permitted transitions are defined by the Classification Lifecycle.

---

# 22. Example 18 — Deprecating a Classification Element

Suppose:

```text

    CLS-OLD — Technical Documentation

```

is replaced by more precise categories:

```text

    Architecture
    Development
    Operations

```

The old element may become:

```text

    Lifecycle State: Deprecated

```

New documents should use the replacement elements.

Existing documents may continue to retain the historical classification where required for traceability.

---

# 23. Example 19 — Retired Classification Element

Suppose:

```text

    CLS-OLD — Technical Documentation

```

eventually becomes:

```text

    Lifecycle State: Retired

```

Historical assignments may still contain:

```text

    Classification: CLS-OLD

```

provided that the historical information is preserved.

Retirement therefore does not necessarily mean deletion.

---

# 24. Example 20 — Validation

Consider the following Classification:

```text

    Document:
        DOC-100

    Classification:
        Architecture

    Architecture:
        Design

```

Validation may evaluate:

```text

    [PASS] Classification Element exists
    [PASS] Parent exists
    [PASS] Hierarchical relationship is valid
    [PASS] Cardinality satisfied
    [PASS] Lifecycle state valid

```

The resulting Classification is conformant with the tested rules.

---

# 25. Example 21 — Validation Failure

Consider:

```text

    Document:
        DOC-101

    Classification:
        Unknown

```

Validation may produce:

```text

    [FAIL] Classification Element does not exist

```

A second example may be:

```text

            Architecture
            │
            └── Testing

```

where the hierarchy violates the Classification Schema.

Validation may produce:

```text

    [FAIL] Invalid parent-child relationship

```

Validation identifies the violation.

It does not silently modify the Classification.

---

# 26. Example 22 — Classification Constraint

Suppose the Classification model defines:

```text

    A child element shall have exactly one parent.

```

The following structure is therefore invalid:

```text

             Architecture
             │
             ├── Design
             │
             └── Testing

                    ▲
                    │
       Development ─┘

```

if `Testing` is required to have exactly one parent.

The constraint prevents ambiguous hierarchy.

---

# 27. Example 23 — Governance of a New Element

Suppose a new concept is proposed:

```text

    AI Architecture

```

A controlled governance process may be:

```text

                 Proposal
                    │
                    ▼

             Semantic Review
                    │
                    ▼

               Model Review
                    │
                    ▼

            Constraint Review
                    │
                    ▼

                 Approval
                    │
                    ▼

             Dictionary Entry
                    │
                    ▼

      Active Classification Element

```

The element becomes canonical only after the applicable governance process has approved it.

---

# 28. Example 24 — Rejected Classification Proposal

Suppose the proposed element is:

```text

    Software Docs

```

A review determines that the concept duplicates an existing element:

```text

    Software Documentation

```

The proposal may therefore be rejected.

The rejection preserves semantic consistency by preventing unnecessary duplication.

---

# 29. Example 25 — Classification Extension

Suppose the core Classification contains:

```text

            Development
            │
            ├── Coding
            └── Testing

```

An extension introduces:

```text

            Development
            │
            ├── Coding
            ├── Testing
            └── Build

```

This can be a valid extension if:

- `Build` represents a distinct concept;
- the extension point permits it;
- the schema permits it;
- constraints remain satisfied;
- governance requirements are met.

The extension does not redefine `Coding` or `Testing`.

---

# 30. Example 26 — Invalid Extension

Suppose an extension attempts to redefine:

```text

    Testing

```

from:

> Activities concerned with verifying software behavior.

to:

> All activities related to software development.

This is not merely an extension.

It changes the semantic meaning of an existing canonical element.

Such a change must therefore be treated as an explicit Classification change and governed accordingly.

---

# 31. Example 27 — Backward Compatibility

Suppose version 1 defines:

```text

    Architecture
    └── Deployment

```

Version 2 introduces:

```text

            Architecture
            │
            ├── Software Architecture
            │
            └── Deployment Architecture

```

If the former `Deployment` element is replaced, the migration should preserve the ability to interpret existing assignments.

For example:

```text

            Deployment
            │
            └── replaced-by  ─────►  Deployment Architecture

```

The exact migration mechanism is implementation dependent.

The semantic requirement is preservation of historical meaning.

---

# 32. Example 28 — Classification Independent of Storage

The same document may be stored in different physical locations:

```text

    Repository A
        /docs/architecture.md

```

or:

```text

    Repository B
        /knowledge/design/architecture.md

```

The Classification may remain:

```text

    Architecture

```

The physical location does not define the semantic classification.

---

# 33. Example 29 — Classification Independent of Format

A document may exist as:

```text

    architecture.md
    architecture.html
    architecture.pdf

```

If these represent the same document and semantic content, conversion of the representation does not inherently constitute a Classification change.

The Classification remains:

```text

    Architecture

```

unless a deliberate Classification decision changes it.

---

# 34. Example 30 — Classification and Versioning

Consider:

```text

    Document:
        DOC-200

    Version:
        1.0

    Classification:
        Architecture

```

A later version may be:

```text

    Document:
        DOC-200

    Version:
        2.0

    Classification:
        Architecture

```

The document version does not inherently require a Classification change.

Classification should change only when the document's semantic classification changes according to the applicable rules.

---

# 35. Example 31 — Classification Change

Suppose a document originally describes architecture:

```text

    Document:
        DOC-201

    Classification:
        Architecture

```

A later revision changes its purpose so that it becomes a deployment procedure.

The Classification may change to:

```text

            Operations
            │
            └── Deployment

```

Such a change should be treated as a Classification change rather than an incidental metadata update.

---

# 36. Example 32 — Traceable Classification Change

A Classification change may be recorded conceptually as:

```text

    Change ID:
        CLS-CHG-001

    Element:
        Deployment

    Change:
        Reclassified as Deployment Procedure

    Reason:
        Document scope changed

    Decision:
        Approved

    Effective Version:
        2.0

```

The exact change-record mechanism is outside the scope of this example.

The important property is traceability.

---

# 37. Example 33 — Dictionary Entry

A canonical Dictionary entry may conceptually be represented as:

```text

    Term:
        Architecture

    Identifier:
        CLS-ARCH

    Definition:
        Classification category for documentation concerning
        the architectural structure and design of a system.

    Status:
        Active

    Related Terms:
        Architectural Principles
        Architectural Concepts
        Design

```

The Dictionary provides terminology and semantic definition.

The Classification Schema provides structural rules.

---

# 38. Example 34 — Canonical Term and Synonym

Suppose:

```text

    Canonical Term:
        Architecture

    Synonym:
        System Architecture

```

If both terms refer to the same concept, `System Architecture` should not automatically become a second Classification Element.

The Dictionary can record the synonym.

This prevents unnecessary semantic duplication.

---

# 39. Example 35 — Deprecated Term

Suppose:

```text

    Preferred Term:
        Deployment Architecture

    Deprecated Term:
        Deployment Design

```

The deprecated term remains recognizable for historical interpretation but should not normally be used for new definitions.

---

# 40. Example 36 — Classification Granularity

Consider two possible structures.

### 40.1. Structure A

```text

            Development
            │
            ├── Coding
            ├── Testing
            ├── Unit Testing
            ├── Integration Testing
            ├── Test Case Creation
            ├── Test Data Preparation
            └── Test Execution

```

### 40.2. Structure B

```text

            Development
            │
            ├── Coding
            └── Testing

```

Neither structure is universally correct.

The appropriate granularity depends on whether each level represents a meaningful semantic distinction.

Classification should avoid unnecessary Classification Inflation while providing sufficient semantic precision.

---

# 41. Example 37 — Over-Classification

Consider:

```text

            Architecture
            │
            └── Architecture Document
                │
                └── Architecture Document Version
                    │
                    └── Architecture Document Version 1

```

If these elements do not represent distinct semantic concepts, the hierarchy is unnecessarily deep.

The additional elements introduce structural complexity without providing meaningful semantic information.

---

# 42. Example 38 — Good Specialization

A more meaningful structure could be:

```text

            Architecture
            │
            ├── Architectural Principles
            ├── Architectural Concepts
            ├── System Architecture
            └── Deployment Architecture

```

Each specialization can represent a distinct semantic category.

---

# 43. Example 39 — Classification Relationship to Knowledge

Classification can contribute semantic information to a broader knowledge structure.

For example:

```text

            Document
            │
            ├── classified-as  ─────►  Architecture
            │
            └── references  ─────►  System Design

```

Classification provides categorization.

The broader relationship structure can represent additional semantic connections.

The responsibilities remain distinct.

---

# 44. Example 40 — Classification and Automation

An automation process may validate a collection of documents:

```text

                Documents
                    │
                    ▼

        Classification Validation
        │
        ├── Valid
        ├── Invalid Element
        ├── Invalid Relationship
        └── Constraint Violation

```

The automation performs validation.

It does not redefine the Classification model.

The rules remain defined by the Classification architecture and specification.

---

# 45. Example 41 — Complete Classification Instance

A simplified complete example may be represented as:

```text

            Classification Model
            │
            ├── Architecture
            │   ├── Principles
            │   ├── Concepts
            │   └── Design
            │
            └── Development
                ├── Coding
                └── Testing


            Document
            │
            └── DOC-001 — Architecture Overview
                │
                └── Classification
                    │
                    └── Architecture

```

The Classification assignment is valid if:

- `Architecture` exists;
- the element is active;
- the assignment is permitted by the Schema;
- applicable cardinality constraints are satisfied;
- no semantic constraint is violated.

---

# 46. Example 42 — Complete Classification with Relationships

A more complete example:

```text

            Architecture
            │
            ├── Principles
            ├── Concepts
            └── Design
                │
                └── related-to  ─────►  Development
                                        │
                                        ├── Coding
                                        └── Testing

```

The hierarchy and the `related-to` relationship have different semantics.

The hierarchy represents specialization.

The relationship represents association.

---

# 47. Example 43 — Complete Lifecycle

A Classification Element may be managed as follows:

```text

                    ┌───────────────┐
                    │    Proposed   │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │    Defined    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │   Approved    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │     Active    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │   Deprecated  │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │    Retired    │
                    └───────────────┘

```

Each transition is subject to the applicable lifecycle and governance rules.

---

# 48. Example 44 — End-to-End Classification Change

Consider the introduction of a new Classification Element:

```text

                 Proposal
                    │
                    ▼

         "Deployment Architecture"
                    │
                    ▼

             Semantic Review
                    │
                    ├── duplicate?  ─────►  No
                    │
                    ▼

               Model Review
                    │
                    ▼

              Schema Review
                    │
                    ▼

            Constraint Review
                    │
                    ▼

           Governance Approval
                    │
                    ▼

             Dictionary Entry
                    │
                    ▼

      Classification Element Created
                    │
                    ▼

                Validation
                    │
                    ▼

                  Active

```

This illustrates how the Classification component can integrate its major architectural concerns into one controlled process.

---

# 49. Example 45 — Invalid End-to-End Change

An uncontrolled process might instead be:

```text

      Developer creates new category
                    │
                    ▼

   Category immediately becomes active
                    │
                    ▼

         Documents start using it
                    │
                    ▼

        Duplicate discovered later

```

This approach bypasses:

- semantic review;
- governance;
- validation;
- Dictionary maintenance.

It therefore illustrates an undesirable Classification evolution process.

---

# 50. Example 46 — Conformance Assessment

A Classification implementation may be assessed using a simplified checklist:

| Requirement Area | Result |
|------------------|--------|
| Architecture | PASS |
| Concepts | PASS |
| Elements | PASS |
| Schema | PASS |
| Semantics | PASS |
| Relationships | PASS |
| Constraints | PASS |
| Lifecycle | PASS |
| Validation | PASS |
| Governance | PASS |
| Dictionary | PASS |
| Extensibility | PASS |

The implementation can therefore be considered conformant if all mandatory requirements are satisfied.

---

# 51. Example 47 — Non-Conforming Implementation

Consider an implementation that:

- allows undefined Classification Elements;
- stores Classification only through directory names;
- permits duplicate canonical concepts;
- ignores lifecycle states;
- bypasses validation;
- silently changes semantic definitions.

The implementation violates multiple Classification requirements.

Its physical storage mechanism is not itself the problem.

The problem is the violation of the architectural and semantic requirements.

---

# 52. Example 48 — Classification Based on Directory Structure

The following structure:

```text

    /docs
        /architecture
            architecture.md
        /development
            testing.md

```

may visually suggest:

```text

    architecture.md  ─────►  Architecture
    testing.md       ─────►  Development

```

However, the directories alone do not establish Classification.

The Classification must be defined through the Classification model and applicable metadata or representation mechanisms.

This distinction preserves the Framework's independence from physical document organization.

---

# 53. Example 49 — Classification Representation

A technology-neutral representation might be:

```text

    Document:
        DOC-301

    Classification:
    {
        Element: "CLS-ARCH",
        Name: "Architecture"
    }

```

The exact serialization is intentionally unspecified.

The same semantic information could be represented through:

- YAML;
- JSON;
- XML;
- database records;
- structured metadata;
- another supported representation.

The representation must preserve the canonical Classification semantics.

---

# 54. Example 50 — Classification Documentation Set

The Classification component can be understood through its complete documentation family:

```text

DF-CLS-001  Architecture
DF-CLS-002  Concepts
DF-CLS-003  Model
DF-CLS-004  Elements
DF-CLS-005  Schema
DF-CLS-006  Lifecycle
DF-CLS-007  Validation
DF-CLS-008  Governance
DF-CLS-009  Relationships
DF-CLS-010  Constraints
DF-CLS-011  Extensibility
DF-CLS-012  Best Practices
DF-CLS-013  Dictionary
DF-CLS-014  Specification
DF-CLS-015  Examples

```

The documents have complementary responsibilities.

```text

    Architecture
        defines the architectural boundary

    Concepts
        defines the conceptual vocabulary

    Model
        defines the conceptual structure

    Elements
        defines Classification units

    Schema
        defines formal structure

    Lifecycle
        defines evolution states

    Validation
        defines verification

    Governance
        defines control

    Relationships
        defines semantic associations

    Constraints
        defines restrictions

    Extensibility
        defines controlled evolution

    Best Practices
        provides guidance

    Dictionary
        defines canonical terminology

    Specification
        defines normative requirements

    Examples
        demonstrates application

```

---

# 55. Example 51 — Normative and Informative Separation

The distinction between documents can be represented as:

```text

                             Classification
                                   │
                  ┌────────────────┴────────────────┐
                  │                                 │
              Normative                        Informative
              │                                │
              ├── Architecture                 ├── Best Practices
              ├── Model                        └── Examples
              ├── Schema
              ├── Lifecycle
              ├── Validation
              ├── Governance
              ├── Relationships
              ├── Constraints
              ├── Extensibility
              ├── Dictionary
              └── Specification

```

The exact normative status of each document is determined by the Classification documentation framework.

Examples remain illustrative and do not create requirements.

---

# 56. Example 52 — Recommended Documentation Flow

A user studying Classification may use the documents in the following sequence:

```text

               Architecture
                    │
                    ▼

                 Concepts
                    │
                    ▼

                  Model
                    │
                    ▼

                 Elements
                    │
                    ▼

                  Schema
                    │
                    ▼

                Lifecycle
                    │
                    ▼

                Validation
                    │
                    ▼

                Governance
                    │
                    ▼

              Relationships
                    │
                    ▼

               Constraints
                    │
                    ▼

              Extensibility
                    │
                    ▼

              Best Practices
                    │
                    ▼

                Dictionary
                    │
                    ▼

              Specification
                    │
                    ▼

                 Examples

```

The Examples document can therefore serve as a practical reference after the normative concepts have been established.

---

# 57. Example 53 — Example Does Not Create a Requirement

Consider an example stating:

```text

    A document is assigned exactly one Classification Element.

```

This does not establish a universal requirement that every document must have exactly one Classification Element.

The actual cardinality is determined by the Classification Schema and Constraints.

The example merely illustrates one valid instance.

---

# 58. Example 54 — Example Does Not Create a Canonical Element

Consider an example using:

```text

    Security

```

The use of this name in an example does not automatically make `Security` a canonical Classification Element.

A canonical element must be defined and approved according to the Classification architecture and governance process.

---

# 59. Example 55 — Example of a Complete Document Record

A complete fictional document record may be represented as:

```text

    Document
    ────────────────────────────────
    ID:
        DOC-500

    Title:
        Deployment Architecture

    Classification:
        Architecture
        └── Deployment Architecture

    Lifecycle:
        Active

    Relationships:
        related-to → Development

    Classification Validation:
        Conformant

```

This example demonstrates how several Classification concepts can coexist without collapsing their responsibilities.

---

# 60. Example 56 — Classification Review

A Classification review may inspect:

```text

    Element:
        Deployment Architecture

    Questions:
        Is the concept distinct?
        Is the name canonical?
        Is the definition clear?
        Is the parent appropriate?
        Are relationships valid?
        Are constraints satisfied?
        Is the lifecycle state valid?
        Is the Dictionary updated?

```

A positive review supports controlled adoption.

---

# 61. Example 57 — Classification Change Impact

Suppose the definition of:

```text

    Architecture

```

changes significantly.

The impact may extend to:

```text

            Architecture
            │
            ├── Child Elements
            ├── Relationships
            ├── Constraints
            ├── Validation Rules
            ├── Dictionary
            ├── Specification
            └── Existing Assignments

```

A semantic change should therefore be evaluated as an architectural change rather than as a simple textual edit.

---

# 62. Example 58 — Preserving Historical Meaning

Suppose a historical document contains:

```text

    Classification:
        Technical Documentation

```

and the Classification Element is later retired.

A historical representation may preserve:

```text

    Historical Classification:
        Technical Documentation

    Status:
        Retired

    Replacement:
        Architecture
        Development
        Operations

```

This permits historical documentation to remain interpretable without keeping the retired element active for new assignments.

---

# 63. Example 59 — Classification Migration

A migration may be represented as:

```text

            Old Classification
                    │
                    ▼

            Migration Analysis
                    │
                    ├── Direct replacement
                    ├── Split
                    ├── Merge
                    └── Retain historically
                    │
                    ▼

            New Classification

```

For example:

```text

            Technical Documentation
            │
            ├── Architecture
            ├── Development
            └── Operations

```

A migration that splits one category into several categories requires explicit semantic analysis.

---

# 64. Example 60 — Classification Quality Assessment

A Classification model can be evaluated using the following questions:

| Question | Expected Result |
|----------|-----------------|
| Are concepts clearly defined? | Yes |
| Are canonical terms unique? | Yes |
| Are elements semantically meaningful? | Yes |
| Is the hierarchy justified? | Yes |
| Are relationships explicit? | Yes |
| Are constraints defined? | Yes |
| Can violations be detected? | Yes |
| Is lifecycle controlled? | Yes |
| Is evolution governed? | Yes |
| Is historical meaning preserved? | Where required |
| Is implementation independent? | Yes |

This provides a practical quality assessment without introducing additional normative requirements.

---

# 65. Example 61 — Classification Anti-Pattern

An implementation may encode Classification as:

```text

    Directory Name = Classification

```

For example:

```text

    /docs/architecture/
    /docs/development/
    /docs/testing/

```

This creates a dependency between Classification and physical organization.

A stronger architecture treats the relationship explicitly:

```text

            Document
            │
            └── Classification
                │
                └── Classification Element

```

The physical organization may still mirror Classification for convenience, but it does not define the semantic model.

---

# 66. Example 62 — Classification as Semantic Knowledge

Classification can be viewed as a semantic structure:

```text

                 Document
                    │
                    ▼

              Classification
                    │
                    ▼

                 Concept
                    │
                    ▼

             Semantic Domain

```

This illustrates the broader principle that Classification is concerned with the meaning and organization of knowledge rather than merely with document storage.

---

# 67. Example 63 — Minimal Conformant Classification

A minimal conceptual Classification system may contain:

```text

            Classification
            │
            └── Architecture

```

with:

```text

    Identifier:
        CLS-ARCH

    Name:
        Architecture

    Definition:
        Documentation concerning architecture.

    Lifecycle:
        Active

```

The implementation may be minimal, but it must still satisfy the applicable normative requirements.

---

# 68. Example 64 — Extended Classification

A richer Classification may contain:

```text

            Architecture
            │
            ├── Principles
            ├── Concepts
            ├── Design
            └── Deployment

            Development
            │
            ├── Coding
            ├── Testing
            └── Build

            Operations
            │
            ├── Deployment
            ├── Monitoring
            └── Maintenance

```

with explicit relationships between related elements.

Such an extension remains conformant when it satisfies the Classification Schema, Constraints, Governance and other applicable requirements.

---

# 69. Example 65 — Summary of Correct Application

A correctly applied Classification system demonstrates the following characteristics:

```text

                 Explicit
                    │
                    ▼

                 Semantic
                    │
                    ▼

                Structured
                    │
                    ▼

                Validated
                    │
                    ▼

                 Governed
                    │
                    ▼

                Traceable
                    │
                    ▼

                Extensible

```

The examples throughout this document illustrate these characteristics from different perspectives.

---

# 70. Final Example Principle

The examples in this document can be summarized by the following principle:

> Classification examples should demonstrate semantic organization without becoming an alternative source of architectural rules.

Examples should make the Classification architecture easier to understand, apply and verify.

They should not redefine the Classification model.

---

# 71. Example Usage Guidelines

When creating additional Classification examples:

1. Use terminology defined by the Classification Dictionary.
2. Respect the Classification Specification.
3. Do not introduce undocumented normative requirements.
4. Clearly distinguish illustrative elements from canonical elements.
5. Preserve the distinction between hierarchy and association.
6. Respect lifecycle semantics.
7. Demonstrate validation where applicable.
8. Demonstrate governance for significant changes.
9. Avoid implementation-specific assumptions.
10. Preserve the distinction between Classification and other Framework components.

---

# 72. Related Documents

## 72.1. Foundation

- DF-FND-001 — Framework Manifest
- DF-FND-002 — Research Journal
- DF-FND-003 — Evolution Timeline
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

## 72.2. Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-004 — Architectural Layers
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology
- DF-ARC-007 — Component Documentation Structure

## 72.3. Classification

- DF-CLS-001 — Classification Architecture
- DF-CLS-002 — Classification Concepts
- DF-CLS-003 — Classification Model
- DF-CLS-004 — Classification Elements
- DF-CLS-005 — Classification Schema
- DF-CLS-006 — Classification Lifecycle
- DF-CLS-007 — Classification Validation
- DF-CLS-008 — Classification Governance
- DF-CLS-009 — Classification Relationships
- DF-CLS-010 — Classification Constraints
- DF-CLS-011 — Classification Extensibility
- DF-CLS-012 — Classification Best Practices
- DF-CLS-013 — Classification Dictionary
- DF-CLS-014 — Classification Specification
- **DF-CLS-015 — Classification Examples**

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of Classification Examples. |

---

**End of Document**