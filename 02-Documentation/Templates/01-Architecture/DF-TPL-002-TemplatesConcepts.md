# Documentation Framework

# DF-TPL-002 — Template Concepts

| Metadata        | Value                           |
| --------------- | ------------------------------- |
| **Document ID** | DF-TPL-002                      |
| **Title**       | Template Concepts               |
| **Family**      | Templates                       |
| **Type**        | Component Architecture Document |
| **Component**   | Templates                       |
| **Author**      | Arnaldo Figueira                |
| **Status**      | Draft                           |
| **Version**     | 1.0                             |
| **Revision**    | 0                               |
| **Baseline**    | 1.0                             |
| **Language**    | English                         |
| **Date**        | 2026-09-13                      |

---

# 1. Introduction

## 1.1. Purpose

This document defines the fundamental concepts of the **Templates** component of the Documentation Framework.

It establishes the conceptual vocabulary required to describe, understand, structure, reuse, validate, govern, and evolve documentation templates.

The concepts defined here provide the semantic foundation for the Template Model, Template Elements, Template Schema, Template Lifecycle, Template Validation, Template Governance, and subsequent Templates component specifications.

## 1.2. Scope

This document defines concepts directly related to documentation templates, including:

* Template
* Template Type
* Template Structure
* Template Element
* Template Section
* Template Schema
* Template Instance
* Template Parameter
* Template Constraint
* Template Version
* Template Relationship
* Template Specialization
* Template Composition
* Template Conformance

These concepts describe the conceptual nature of templates without defining implementation technologies, repository structures, storage mechanisms, or document-management workflows.

## 1.3. Conceptual Position

Templates belong to the **Documentation Layer** of the Documentation Framework.

The Templates component operates together with other Documentation Layer components, particularly:

* Metadata;
* Document Identity;
* Classification.

The Templates component defines reusable structures for documentation. It does not redefine the meaning or responsibilities of these other components.

---

# 2. Template Concept

## 2.1. Definition

A **Template** is a reusable structural definition that specifies how a category of documentation is organized and represented.

A Template defines a reusable documentation structure without representing a specific document instance.

A Template may define:

* structural organization;
* required and optional elements;
* sections;
* ordering;
* semantic roles;
* metadata requirements;
* classification compatibility;
* structural constraints;
* reusable composition rules.

## 2.2. Template Characteristics

A Template is:

* reusable;
* structurally defined;
* semantically explicit;
* technology independent;
* independent of physical storage;
* independent of repository organization;
* capable of being instantiated into documentation;
* subject to validation and governance.

A Template is not itself a document instance.

---

# 3. Template Type

## 3.1. Definition

A **Template Type** identifies the conceptual category of a Template according to the kind of documentation structure it defines.

Template Types provide a means of distinguishing templates according to their intended structural or documentary purpose.

A Template Type may be associated with:

* a particular document category;
* a documentation purpose;
* a structural pattern;
* a specialization of another Template Type.

## 3.2. Responsibility

Template Type classification belongs to the conceptual organization of Templates.

It must not be confused with the **Classification** component, which is responsible for document classification.

Templates may define structures compatible with classifications, but Templates do not assume responsibility for classifying document instances.

---

# 4. Template Structure

## 4.1. Definition

A **Template Structure** is the ordered organization of structural elements that defines the composition of a Template.

It establishes how the constituent parts of a template are arranged.

A Template Structure may define:

* hierarchy;
* ordering;
* containment;
* required structures;
* optional structures;
* repeated structures;
* structural relationships.

## 4.2. Structural Independence

Template Structure describes conceptual organization rather than physical organization.

It does not define:

* directories;
* filesystems;
* repositories;
* storage locations;
* database schemas;
* source-control structures.

---

# 5. Template Element

## 5.1. Definition

A **Template Element** is a distinct structural or semantic unit defined within a Template.

Template Elements provide the basic building blocks from which Template Structures are composed.

Examples may include:

* title;
* document identification area;
* metadata area;
* section;
* subsection;
* table;
* reference area;
* example area.

The definitive set of Template Elements is established by the Template Elements document and subsequent Template Specification.

## 5.2. Element Semantics

Each Template Element may have:

* an identity;
* a semantic purpose;
* a structural role;
* cardinality;
* ordering rules;
* required or optional status;
* constraints;
* relationships with other elements.

---

# 6. Template Section

## 6.1. Definition

A **Template Section** is a structural subdivision of a Template used to organize related documentation content.

Sections provide hierarchical organization within a Template.

A section may contain:

* content structures;
* subordinate sections;
* Template Elements;
* repeated structures;
* references to other template structures.

## 6.2. Section Hierarchy

Sections may form hierarchical structures.

For example:

```text

            Template
            │
            └── Section
                │
                ├── Section
                │   │
                │   ├── Element
                │   │
                │   └── Element
                │
                ├── Section
                │
                └── Element

```

The hierarchy is part of the Template Structure and does not determine physical document storage.

---

# 7. Template Schema

## 7.1. Definition

A **Template Schema** is the formal structural definition that specifies the valid composition of a Template.

