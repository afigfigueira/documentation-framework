# Documentation Framework

# DF-MTD-005 — Metadata Schema

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-005 |
| **Title** | Metadata Schema |
| **Family** | Metadata |
| **Type** | Schema |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Metadata Schema defines the formal organization of Metadata within the Documentation Framework.

It specifies how Metadata Elements are organized into a coherent structural model while remaining independent of implementation technologies, serialization formats and storage mechanisms.

The Metadata Schema establishes the canonical structure from which Metadata Profiles and Metadata Instances are derived.

---

# 2. Purpose

The purpose of the Metadata Schema is to define the structural organization of Metadata.

It provides:

- the canonical organization of Metadata Elements;
- structural constraints;
- Metadata composition rules;
- Metadata grouping principles;
- the structural foundation for Metadata Profiles.

---

# 3. Scope

This document defines the architectural structure of Metadata.

It specifies:

- Metadata organization;
- Metadata composition;
- Metadata groups;
- structural relationships;
- structural constraints.

It does not define:

- Metadata concepts;
- Metadata Element semantics;
- Metadata validation;
- implementation formats;
- serialization rules.

---

# 4. Architectural Position

The Metadata Schema is positioned between the conceptual Metadata Model and the specialized Metadata Profiles.

```text

            Metadata Concepts
                    │
                    ▼

              Metadata Model
                    │
                    ▼

             Metadata Schema
                    │
                    ▼

            Metadata Profiles
                    │
                    ▼

            Metadata Instances

```

The Schema formalizes structure without altering semantics.

---

# 5. Definition

A Metadata Schema is the canonical structural definition of Metadata.

It defines how Metadata Elements are organized, grouped and composed.

The Schema establishes structural consistency while remaining independent of implementation.

---

# 6. Design Objectives

The Metadata Schema has the following objectives.

- provide a canonical Metadata structure;
- support structural consistency;
- enable Metadata reuse;
- facilitate extensibility;
- preserve compatibility;
- support specialized Metadata Profiles.

---

# 7. Schema Composition

The Metadata Schema is composed of Metadata Elements organized into logical groups.

```text

                    Metadata Schema
                    │
                    ├── Metadata Group
                    │   ├── Metadata Element
                    │   ├── Metadata Element
                    │   └── Metadata Element
                    │
                    ├── Metadata Group
                    │   ├── Metadata Element
                    │   └── Metadata Element
                    │
                    └── Metadata Group
                        ├── Metadata Element
                        ├── Metadata Element
                        └── Metadata Element

```

Grouping exists solely to organize Metadata.

Groups do not modify the semantics of Metadata Elements.

---

# 8. Metadata Groups

Metadata Elements may be organized into conceptual groups.

Typical groups include:

- Identity Metadata
- Descriptive Metadata
- Structural Metadata
- Lifecycle Metadata
- Governance Metadata
- Traceability Metadata
- Discovery Metadata
- Automation Metadata

The Metadata Schema defines the grouping mechanism.

Individual Metadata Profiles determine which groups are applicable.

---

# 9. Metadata Composition Rules

The Metadata Schema shall satisfy the following composition rules.

## 9.1. Rule 1

Metadata is composed exclusively of Metadata Elements.

---

## 9.2. Rule 2

Each Metadata Element belongs to one conceptual group.

---

## 9.3. Rule 3

Metadata Groups organize Metadata Elements but do not change their meaning.

---

## 9.4. Rule 4

Metadata Elements may appear in multiple Metadata Profiles.

---

## 9.5. Rule 5

Metadata Profiles shall not redefine Metadata Element semantics.

---

# 10. Structural Relationships

The Metadata Schema establishes the following structural relationships.

| Source | Relationship | Target |
|----------|-------------|--------|
| Metadata Schema | organizes | Metadata Groups |
| Metadata Group | contains | Metadata Elements |
| Metadata Profile | specializes | Metadata Schema |
| Metadata Instance | conforms to | Metadata Profile |

