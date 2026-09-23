# Documentation Framework

# DF-TPL-014 — Template Specification

| Metadata        | Value                        |
| --------------- | ---------------------------- |
| **Document ID** | DF-TPL-014                   |
| **Title**       | Template Specification       |
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

This document defines the normative specification of the **Templates Component** of the Documentation Framework.

It consolidates the architectural, conceptual, structural, behavioral, and extensibility requirements established by the Templates documentation and provides a canonical reference for Template conformance.

The specification defines what a Template is, how Templates are structurally represented, how their elements and relationships are defined, how constraints are expressed, and how Templates are versioned, instantiated, validated, governed, and extended.

This document does not replace the detailed Templates documents. It provides their normative synthesis and establishes the requirements that implementations and dependent Documentation Framework components must respect.

---

## 1.2. Scope

This specification covers:

* Template definition;
* Template Types;
* Template Structures;
* Template Sections;
* Template Elements;
* Template Schemas;
* Template Parameters;
* Template Relationships;
* Template Constraints;
* Template Composition;
* Template Specialization;
* Template Versions;
* Template Instances;
* Template Lifecycle;
* Template Validation;
* Template Governance;
* Template Extensibility;
* cross-component compatibility;
* Template conformance.

This specification does not define:

* Metadata semantics;
* Document Identity semantics;
* Classification semantics;
* document workflow;
* policy management;
* baseline management;
* document registry;
* knowledge graph management;
* physical repository organization;
* document storage;
* serialization formats;
* implementation languages;
* specific software technologies.

---

# 2. Normative Language

The following terms are used with their normative meaning:

* **MUST** — a mandatory requirement.
* **MUST NOT** — a mandatory prohibition.
* **SHOULD** — a recommended requirement that may be omitted only for a justified reason.
* **SHOULD NOT** — a recommendation against a practice that may be used only for a justified reason.
* **MAY** — an optional capability.

Requirements in this document apply to conformant Template definitions and Template implementations within the scope of the Documentation Framework.

---

# 3. Template Definition

A **Template** is a reusable definition of a documentation structure intended to standardize the creation and representation of Document Instances.

A Template:

* MUST define or reference a Template Type;
* MUST define a Template Structure;
* MUST define its applicable Template Elements;
* MUST conform to its Template Schema;
* MUST respect its applicable Template Constraints;
* MUST maintain explicit semantic meaning;
* MUST remain independent of physical storage and repository organization.

A Template MUST NOT be considered a Document Instance.

A Template defines the structure and requirements applicable to documents; a Document Instance represents a concrete document produced using that structure.

---

# 4. Template Structural Model

The canonical Template structural model is:

```text

            Template
            │
            ├── Template Type
            │
            ├── Template Structure
            │   │
            │   └── Template Section
            │       │
            │       └── Template Element
            │
            ├── Template Schema
            │
            ├── Template Parameter
            │
            ├── Template Constraint
            │
            ├── Template Relationship
            │
            └── Template Version

```

A conformant Template MUST preserve the distinctions represented by this model.

The Template Model defines the conceptual relationships between these entities.

The Template Schema defines their structural representation.

The Template Constraints define what is permitted.

Template Validation determines whether a Template conforms to its applicable requirements.

---

# 5. Template Type

A **Template Type** identifies the conceptual category of a Template.

Template Types provide semantic classification of Templates without replacing the Classification Component.

A Template MUST be associated with a Template Type where such association is required by the applicable Template Schema.

Template Types MUST NOT be used to redefine document Classification.

---

# 6. Template Structure

A **Template Structure** defines the conceptual organization of a Template.

A Template Structure may contain:

* Template Sections;
* Template Elements;
* ordering information;
* occurrence information;
* applicability information;
* structural relationships.

A Template Structure MUST describe documentation structure rather than physical storage structure.

A Template Structure MUST NOT define:

* repository locations;
* directories;
* database storage;
* file-system organization;
* serialization mechanisms.

---

# 7. Template Sections

A **Template Section** is a structural subdivision of a Template Structure.

Template Sections provide logical organization for Template Elements.

A Template Section MAY contain:

* Template Elements;
* nested structural organization;
* ordering information;
* occurrence requirements;
* applicability constraints.

Section organization MUST remain semantically meaningful and SHOULD avoid unnecessary structural complexity.

---

# 8. Template Elements

