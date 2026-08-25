# Documentation Framework

# DF-CLS-005 — Classification Schema

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-005 |
| **Title** | Classification Schema |
| **Family** | Classification |
| **Type** | Structure |
| **Component** | Classification |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Classification Model defines the conceptual structure used to classify documents.

The Classification Elements document defines the semantic elements that constitute that structure:

- Family;
- Type;
- Class.

This document defines the **Classification Schema**.

The schema provides the formal structural description of a Classification instance while preserving the semantic distinctions established by the previous Classification documents.

The schema is intentionally independent of any particular implementation technology or serialization format.

---

# 2. Purpose

The purpose of the Classification Schema is to define the formal structure of a Classification instance.

It establishes:

- the structure of a Classification;
- its constituent elements;
- the relationship between Family and Type;
- the role of Class;
- the distinction between classification and identity;
- the relationship between Classification and Document;
- the conceptual constraints necessary for a valid structural representation.

The schema therefore provides the structural contract against which Classification instances can subsequently be validated.

---

# 3. Scope

This document defines the structural schema of Classification.

It covers:

- Classification;
- Family;
- Type;
- Class;
- Classification values;
- structural relationships;
- structural composition.

It does not define:

- the complete vocabulary of Family values;
- the complete vocabulary of Type values;
- the complete vocabulary of Class values;
- lifecycle rules;
- governance rules;
- validation procedures;
- relationship semantics beyond the structural model;
- extensibility mechanisms;
- implementation-specific serialization formats.

---

# 4. Architectural Context

Classification is part of the Metadata associated with a document.

The architectural blueprint explicitly identifies Classification as a Metadata category containing:

- Family;
- Type;
- Class.

It also establishes that Classification provides semantic organization independently of physical directory organization.

Conceptually:

```text

            Document
            │
            ├── Metadata
            │   │
            │   └── Classification
            │       ├── Family
            │       ├── Type
            │       └── Class
            │
            └── Content

```

---

# 5. Schema Definition

The Classification Schema can be represented conceptually as:

```text

            Classification
            │
            ├── Family
            │
            ├── Type
            │
            └── Class

```

The three elements constitute the structural representation of Classification.

---

# 6. Classification Structure

A Classification instance consists of the following conceptual elements:

| Element | Role |
|---------|------|
| **Family** | Broad documentary domain |
| **Type** | Specific documentary category within the Family |
| **Class** | Documentary nature or role |

This structure follows the established Classification Model.

---

# 7. Classification Element Model

The structural model is:

```text

            Classification
            ├── Family
            │
            ├── Type
            │
            └── Class

```

The schema therefore treats Family, Type and Class as members of the same Classification structure.

They are not three sequential hierarchical levels.

---

# 8. Family Schema Element

The `Family` element represents the broad documentary domain.

Conceptually:

```text

            Family
            └── Value

```

The value identifies the specific Family.

For example:

```text

    Family  =  META

```

The research history establishes Family as the first classification dimension and describes Family values such as `META`, `ARC`, `ANL`, `REF`, `STD`, and `RFC`.

The complete authoritative Family vocabulary is not defined by this schema.

---

# 9. Type Schema Element

The `Type` element represents a specific documentary category within a Family.

Conceptually:

```text

            Type
            └── Value

```

For example:

```text

    Family  =  META
    Type    =  DCL

```

The historical classification model explicitly records examples such as:

```text

    META-DCL
    META-WFL
    META-CON
    META-REF

```

and establishes that Type provides a second level of classification within Family.

---

# 10. Class Schema Element

The `Class` element represents the nature or role of the document.

Conceptually:

```text

            Class
            └── Value

```

For example:

```text

    Class  =  <classification class>

```

The research material establishes that Class was introduced because documents may have different documentary roles, such as defining norms, recording research, or describing architecture.

The available architectural material does not establish a definitive enumeration of Class values.

Consequently, this schema does not define one.

---

# 11. Family-Type Relationship

The schema establishes a structural dependency between Family and Type:

```text

                  Family
                    │
                    ▼

                   Type

```

Type is interpreted within the context of its Family.

Conceptually:

```text

    Family  =  META
    Type    =  DCL

```

represents a more specific classification than:

```text

    Family  =  META

```

alone.

---

# 12. Class Relationship

Class is structurally associated with Classification but is not defined as a child of Type.

The schema is therefore:

```text

            Classification
            ├── Family
            │   └── Type
            │
            └── Class

```

