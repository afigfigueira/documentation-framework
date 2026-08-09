# Documentation Framework

# DF-CLS-002 — Classification Concepts

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-002 |
| **Title** | Classification Concepts |
| **Family** | Classification |
| **Type** | Architecture |
| **Component** | Classification |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

Classification is the architectural capability through which documents are organized according to their semantic characteristics.

The Classification component belongs to the Documentation Layer and provides semantic organization independently of the physical representation, storage mechanism or location of a document.

This document defines the fundamental concepts required to understand Classification.

It establishes the conceptual vocabulary that will be used by the subsequent Classification documents.

---

# 2. Purpose

The purpose of this document is to establish a common conceptual foundation for the Classification component.

It defines the meaning and boundaries of concepts such as:

- Classification;
- Classification Scheme;
- Classification Element;
- Classification Value;
- Classification Category;
- Family;
- Type;
- Class;
- Classification Assignment;
- Classification Context.

The concepts defined here provide the vocabulary required to describe the Classification Model and its subsequent specifications.

---

# 3. Scope

This document defines the conceptual meaning of Classification.

It does not define:

- the formal Classification Model;
- the structure of Classification Elements;
- the Classification Schema;
- lifecycle states;
- validation rules;
- governance rules;
- relationship types;
- constraints;
- extensibility mechanisms;
- implementation details.

These concerns are addressed by subsequent documents in the Classification component.

---

# 4. Classification

**Classification** is the semantic organization of documents according to defined classification criteria.

Classification determines how a document is positioned within a controlled semantic structure.

Conceptually:

```text

                 Document
                    │
                    ▼

              Classification
                    │
                    ├── Family
                    ├── Type
                    └── Class

```

Classification is therefore concerned with the semantic organization of documents rather than their physical organization.

---

# 5. Purpose of Classification

Classification provides a means of organizing documentation according to meaning.

It supports:

- organization;
- navigation;
- discovery;
- governance.

These purposes are consistent with the architectural role assigned to Classification within the Documentation Framework.

Classification therefore contributes to making the documentation system understandable as a structured body of knowledge rather than merely as a collection of files.

---

# 6. Classification and Knowledge

The Documentation Framework is knowledge-oriented.

Documents are treated as structured units of knowledge, and Classification contributes to organizing those units according to semantic characteristics.

Conceptually:

```text

                Knowledge
                    │
                    ▼

              Documentation
                    │
                    ▼

                Documents
                    │
                    ▼

              Classification

```

Classification therefore operates at the level of document semantics.

It does not attempt to classify the content of a document as a substitute for the document itself.

---

# 7. Classification Context

A **Classification Context** is the semantic context in which a classification value is interpreted.

A classification value has meaning only within its defined context.

Conceptually:

```text

          Classification Context
                    │
                    ▼

           Classification Value

```

The context prevents identical labels from being interpreted as identical concepts when they belong to different semantic domains.

---

# 8. Classification Scheme

A **Classification Scheme** is a defined semantic structure used to organize classification categories.

A scheme establishes:

- a classification domain;
- the categories belonging to that domain;
- the semantic interpretation of those categories.

Conceptually:

```text

                    Classification Scheme
                              │
                              ├── Category
                              ├── Category
                              └── Category

```

The formal structure of a Classification Scheme is defined later by **DF-CLS-005 — Classification Schema**.

---

# 9. Classification Element

A **Classification Element** is a conceptual component used to express some aspect of a document's classification.

Classification Elements provide the dimensions through which classification can be expressed.

At the conceptual level:

```text

                    Classification
                    │
                    ├── Element
                    ├── Element
                    └── Element

```

The detailed Classification Elements are defined by **DF-CLS-004 — Classification Elements**.

---

# 10. Classification Value

A **Classification Value** is a semantic value assigned to a Classification Element.

Conceptually:

```text

         Classification Element
                    │
                    ▼

          Classification Value

```

For example, a Family element may receive a Family value.

The value itself is interpreted according to the Classification Scheme to which it belongs.

---

# 11. Classification Category

A **Classification Category** is a defined semantic category within a Classification Scheme.

A category provides a recognized classification option rather than an arbitrary textual label.

Conceptually:

```text

                  Classification Scheme
                            │
                            ├── Category A
                            ├── Category B
                            └── Category C

```

Classification Categories are therefore controlled semantic concepts.

---

# 12. Family

A **Family** represents a broad documentary domain.

Family provides a high-level semantic grouping for documents.

Conceptually:

```text

                    Family
                    │
                    ├── Document
                    ├── Document
                    └── Document

```

The Family concept emerged historically as a means of organizing documents into broad knowledge domains.

For example, the evolution of the framework introduced the `META` Family to represent documents whose domain of knowledge was the Documentation Framework itself.

Family therefore answers the conceptual question:

> What broad documentary domain does this document belong to?

---

# 13. Type

A **Type** represents a more specific documentary classification within a Family.

Type refines the semantic organization established by Family.

Conceptually:

```text

                    Family
                      │
                      ├── Type
                      ├── Type
                      └── Type

```

The historical evolution of the framework demonstrates this relationship through combinations such as `META-DCL`, where `META` represents the Family and `DCL` represents a more specific classification within that Family.

Type therefore answers the conceptual question:

> What specific kind of document exists within this Family?

---

# 14. Class

A **Class** represents a semantic characteristic describing the nature or role of a document.

Class is conceptually distinct from Family and Type.

The Classification component therefore distinguishes:

```text

    Family
    Type
    Class

```

rather than treating all three concepts as different levels of the same hierarchy.

Class may provide a semantic distinction that can apply across different Families or Types.

---

# 15. Family, Type and Class

The three concepts can be understood as complementary dimensions:

```text

                    Classification
                    │
                    ├── Family
                    │   └── broad documentary domain
                    │
                    ├── Type
                    │   └── specific documentary kind
                    │
                    └── Class
                        └── documentary nature or role

```

Family and Type provide a progressively more specific documentary organization.

Class provides an additional semantic dimension.

The precise relationships between these concepts belong to the Classification Model.

---

# 16. Classification Assignment

A **Classification Assignment** is the association between a document and a classification value.

Conceptually:

```text

                Document
                    │
               assignment
                    │
                    ▼

           Classification Value

```

An assignment states that a particular classification value applies to a particular document.

The assignment does not redefine the meaning of the classification value.

The meaning is defined by the Classification Scheme and its categories.

---

# 17. Classification Membership

A document is considered a member of a classification category when a valid Classification Assignment associates the document with that category.

Conceptually:

```text

         Classification Category
                    │
                contains
                    │
                    ▼

                Documents

```

Membership is therefore a semantic relationship rather than a physical containment relationship.

A document may be physically stored elsewhere without changing its classification membership.

---

# 18. Classification Vocabulary

A **Classification Vocabulary** is the set of recognized terms used to express classification concepts.

The vocabulary provides consistency of terminology.

For example:

```text

    Family
    Type
    Class

```

are classification concepts, while particular values belonging to these concepts constitute the controlled vocabulary used for classification.

The formal authoritative vocabulary is established later by the Classification Dictionary.

---

# 19. Controlled Classification

Classification is controlled when its values are derived from explicitly defined classification concepts.

Conceptually:

```text

            Controlled Scheme
                    │
                    ▼

           Defined Categories
                    │
                    ▼

        Classification Assignment

```

Controlled classification prevents arbitrary values from being introduced without semantic definition.

---

# 20. Classification Semantics

Classification values possess explicit semantics.

A classification label is not sufficient by itself to establish meaning.

Conceptually:

```text

                    Classification Category
                    │
                    ├── Identifier
                    ├── Label
                    └── Meaning

```

The meaning of a category must remain stable and unambiguous within its classification context.

This follows the framework's broader requirement for explicit semantics and a single authoritative definition for architectural concepts.

---

# 21. Classification Identity

A classification category has an identity distinct from the identity of any document to which it is assigned.

Conceptually:

```text

            Document Identity
                    │
                    └── identifies Document

         Classification Identity
                    │
                    └── identifies Classification Concept

```

A classification value therefore cannot be treated as a Document Identity.

This distinction is essential because changing a document's classification does not create a different document.

---

# 22. Classification and Document Identity

Document Identity establishes the permanent identity of a document.

Classification establishes the semantic organization of that document.

Conceptually:

```text

                    Document
                    │
                    ├── Identity
                    │       └── Who is this document?
                    │
                    └── Classification
                              └── How is this document categorized?

```

Document Identity remains stable independently of changes to document metadata, content, filename, repository or location.

Classification therefore complements Document Identity rather than replacing it.

---

# 23. Classification and Metadata

Metadata describes a document as an architectural entity.

Classification organizes the document semantically.

The Metadata component explicitly supports document classification but does not itself perform classification.

Conceptually:

```text

                 Metadata
                    │
                represents
                    │ 
                    ▼

        Classification Information
                    │
              interpreted by
                    │ 
                    ▼

              Classification

```

