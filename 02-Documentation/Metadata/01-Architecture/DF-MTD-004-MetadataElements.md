# Documentation Framework

# DF-MTD-004 — Metadata Elements

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-004 |
| **Title** | Metadata Elements |
| **Family** | Metadata |
| **Type** | Elements |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

Metadata is composed of a collection of Metadata Elements.

Each Metadata Element represents one atomic architectural characteristic of a document.

Metadata Elements constitute the fundamental building blocks of the Metadata component and provide the descriptive information consumed by the remaining components of the Documentation Framework.

---

# 2. Purpose

The purpose of this document is to define the architectural characteristics of Metadata Elements.

It specifies:

- what a Metadata Element is;
- its architectural role;
- its lifecycle;
- its characteristics;
- its relationships with other Metadata concepts.

This document does not define the individual Metadata Elements of the Documentation Framework.

Those definitions are maintained by the Metadata Dictionary.

---

# 3. Scope

This specification applies to every Metadata Element defined by the Documentation Framework.

It defines:

- Metadata Element characteristics;
- Metadata Element responsibilities;
- Metadata Element lifecycle;
- Metadata Element relationships;
- Metadata Element constraints.

It does not define:

- Metadata Schemas;
- Metadata Profiles;
- Metadata validation rules;
- implementation details.

---

# 4. Architectural Position

Metadata Elements are the smallest architectural units within the Metadata component.

Conceptually.

```text

                    Metadata
                    │
                    ├── Metadata Element
                    ├── Metadata Element
                    ├── Metadata Element
                    └── Metadata Element

```

Every Metadata instance is composed exclusively of Metadata Elements.

---

# 5. Definition

A Metadata Element is the smallest indivisible architectural unit used to describe a document.

Each Metadata Element represents one descriptive concept.

Its semantic meaning is stable and independent of any implementation technology.

---

# 6. Purpose of Metadata Elements

Metadata Elements exist to provide standardized descriptive information about documents.

Each Metadata Element contributes one specific architectural characteristic.

Collectively, Metadata Elements allow documents to become:

- self-describing;
- consistently identifiable;
- semantically classifiable;
- governable;
- discoverable;
- traceable.

---

# 7. Characteristics

Every Metadata Element shall possess the following characteristics.

## 7.1. Atomic

A Metadata Element represents exactly one architectural concept.

---

## 7.2. Canonical

Every Metadata Element has one authoritative definition.

---

## 7.3. Explicit

Its meaning shall be unambiguous.

---

## 7.4. Stable

Its semantic meaning shall not change over time.

---

## 7.5. Reusable

The same Metadata Element may appear in multiple Metadata Profiles.

---

## 7.6. Technology Independent

Its definition shall not depend on implementation technologies.

---

## 7.7. Extensible

New Metadata Elements may be introduced without modifying existing ones.

---

# 8. Responsibilities

Each Metadata Element is responsible for:

- representing one descriptive characteristic;
- preserving its semantic meaning;
- supporting Metadata consistency;
- contributing to document description.

Metadata Elements shall not:

- perform validation;
- implement business rules;
- determine document identity;
- classify documents;
- control document lifecycle.

---

# 9. Metadata Element Structure

Conceptually, every Metadata Element is composed of three architectural parts.

```text
Metadata Element

                    │
                    ├── Definition
                    ├── Semantics
                    └── Value

```

## 9.1. Definition

Provides the canonical architectural meaning.

---

## 9.2. Semantics

Defines how the Metadata Element shall be interpreted.

---

## 9.3. Value

Represents the information associated with a specific document.

---

# 10. Metadata Element Categories

Metadata Elements may belong to different conceptual categories.

Examples include:

- Identity Elements
- Descriptive Elements
- Structural Elements
- Lifecycle Elements
- Governance Elements
- Traceability Elements
- Discovery Elements
- Automation Elements

These categories organize Metadata Elements conceptually.

They do not alter their architectural behavior.

---

# 11. Metadata Element Relationships

Metadata Elements participate in the Metadata Model through explicit relationships.

```text

                Metadata
                    │
                    ▼

             Metadata Element
                    │
                    ▼

              Metadata Value

```

Metadata Elements are defined by the Metadata Schema.

Metadata Values instantiate Metadata Elements.

Metadata Profiles determine where Metadata Elements are used.

---

# 12. Metadata Element Lifecycle

Each Metadata Element follows a controlled architectural lifecycle.

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

                Published
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

Deprecation does not invalidate existing Metadata.

Deprecated Metadata Elements remain documented for compatibility purposes.

---

# 13. Architectural Constraints

Metadata Elements shall satisfy the following constraints.

## 13.1. Single Meaning

A Metadata Element shall represent one architectural concept only.

---

## 13.2. Unique Definition

Each Metadata Element shall possess one authoritative definition.

---

## 13.3. Non-Redundancy

Equivalent Metadata Elements shall not coexist.

---

## 13.4. Stable Semantics

Semantic meaning shall remain stable throughout architectural evolution.

---

## 13.5. Controlled Evolution

Changes shall occur only through controlled architectural evolution.

---

# 14. Architectural Rules

The Documentation Framework establishes the following rules.

## 14.1. Rule 1 — Atomicity

Metadata Elements shall not combine multiple concepts.

---

## 14.2. Rule 2 — Independence

Metadata Elements shall remain independent of implementation.

---

## 14.3. Rule 3 — Consistency

Metadata Elements shall preserve their semantics across all Metadata Profiles.

---

## 14.4. Rule 4 — Reuse

Metadata Elements shall be reused whenever possible.

---

## 14.5. Rule 5 — No Duplication

Duplicate Metadata Elements shall not exist.

---

# 15. Metadata Element Identification

Every Metadata Element shall possess a permanent architectural identity.

This identity shall remain stable regardless of:

- Metadata Schemas;
- Metadata Profiles;
- implementation technologies;
- serialization formats.

The identification mechanism itself is defined separately from the Metadata Element architecture.

---

# 16. Relationship with Other Metadata Documents

The Metadata Elements specification collaborates with the remaining Metadata documents.

| Document | Responsibility |
|----------|----------------|
| Metadata Concepts | Defines Metadata concepts. |
| Metadata Model | Defines conceptual organization. |
| Metadata Elements | Defines the architectural building blocks. |
| Metadata Schema | Organizes Metadata Elements. |
| Metadata Dictionary | Defines every Metadata Element individually. |
| Metadata Specification | Provides the complete normative specification. |

---

# 17. Conformance

A Metadata implementation conforms to this specification when:

- every Metadata Element represents exactly one concept;
- Metadata Elements preserve semantic stability;
- Metadata Elements remain technology independent;
- Metadata Elements possess canonical definitions;
- Metadata Elements are reusable across Metadata Profiles;
- Metadata Elements evolve through controlled architectural evolution.

---

# 18. Related Documents

## 18.1. Architecture

- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology

## 18.2. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-005 — Metadata Schema
- DF-MTD-013 — Metadata Dictionary
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---