and not:

```text

            Classification
            └── Family
                └── Type
                    └── Class

```

This preserves the distinction established by the Classification Model.

---

# 13. Classification Tuple

The structural contents of Classification can be represented as:

```text

            Classification = {
                Family,
                Type,
                Class
            }

```

or conceptually:

```text

            Classification = (Family, Type, Class)

```

This representation describes the schema.

It does not prescribe a serialization language.

---

# 14. Classification Value

Each schema element contains or refers to a classification value.

Conceptually:

```text

            Classification
            │
            ├── Family  →  Family Value
            ├── Type    →  Type Value
            └── Class   →  Class Value

```

The schema establishes the positions of the values.

The Classification Dictionary establishes their authoritative meanings and vocabulary.

---

# 15. Structural Dependency

The schema establishes the following dependency:

```text

            Classification
            │
            ├── Family
            │   │
            │   └── Type
            │
            └── Class

```

This means that the interpretation of Type depends on the Family context.

Class remains a separate classification dimension.

---

# 16. Classification and Document

A Classification instance is associated with a Document.

Conceptually:

```text

            Document
            │
            └── Classification
                ├── Family
                ├── Type
                └── Class

```

Classification therefore describes the document.

It does not constitute the document itself.

---

# 17. Classification and Metadata

Classification belongs to the document's descriptive Metadata.

The architectural material explicitly separates the Document from its Metadata and Content and identifies Classification as one of the Metadata categories.

Conceptually:

```text

            Document
            │
            ├── Metadata
            │   └── Classification
            │       ├── Family
            │       ├── Type
            │       └── Class
            │
            └── Content

```

---

# 18. Classification and Document Identity

Classification is distinct from Document Identity.

The architectural blueprint establishes that Metadata describes a document while Document Identity identifies it.

Conceptually:

```text

            Document
            │
            ├── Identity
            │
            └── Classification

```

Therefore:

```text

    Classification  ≠  Document Identity

```

---

# 19. Document ID

The framework's Document ID has a semantic structure.

The established example is:

```text

    META-DCL-001

```

where:

```text

    META  =  Family
    DCL   =  Type
    001   =  sequential identifier

```

This structure is explicitly established by the architectural blueprint.

The Classification Schema therefore recognizes the semantic relationship between the Document ID and Family/Type.

---

# 20. Document ID versus Classification

The Document ID and Classification must not be treated as the same structure.

Conceptually:

```text

            Document
            │
            ├── Document Identity
            │   └── Document ID
            │
            └── Classification
                ├── Family
                ├── Type
                └── Class

```

Historically, the Document ID embeds Family and Type.

This does not eliminate the conceptual distinction between identity and classification.

---

# 21. Sequential Identifier

The sequential component of the Document ID identifies an individual document within a classification context.

For example:

```text

    META-DCL-001
    META-DCL-002
    META-DCL-003

```

The research journal explicitly states that the sequential numbering was introduced to distinguish documents belonging to the same category.

The sequential identifier is therefore not a Classification element.

---

# 22. Classification Schema and Physical Location

Physical location is outside the Classification Schema.

The architecture explicitly separates identity and physical location: a document may move between directories or repositories while continuing to represent the same document.

Consequently:

```text

            Classification
            │
            └── independent of
                    │
                    ▼

             Physical Location

```

---

# 23. Structural Representation

The schema may be represented abstractly as:

```text

            Classification {
                Family: Value
                Type: Value
                Class: Value
            }

```

This is a conceptual schema notation.

It is not intended to establish a programming language or data serialization format.

---

# 24. Example Classification

A conceptual Classification instance can therefore be represented as:

```text

            Classification {
                Family = META
                Type   = DCL
                Class  = <Class Value>
            }

```

The values illustrate the schema structure.

Only `META` and the Family/Type relationship are directly established by the existing framework material; the example intentionally leaves Class unspecified because the available source material does not define an authoritative Class vocabulary.

---

# 25. Example Document ID

The corresponding historical Document ID pattern is:

```text

    META-DCL-001

```

Its semantic interpretation is:

```text

    Family  =  META
    Type    =  DCL
    Identity Sequence  =  001

```

This demonstrates the relationship between Classification and Document Identity without making the sequential identifier part of Classification.

---

# 26. Schema Levels

The Classification Schema can be understood at three structural levels:

```text

    Level 1
    Classification

    Level 2
    Family
    Type
    Class

    Level 3
    Values

```