A **Template Element** is an identifiable structural or content-bearing component of a Template.

The canonical Template Element categories are:

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

A Template Element MUST have a defined purpose within its Template Structure.

Template Elements MAY be:

* mandatory or optional;
* singular or repeated;
* ordered;
* parameterized;
* reusable;
* constrained;
* related to other elements.

Metadata Elements, Identity Elements, and Classification Elements provide structural locations or requirements for information belonging to their respective components.

They MUST NOT redefine the semantics of:

* Metadata;
* Document Identity;
* Classification.

---

# 9. Template Schema

A **Template Schema** defines the formal structural representation of a Template.

The Template Schema MUST represent, as applicable:

* Template Type;
* Template Structure;
* Template Sections;
* Template Elements;
* ordering;
* occurrence;
* parameters;
* constraints;
* relationships;
* composition;
* specialization;
* version information;
* instance applicability.

The distinction between Model and Schema MUST be preserved:

```text

            Template Model
            │
            └── defines conceptual relationships

            Template Schema
            │
            └── defines structural representation

            Template Validation
            │
            └── evaluates conformance

```

A Template Schema MUST remain independent of a specific serialization technology unless an implementation specification explicitly defines such a representation.

---

# 10. Template Parameters

A **Template Parameter** defines a controlled point of variation within a Template.

Parameters MAY control:

* content;
* structural alternatives;
* applicability;
* reusable values;
* configurable Template behavior.

Parameter definitions MUST be distinguishable from parameter values.

A Template Parameter MUST have a defined semantic purpose and MUST comply with applicable Parameter Constraints.

Parameterization MUST NOT introduce uncontrolled variation that compromises Template consistency.

---

# 11. Template Relationships

A **Template Relationship** defines an explicit relationship between Template entities.

The canonical relationship categories are:

* Containment;
* Reference;
* Dependency;
* Composition;
* Specialization;
* Association.

These relationship types MUST remain semantically distinct.

In particular:

* Reference MUST NOT be interpreted as Composition;
* Dependency MUST NOT be interpreted as Specialization;
* Containment MUST NOT be treated as equivalent to every other relationship type.

Relationships MAY be:

* directional;
* cardinality-constrained;
* version-contextual;
* subject to additional constraints.

Relationship definitions MUST remain explicit and traceable.

---

# 12. Template Constraints

A **Template Constraint** defines a restriction on what is permitted within a Template.

Canonical constraint categories include:

* Structural Constraint;
* Element Constraint;
* Occurrence Constraint;
* Cardinality Constraint;
* Parameter Constraint;
* Relationship Constraint;
* Composition Constraint;
* Specialization Constraint;
* Applicability Constraint.

Constraints MAY apply to:

* the complete Template;
* a Template Structure;
* a Template Section;
* a Template Element;
* a Template Parameter;
* a Template Relationship;
* a composition;
* a specialization.

The distinction between Constraints and Validation MUST be preserved:

```text

            Template Constraints
            │
            └── define what is permitted

            Template Validation
            │
            └── determines whether requirements are satisfied

```

A Constraint MUST NOT be interpreted as a validation result.

---

# 13. Template Composition

**Template Composition** defines the construction of a Template through the combination of existing Template structures or reusable Template Elements.

Composition SHOULD be used to promote:

* reuse;
* consistency;
* modularity;
* controlled structural construction.

Composition MUST preserve the semantic identity of the participating Templates and Elements.

Composition MUST NOT be used merely to create implicit dependencies.

Composition Constraints MAY restrict which Templates or Elements can participate in a composition.

---

# 14. Template Specialization

**Template Specialization** defines a more specific Template derived from an existing Template definition.

A specialization MAY:

* refine structure;
* restrict applicability;
* specialize Elements;
* introduce additional constraints;
* provide additional parameters;
* adapt an existing Template to a more specific documentation context.

A specialization MUST preserve the semantic relationship with its source Template.

Specialization MUST NOT be confused with Composition.

A specialized Template MUST remain independently identifiable as a Template definition.

---

# 15. Template Version

A **Template Version** identifies a particular version of a Template definition.

Template Version provides the temporal and structural context required to distinguish successive Template definitions.

Template Version MUST remain distinct from:

* Document Identity;
* Document Edition;
* Document Revision;
* Document Baseline;
* Document Instance.

Changes to a Template that produce a materially different definition SHOULD result in a new Template Version according to applicable governance rules.

