# Documentation Framework

# DF-TPL-015 — Template Examples

| Metadata        | Value                        |
| --------------- | ---------------------------- |
| **Document ID** | DF-TPL-015                   |
| **Title**       | Template Examples            |
| **Family**      | Templates                    |
| **Type**        | Component Reference Document |
| **Component**   | Templates                    |
| **Author**      | Arnaldo Figueira             |
| **Status**      | Draft                        |
| **Version**     | 1.0                          |
| **Revision**    | 0                            |
| **Baseline**    | 1.0                          |
| **Language**    | English                      |
| **Date:**       | 2026-09-23                   |

---

# 1. Introduction

## 1.1. Purpose

This document provides representative examples of Templates defined according to the Documentation Framework Templates Component.

The examples demonstrate how the concepts, structures, elements, parameters, constraints, relationships, composition, specialization, versioning, lifecycle, validation, and governance mechanisms defined by the Templates Component may be applied.

The examples are illustrative and are not themselves normative Template definitions unless explicitly adopted and governed as such.

---

## 1.2. Scope

This document provides examples of:

* basic Templates;
* structured Templates;
* reusable Template Elements;
* parameterized Templates;
* composed Templates;
* specialized Templates;
* constrained Templates;
* Template relationships;
* Template Version usage;
* Template Instance creation;
* Template lifecycle;
* Template validation;
* Template governance.

The examples do not define:

* a physical repository structure;
* a specific serialization format;
* an implementation language;
* a database representation;
* a document-management workflow.

---

# 2. Example Conventions

The examples use the following notation:

```text

    [TEMPLATE]
        Template definition

    [SECTION]
        Template Section

    [ELEMENT]
        Template Element

    [PARAMETER]
        Template Parameter

    [CONSTRAINT]
        Template Constraint

    [RELATIONSHIP]
        Template Relationship

```

The notation is illustrative and does not constitute a required serialization format.

---

# 3. Basic Template Example

A simple Template may define the structure of a technical document.

```text

    Template: Technical Document

    Type:
        Technical Documentation

    Structure:
        Section: Introduction
            Element: Purpose
            Element: Scope

        Section: Main Content
            Element: Content

        Section: References
            Element: Related Documents

```

This Template defines reusable documentation structure without defining how the resulting document is stored.

---

# 4. Structured Template Example

A more detailed Template may define a document with several mandatory and optional elements.

```text

    Template: Architecture Document

    Structure:

        Section: Metadata
            Element: Document Identifier
            Element: Title
            Element: Status
            Element: Version
            Element: Revision

        Section: Introduction
            Element: Purpose
            Element: Scope

        Section: Architecture
            Element: Architectural Position
            Element: Components
            Element: Relationships
            Element: Constraints

        Section: Governance
            Element: Responsibilities
            Element: Governance Rules

        Section: References
            Element: Related Documents

```

The Template defines the expected structure while the semantics of Metadata and Document Identity remain the responsibility of their respective components.

---

# 5. Optional Element Example

A Template may contain optional elements.

```text

    Section: References

        Element: Related Documents
            Occurrence: Optional

        Element: External References
            Occurrence: Optional

```

The optionality is a Template structural property.

It does not determine whether a particular document is complete unless the applicable Template Constraints establish such a requirement.

---

# 6. Repeated Element Example

A Template Element may occur multiple times.

```text

    Section: Requirements

        Element: Requirement
            Occurrence: One or More

```

A Template Instance may therefore contain:

```text

    Requirement 1
    Requirement 2
    Requirement 3
...

```

The Template defines the permitted occurrence model; the Template Instance contains the concrete occurrences.

---

# 7. Ordered Element Example

A Template may explicitly define ordering.

```text

    Section: Document Structure

        1. Purpose
        2. Scope
        3. Concepts
        4. Architecture
        5. Constraints
        6. References

```

Ordering is part of the Template Structure.

An implementation MUST preserve the semantic ordering requirements established by the Template Schema and applicable Constraints.

---

# 8. Parameterized Template Example

A Template may use parameters to support controlled variation.

```text

    Template: Component Document

    Parameter:
        ComponentName

    Parameter:
        ComponentPurpose

    Structure:

        Section: Introduction
            Element: Component Name
                Parameter: ComponentName

            Element: Purpose
                Parameter: ComponentPurpose

        Section: Architecture
            Element: Architectural Position

        Section: References
            Element: Related Documents

```