Conceptually:

```text

            Classification
            │
            ├── Family
            │   └── Value
            │
            ├── Type
            │   └── Value
            │
            └── Class
                └── Value

```

---

# 27. Schema versus Vocabulary

The schema defines the structure.

The vocabulary defines the permitted semantic values.

The distinction is:

```text

            Schema
            │
            ├── Family
            ├── Type
            └── Class

            Vocabulary
            │
            ├── Family Values
            ├── Type Values
            └── Class Values

```

The Classification Dictionary is responsible for the vocabulary.

Therefore, this document does not attempt to enumerate all valid values.

---

# 28. Schema versus Dictionary

The relationship between the two components is:

```text

          Classification Schema
                    │
            defines structure
                    │
                    ▼

         Classification Elements
                    │
           receive values from
                    │
                    ▼

        Classification Dictionary

```

The schema determines where values occur.

The dictionary determines what those values mean.

---

# 29. Schema versus Validation

The schema defines the structural form against which classification instances can be evaluated.

Validation determines whether a concrete instance conforms to that structure and to the associated semantic rules.

Conceptually:

```text

          Classification Schema
                    │
                    ▼

            Expected Structure
                    │
                    ▼

         Classification Instance
                    │
                    ▼

                Validation

```

Detailed validation rules belong to **DF-CLS-007 — Classification Validation**.

---

# 30. Schema versus Constraints

The schema defines structural relationships.

Constraints define restrictions imposed upon those relationships.

For example:

```text

            Schema
            │
            └── Family  →  Type

            Constraints
            │
            └── restrictions on valid combinations

```

The detailed constraints are defined by **DF-CLS-010 — Classification Constraints**.

---

# 31. Schema versus Lifecycle

The schema describes the structure of Classification.

It does not describe how classification definitions change over time.

Lifecycle concerns belong to **DF-CLS-006 — Classification Lifecycle**.

---

# 32. Schema versus Governance

The schema does not determine who may create, modify, approve or retire classification definitions.

Those responsibilities belong to **DF-CLS-008 — Classification Governance**.

---

# 33. Schema versus Relationships

The schema defines the structural relationship between:

- Classification and its elements;
- Family and Type.

It does not attempt to define the complete relationship model of Classification.

That subject belongs to **DF-CLS-009 — Classification Relationships**.

---

# 34. Schema Cardinality

The conceptual schema identifies the three Classification elements.

However, the currently established source material does not define authoritative cardinality rules specifying whether:

- every element must always have a value;
- some elements may be omitted;
- multiple values may occur;
- a Classification may contain additional elements.

Therefore, this document does not introduce such rules as normative requirements.

Those rules must be established through the Classification Constraints and Validation documents if required.

---

# 35. Schema Extensibility

The current schema establishes:

```text

            Classification
            ├── Family
            ├── Type
            └── Class

```

The introduction of additional classification elements is not defined by this document.

Any extension must preserve the established semantic meaning of the existing elements.

Extensibility rules belong to **DF-CLS-011 — Classification Extensibility**.

---

# 36. Schema Stability

The schema shall preserve the semantic identity of its established elements.

The following meanings are therefore stable at the current architectural level:

```text

    Family  →  broad documentary domain

    Type    →  specific documentary category

    Class   →  documentary nature or role

```

Changing these meanings would constitute an architectural change rather than a simple schema modification.

---

# 37. Schema Independence

The Classification Schema is independent of:

- filesystem structure;
- repository implementation;
- document storage system;
- Markdown;
- JSON;
- YAML;
- XML;
- programming languages;
- database technologies.

The schema defines semantics and structure rather than technology.

This is consistent with the architectural principle of separating logical document organization from physical organization.

---

# 38. Abstract Schema

The complete abstract schema is:

```text

            Classification
            │
            ├── Family
            │   └── Family Value
            │
            ├── Type
            │   └── Type Value
            │
            └── Class
                └── Class Value

```

with the relationship:

```text

            Family
            │
            └── Type

```

and the document relationship:

```text

            Document
            │
            └── Classification

```

---

# 39. Conceptual Schema Diagram

```text

                    ┌───────────────────────────┐
                    │          Document         │
                    ├───────────────────────────┤
                    │                           │
                    │   ┌───────────────────┐   │
                    │   │   Classification  │   │
                    │   ├───────────────────┤   │
                    │   │ Family            │   │
                    │   │ Type              │   │
                    │   │ Class             │   │
                    │   └───────────────────┘   │
                    │                           │
                    └───────────────────────────┘

```