A Template Version MUST be usable as the context for validation and conformance evidence.

---

# 16. Template Instance

A **Template Instance** is a concrete application of a Template.

A Template Instance represents the use of a Template definition to establish the structure of a concrete documentation artifact.

The distinction MUST be preserved:

```text

            Template
            │
            └── defines reusable structure

            Template Version
            │
            └── identifies a particular Template definition version

            Template Instance
            │
            └── represents a concrete application of the Template

```

A Template Instance MUST NOT redefine the Template itself.

Template Instance management MUST NOT be confused with Document Instance lifecycle management.

---

# 17. Template Lifecycle

A Template MUST follow the applicable Template Lifecycle.

The canonical lifecycle states are:

```text

                  Draft
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

Additional permitted transitions include:

```text

    Defined     ─────►  Draft
    Deprecated  ─────►  Active
    Active      ─────►  Retired

```

Lifecycle state and Template Version MUST remain distinct.

Lifecycle state identifies the current lifecycle condition of a Template.

Template Version identifies a particular version of its definition.

Retirement MUST NOT imply automatic deletion or loss of historical information.

Historical Template definitions SHOULD be preserved when required for traceability, conformance, or knowledge preservation.

---

# 18. Template Validation

**Template Validation** determines whether a Template satisfies applicable conformance requirements.

Validation MAY operate at the following levels:

1. Structural Validation;
2. Element Validation;
3. Schema Validation;
4. Compatibility Validation;
5. Semantic Validation;
6. Cross-Template Validation.

Validation MAY evaluate:

* structure;
* elements;
* schema conformance;
* parameters;
* constraints;
* relationships;
* Metadata compatibility;
* Document Identity compatibility;
* Classification compatibility;
* semantic consistency;
* cross-template consistency.

Validation results are:

* **Conformant**;
* **Non-Conformant**;
* **Indeterminate**.

Validation evidence MUST be traceable to the applicable Template Version.

Validation MUST NOT:

* approve a Template;
* define lifecycle state;
* establish governance authority;
* redefine constraints;
* redefine relationships.

---

# 19. Template Governance

**Template Governance** controls the authoritative evolution of Templates.

Governance includes, as applicable:

* Template Authority;
* Template Ownership;
* Template Change;
* Change Assessment;
* Template Review;
* Template Approval;
* version governance;
* backward compatibility;
* deprecation;
* retirement;
* preservation;
* governance records;
* traceability.

Governance decision outcomes include:

* Proposed;
* Accepted;
* Rejected;
* Deferred;
* Returned for Revision.

Governance MUST remain distinct from Validation.

Validation provides evidence about conformance.

Governance determines whether a Template change is authorized and accepted.

---

# 20. Template Extensibility

A Template MAY be extended through controlled mechanisms defined by the Templates Component.

Canonical extensibility mechanisms are:

* Specialization;
* Composition;
* Parameterization;
* Element Reuse;
* Structural Extension.

Extensions MUST:

* preserve Template semantics;
* remain traceable;
* respect applicable Constraints;
* remain subject to Validation;
* comply with Governance requirements;
* preserve architectural boundaries.

Extensions MUST NOT introduce dependencies that violate the Documentation Framework architecture.

Future extensibility mechanisms MAY include:

* inheritance;
* multi-level specialization;
* parameterized composition;
* conditional structures;
* reusable structural patterns;
* semantic Templates;
* Template profiles;
* extension modules;
* machine-readable Template definitions;
* automated Template generation;
* AI-assisted specialization;
* semantic impact analysis.

Such mechanisms MUST preserve the established Template concepts and responsibilities.

---

# 21. Cross-Component Compatibility

Templates interact with other Documentation Layer components while remaining responsible only for Template concerns.

## 21.1. Metadata

Templates MAY define locations and requirements for Metadata through Metadata Elements.

Templates MUST NOT define Metadata semantics.

Metadata compatibility MAY be evaluated during Template Validation.

---

## 21.2. Document Identity

Templates MAY define structural locations and requirements for Document Identity information through Identity Elements.

Templates MUST NOT define Document Identity semantics.

Document Identity compatibility MAY be evaluated during Template Validation.

---

## 21.3. Classification

Templates MAY define structural locations and requirements for Classification information through Classification Elements.

Templates MUST NOT define Classification semantics.

Classification compatibility MAY be evaluated during Template Validation.

---

## 21.4. Workflow

Workflow MAY use Template lifecycle and validation information.

Templates MUST NOT define document workflow.

---

## 21.5. Registry

The Registry MAY reference Templates and Template Versions.

Templates MUST NOT define registry management.

---

## 21.6. Automation

Automation MAY use Template definitions for:

* validation;
* generation;
* metadata placement;
* structural generation;
* consistency verification.

Automation MUST consume Template semantics rather than redefine them.

---

# 22. Conformance Requirements

A Template is conformant when it satisfies all applicable requirements of the Templates Component.

A conformant Template MUST:

1. have a valid Template definition;
2. have a valid Template Type where required;
3. define a valid Template Structure;
4. use valid Template Elements;
5. conform to its Template Schema;
6. satisfy applicable Template Constraints;
7. maintain valid Template Relationships;
8. satisfy applicable Parameter requirements;
9. maintain valid Composition and Specialization semantics;
10. have a valid Template Version;
11. satisfy applicable compatibility requirements;
12. satisfy applicable validation requirements;
13. comply with applicable Governance requirements;
14. respect Templates component boundaries;
15. remain independent of physical storage and repository organization.

Non-conformance MUST be reported through Template Validation.

---

# 23. Canonical Abstract Template Definition

The canonical abstract representation of a Template is:

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
            ├── Schema
            │
            ├── Parameters
            │
            ├── Constraints
            │
            ├── Relationships
            │
            └── Version

```