The schema defines the structural rules necessary to determine whether a Template conforms to its intended structure.

A Template Schema may define:

* allowed elements;
* required elements;
* optional elements;
* ordering;
* cardinality;
* nesting;
* structural constraints;
* relationships between elements.

The complete schema model is defined by **DF-TPL-005 — Template Schema**.

---

# 8. Template Instance

## 8.1. Definition

A **Template Instance** is a concrete realization of a Template used to structure a specific documentation instance.

The distinction is fundamental:

```text

                 Template
                    │
              instantiation
                    │
                    ▼

            Template Instance
                    │
                applied to
                    │
                    ▼

                 Document

```

A Template defines reusable structure.

A Template Instance represents the application of that structure to a specific documentary context.

## 8.2. Instance Independence

A Template Instance does not become the Template itself.

Changes to a Template must therefore be governed so that the relationship between the template definition and existing instances remains explicit and traceable.

---

# 9. Template Parameter

## 9.1. Definition

A **Template Parameter** is a defined input used to adapt a Template without modifying its underlying structural definition.

Parameters allow a reusable Template to support controlled variation.

Examples may include:

* terminology;
* optional sections;
* structural choices;
* domain-specific values;
* presentation-independent configuration.

Template parameters must remain semantically explicit and subject to the constraints defined by the Template.

---

# 10. Template Constraint

## 10.1. Definition

A **Template Constraint** is a rule that restricts the valid structure, composition, or use of a Template.

Constraints may apply to:

* elements;
* sections;
* ordering;
* cardinality;
* nesting;
* parameters;
* composition;
* specialization;
* relationships.

Constraints establish boundaries within which a Template remains conformant.

The detailed constraint model is defined by **DF-TPL-010 — Template Constraints**.

---

# 11. Template Version

## 11.1. Definition

A **Template Version** identifies a defined state of a Template across its controlled evolution.

Template versions provide traceability for structural changes without redefining the identity of the Template itself.

Versioning of Templates must remain distinct from:

* Document Identity;
* document revision;
* operational document versioning;
* baselines.

The Templates component defines the conceptual requirements for Template evolution; it does not redefine the Document Identity component or the Baselines component.

---

# 12. Template Relationship

## 12.1. Definition

A **Template Relationship** is an explicitly defined semantic association between Templates or between a Template and another relevant Template concept.

Examples include:

* composition;
* specialization;
* inheritance;
* dependency;
* compatibility;
* reference.

Relationships must have explicit semantics and must not be inferred solely from physical organization.

The definitive relationship model is established by **DF-TPL-009 — Template Relationships**.

---

# 13. Template Specialization

## 13.1. Definition

**Template Specialization** is the controlled derivation of a more specific Template from an existing Template.

A specialized Template preserves the applicable semantics of its source Template while introducing controlled specialization.

Conceptually:

```text

              Base Template
                    │
              specialization
                    │
                    ▼

           Specialized Template

```

Specialization must not create an unrelated duplicate Template.

It is an explicit mechanism for reuse and controlled refinement.

---

# 14. Template Composition

## 14.1. Definition

**Template Composition** is the construction of a Template by combining reusable Template structures or elements.

Composition supports modular Template design and reuse.

Conceptually:

```text

            Template A ─┐
                        │
                        ├──►  Composite Template
                        │
            Template B ─┘

```

Composition must preserve the semantic identity and constraints of the participating structures.

---

# 15. Template Conformance

## 15.1. Definition

**Template Conformance** is the state in which a Template or Template Instance satisfies the applicable structural, semantic, and governance requirements defined for it.

Conformance may include:

* structural conformance;
* element conformance;
* schema conformance;
* metadata compatibility;
* classification compatibility;
* semantic conformance;
* relationship conformance;
* architectural conformance.

Detailed validation rules are defined by **DF-TPL-007 — Template Validation**.

---

# 16. Relationship Between Core Concepts

The principal conceptual relationships can be summarized as follows:

```text
    
            Template
            │
            ├── has Template Type
            │
            ├── has Template Structure
            │   │
            │   ├── contains Template Sections
            │   │
            │   └── contains Template Elements
            │
            ├── conforms to Template Schema
            │
            ├── may define Template Parameters
            │
            ├── is governed by Template Constraints
            │
            ├── evolves through Template Versions
            │
            ├── may participate in Template Relationships
            │
            ├── may be specialized
            │
            ├── may be composed
            │
            └── may produce Template Instances

```

A Template Instance is a concrete application of a Template:

```text

                 Template
                    │
             instantiated as
                    │
                    ▼

            Template Instance
                    │
                structures
                    │
                    ▼

                 Document

```

---

# 17. Relationship with Other Components

## 17.1. Metadata

Templates define how metadata structures may be represented within documentation.

Templates do not define the meaning or governance of Metadata itself.

The Metadata component remains authoritative for metadata concepts and responsibilities.

## 17.2. Document Identity

Templates may provide a structural location for document identity information.

Templates do not assign, generate, preserve, or govern document identities.

Document Identity remains authoritative for documentary identity.

## 17.3. Classification

Templates may define structures compatible with particular classifications.

