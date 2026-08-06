# Documentation Framework

# DF-MTD-015 — Metadata Examples

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-015 |
| **Title** | Metadata Examples |
| **Family** | Metadata |
| **Type** | Examples |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

This document provides illustrative examples demonstrating how the architectural concepts defined throughout the Metadata component may be applied.

The examples are intended to improve understanding of the Metadata architecture.

They are informative only.

They do not define additional architectural requirements.

---

# 2. Purpose

The purpose of this document is to:

- illustrate Metadata concepts;
- demonstrate the interaction between Metadata artifacts;
- provide architectural examples;
- clarify the intended use of Metadata specifications.

---

# 3. Scope

This document contains examples of:

- Metadata Elements;
- Metadata Schemas;
- Metadata Profiles;
- Metadata Instances;
- Metadata Relationships;
- Metadata Validation;
- Metadata Governance.

The examples are implementation independent.

---

# 4. Example 1 — Metadata Element

The following example illustrates a Metadata Element.

| Attribute | Example |
|-----------|---------|
| Identifier | MTD-DOC-001 |
| Name | Document Identifier |
| Category | Identity Metadata |
| Definition | Uniquely identifies a document within a Documentation Framework repository. |
| Value Type | Identifier |
| Cardinality | Exactly One |
| Required | Yes |

This example illustrates the architectural definition of a Metadata Element.

---

# 5. Example 2 — Metadata Group

Metadata Elements may be organized into logical groups.

```text

                    Identity Metadata
                    │
                    ├── Document Identifier
                    ├── Document Version
                    ├── Document Revision
                    └── Baseline

```

The grouping improves organization without altering the semantics of individual Metadata Elements.

---

# 6. Example 3 — Metadata Schema

A Metadata Schema organizes Metadata Elements.

```text

                    Metadata Schema
                    │
                    ├── Identity Metadata
                    │   ├── Document Identifier
                    │   ├── Version
                    │   └── Revision
                    │
                    ├── Classification Metadata
                    │   ├── Category
                    │   ├── Status
                    │   └── Language
                    │
                    └── Lifecycle Metadata
                        ├── Created Date
                        ├── Updated Date
                        └── Lifecycle State

```

The schema defines the architectural organization of Metadata.

---

# 7. Example 4 — Metadata Profile

Different document categories may require different Metadata Profiles.

```text

                    Canonical Metadata Schema
                    │
                    ├──────────────────────────────┐
                    ▼                              ▼

              Specification                     Template
             Metadata Profile               Metadata Profile

```

Each profile specializes the canonical Metadata Schema while preserving Metadata semantics.

---

# 8. Example 5 — Metadata Instance

A Metadata Instance represents Metadata associated with a specific document.

Example.

| Metadata Element | Example Value |
|------------------|---------------|
| Document Identifier | DF-MTD-015 |
| Title | Metadata Examples |
| Version | 1.0 |
| Revision | 0 |
| Status | Draft |
| Language | English |

The values shown are illustrative only.

---

# 9. Example 6 — Metadata Lifecycle

Metadata evolves through lifecycle states.

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

The Metadata Lifecycle governs the evolution of Metadata definitions.

---

# 10. Example 7 — Metadata Validation

Validation evaluates Metadata against the applicable architectural specifications.

```text

                    Metadata Instance
                    │
                    ▼

                    Validation
                    │
                    ├────────────────────────┐
                    ▼                        ▼

                Compliant              Non-Compliant

```

Validation determines architectural compliance only.

---

# 11. Example 8 — Metadata Governance

Governance authorizes Metadata evolution.

```text

                 Metadata Change Proposal
                            │
                            ▼

                   Architectural Review
                            │
                            ▼

                   Governance Decision
                            │
               ┌────────────┴────────────┐
               ▼                         ▼

            Approved                 Rejected

```

Governance controls Metadata evolution.

---

# 12. Example 9 — Metadata Relationships

Metadata concepts are connected through explicit relationships.

```text

            Metadata Profile
                    │
               specializes
                    ▼

             Metadata Schema
                    │
                contains
                    ▼

            Metadata Elements
                    │
               described by
                    ▼

           Metadata Dictionary

```