Behavioral and governance aspects associated with the Template are:

```text

            Template
            │
            ├── Lifecycle
            │
            ├── Validation
            │
            ├── Governance
            │
            └── Extensibility

```

This abstract representation is normative at the conceptual level.

It does not prescribe a physical or technological representation.

---

# 24. Normative Invariants

The following invariants MUST be preserved.

### 24.1. Template Identity

A Template MUST remain distinguishable from its Template Instance and Template Version.

### 24.2. Structural Separation

Template Structure MUST remain distinct from physical repository structure.

### 24.3. Model and Schema Separation

Template Model MUST remain distinct from Template Schema.

### 24.4. Constraint and Validation Separation

Template Constraints MUST remain distinct from Template Validation.

### 24.5. Lifecycle and Governance Separation

Template Lifecycle MUST remain distinct from Template Governance.

### 24.6. Composition and Specialization Separation

Template Composition MUST remain distinct from Template Specialization.

### 24.7. Cross-Component Responsibility

Metadata, Document Identity, and Classification semantics MUST remain outside the Templates Component.

### 24.8. Technology Independence

The conceptual Template definition MUST NOT depend on a specific implementation technology, programming language, storage mechanism, or serialization format.

### 24.9. Traceability

Template Versions, validation results, governance decisions, and significant Template changes MUST remain traceable where applicable.

### 24.10. Controlled Evolution

Template evolution MUST occur through controlled and explicitly defined mechanisms.

---

# 25. Implementation Independence

This specification defines conceptual and normative requirements rather than an implementation technology.

A conformant implementation MAY use:

* files;
* databases;
* APIs;
* programming languages;
* structured data formats;
* document-generation systems;
* automated validation systems.

Such implementation choices MUST NOT alter the semantic definitions established by the Templates Component.

In particular, an implementation MUST NOT make the Template model dependent on:

* a particular file system;
* a particular database;
* a particular programming language;
* a particular document format;
* a particular source-control system.

---

# 26. Specification Evolution

This specification SHALL evolve through controlled refinement.

Future changes SHOULD prioritize:

* semantic stability;
* backward compatibility;
* reuse;
* explicit semantics;
* architectural consistency;
* traceability;
* controlled extensibility;
* technology independence.

New Template concepts SHOULD NOT be introduced when an existing concept can be reused, extended, or specialized.

Changes to this specification MUST be subject to the applicable Template Governance process.

Historical versions of the specification SHOULD be preserved where required for traceability and knowledge preservation.

---

# 27. Related Documents

The following documents define the detailed normative and descriptive foundations of this specification:

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
* **DF-RDM-040 — Templates Roadmap**

---

# 28. Change History

| Version | Revision | Date       | Change                         |
| ------- | -------: | ---------- | ------------------------------ |
| 1.0     |        0 | 2026-09-23 | Initial Template Specification |

---

**End of Document**

---