Metadata provides the representation.

Classification provides the semantic meaning.

---

# 24. Classification and Templates

Templates may provide a standardized representation for classification information.

However, a Template does not define the semantic meaning of a classification concept.

Conceptually:

```text

              Classification
                    │
             defines meaning
                    │
                    ▼

        Classification Information
                    │
           represented through
                    │
                    ▼

                Template

```

This preserves the separation between semantic concepts and document representation.

---

# 25. Classification and Physical Organization

Classification is independent from physical organization.

A document's classification shall not be determined by:

- directory name;
- repository;
- filename;
- storage location;
- document format.

Conceptually:

```text

          Semantic Organization
                    │
            independent from
                    │ 
                    ▼

            Physical Organization

```

The same document classification can therefore remain valid while the document moves between repositories or locations.

---

# 26. Classification Dimension

A **Classification Dimension** represents a distinct semantic aspect through which documents may be classified.

The principal classification dimensions established by the framework are:

```text

    Family
    Type
    Class

```

These dimensions are conceptually different.

Family and Type provide hierarchical specificity.

Class provides a distinct semantic characteristic.

The formal dimensional model is defined by **DF-CLS-003 — Classification Model**.

---

# 27. Classification Hierarchy

A **Classification Hierarchy** is an ordered semantic structure in which one classification concept specializes another.

Within the Classification component, the principal hierarchy is:

```text

                  Family
                    │
                    ▼

                   Type

```

This hierarchy should not be assumed to include Class.

Class represents a separate classification dimension unless the formal model establishes a specific relationship.

---

# 28. Classification Relationship

A **Classification Relationship** connects classification concepts or associates classification concepts with documents.

Examples conceptually include:

```text

                    Family
                      │
                      └── Type

                    Document
                       │
                       └── Classification Assignment
                                       │
                                       └── Classification Category

```

The complete set of relationship types is deferred to **DF-CLS-009 — Classification Relationships**.

---

# 29. Classification Constraint

A **Classification Constraint** is a condition that limits the valid use of classification concepts.

Examples include:

- whether a value may be assigned;
- whether a Type is valid within a Family;
- whether a classification combination is permitted.

Constraints are not defined in detail in this document.

They are specified by **DF-CLS-010 — Classification Constraints**.

---

# 30. Classification Lifecycle

Classification concepts may evolve over time.

A classification category may be:

- introduced;
- active;
- deprecated;
- retired.

The lifecycle of classification concepts is distinct from the lifecycle of the documents to which they are assigned.

Detailed lifecycle semantics are defined by **DF-CLS-006 — Classification Lifecycle**.

---

# 31. Classification Governance

Classification Governance concerns the controlled management of classification concepts and their evolution.

Governance may establish:

- ownership;
- authority;
- approval;
- change control;
- maintenance responsibilities.

Governance is distinct from Classification itself.

The Classification component defines the semantic concepts, while governance defines how those concepts are controlled.

Detailed governance is deferred to **DF-CLS-008 — Classification Governance**.

---

# 32. Classification Validation

Classification Validation determines whether a classification assignment conforms to the defined Classification Model and Classification Schema.

Conceptually:

```text

        Classification Assignment
                    │
                    ▼

        Classification Validation
                    │
                    ├── Valid
                    └── Invalid

```

Validation is therefore concerned with correctness rather than with defining classification semantics.

Detailed validation is defined by **DF-CLS-007 — Classification Validation**.

---

# 33. Classification Extensibility

Classification shall support the controlled introduction of new classification concepts.

Extensibility may involve:

- new categories;
- additional classification dimensions;
- additional semantic relationships;
- extensions to existing schemes.

Extensions shall preserve the semantics and compatibility of existing concepts.

Detailed extensibility is defined by **DF-CLS-011 — Classification Extensibility**.

---

# 34. Classification Dictionary

The **Classification Dictionary** is the authoritative collection of definitions for Classification terminology and classification concepts.

Conceptually:

```text

                    Classification Dictionary
                    │
                    ├── Concept
                    ├── Definition
                    ├── Concept
                    └── Definition

```

The dictionary provides the authoritative vocabulary for the Classification component.

Its detailed structure is defined by **DF-CLS-013 — Classification Dictionary**.

---

# 35. Classification Specification

The **Classification Specification** is the consolidated normative definition of the Classification component.

The preceding documents progressively establish:

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

