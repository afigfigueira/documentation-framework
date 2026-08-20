# Documentation Framework

# DF-CLS-004 — Classification Elements

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-004 |
| **Title** | Classification Elements |
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

The Classification component organizes documents according to their semantic characteristics.

The Classification Model established three principal classification dimensions:

- **Family**;
- **Type**;
- **Class**.

This document defines these classification elements in greater detail.

The purpose is to establish the semantic responsibility of each element without defining the formal representation of the classification structure.

The formal representation is defined separately by **DF-CLS-005 — Classification Schema**.

---

# 2. Purpose

The purpose of this document is to define the elements that constitute the Classification structure.

It establishes:

- the identity of each classification element;
- its semantic purpose;
- its scope;
- its relationship with the other classification elements;
- its relationship with Document Identity;
- its relationship with the Document ID.

The elements defined by this document are:

```text

            Classification
            │
            ├── Family
            ├── Type
            └── Class

```

The framework's architectural material explicitly identifies Family, Type and Class as the properties through which documents are classified.

---

# 3. Scope

This document defines the semantic characteristics of:

- Family;
- Type;
- Class.

It does not define:

- the complete Classification Model;
- the formal Classification Schema;
- lifecycle states;
- validation rules;
- governance rules;
- classification relationships;
- classification constraints;
- extensibility mechanisms;
- implementation-specific representations.

---

# 4. Classification Element

A **Classification Element** is a defined semantic property through which a document's classification is expressed.

The Classification structure contains three principal elements:

```text id="cls-el-001"

            Classification
            │
            ├── Family
            ├── Type
            └── Class

```

Each element has a distinct responsibility.

The elements must not be treated as interchangeable labels.

---

# 5. Element Responsibilities

The principal responsibilities are:

| Element | Responsibility |
|---------|----------------|
| **Family** | Identifies the broad documentary domain |
| **Type** | Identifies the specific documentary category within a Family |
| **Class** | Identifies the nature or role of the document |

This distinction preserves the conceptual separation established by the Classification Model.

---

# 6. Family

## 6.1. Definition

**Family** identifies the broad documentary domain to which a document belongs.

It provides the highest-level classification dimension currently defined by the framework.

Conceptually:

```text id="cls-el-002"

            Family
            │
            ├── Type
            ├── Type
            └── Type

```

A Family groups documents that belong to the same broad semantic domain.

---

## 6.2. Purpose

The purpose of Family is to provide broad semantic organization.

Family answers the question:

> **What broad documentary domain does this document belong to?**

The architectural material describes Family as a means of organizing knowledge.

---

## 6.3. Scope

Family operates at the broad documentary level.

It should therefore not be used to represent:

- a specific document;
- a document version;
- a document revision;
- a physical directory;
- a repository;
- a file format.

---

## 6.4. Family Identity

A Family is identified by its classification value.

For example:

```text id="cls-el-003"

    META

```

represents a Family value used by the Documentation Framework.

The introduction of the `META` Family established a documentary domain concerned with the Documentation Framework itself.

---

## 6.5. Family Stability

The semantic meaning of a Family should remain stable once established.

Changing the meaning of an existing Family would affect every Type and document associated with that Family.

Therefore, changes to Family semantics require controlled architectural evolution.

---

# 7. Type

## 7.1. Definition

**Type** identifies a specific documentary category within a Family.

Type provides a more precise classification than Family.

Conceptually:

```text id="cls-el-004"

            Family
            │
            ├── Type
            ├── Type
            └── Type

```

The historical framework explicitly established the relationship in which Type specializes Family.

---

## 7.2. Purpose

The purpose of Type is to refine the broad classification established by Family.

Type answers the question:

> **What specific documentary category is this document within its Family?**

---

## 7.3. Type and Family

A Type is interpreted in the context of a Family.

Conceptually:

```text id="cls-el-005"

                  Family
                    │
                    ▼

                  Type

```

The same Type value should therefore not automatically be assumed to have identical meaning across unrelated classification contexts.

---

## 7.4. Historical Representation

The framework historically represented Family and Type together in Document IDs.

For example:

```text id="cls-el-006"

    META-DCL-001

```

where:

```text

    META = Family
    DCL  = Type
    001  = sequential document identifier

```

This interpretation is explicitly documented in the architectural material.

---

## 7.5. Type Specialization

Type provides specialization rather than a replacement for Family.

Therefore:

```text id="cls-el-007"

            Family
            │
            └── Type

```

means:

> the Type identifies a more specific documentary category within the Family.