Templates do not classify documents.

Classification remains responsible for classification concepts and rules.

## 17.4. Workflow

Templates may provide structures required by workflow-managed documentation.

Templates do not define workflow states, transitions, approvals, or operational processes.

## 17.5. Validation

Templates define structural requirements that can be evaluated by validation mechanisms.

The Templates component defines the applicable conceptual constraints; the Validation architecture is responsible for validation mechanisms.

## 17.6. Automation

Templates provide reusable structures that may be consumed by automation.

Templates do not define automation mechanisms.

---

# 18. Conceptual Boundaries

The following distinctions are fundamental.

| Concept                     | Responsibility                                             |
| --------------------------- | ---------------------------------------------------------- |
| **Template**                | Defines reusable documentation structure                   |
| **Template Type**           | Defines the conceptual category of a Template              |
| **Template Structure**      | Defines structural organization                            |
| **Template Element**        | Defines a structural or semantic unit                      |
| **Template Section**        | Organizes related structures hierarchically                |
| **Template Schema**         | Defines valid structural composition                       |
| **Template Instance**       | Represents a concrete application of a Template            |
| **Template Parameter**      | Enables controlled Template variation                      |
| **Template Constraint**     | Restricts valid Template structure or use                  |
| **Template Version**        | Identifies a controlled Template state                     |
| **Template Relationship**   | Defines explicit associations between Template concepts    |
| **Template Specialization** | Derives a more specific Template from an existing Template |
| **Template Composition**    | Combines reusable Template structures                      |
| **Template Conformance**    | Establishes compliance with applicable requirements        |

These concepts must not absorb responsibilities belonging to other Documentation Framework components.

---

# 19. Conceptual Principles

The Templates component shall apply the following principles to its conceptual model.

## 19.1. Reusability

Templates shall be defined for reuse rather than for a single document instance.

## 19.2. Explicit Semantics

Every Template concept shall have an explicit and stable meaning.

## 19.3. Structural Separation

Template structure shall remain distinct from document content and physical storage.

## 19.4. Responsibility Separation

Templates shall not assume responsibilities belonging to Metadata, Document Identity, Classification, Workflow, Policies, Registry, Baselines, or other components.

## 19.5. Technology Independence

Template concepts shall remain independent of specific markup languages, software platforms, repositories, or implementation technologies.

## 19.6. Controlled Variation

Variation shall be expressed through explicit mechanisms such as parameters, specialization, and composition rather than uncontrolled duplication.

## 19.7. Traceability

Template evolution and relationships shall remain identifiable and traceable.

## 19.8. Architectural Consistency

Template concepts shall remain consistent with the Layered Architecture and established Documentation Framework terminology.

---

# 20. Conceptual Invariants

The following invariants apply to the Templates conceptual model:

1. A Template is not a Document Instance.
2. A Template Instance is not the Template definition.
3. Template Structure is independent of physical storage.
4. Template Elements are defined within Template Structures.
5. Template Schemas constrain valid Template Structures.
6. Template Constraints restrict valid Template composition or use.
7. Template specialization must preserve applicable inherited semantics.
8. Template composition must preserve explicit component semantics.
9. Template concepts must not redefine concepts owned by other components.
10. Template evolution must remain controlled and traceable.

---

# 21. Conceptual Model Summary

The Templates component establishes a layered conceptual model:

```text

                             Template
                                │
               ┌────────────────┼────────────────┐
               │                │                │
            Template         Template         Template
              Type          Structure          Schema
                                │
                   ┌────────────┴────────────┐
                   │                         │
           Template Sections         Template Elements
                   │
                   ▼

          Template Parameters
                   │
                   ▼

          Template Constraints
                   │
                   ▼

           Template Instance
                   │
                   ▼

                Document

```

Templates may additionally participate in controlled:

```text

    Specialization
    Composition
    Relationships
    Versioning
    Conformance

```

This model provides the conceptual foundation for the subsequent structural and behavioral documentation of the Templates component.

---

# 22. Related Documents

* **DF-RDM-040 — Templates Roadmap**
* **DF-TPL-001 — Templates Architecture**
* **DF-TPL-003 — Template Model**
* **DF-TPL-004 — Template Elements**
* **DF-TPL-005 — Template Schema**
* **DF-TPL-006 — Template Lifecycle**
* **DF-TPL-007 — Template Validation**
* **DF-TPL-008 — Template Governance**
* **DF-TPL-009 — Template Relationships**
* **DF-TPL-010 — Template Constraints**
* **DF-TPL-011 — Template Extensibility**
* **DF-TPL-012 — Template Best Practices**
* **DF-TPL-013 — Template Dictionary**
* **DF-TPL-014 — Template Specification**
* **DF-TPL-015 — Template Examples**

---

# 23. Change History

| # | Date       | Author           | Type            | Document   | Description                                            |
| - | ---------- | ---------------- | --------------- | ---------- | ------------------------------------------------------ |
| 1 | 13/09/2026 | Arnaldo Figueira | Add New Content | DF-TPL-002 | Initial definition of Templates conceptual vocabulary. |

---

**End of Document**