```

The consolidated specification is defined by **DF-CLS-014 — Classification Specification**.

---

# 36. Conceptual Boundaries

The following boundaries apply to the Classification concepts.

| Concept | Responsibility |
|---------|----------------|
| Classification | Semantic organization of documents |
| Scheme | Defines a classification domain |
| Element | Represents a classification dimension/component |
| Value | Represents an assigned semantic value |
| Category | Defines a controlled classification concept |
| Family | Broad documentary domain |
| Type | Specific documentary kind within a Family |
| Class | Documentary nature or role |
| Assignment | Associates a document with a classification value |
| Context | Establishes the semantic interpretation of a value |
| Dictionary | Provides authoritative terminology and definitions |

These concepts provide the vocabulary for the Classification component without defining its complete formal model.

---

# 37. Conceptual Model

At the conceptual level, Classification can be represented as:

```text

                                  Classification
                                        │
              ┌─────────────────────────┼─────────────────────────┐
              │                         │                         │
              ▼                         ▼                         ▼

           Family                     Type                      Class
              │                         │
              └────────────┬────────────┘
                           │
                           ▼

                     Classification
                        Context
                           │
                           ▼

                  Classification Value
                           │
                           ▼

                Classification Category
                           │
                           ▼

                     Classification
                       Assignment
                           │
                           ▼

                        Document

```

This diagram is conceptual only.

The formal relationships and cardinalities are deferred to the Classification Model.

---

# 38. Conceptual Principles

The Classification concepts are governed by the following principles:

## 38.1. Semantic Independence

Classification represents semantic organization rather than physical organization.

## 38.2. Explicit Meaning

Every classification concept shall have an explicit meaning.

## 38.3. Controlled Vocabulary

Classification values shall belong to defined semantic categories.

## 38.4. Separation of Responsibilities

Classification shall remain distinct from Identity, Metadata, Storage, Governance and Discovery.

## 38.5. Stable Identity

Classification changes shall not implicitly change Document Identity.

## 38.6. Technology Independence

Classification concepts shall not depend on implementation technologies.

## 38.7. Extensibility

Classification concepts shall support controlled evolution.

---

# 39. Historical Context

Classification emerged progressively during the evolution of the Documentation Framework.

The framework history records that Families, Types and Classes were introduced as part of the development of the documentation architecture.

The creation of the `META` Family was an important step because it established a documentary domain concerned with the Documentation Framework itself.

The early `META-DCL` concept was specifically associated with defining categories, types, conventions and classification.

These historical concepts provide context for the formal Classification component but do not, by themselves, constitute its final specification.

---

# 40. Conceptual Evolution

The Classification component follows the same incremental evolution strategy established for the other Documentation Layer components.

The Metadata roadmap, for example, explicitly structures its component evolution into successive stages, with each stage extending previously established concepts without redefining them.

The Classification component follows the corresponding M6 document sequence:

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

Each document has a distinct responsibility.

---

# 41. Conformance

A Classification implementation conforms conceptually to this document when:

- Classification is understood as semantic organization;
- classification concepts have explicit meanings;
- Family, Type and Class remain conceptually distinguishable;
- Family represents a broad documentary domain;
- Type provides more specific documentary classification;
- Class represents documentary nature or role;
- classification values belong to defined semantic contexts;
- classification assignments associate documents with classification concepts;
- Classification remains distinct from Document Identity;
- Classification remains distinct from Metadata;
- Classification remains independent from physical organization;
- Classification terminology has authoritative definitions.

---

# 42. Summary

Classification provides the semantic organization of documents within the Documentation Framework.

The principal concepts are:

```text

                    Classification
                    │
                    ├── Scheme
                    ├── Element
                    ├── Value
                    ├── Category
                    ├── Family
                    ├── Type
                    ├── Class
                    ├── Assignment
                    └── Context

```

Family provides broad documentary organization.

Type provides more specific organization within a Family.

Class provides an additional semantic description of documentary nature or role.

Classification remains independent from Document Identity, Metadata and physical document organization.

These concepts establish the vocabulary required for the formal Classification Model defined by **DF-CLS-003**.

---

# 43. Related Documents

## Foundation

- DF-FND-001 — Framework Manifest
- DF-FND-002 — Research Journal
- DF-FND-003 — Evolution Timeline
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

## Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-004 — Architectural Layers
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology
- DF-ARC-007 — Component Documentation Structure

## Documentation Layer

- DF-MTD-001 — Metadata Architecture
- Document Identity component
- Templates component

## Classification

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
- DF-CLS-015 — Classification Examples

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of Classification Concepts. |

---

**End of Document**

---