It does not mean that Family and Type are independent classifications with unrelated meanings.

---

# 8. Class

## 8.1. Definition

**Class** identifies the nature or role of a document.

Class provides a semantic dimension distinct from the Family → Type hierarchy.

Conceptually:

```text id="cls-el-008"

            Classification
            │
            ├── Family
            ├── Type
            └── Class

```

---

## 8.2. Purpose

The purpose of Class is to distinguish documents according to their documentary nature or role.

Class answers the question:

> **What is the nature or role of this document?**

This distinction is important because two documents may belong to the same Family and Type while performing different documentary roles.

---

## 8.3. Class Independence

Class is not defined as a third hierarchical level below Type.

The conceptual structure is therefore:

```text id="cls-el-009"

            Family
            │
            └── Type

            Class

```

rather than:

```text

          Family
            │
            └── Type
                 │
                 └── Class

```

The latter interpretation is not established by the current framework material and should not be assumed.

---

# 9. Classification Elements as Dimensions

The three elements provide complementary classification dimensions.

```text id="cls-el-010"

                    Classification
                   /      |       \
                  /       |        \
                 ▼        ▼         ▼
              Family     Type     Class

```

Their semantic responsibilities are:

```text

            Family →  documentary domain

            Type   →  documentary category

            Class  →  documentary nature or role

```

---

# 10. Element Relationship

The elements have the following conceptual relationship:

```text id="cls-el-011"

                  Family
                    │
               specializes
                    │ 
                    ▼

                   Type


                  Class
                    │
                describes
                    │
                    ▼

                 Document

```

Family and Type therefore participate in a hierarchical relationship.

Class provides an additional semantic dimension.

---

# 11. Family-Type Combination

A Family and Type together provide a more precise documentary classification.

Conceptually:

```text id="cls-el-012"

              Family + Type
                    │
                    ▼

      Specific Documentary Category

```

For example:

```text

    META + DCL

```

produces:

```text

    META-DCL

```

The framework historically used this structure for document classification and Document IDs.

---

# 12. Classification Tuple

The three elements can be represented conceptually as:

```text id="cls-el-013"

    Classification = (Family, Type, Class)

```

For example:

```text

    (Family, Type, Class)

```

The tuple is a conceptual representation.

It does not define serialization syntax.

The formal representation belongs to **DF-CLS-005 — Classification Schema**.

---

# 13. Element Value

Each classification element may have a defined value.

Conceptually:

```text id="cls-el-014"

            Classification
            │
            ├── Family = Family Value
            ├── Type   = Type Value
            └── Class  = Class Value

```

The element identifies the semantic dimension.

The value identifies the specific member of that dimension.

---

# 14. Element Identifier

Each classification element requires an identifiable semantic definition.

At the conceptual level:

| Element | Semantic Identifier |
|---------|---------------------|
| Family | Family |
| Type | Type |
| Class | Class |

The element identifier is not the same thing as the value assigned to that element.

For example:

```text

    Element = Family
    Value   = META

```

and:

```text

    Element = Type
    Value   = DCL

```

---

# 15. Element Label

An element may have a human-readable label.

For example:

```text

    Family
    Type
    Class

```

Labels are presentation characteristics.

They do not themselves determine semantic identity.

A formal schema may define how labels are represented, but such representation is outside the scope of this document.

---

# 16. Element Definition

Each element requires an authoritative definition.

Conceptually:

```text id="cls-el-015"

            Classification Element
            │
            ├── Identifier
            ├── Name
            ├── Definition
            └── Semantic Role

```

The Classification Dictionary will provide the authoritative terminology and definitions for the component.

---

# 17. Family Element Definition

The Family element can be summarized as:

| Property | Definition |
|----------|------------|
| **Name** | Family |
| **Purpose** | Broad documentary classification |
| **Scope** | Documentary domain |
| **Hierarchy** | Highest classification level |
| **Relationship** | Parent of Type |
| **Example** | META |

---

# 18. Type Element Definition

The Type element can be summarized as:

| Property | Definition |
|----------|------------|
| **Name** | Type |
| **Purpose** | Specific documentary classification |
| **Scope** | Within a Family |
| **Hierarchy** | Specializes Family |
| **Relationship** | Child of Family |
| **Example** | DCL |

---

# 19. Class Element Definition

The Class element can be summarized as:

| Property | Definition |
|----------|------------|
| **Name** | Class |
| **Purpose** | Documentary nature or role |
| **Scope** | Document |
| **Hierarchy** | Independent dimension |
| **Relationship** | Describes documentary nature |
| **Example** | To be defined by the Classification Dictionary |

