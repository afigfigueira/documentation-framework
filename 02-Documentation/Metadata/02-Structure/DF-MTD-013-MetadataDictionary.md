# Documentation Framework

# DF-MTD-013 — Metadata Dictionary

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-013 |
| **Title** | Metadata Dictionary |
| **Family** | Metadata |
| **Type** | Dictionary |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Metadata Dictionary is the authoritative catalog of all Metadata Elements defined by the Documentation Framework.

It establishes the canonical definitions, meanings and architectural characteristics of every Metadata Element.

The Metadata Dictionary serves as the single source of truth for Metadata semantics and ensures that every Metadata Element is interpreted consistently throughout the Documentation Framework.

---

# 2. Purpose

The purpose of the Metadata Dictionary is to provide the canonical reference for Metadata Elements.

It establishes:

- canonical Metadata Element definitions;
- Metadata terminology;
- Metadata semantics;
- Metadata characteristics;
- Metadata classification;
- Metadata lifecycle information.

---

# 3. Scope

This document specifies:

- the purpose of the Metadata Dictionary;
- the organization of dictionary entries;
- Metadata Element definitions;
- Metadata Element attributes;
- dictionary maintenance principles.

It does not define:

- Metadata architecture;
- Metadata schemas;
- Metadata profiles;
- validation rules;
- implementation formats.

---

# 4. Dictionary Principles

The Metadata Dictionary follows the principles below.

## 4.1. Canonical Definition

Every Metadata Element shall possess one authoritative definition.

---

## 4.2. Semantic Stability

Metadata definitions shall remain stable throughout their lifecycle.

---

## 4.3. Uniqueness

Each Metadata Element shall appear exactly once in the Metadata Dictionary.

---

## 4.4. Technology Independence

Metadata definitions shall remain independent of implementation technologies.

---

## 4.5. Traceability

Changes to Metadata definitions shall remain historically traceable.

---

# 5. Purpose of a Dictionary Entry

Each Dictionary Entry defines one Metadata Element.

A Dictionary Entry provides the complete architectural description of that Metadata Element independently of any implementation.

---

# 6. Dictionary Organization

The Metadata Dictionary is organized as a collection of Dictionary Entries.

Conceptually.

```text

                    Metadata Dictionary
                    │
                    ├── Dictionary Entry
                    │
                    ├── Dictionary Entry
                    │
                    ├── Dictionary Entry
                    │
                    └── ...

```

Each Dictionary Entry describes one Metadata Element.

---

# 7. Dictionary Entry Structure

Every Dictionary Entry should contain the following architectural information.

| Attribute | Description |
|-----------|-------------|
| Identifier | Unique Metadata Element identifier |
| Name | Canonical Metadata Element name |
| Category | Metadata Group or conceptual category |
| Definition | Canonical architectural definition |
| Purpose | Why the Metadata Element exists |
| Semantics | Architectural meaning |
| Value Type | Abstract value classification |
| Cardinality | Permitted occurrence |
| Required | Whether required by the canonical Metadata architecture |
| Default Value | Default value, if applicable |
| Lifecycle Status | Current lifecycle state |
| Version | Current architectural version |
| Revision | Current revision |
| Related Elements | Architecturally related Metadata Elements |
| Constraints | Applicable Metadata Constraints |
| Notes | Additional architectural observations |

The precise representation of Dictionary Entries is implementation independent.

---

# 8. Dictionary Classification

Metadata Elements may be classified according to their architectural purpose.

Typical classifications include:

- Identity Metadata
- Descriptive Metadata
- Structural Metadata
- Lifecycle Metadata
- Governance Metadata
- Traceability Metadata
- Discovery Metadata
- Automation Metadata

These classifications improve organization without affecting semantics.

---

# 9. Dictionary Responsibilities

The Metadata Dictionary is responsible for:

- defining Metadata Elements;
- preserving Metadata semantics;
- maintaining canonical terminology;
- supporting Metadata reuse;
- recording Metadata evolution.

The Metadata Dictionary is not responsible for:

- validating Metadata;
- governing Metadata;
- storing Metadata;
- interpreting document content.

---

# 10. Dictionary Lifecycle

Dictionary Entries evolve according to the Metadata Lifecycle.

Typical lifecycle events include:

- creation;
- refinement;
- publication;
- deprecation;
- retirement.

The Dictionary shall preserve historical information for every Metadata Element.

---

# 11. Dictionary Maintenance

The Metadata Dictionary shall be maintained through controlled architectural governance.

Maintenance activities include:

- adding new Metadata Elements;
- updating definitions;
- recording deprecation;
- documenting replacements;
- preserving historical versions.

Every modification shall be traceable.

---

# 12. Dictionary Relationships

The Metadata Dictionary interacts with several Metadata specifications.

| Document | Relationship |
|----------|--------------|
| Metadata Concepts | Defines the conceptual foundation of Metadata Elements. |
| Metadata Model | Defines how Metadata Elements relate. |
| Metadata Elements | Defines the architectural characteristics of Metadata Elements. |
| Metadata Schema | Organizes Metadata Elements structurally. |
| Metadata Profiles | Select Metadata Elements for specific document categories. |
| Metadata Lifecycle | Governs Metadata Element evolution. |
| Metadata Validation | Uses Dictionary definitions during validation. |
| Metadata Governance | Approves Dictionary evolution. |

The Dictionary references Metadata Elements but does not redefine their architecture.

---

# 13. Dictionary Entry Example

The following example illustrates the architectural structure of a Dictionary Entry.

| Attribute | Example |
|-----------|---------|
| Identifier | MTD-001 |
| Name | Document Identifier |
| Category | Identity Metadata |
| Definition | Unique identifier assigned to a document. |
| Purpose | Enables unambiguous document identification. |
| Value Type | Identifier |
| Cardinality | Exactly One |
| Required | Yes |
| Lifecycle Status | Published |
| Version | 1.0 |

The example is illustrative only.

It does not define canonical Metadata Elements.

---

# 14. Architectural Characteristics

The Metadata Dictionary possesses the following characteristics.

## 14.1. Authoritative

Provides the canonical definition of every Metadata Element.

---

## 14.2. Consistent

Maintains one semantic definition for each Metadata Element.

---

## 14.3. Technology Independent

Independent of implementation technologies.

---

## 14.4. Traceable

Preserves historical evolution.

---

## 14.5. Stable

Definitions evolve through controlled governance.

---

## 14.6. Reusable

Supports all Metadata Profiles and Metadata Schemas.

---

# 15. Conformance

A Metadata Dictionary conforms to this specification when:

- every Metadata Element possesses exactly one Dictionary Entry;
- Metadata definitions are canonical;
- Metadata semantics remain stable;
- Metadata evolution is traceable;
- Dictionary Entries remain technology independent.

---

# 16. Related Documents

## 16.1. Architecture

- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology

## 16.2. Metadata

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
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---