Relationships preserve conceptual consistency.

---

# 13. Example 10 — Metadata Extension

Metadata evolves through controlled extensions.

```text

           Canonical Metadata
                    │
                    ▼

           Extension Proposal
                    │
                    ▼

           Governance Approval
                    │
                    ▼

            Extended Metadata

```

Extensions preserve compatibility with the existing Metadata architecture.

---

# 14. Example 11 — Metadata Dictionary Entry

Illustrative Dictionary Entry.

| Attribute | Example |
|-----------|---------|
| Identifier | MTD-CLS-001 |
| Name | Classification |
| Category | Classification Metadata |
| Definition | Indicates the classification assigned to a document. |
| Value Type | Classification |
| Cardinality | Exactly One |
| Required | Yes |
| Lifecycle Status | Published |

This example illustrates the architectural structure of a Dictionary Entry.

---

# 15. Example 12 — Complete Metadata Overview

The following conceptual model illustrates the interaction of the principal Metadata artifacts.

```text

                           Metadata Architecture
                                     │
                                     ▼

                             Metadata Concepts
                                     │
                                     ▼

                               Metadata Model
                                     │
                                     ▼

                             Metadata Elements
                                     │
                                     ▼

                              Metadata Schema
                                     │
                    ┌────────────────┴────────────────┐
                    ▼                                 ▼

            Metadata Profile                 Metadata Dictionary
                    │                                 │
                    └────────────────┬────────────────┘
                                     ▼

                             Metadata Instance
                                     │
                    ┌────────────────┴────────────────┐
                    ▼                                 ▼

           Metadata Validation               Metadata Governance
                    │                                 │
                    └────────────────┬────────────────┘
                                     ▼

                            Metadata Lifecycle
                                     │
                                     ▼

                          Metadata Extensibility

```

This diagram summarizes the architectural interaction of the Metadata component.

---

# 16. Informative Nature

All examples contained in this document are informative.

They are intended solely to clarify the Metadata architecture.

Examples:

- do not introduce new concepts;
- do not modify normative specifications;
- do not replace architectural definitions;
- do not constrain implementation choices.

---

# 17. Relationship with Other Documents

This document complements the normative Metadata documentation.

| Document | Relationship |
|----------|--------------|
| Metadata Concepts | Illustrates Metadata concepts. |
| Metadata Model | Illustrates conceptual organization. |
| Metadata Elements | Illustrates Metadata Elements. |
| Metadata Schema | Illustrates Metadata organization. |
| Metadata Lifecycle | Illustrates Metadata evolution. |
| Metadata Validation | Illustrates validation scenarios. |
| Metadata Governance | Illustrates governance decisions. |
| Metadata Dictionary | Illustrates Dictionary Entries. |
| Metadata Specification | Provides examples supporting the normative specification. |

---

# 18. Architectural Characteristics

Metadata Examples possess the following characteristics.

## 18.1. Informative

Examples are explanatory rather than normative.

---

## 18.2. Technology Independent

Examples avoid implementation-specific details.

---

## 18.3. Consistent

Examples remain aligned with the canonical Metadata architecture.

---

## 18.4. Reusable

Examples may be reused throughout the Documentation Framework documentation.

---

## 18.5. Illustrative

Examples improve understanding without extending the specification.

---

# 19. Conformance

Conformance with the Documentation Framework is **not** determined by reproducing the examples contained in this document.

Implementations shall conform to the normative requirements defined by **DF-MTD-014 — Metadata Specification**.

---

# 20. Related Documents

## 20.1. Foundation

- DF-FND-004 — Architectural Blueprint
- DF-FND-006 — Design Rationale

## 20.2. Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components

## 20.3. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema
- DF-MTD-006 — Metadata Lifecycle
- DF-MTD-007 — Metadata Validation
- DF-MTD-008 — Metadata Governance
- DF-MTD-009 — Metadata Relationships
- DF-MTD-010 — Metadata Constraints
- DF-MTD-011 — Metadata Extensibility
- DF-MTD-012 — Metadata Best Practices
- DF-MTD-013 — Metadata Dictionary
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---