The current source material establishes the semantic role of Class but does not establish an authoritative enumeration of Class values. That enumeration should therefore not be invented in this document.

---

# 20. Element Optionality

The existence of a classification element and the requirement that it receive a value are separate questions.

This document establishes the three elements as part of the Classification model.

It does not establish whether every document must have a value for every element.

Such cardinality and mandatory/optional rules belong to:

- the Classification Schema;
- Classification Constraints;
- Classification Validation.

---

# 21. Element Uniqueness

Classification elements do not identify documents uniquely.

For example, multiple documents may have:

```text

    Family = META
    Type   = DCL
    Class  = <same value>

```

These documents remain distinct because Document Identity identifies the individual documents.

The architectural material explicitly distinguishes the sequential component of the Document ID as the identifier that distinguishes documents within the same classification.

---

# 22. Elements and Document Identity

The relationship is:

```text id="cls-el-016"

            Document
            │
            ├── Document Identity
            │
            └── Classification
                ├── Family
                ├── Type
                └── Class

```

Document Identity answers:

> Which document is this?

Classification answers:

> How is this document semantically categorized?

The two responsibilities remain separate.

---

# 23. Elements and Document ID

The historical Document ID demonstrates the relationship between classification and identity:

```text id="cls-el-017"

            META-DCL-001
            │    │   │
            │    │   └── Document Identity sequence
            │    │
            │    └────── Type
            │
            └─────────── Family

```

The classification components of the identifier provide semantic information.

The final sequential component identifies the particular document.

Therefore:

```text

    Classification ≠ Document Identity

```

---

# 24. Elements and Metadata

Classification Elements are represented as part of the document's metadata.

The architectural blueprint defines Metadata as a structured set of properties associated with a document and identifies Classification as one of its categories.

Conceptually:

```text id="cls-el-018"

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

Metadata provides the structured document description.

The Classification component defines the semantics of the classification elements.

---

# 25. Elements and Physical Organization

Classification Elements are independent of physical organization.

They must not derive their meaning from:

- directory names;
- filenames;
- repository paths;
- storage systems;
- file formats.

The architectural blueprint explicitly distinguishes logical organization from physical location and states that the document remains the same when its file is moved between directories.

---

# 26. Element Values and Controlled Vocabulary

Element values should belong to a controlled classification vocabulary.

Conceptually:

```text id="cls-el-019"

         Classification Element
                    │
                    ▼

            Controlled Values
                    │
                    ▼

         Document Classification

```

For example:

```text

    Family  →  META
    Type    →  DCL

```

The Classification Dictionary will provide the authoritative definitions of permitted classification terminology.

---

# 27. Element Semantics

The meaning of an element must remain distinct from the meaning of its values.

For example:

```text

    Element:
    Family

    Value:
    META

```

means:

- `Family` defines the classification dimension;
- `META` identifies a specific value within that dimension.

Similarly:

```text

    Element:
    Type

    Value:
    DCL

```

means:

- `Type` defines the classification dimension;
- `DCL` identifies a specific value within that dimension.

---

# 28. Element Independence

Each classification element has a distinct responsibility.

The following interpretations are therefore avoided:

```text

Family = Type

```

or:

```text

    Type = Class

```

or:

```text

    Class = third hierarchy level

```

Instead:

```text

          Family
            │
            └── Type

          Class

```

This preserves the conceptual distinctions established by the Classification Model.

---

# 29. Element Evolution

Classification Elements may evolve as the Documentation Framework develops.

Evolution shall preserve the established meaning of existing elements.

The framework's architectural approach explicitly favors incremental growth while maintaining separation of responsibilities.

Therefore:

- new elements may be introduced through controlled architectural evolution;
- existing elements should not be silently redefined;
- existing classifications should remain interpretable;
- changes should preserve compatibility where required.

Detailed extensibility rules belong to **DF-CLS-011 — Classification Extensibility**.

---

# 30. Element Lifecycle

The lifecycle of an element is distinct from the lifecycle of a document.

For example:

```text

    Classification Element Lifecycle
                    │
                    ├── Definition
                    ├── Activation
                    ├── Deprecation
                    └── Retirement

```

This document does not define those lifecycle states.

They are specified by **DF-CLS-006 — Classification Lifecycle**.

---

# 31. Element Validation

An element value is valid only when it conforms to the rules applicable to its classification context.

Conceptually:

```text id="cls-el-020"

                 Element
                    │
                    ▼

                  Value
                    │
                    ▼

                Validation