---

# 11. Cardinality

The Metadata Schema supports structural cardinality independently of implementation.

Typical cardinalities include:

- exactly one;
- zero or one;
- one or many;
- zero or many.

Cardinality constraints are defined by Metadata Profiles rather than by the Metadata Schema itself.

---

# 12. Mandatory and Optional Elements

The Metadata Schema identifies Metadata Elements independently of their usage requirements.

Whether a Metadata Element is:

- mandatory;
- optional;
- conditional;

is determined by the applicable Metadata Profile.

The Schema itself remains neutral regarding element obligation.

---

# 13. Structural Constraints

The Metadata Schema shall satisfy the following constraints.

## 13.1. Canonical Organization

There shall be one authoritative Metadata Schema.

---

## 13.2. Structural Independence

The Schema shall remain independent of implementation technologies.

---

## 13.3. Semantic Preservation

Structural organization shall not modify Metadata semantics.

---

## 13.4. Extensibility

The Schema shall permit new Metadata Elements without restructuring the existing architecture.

---

## 13.5. Stability

The Schema shall evolve incrementally while preserving compatibility.

---

# 14. Metadata Profile Specialization

Metadata Profiles specialize the Metadata Schema.

Profiles may:

- select Metadata Groups;
- select Metadata Elements;
- define mandatory Metadata;
- define optional Metadata;
- define conditional Metadata;
- define structural constraints.

Profiles shall not:

- redefine Metadata semantics;
- modify Metadata Element definitions;
- alter the Metadata Model.

---

# 15. Metadata Instance Conformance

Every Metadata Instance shall conform to exactly one Metadata Profile.

A Metadata Instance is considered structurally valid when:

- all required Metadata Elements are present;
- no prohibited Metadata Elements are present;
- structural rules defined by the Metadata Profile are respected.

Semantic validation is outside the scope of this document.

---

# 16. Schema Evolution

The Metadata Schema evolves through controlled architectural evolution.

Schema evolution may include:

- introduction of new Metadata Groups;
- introduction of new Metadata Elements;
- controlled deprecation;
- structural refinement.

Schema evolution shall preserve compatibility whenever possible.

---

# 17. Architectural Characteristics

The Metadata Schema possesses the following characteristics.

## 17.1. Canonical

One authoritative structural definition.

---

## 17.2. Technology Independent

Independent of implementation technologies.

---

## 17.3. Format Independent

Independent of serialization formats.

---

## 17.4. Repository Independent

Independent of repositories.

---

## 17.5. Extensible

Supports controlled architectural evolution.

---

## 17.6. Reusable

Supports multiple Metadata Profiles.

---

## 17.7. Stable

Structural changes occur only through architectural governance.

---

# 18. Relationship with Other Metadata Documents

| Document | Responsibility |
|----------|----------------|
| Metadata Concepts | Defines Metadata concepts. |
| Metadata Model | Defines conceptual relationships. |
| Metadata Elements | Defines architectural building blocks. |
| Metadata Schema | Defines structural organization. |
| Metadata Lifecycle | Defines Metadata evolution. |
| Metadata Validation | Defines validation rules. |
| Metadata Dictionary | Defines individual Metadata Elements. |
| Metadata Specification | Defines the complete normative specification. |

---

# 19. Conformance

A Metadata implementation conforms to this specification when:

- Metadata follows the canonical Metadata Schema;
- Metadata Elements remain structurally organized;
- Metadata Profiles specialize rather than redefine the Metadata Schema;
- Metadata Instances conform to one Metadata Profile;
- structural consistency is preserved across the Metadata architecture.

---

# 20. Related Documents

## 20.1. Architecture

- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components

## 20.2. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-006 — Metadata Lifecycle
- DF-MTD-007 — Metadata Validation
- DF-MTD-013 — Metadata Dictionary
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---