The Template remains the same while parameter values vary between Template Instances.

For example:

```text

    ComponentName     =  Templates
    ComponentPurpose  =  Define reusable documentation structures

```

and:

```text

    ComponentName     =  Metadata
    ComponentPurpose  =  Define document metadata

```

Parameterization provides controlled variation without duplicating the complete Template.

---

# 9. Reusable Element Example

A reusable Template Element may be defined independently and incorporated into multiple Templates.

```text

    Reusable Element:
        Document Status

    Purpose:
        Represents the status information required by applicable documentation.

    Used by:
        Technical Document Template
        Architecture Document Template
        Component Document Template

```

Reuse promotes consistency and reduces duplicated structural definitions.

The reusable Element remains subject to the Constraints and Schema of each Template in which it is used.

---

# 10. Composition Example

A Template may be constructed from existing reusable structures.

```text

    Template: Component Architecture Document

    Composition:

        ├── Common Document Structure
        │
        ├── Architecture Structure
        │
        └── Reference Structure

```

Conceptually:

```text

            Component Architecture Document
            │
            ├── Common Document Structure
            │
            ├── Architecture Structure
            │
            └── Reference Structure

```

Composition combines existing structures.

It does not imply that one Template is a specialization of another.

---

# 11. Specialization Example

A general Template may be specialized for a more specific purpose.

```text

    Base Template:
        Technical Document

    Specialized Template:
        Architecture Document

```

The specialization may refine the base structure:

```text

            Technical Document
            │
            ├── Introduction
            │
            ├── Main Content
            │
            └── References
                    │
                    ▼

          Architecture Document
          │
          ├── Introduction
          │
          ├── Architectural Position
          │
          ├── Components
          │
          ├── Relationships
          │
          ├── Constraints
          │
          └── References

```

The Architecture Document remains semantically related to the Technical Document while providing a more specific structure.

---

# 12. Constraint Example

A Template may require specific structural conditions.

```text

    Template Constraint:

        Every Architecture Document MUST contain:

            Purpose
            Scope
            Architectural Position
            Components
            Relationships

```

Another constraint may restrict occurrence:

```text

    Occurrence Constraint:

        Purpose
            Minimum occurrence: 1
            Maximum occurrence: 1

```

A parameter constraint may define a requirement for a parameter:

```text

    Parameter Constraint:

        ComponentName
            MUST have a non-empty value

```

Constraints define what is permitted.

Validation determines whether the resulting Template definition satisfies those constraints.

---

# 13. Relationship Example

A Template may define relationships between its elements.

```text

    Template Relationship:

        Component
        │
        └── contains  ─────►  Component Responsibility

```

A different relationship may reference another Template:

```text

    Template Relationship:

        Architecture Document Template
        │
        └── references  ─────►  Architecture Concepts Template

```

The relationship type MUST be explicitly identified.

A reference MUST NOT automatically be interpreted as composition.

---

# 14. Cross-Template Dependency Example

A Template may depend on another Template.

```text

    Template A:
        Component Architecture Document

    Dependency:
        Architecture Concepts Template

```

The dependency indicates that Template A relies on concepts or structures provided by Template B.

The dependency does not imply:

* composition;
* specialization;
* inheritance.

These remain distinct relationship semantics.

---

# 15. Template Version Example

A Template may evolve through multiple versions.

```text

    Template:
        Architecture Document

    Version 1.0:
        Introduction
        Architecture
        References

    Version 2.0:
        Introduction
        Architecture
        Governance
        References

```

The versions represent different definitions of the same Template.

A Template Version MUST NOT be interpreted as a Document Revision.

---

# 16. Template Instance Example

A Template Instance represents the application of a Template.

Given:

```text

    Template:
        Component Document

```

with:

```text

    ComponentName     =  Templates
    ComponentPurpose  =  Define reusable documentation structures

```

a corresponding Template Instance may conceptually produce:

```text

    Component Document

        Component Name:
            Templates

        Purpose:
            Define reusable documentation structures

        Architecture:
            ...

        References:
            ...

```

The concrete values belong to the Template Instance.

