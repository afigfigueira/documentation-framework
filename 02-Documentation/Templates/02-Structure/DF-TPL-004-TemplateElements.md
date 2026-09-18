# Documentation Framework

# DF-TPL-004 — Template Elements

| Metadata        | Value                           |
| --------------- | ------------------------------- |
| **Document ID** | DF-TPL-004                      |
| **Title**       | Template Elements               |
| **Family**      | Templates                       |
| **Type**        | Component Architecture Document |
| **Component**   | Templates                       |
| **Author**      | Arnaldo Figueira                |
| **Status**      | Draft                           |
| **Version**     | 1.0                             |
| **Revision**    | 0                               |
| **Baseline**    | 1.0                             |
| **Language**    | English                         |

---

# 1. Introduction

## 1.1. Purpose

This document defines the elements that may constitute a Template Structure within the Templates component of the Documentation Framework.

It establishes the conceptual taxonomy, purpose, characteristics, and structural role of Template Elements defined by the Template Model.

The objective is to provide a consistent vocabulary for describing the structural building blocks of reusable documentation Templates.

## 1.2. Scope

This document defines:

* Template Element;
* structural element categories;
* content-oriented elements;
* organizational elements;
* reference elements;
* metadata-related structural elements;
* identity-related structural elements;
* classification-related structural elements;
* parameterized elements;
* reusable structural elements;
* element relationships;
* element composition;
* element ordering;
* element applicability;
* element boundaries.

This document does not define:

* Template Schema syntax;
* detailed validation algorithms;
* governance procedures;
* document metadata definitions;
* document identity rules;
* document classification rules;
* workflow;
* repository organization;
* physical document formats.

---

# 2. Element Model Position

Template Elements occupy the lowest structural level of the primary Template Structure.

```text

            Template
            │
            └── Template Structure
                │
                └── Template Section
                    │
                    └── Template Element

```

A Template Element represents a structural unit used to define the organization or expected content of a Template.

Template Elements are conceptual objects.

They are not equivalent to:

* files;
* directories;
* database records;
* physical document objects;
* source-code constructs.

---

# 3. Template Element Definition

A **Template Element** is a structural unit within a Template Section that defines a specific part of the structure expected by a Template.

A Template Element may define:

* structural position;
* semantic purpose;
* element type;
* occurrence;
* ordering;
* content expectations;
* parameterization;
* relationships;
* applicability;
* constraints.

The detailed representation of these characteristics is established by the Template Schema.

---

# 4. Element Characteristics

A Template Element may be characterized by the following conceptual properties.

| Characteristic     | Purpose                                      |
| ------------------ | -------------------------------------------- |
| **Element Type**   | Identifies the semantic kind of element      |
| **Name**           | Provides a human-readable designation        |
| **Description**    | Explains the element's intended purpose      |
| **Position**       | Identifies the element's structural position |
| **Order**          | Defines relative ordering when significant   |
| **Occurrence**     | Defines permitted or required repetition     |
| **Content**        | Defines the expected structural content      |
| **Parameters**     | Defines controlled variation                 |
| **Relationships**  | Defines associations with other elements     |
| **Constraints**    | Defines applicable structural restrictions   |
| **Applicability**  | Defines where or when the element applies    |

These characteristics describe the model and do not prescribe a physical representation.

---

# 5. Element Categories

Template Elements may be organized into the following conceptual categories:

```text

            Template Element
            │
            ├── Structural Element
            │
            ├── Content Element
            │
            ├── Reference Element
            │
            ├── Metadata Element
            │
            ├── Identity Element
            │
            ├── Classification Element
            │
            ├── Parameterized Element
            │
            └── Reusable Element

```

These categories describe structural roles.

They do not establish additional Documentation Framework components.

---

# 6. Structural Elements

A **Structural Element** defines organization within a Template.

Structural Elements may be used to represent:

* grouping;
* ordering;
* nesting;
* boundaries;
* structural dependencies.

Conceptually:

```text

            Template Section
            │
            └── Structural Element
                │
                ├── Content Element
                │
                └── Content Element

```

Structural Elements define organization rather than document content semantics.

---

# 7. Content Elements

A **Content Element** represents an expected content-bearing part of a Template.

Examples include conceptual requirements for:

* titles;
* descriptions;
* explanatory content;
* lists;
* tables;
* examples;
* other documentation content.

The Template Element defines the structural expectation.

It does not define the actual content of a particular Document Instance.

```text

            Template
            │
            └── Content Element
                │
                └── expected content

```

The actual content is supplied when the Template is applied.

---

# 8. Reference Elements

A **Reference Element** represents a structural location or requirement for a reference within a Template.

References may connect a Template-defined structure with:

* another Template Element;
* another Template Section;
* another Template;
* an external conceptual reference;
* a documentation reference.

Reference Elements define structural expectations.

They do not implement the Documentation Framework's Registry, Knowledge Graph, or navigation mechanisms.

---

# 9. Metadata Elements

A **Metadata Element** represents a structural location or requirement for metadata within a Template.

The Templates component does not define metadata itself.

Instead:

```text

            Metadata Component
                    │
             defines metadata
                    │
                    ▼

             Template Element
                    │
       provides structural location
                    │
                    ▼

            Template Structure

```

A Metadata Element therefore establishes how metadata may participate structurally in a Template without redefining the Metadata component.

Metadata semantics remain the responsibility of the Metadata component.

---

# 10. Identity Elements

An **Identity Element** represents a structural location or requirement for document identity information within a Template.

Templates may require or organize identity information, but they do not assign, generate, or govern document identity.

The responsibility boundary is:

```text

        Document Identity
        │
        └── defines document identity
                        │
                        ▼

       Template
       │
       └── defines structural location
                        │
                        ▼

Identity Element

```

The semantics of document identity remain defined by the Document Identity component.

---

# 11. Classification Elements

A **Classification Element** represents a structural location or requirement for classification-related information.

Templates may provide structural locations for classification information without defining classification itself.

```text

              Classification
                    │
          defines classification
                    │
                    ▼

            Template Element
                    │
         organizes representation
                    │
                    ▼

            Template Structure

```

Classification semantics remain the responsibility of the Classification component.

---

# 12. Parameterized Elements

A **Parameterized Element** is a Template Element whose structure or behavior may vary according to one or more Template Parameters.

```text

             Template Element
                    │
                    ├── Parameter
                    │
                    ▼

             Resolved Element

```

Parameterization enables controlled variation while preserving the identity of the Template itself.

A parameterized element may vary in aspects such as:

* content requirements;
* structural presence;
* naming;
* cardinality;
* optionality;
* references;
* applicable structure.

Parameter definitions belong to the Template.

Parameter values belong to the Template Instance or application context.

---

# 13. Reusable Elements

A **Reusable Element** represents a Template Element intended for reuse within multiple Template Structures.

Reuse may occur through:

* composition;
* specialization;
* structural referencing;
* other mechanisms defined by the Templates component.

Reusable elements promote:

* consistency;
* reduced duplication;
* controlled evolution;
* structural standardization.

Reuse must remain explicit.

Structural similarity alone does not establish reuse.

---

# 14. Element Composition

Template Elements may be composed into larger structures.

```text

            Template Section
            │
            ├── Element A
            │
            ├── Element B
            │   │
            │   ├── Element B.1
            │   │
            │   └── Element B.2
            │
            └── Element C

```

Composition establishes structural relationships between elements.

An element may therefore act as:

* a standalone structural unit;
* a container for subordinate elements;
* a component of a reusable structure.

Composition must preserve the semantic meaning of each participating element.

---

# 15. Element Containment

The primary containment relationship is:

```text

            Template
            │
            └── Template Structure
                │
                └── Template Section
                    │
                    └── Template Element

```

An element belongs to a Template Section.

A Template Element may contain subordinate elements when hierarchical composition is permitted.

```text

            Element A
            │
            ├── Element B
            │
            └── Element C

```

Containment is conceptual and does not imply physical storage containment.

---

# 16. Element Ordering

Elements may have an explicit order within their containing structure.

```text

            Section
            │
            ├── Element 1
            │
            ├── Element 2
            │
            └── Element 3

```

Ordering may be:

* required;
* significant;
* optional;
* unconstrained.

The applicable ordering semantics are determined by the Template definition and later formalized by the Template Schema.

Physical order in a file, repository, or storage system must not be assumed to define Template order.

---

# 17. Element Occurrence

A Template Element may have an occurrence requirement.

Conceptually, occurrence may be represented as:

```text

            Element
            │
            ├── minimum occurrence
            │
            └── maximum occurrence

```

This permits structural requirements such as:

```text

    Required element
        minimum = 1

    Optional element
        minimum = 0

    Repeatable element
        maximum > 1

    Single element
        maximum = 1

```

Exact occurrence semantics belong to the Template Schema and Constraint definitions.

---

# 18. Element Optionality

An element may be:

* required;
* optional;
* conditionally applicable.

```text

    Required
        ─────►  must be present

    Optional
        ─────►  may be present

    Conditional
        ─────►  presence depends on defined applicability

```

Optionality is a structural property.

It must not be confused with workflow state, document approval, or policy enforcement.

---

# 19. Element Applicability

Element applicability defines the conditions under which an element participates in a Template Structure.

Applicability may depend on:

* Template specialization;
* Template composition;
* Template Parameters;
* structural context;
* Template Type;
* applicable Template Version.

Applicability must be explicitly represented when it affects Template conformance.

---

# 20. Element Relationships

Template Elements may participate in explicit relationships.

Examples include:

```text

            Element A
            │
            ├── contains     ─────►  Element B
            │
            ├── references   ─────►  Element C
            │
            ├── depends on   ─────►  Element D
            │
            └── specializes  ─────►  Element E

```

Relationships express structural or semantic associations.

They must not be inferred from physical proximity.

Detailed relationship types are defined by **DF-TPL-009 — Template Relationships**.

---

# 21. Element Constraints

Template Elements may be subject to Template Constraints.

```text

            Template Element
            │
            └── Constraint

```