```

The formal validation rules are outside the scope of this document.

They belong to **DF-CLS-007 — Classification Validation** and **DF-CLS-010 — Classification Constraints**.

---

# 32. Element Relationships

The principal relationships between the elements are:

```text id="cls-el-021"

Family
  │
  │ specializes
  ▼

Type


                  Class
                    │
              characterizes
                    │
                    ▼

                 Document

```

These relationships provide the semantic foundation for the classification structure.

Additional classification relationships are defined separately by **DF-CLS-009 — Classification Relationships**.

---

# 33. Element Constraints

The conceptual constraints established by this document are:

1. Family identifies a broad documentary domain.
2. Type identifies a specific category within a Family.
3. Type specializes Family.
4. Class identifies documentary nature or role.
5. Class is not implicitly subordinate to Type.
6. Classification elements do not provide Document Identity.
7. Element values require defined semantic meaning.
8. Classification elements are independent of physical document location.

Formal constraints are deferred to **DF-CLS-010 — Classification Constraints**.

---

# 34. Element Naming

The canonical names of the current classification elements are:

```text

    Family
    Type
    Class

```

These names shall be used consistently throughout the Documentation Framework.

Alternative names should not be introduced for the same semantic concepts unless explicitly established through architectural evolution.

---

# 35. Element Terminology

The following terminology is normative at the conceptual level:

| Term | Meaning |
|------|---------|
| **Classification Element** | A semantic dimension of Classification |
| **Family** | Broad documentary domain |
| **Type** | Specific documentary category within a Family |
| **Class** | Documentary nature or role |
| **Element Value** | A specific value assigned to an element |

This terminology shall be used consistently by subsequent Classification documents.

---

# 36. Element Model

The complete conceptual element model is:

```text id="cls-el-022"

                    ┌───────────────────────────────┐
                    │         Classification        │
                    ├───────────────────────────────┤
                    │    Family                     │
                    │    Type                       │
                    │    Class                      │
                    └───────────────┬───────────────┘
                                    │
                                    ▼

                           ┌─────────────────┐
                           │ Element Values  │
                           └─────────────────┘

```

Family and Type have a hierarchical relationship:

```text id="cls-el-023"

          Family
            │
            └── Type

```

Class remains an independent classification dimension:

```text id="cls-el-024"

      Classification
            ├── Family
            ├── Type
            └── Class

```

---

# 37. Element Representation

This document defines the semantic elements, not their serialization.

A future representation may express:

```text

    Family = META
    Type   = DCL
    Class  = <value>

```

but the exact representation format is outside this document.

The formal representation is defined by **DF-CLS-005 — Classification Schema**.

---

# 38. Element Dictionary

The Classification Dictionary will provide the authoritative definitions for:

- Family;
- Type;
- Class;
- their associated terminology;
- their permitted values where applicable.

This document establishes the conceptual definitions required before the Dictionary is produced.

---

# 39. Conformance

A Classification implementation conforms conceptually to this document when:

- it recognizes Family, Type and Class as distinct classification elements;
- Family represents a broad documentary domain;
- Type represents a specific documentary category within a Family;
- Type specializes Family;
- Class represents documentary nature or role;
- Class is not implicitly modeled as a third hierarchy level;
- classification elements remain distinct from Document Identity;
- element values have defined semantics;
- classification does not depend on physical document organization.

---

# 40. Summary

The Classification component defines three principal elements:

```text id="cls-el-025"

            Classification
            │
            ├── Family
            ├── Type
            └── Class

```

Their responsibilities are:

```text

    Family →  broad documentary domain

    Type   →  specific documentary category

    Class  →  documentary nature or role

```

Family and Type form a hierarchy:

```text

          Family
            │
            └── Type

```

Class represents an additional classification dimension:

```text

            Classification
            ├── Family
            ├── Type
            └── Class

```

The elements describe a document but do not identify it.

The distinction remains:

```text

Classification → describes semantic organization

Document Identity → identifies the document

```

The formal representation of these elements is deferred to **DF-CLS-005 — Classification Schema**.

---

# 41. Related Documents

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
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema

## Classification

- DF-CLS-001 — Classification Architecture
- DF-CLS-002 — Classification Concepts
- DF-CLS-003 — Classification Model
- **DF-CLS-004 — Classification Elements**
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
| 1.0 | Initial definition of Classification Elements. |

---

**End of Document**

---