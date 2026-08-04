# Documentation Framework

# DF-MTD-002 — Metadata Concepts

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-002 |
| **Title** | Metadata Concepts |
| **Family** | Metadata |
| **Type** | Concepts |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Metadata component is founded upon a collection of architectural concepts that define the semantics of document description within the Documentation Framework.

These concepts establish the canonical vocabulary required to model, describe and evolve Metadata consistently across the framework.

This document defines those concepts independently of any implementation technology, serialization format or storage mechanism.

---

# 2. Purpose

The purpose of this document is to establish the conceptual model of the Metadata component.

It defines:

- the fundamental Metadata concepts;
- the semantics of each concept;
- the relationships between concepts;
- the conceptual boundaries of the Metadata domain.

---

# 3. Scope

This document defines the architectural concepts used by the Metadata component.

It does not define:

- Metadata structures;
- Metadata schemas;
- Metadata elements;
- validation rules;
- implementation models.

These topics are specified in dedicated Metadata documents.

---

# 4. Conceptual Principles

The Metadata conceptual model follows the principles below.

## 4.1. Explicit Semantics

Every Metadata concept shall possess one clearly defined meaning.

---

## 4.2. Single Source of Truth

Each concept shall have one authoritative definition.

---

## 4.3. Technology Independence

Concepts shall remain independent of implementation technologies.

---

## 4.4. Conceptual Stability

Concepts shall evolve only through controlled architectural evolution.

---

## 4.5. Separation of Responsibilities

Concepts shall describe architectural meaning without introducing implementation concerns.

---

# 5. Core Concepts

## 5.1. Metadata

### 5.1.1. Definition

Metadata is structured descriptive information that characterizes a document independently of its content.

Metadata provides architectural information about a document rather than the knowledge contained within it.

### 5.1.2. Purpose

To make every document self-describing.

---

## 5.2. Metadata Element

### 5.2.1. Definition

A Metadata Element is an individual architectural unit of Metadata representing one specific descriptive characteristic of a document.

Each Metadata Element has a single architectural meaning.

### 5.2.2. Examples

- Document ID
- Title
- Version
- Language

The complete definition of Metadata Elements is provided by the Metadata Elements specification.

---

## 5.3. Metadata Value

### 5.3.1. Definition

A Metadata Value is the information assigned to a Metadata Element for a specific document.

The same Metadata Element may possess different values in different documents while preserving its semantic meaning.

---

## 5.4. Metadata Model

### 5.4.1. Definition

The Metadata Model defines the conceptual organization of Metadata and the relationships between Metadata concepts.

It establishes the abstract structure used by the Documentation Framework.

The Metadata Model is independent of any concrete representation.

---

## 5.5. Metadata Schema

### 5.5.1. Definition

A Metadata Schema specifies the formal structure used to organize Metadata Elements.

It defines which Metadata Elements may exist and how they are organized.

The Metadata Schema does not define implementation formats.

---

## 5.6. Metadata Profile

### 5.6.1. Definition

A Metadata Profile is a constrained view of a Metadata Schema intended for a specific category of documents.

A profile selects the Metadata Elements required by a particular document type without modifying the underlying Metadata Schema.

---

## 5.7. Metadata Dictionary

### 5.7.1. Definition

The Metadata Dictionary is the authoritative catalog of every Metadata Element defined by the Documentation Framework.

It provides the canonical definition of each Metadata Element together with its semantic meaning.

---

## 5.8. Metadata Specification

### 5.8.1. Definition

The Metadata Specification formally defines the Metadata architecture, model, elements, constraints and behavior.

It constitutes the normative reference for Metadata within the Documentation Framework.

---

# 6. Supporting Concepts

## 6.1. Mandatory Metadata

Metadata that shall be present for a document to comply with the Documentation Framework.

---

## 6.2. Optional Metadata

Metadata that may be present depending on the document category or architectural requirements.

---

## 6.3. Standard Metadata

Metadata defined as part of the Documentation Framework.

Standard Metadata is common across all compliant implementations.

---

## 6.4. Extended Metadata

Metadata introduced through controlled architectural extension while preserving compatibility with the standard Metadata model.

---

## 6.5. Metadata Consumer

An architectural component that reads or interprets Metadata in order to perform its responsibilities.

Examples include:

- Document Identity
- Registry
- Workflow
- Validation

Metadata Consumers never own Metadata.

---

## 6.6. Metadata Producer

An architectural component responsible for creating, maintaining or updating Metadata.

The Documentation Framework may include multiple Metadata Producers.

Each Producer shall preserve Metadata semantics.

---

# 7. Concept Relationships

The Metadata concepts form a coherent conceptual model.

```text

     ┌───────────────────────────────────────────────────┐
     │                                                   │
     │                     Metadata                      │
     │                        │                          │
     │        ┌───────────────┼───────────────┐          │
     │        │                               │          │
     │        ▼                               ▼          │
     │    Metadata                        Metadata       │
     │     Element                          Model        │
     │        │                               │          │
     │        ▼                               ▼          │
     │    Metadata                        Metadata       │
     │      Value                           Schema       │
     │                                        │          │
     │                                        ▼          │
     │                                    Metadata       │
     │                                     Profile       │
     │                                                   │
     └───────────────────────────────────────────────────┘

             ┌─────────────────────────────────┐
             │                                 │
             │             Metadata            │
             │            Dictionary           │
             │                │                │
             │                ▼                │
             │             Metadata            │
             │           Specification         │
             │                                 │
             └─────────────────────────────────┘

```

Each concept possesses a unique responsibility within the Metadata domain.

---

# 8. Concept Boundaries

The Metadata component defines descriptive concepts only.

It does not define:

- document identity;
- document classification;
- workflow states;
- governance rules;
- relationships between documents;
- validation procedures.

These concepts belong to their respective architectural components.

---

# 9. Architectural Characteristics

The Metadata conceptual model possesses the following characteristics.

## 9.1. Canonical

Every concept has one authoritative definition.

---

## 9.2. Consistent

Concepts preserve the same meaning throughout the Documentation Framework.

---

## 9.3. Independent

Concepts remain independent of implementation technologies.

---

## 9.4. Extensible

New concepts may be introduced through controlled architectural evolution.

---

## 9.5. Stable

Existing concepts shall remain stable whenever possible.

---

## 9.6. Reusable

Concepts may be reused by multiple architectural components.

---

# 10. Concept Lifecycle

Metadata concepts evolve according to the following principles.

- concepts are introduced explicitly;
- concepts are uniquely defined;
- concepts may be extended but not reinterpreted;
- concepts remain backward compatible whenever possible;
- deprecated concepts shall remain documented.

---

# 11. Conformance

A Metadata implementation conforms to this conceptual model when:

- every Metadata concept has a single semantic meaning;
- Metadata Elements preserve their definitions;
- Metadata Values do not redefine Metadata Elements;
- Metadata Profiles remain compatible with the Metadata Schema;
- Metadata extensions preserve the canonical Metadata model.

---

# 12. Related Documents

## 12.1. Architecture

- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components
- DF-ARC-006 — Terminology

## 12.2. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema
- DF-MTD-013 — Metadata Dictionary
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---