Constraints may govern:

* occurrence;
* ordering;
* content requirements;
* parameter applicability;
* element relationships;
* composition;
* specialization.

The element model identifies the association between an element and its constraints.

Detailed constraint semantics are deferred to **DF-TPL-010 — Template Constraints**.

---

# 22. Element and Template Schema

Template Elements provide the conceptual structures that are subsequently represented by the Template Schema.

```text

            Template Elements
                    │
                    ▼

            Template Structure
                    │
                    ▼

             Template Schema

```

The Template Schema formalizes the structural rules required to represent and evaluate a Template.

This document therefore defines the elements conceptually without prescribing schema syntax.

Schema representation is defined by **DF-TPL-005 — Template Schema**.

---

# 23. Element and Template Instance

When a Template is applied, Template Elements participate in the resulting Template Instance.

```text

             Template Element
                    │
         applied through Template
                    │
                    ▼

        Template Instance Element

```

The application may resolve:

* parameters;
* optional elements;
* conditional elements;
* composition;
* specialization;
* applicable constraints.

The resulting structure belongs to the Template Instance.

The Template definition itself remains unchanged by a particular application.

---

# 24. Element Lifecycle Considerations

Template Elements evolve as part of the Template definition.

An element may be:

* introduced;
* modified;
* deprecated;
* replaced;
* removed.

Element evolution is governed by the lifecycle of the containing Template and its Template Versions.

```text

            Template Version 1
                    │
                    ├── Element A
                    │
                    ▼

            Template Version 2
            │
            ├── Element A
            │
            └── Element B

```

Detailed lifecycle rules are defined by **DF-TPL-006 — Template Lifecycle**.

---

# 25. Element Responsibility Boundaries

Template Elements must remain within the responsibility of Templates.

| Concern                            | Template Element Responsibility |
| ---------------------------------- | ------------------------------- |
| **Structural organization**        | Defines                         |
| **Structural content expectation** | Defines                         |
| **Reusable structure**             | Supports                        |
| **Parameterization**               | Supports                        |
| **Element relationships**          | Represents                      |
| **Structural constraints**         | Associates                      |
| **Metadata semantics**             | Does not define                 |
| **Document identity semantics**    | Does not define                 |
| **Classification semantics**       | Does not define                 |
| **Workflow**                       | Does not define                 |
| **Repository organization**        | Does not define                 |
| **Document storage**               | Does not define                 |
| **Document lifecycle**             | Does not define                 |

This separation preserves the independence of Documentation Framework components.

---

# 26. Element Model Invariants

The following invariants apply to Template Elements.

## 26.1. Structural Membership

A Template Element belongs to a Template Structure through a Template Section or permitted structural composition.

## 26.2. Explicit Semantics

Every Template Element must have an identifiable structural purpose.

## 26.3. Explicit Relationships

Relationships between elements must be explicit when they affect structural or semantic interpretation.

## 26.4. Definition/Application Separation

A Template Element definition must remain distinct from its representation within a Template Instance.

## 26.5. Component Responsibility

Template Elements must not redefine concepts owned by other Documentation Framework components.

## 26.6. Physical Independence

Template Elements must remain independent of physical storage, repository, filename, directory, and serialization technology.

## 26.7. Controlled Variation

Variation between applications must be represented through established mechanisms such as Template Parameters, specialization, composition, or applicable structural rules.

## 26.8. Conformance Support

The element model must provide sufficient information for applicable structural conformance to be determined.

---

# 27. Element Model Summary

The Template Element model can be summarized as:

```text

            Template
            │
            └── Template Structure
                │
                └── Template Section
                    │
                    └── Template Element
                        │
                        ├── Structural
                        │
                        ├── Content
                        │
                        ├── Reference
                        │
                        ├── Metadata-related
                        │
                        ├── Identity-related
                        │
                        ├── Classification-related
                        │
                        ├── Parameterized
                        │
                        └── Reusable

```

The element model provides the structural vocabulary required to describe reusable Templates while preserving the responsibility boundaries established by the Documentation Framework architecture.

---

# 28. Related Documents

* DF-RDM-040 — Templates Roadmap
* DF-ARC-007 — Component Documentation Structure
* DF-TPL-001 — Templates Architecture
* DF-TPL-002 — Template Concepts
* DF-TPL-003 — Template Model
* DF-TPL-005 — Template Schema
* DF-TPL-006 — Template Lifecycle
* DF-TPL-007 — Template Validation
* DF-TPL-008 — Template Governance
* DF-TPL-009 — Template Relationships
* DF-TPL-010 — Template Constraints
* DF-TPL-011 — Template Extensibility
* DF-TPL-012 — Template Best Practices
* DF-TPL-013 — Template Dictionary
* DF-TPL-014 — Template Specification
* DF-TPL-015 — Template Examples

---

# 29. Change History

| Version | Revision | Date       | Author           | Description                          |
| ------- | -------: | ---------- | ---------------- | ------------------------------------ |
| 1.0     |        0 | 2026-09-18 | Arnaldo Figueira | Initial Template Elements definition |