The reusable structure remains defined by the Template.

---

# 17. Lifecycle Example

A newly created Template may progress through its lifecycle:

```text

                  Draft
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active

```

When replacement becomes necessary:

```text

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

A deprecated Template may be reactivated where governance permits:

```text

                Deprecated
                    │
                    ▼

                  Active

```

Lifecycle transitions MUST comply with the applicable governance requirements.

---

# 18. Validation Example

Consider the following Template:

```text

    Template:
        Architecture Document

    Required Elements:

        Purpose
        Scope
        Architecture
        References

```

Validation may produce:

```text

    Structural Validation:
        Conformant

    Element Validation:
        Conformant

    Schema Validation:
        Conformant

    Constraint Validation:
        Non-Conformant

    Result:
        Non-Conformant

```

The validation finding may identify:

```text

    Missing required element:
        Scope

```

The validation result does not itself approve or reject the Template.

Governance remains responsible for the corresponding governance decision.

---

# 19. Governance Example

A proposed Template change may follow:

```text

             Template Change
                    │
                    ▼

            Change Assessment
                    │
                    ▼

             Template Review
                    │
                    ▼

                Validation
                    │
                    ▼

           Governance Decision
           │
           ├── Accepted
           │
           ├── Rejected
           │
           ├── Deferred
           │
           └── Returned for Revision

```

Validation provides evidence for the governance process.

It does not replace the governance decision.

---

# 20. Compatibility Example

A Template may define a location for document identity information:

```text

    Section: Document Identity

        Element: Document Identifier
        Element: Edition
        Element: Revision

```

The Template establishes where the information is structurally represented.

The semantics of:

* Document Identifier;
* Edition;
* Revision

remain defined by the Document Identity Component.

Similarly, a Template may contain:

```text

    Section: Metadata

        Element: Author
        Element: Status
        Element: Language

```

without redefining Metadata semantics.

---

# 21. Combined Example

The following example combines several Template mechanisms.

```text

    Template:
        Component Architecture Document

    Type:
        Architecture Documentation

    Version:
        2.0

    Structure:

        Section: Metadata
            Element: Document Metadata

        Section: Introduction
            Element: Purpose
            Element: Scope

        Section: Architecture
            Element: Architectural Position
            Element: Components
            Element: Relationships

        Section: Constraints
            Element: Architectural Constraints

        Section: References
            Element: Related Documents
                Occurrence: Zero or More

    Parameters:

        ComponentName
        ComponentPurpose

    Relationships:

        references  ─────►  Architecture Concepts Template
        references  ─────►  Architecture Model Template

    Constraints:

        Purpose MUST occur exactly once
        Scope MUST occur exactly once
        ComponentName MUST be provided
        Related Documents MAY occur multiple times

```

This example demonstrates:

* Template Type;
* Template Structure;
* Template Sections;
* Template Elements;
* Template Parameters;
* Template Relationships;
* Template Constraints;
* Template Version;
* compatibility with other Templates.

---

# 22. Example of Controlled Specialization

A generic component Template may be specialized into several documentation Templates.

```text

            Component Template
            │
            ├── Component Architecture Template
            │
            ├── Component Structure Template
            │
            ├── Component Behavior Template
            │
            └── Component Reference Template

```

Each specialization may retain common structural elements while introducing domain-specific structure.

This approach avoids duplicating common Template definitions.

---

# 23. Example of Template Reuse

A common reusable structure may be used across several Templates:

```text

    Reusable Structure:
        Standard Introduction

    Contains:
        Purpose
        Scope

```

It may be composed into:

```text

    Architecture Document Template
    Component Document Template
    Reference Document Template
    Specification Document Template

```

The shared structure promotes consistency across documentation types.

---

# 24. Example of Template Conformance

A Template may be evaluated against its requirements.

```text

    Template:
        Component Architecture Document

    Schema:
        Conformant

    Elements:
        Conformant

    Parameters:
        Conformant

    Relationships:
        Conformant

    Constraints:
        Conformant

    Cross-Template Compatibility:
        Conformant

    Overall Conformance:
        Conformant

```

The conformance result applies to the evaluated Template definition and its applicable Template Version.

---

# 25. Example of Non-Conformance

A Template may fail conformance when it violates a mandatory requirement.

```text

    Template Constraint:

        Every Architecture Document MUST contain
        an Architectural Position Element.