Family and Type are related hierarchically:

```text

               ┌──────────┐
               │  Family  │
               └────┬─────┘
                    │
                    ▼
               ┌──────────┐
               │   Type   │
               └──────────┘

```

Class is an independent classification dimension:

```text

                ┌──────────┐
                │  Class   │
                └──────────┘

```

---

# 40. Structural Invariants

The schema establishes the following structural invariants:

1. Classification contains the Family, Type and Class dimensions.
2. Family represents the broad documentary domain.
3. Type specializes Family.
4. Class represents documentary nature or role.
5. Class is not structurally subordinate to Type.
6. Classification is associated with a Document.
7. Classification is distinct from Document Identity.
8. The sequential Document ID component is not a Classification element.
9. Classification is independent of physical location.
10. Classification values require semantic definitions.

---

# 41. Schema Conformance

A Classification structure conforms to this schema when it preserves the established conceptual structure:

```text

                    Classification
                    ├── Family
                    ├── Type
                    └── Class

```

and preserves the following semantic relationships:

```text

    Family          →  Type
    Classification  →  Document
    Classification  ≠  Document Identity
    Classification  ≠  Physical Location

```

Conformance to the complete Classification system additionally depends on the vocabulary, constraints, validation and governance rules defined by the remaining Classification documents.

---

# 42. Implementation Neutrality

This schema deliberately avoids selecting a concrete implementation representation.

For example, the following are implementation possibilities rather than schema definitions:

```text

    JSON
    YAML
    XML
    Database
    Object Model
    Markdown Metadata

```

The schema must remain meaningful regardless of the implementation mechanism.

---

# 43. Relationship with Metadata Schema

Classification is a Metadata category.

Therefore, the Classification Schema is a specialized schema defining the structure of one Metadata category.

Conceptually:

```text

            Metadata Schema
            │
            ├── Identification
            ├── Classification
            │   ├── Family
            │   ├── Type
            │   └── Class
            ├── Lifecycle
            ├── Ownership
            ├── Localization
            └── Technical Information

```

The architectural blueprint establishes these categories as conceptual Metadata groupings.

---

# 44. Evolution Compatibility

The framework's Metadata architecture establishes incremental evolution as a design principle.

New properties may be introduced provided that they:

- do not alter the meaning of existing properties;
- maintain compatibility;
- respect separation of responsibilities.

The same principle applies to the Classification Schema.

---

# 45. Normative Structural Definition

The normative conceptual structure of the Classification Schema is:

```text

            Classification
                Family
                Type
                Class

```

with:

```text

    Family  →  Type

```

and:

```text

    Classification  →  Document

```

The schema does not establish an additional hierarchy involving Class.

---

# 46. Summary

The Classification Schema formalizes the structure established by the preceding Classification documents.

The schema is:

```text

            Classification
            │
            ├── Family
            ├── Type
            └── Class

```

Family identifies the broad documentary domain.

Type identifies the specific documentary category within that Family.

Class identifies the documentary nature or role.

The relationship between Family and Type is:

```text

            Family
            │
            └── Type

```

The relationship with the document is:

```text

            Document
            │
            └── Classification

```

Document Identity remains separate:

```text

            Document
            ├── Document Identity
            └── Classification

```

The historical Document ID:

```text

META-DCL-001

```

demonstrates the semantic relationship between Family, Type and document identity, with `001` serving as the sequential identifier rather than as a Classification element.

The Classification Schema therefore provides the structural foundation for:

- Classification Validation;
- Classification Constraints;
- Classification Dictionary;
- Classification Specification;
- Classification Examples.

---

# 47. Related Documents

## 47.1. Foundation

- DF-FND-001 — Framework Manifest
- DF-FND-002 — Research Journal
- DF-FND-003 — Evolution Timeline
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

## 47.2. Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-004 — Architectural Layers
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology
- DF-ARC-007 — Component Documentation Structure

## 47.3. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema

## 47.4. Classification

- DF-CLS-001 — Classification Architecture
- DF-CLS-002 — Classification Concepts
- DF-CLS-003 — Classification Model
- DF-CLS-004 — Classification Elements
- **DF-CLS-005 — Classification Schema**
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
| 1.0 | Initial definition of the Classification Schema. |

---

**End of Document**