```

Template definition:

```text

    Section: Architecture

        Element: Components
        Element: Relationships

```

Validation result:

```text

    Result:
        Non-Conformant

    Finding:
        Required Architectural Position Element is missing.

```

The finding identifies the violated requirement without changing the Template definition automatically.

---

# 26. Example of Template Evolution

A Template may evolve incrementally.

### 26.1. Version 1.0

```text

    Introduction
    Architecture
    References

```

### 26.2. Version 1.1

```text

    Introduction
    Architecture
    Constraints
    References

```

### 26.3. Version 2.0

```text

    Metadata
    Introduction
    Architecture
    Constraints
    Governance
    References

```

The exact versioning policy is determined by applicable Template Governance.

The examples illustrate the distinction between structural evolution and the lifecycle state of the Template.

---

# 27. Example of Retired Template Preservation

A Template may become obsolete:

```text

    Template:
        Legacy Architecture Document

    Lifecycle:
        Retired

```

The Template definition may nevertheless be preserved because historical Document Instances were created using it.

Preservation allows historical documentation to remain understandable and traceable.

Retirement therefore does not imply deletion.

---

# 28. Example of a Minimal Template

A minimal valid Template may consist of:

```text

    Template:
        Simple Note

    Type:
        Note

    Structure:
        Section: Content
            Element: Text

    Version:
        1.0

```

Additional concepts such as Parameters, Relationships, Composition, or Specialization are not required when they are not applicable.

A Template SHOULD remain as simple as its intended purpose permits.

---

# 29. Example of a Complex Template

A complex Template may contain:

```text

            Template
            │
            ├── Type
            │
            ├── Structure
            │   │
            │   └── Sections
            │       │
            │       └── Elements
            │
            ├── Parameters
            │
            ├── Constraints
            │
            ├── Relationships
            │
            ├── Composition
            │
            ├── Specialization
            │
            ├── Version
            │
            ├── Lifecycle
            │
            ├── Validation
            │
            └── Governance

```

Complexity is justified only when required by the documentation purpose.

The existence of available Template mechanisms does not require every Template to use them.

---

# 30. Example Design Principles

The examples demonstrate several general principles.

## 30.1. Reuse Before Duplication

Existing structures and Elements SHOULD be reused whenever appropriate.

## 30.2. Explicit Semantics

Relationships, Constraints, Parameters, Composition, and Specialization SHOULD be explicit.

## 30.3. Controlled Variation

Parameters SHOULD be preferred over duplicated Templates when the variation is controlled and semantically equivalent.

## 30.4. Appropriate Specialization

Specialization SHOULD be used when a more specific Template retains a meaningful semantic relationship with a more general Template.

## 30.5. Appropriate Composition

Composition SHOULD be used when independent structures can be combined without implying specialization.

## 30.6. Simplicity

Templates SHOULD contain only the structural mechanisms required by their purpose.

## 30.7. Traceability

Significant Template evolution SHOULD remain traceable through Template Versions and applicable Governance records.

---

# 31. Example Summary

The examples demonstrate the principal capabilities of the Templates Component:

```text

            Template
            │
            ├── Structure
            │   │
            │   └── Sections
            │       │
            │       └── Elements
            │
            ├── Parameters
            │
            ├── Relationships
            │
            ├── Constraints
            │
            ├── Composition
            │
            ├── Specialization
            │
            ├── Version
            │
            ├── Instance
            │
            ├── Lifecycle
            │
            ├── Validation
            │
            ├── Governance
            │
            └── Extensibility

```

These mechanisms allow Templates to provide reusable, explicit, structured, and controlled documentation definitions while remaining independent of document storage, repository organization, and implementation technology.

---

# 32. Related Documents

The following documents define the concepts and requirements demonstrated by these examples:

* **DF-TPL-001 — Templates Architecture**
* **DF-TPL-002 — Template Concepts**
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
* **DF-RDM-040 — Templates Roadmap**

---

# 33. Change History

| Version | Revision | Date       | Change                    |
| ------- | -------: | ---------- | ------------------------- |
| 1.0     |        0 | 2026-09-23 | Initial Template Examples |

---

**End of Document**

---