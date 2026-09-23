# Documentation Framework

# DF-TPL-013 — Template Dictionary

| Metadata        | Value                        |
| --------------- | ---------------------------- |
| **Document ID** | DF-TPL-013                   |
| **Title**       | Template Dictionary          |
| **Family**      | Templates                    |
| **Type**        | Component Reference Document |
| **Component**   | Templates                    |
| **Author**      | Arnaldo Figueira             |
| **Status**      | Draft                        |
| **Version**     | 1.0                          |
| **Revision**    | 0                            |
| **Baseline**    | 1.0                          |
| **Language**    | English                      |
| **Date**        | 2026-09-23                   |

---

## 1. Introduction

### 1.1. Purpose

This document defines the authoritative terminology of the Templates component of the Documentation Framework.

The Template Dictionary provides concise definitions for the principal concepts, entities, properties, relationships, and terms used throughout the Templates component.

Its purpose is to ensure:

* terminology consistency;
* semantic precision;
* unambiguous communication;
* consistent interpretation across Template documents;
* controlled evolution of Template terminology.

### 1.2. Scope

This dictionary covers terminology specific to the Templates component, including:

* Template concepts;
* Template structural concepts;
* Template Elements;
* Template Relationships;
* Template Constraints;
* Template lifecycle concepts;
* Template extensibility concepts;
* Template validation concepts.

Terms owned by other Documentation Framework components are referenced but are not redefined here.

---

# 2. Dictionary Conventions

The following conventions apply.

### 2.1. Term

The canonical name of a concept.

### 2.2. Definition

The authoritative concise meaning of the term within the Templates component.

### 2.3. Related Terms

Terms that have a direct semantic relationship with the defined term.

### 2.4. Responsibility

When necessary, the responsible Template concept or document is identified.

---

# 3. Core Template Terms

| Term                        | Definition                                                                                                            | Related Terms                                        |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| **Template**                | A reusable structural definition for creating and representing documentation of a defined kind.                       | Template Type, Template Structure, Template Instance |
| **Template Type**           | A classification of Templates according to their defined structural or semantic purpose.                              | Template                                             |
| **Template Structure**      | The conceptual organization of Sections and Elements that defines the structure of a Template.                        | Template Section, Template Element                   |
| **Template Schema**         | The formal structural representation of a Template definition.                                                        | Template Model, Template Constraint                  |
| **Template Instance**       | A concrete application of a Template to create or represent a specific documentation structure.                       | Template, Document Instance                          |
| **Template Version**        | A version of a Template definition representing a controlled stage of its evolution.                                  | Template Lifecycle, Template Governance              |
| **Template Parameter**      | A defined variable of a Template that permits controlled structural or contextual variation.                          | Parameterization, Template Instance                  |
| **Template Constraint**     | An explicit restriction or condition applicable to a Template entity or relationship.                                 | Constraint, Template Validation                      |
| **Template Relationship**   | An explicitly defined semantic or structural relationship between Template entities.                                  | Composition, Specialization, Reference               |
| **Template Specialization** | A Template derived from another Template to provide a more specific definition.                                       | Specialization Relationship                          |
| **Template Composition**    | The incorporation of reusable Template structures into another Template.                                              | Composition Relationship                             |
| **Template Conformance**    | The condition in which a Template or Template Instance satisfies its applicable structural and semantic requirements. | Template Validation                                  |

---

# 4. Template Structural Terms

| Term                       | Definition                                                                                  | Related Terms                            |
| -------------------------- | ------------------------------------------------------------------------------------------- | ---------------------------------------- |
| **Template Section**       | A logical structural subdivision of a Template Structure.                                   | Template Structure, Template Element     |
| **Template Element**       | A fundamental structural unit used within a Template Structure.                             | Section, Element Category                |
| **Structural Element**     | A Template Element whose primary purpose is to represent structural organization.           | Template Element                         |
| **Content Element**        | A Template Element intended to represent a location or structure for documentation content. | Template Element                         |
| **Reference Element**      | A Template Element intended to represent a reference to another defined entity or resource. | Template Element, Reference Relationship |
| **Metadata Element**       | A Template Element that provides a structural location for Metadata information.            | Metadata, Template Element               |
| **Identity Element**       | A Template Element that provides a structural location for Document Identity information.   | Document Identity, Template Element      |
| **Classification Element** | A Template Element that provides a structural location for Classification information.      | Classification, Template Element         |
| **Parameterized Element**  | A Template Element whose structure or applicability is controlled by a Template Parameter.  | Template Parameter                       |
| **Reusable Element**       | A Template Element intended for use by more than one Template.                              | Element Reuse                            |

---

# 5. Structural Property Terms

| Term                   | Definition                                                                                                       | Related Terms            |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------- | ------------------------ |
| **Ordering**           | The defined sequence in which Template Sections or Elements occur.                                               | Template Schema          |
| **Occurrence**         | The permitted number of instances of a Template Section or Element within a defined context.                     | Occurrence Constraint    |
| **Optionality**        | The property indicating whether a Template entity is required or may be omitted.                                 | Occurrence Constraint    |
| **Applicability**      | The condition determining whether a Template entity, relationship, or structure applies in a particular context. | Applicability Constraint |
| **Structural Context** | The Template structure within which an entity is defined or interpreted.                                         | Template Structure       |
| **Containment**        | The structural relationship in which an entity belongs to another Template structural entity.                    | Containment Relationship |

---

# 6. Relationship Terms

| Term                            | Definition                                                                                           | Related Terms           |
| ------------------------------- | ---------------------------------------------------------------------------------------------------- | ----------------------- |
| **Relationship**                | An explicit connection between two defined Template entities.                                        | Template Relationship   |
| **Containment Relationship**    | A relationship representing structural membership of one entity within another.                      | Containment             |
| **Reference Relationship**      | A relationship representing an explicit link without structural ownership or composition.            | Reference Element       |
| **Dependency Relationship**     | A relationship indicating that one Template entity relies on another for a defined purpose.          | Dependency              |
| **Composition Relationship**    | A relationship in which one Template incorporates another Template or reusable Template structure.   | Template Composition    |
| **Specialization Relationship** | A relationship in which one Template is derived from another Template.                               | Template Specialization |
| **Association Relationship**    | A semantic relationship that does not imply containment, dependency, composition, or specialization. | Association             |
| **Direction**                   | The semantic orientation of a relationship from source to target.                                    | Source, Target          |
| **Source**                      | The originating participant of a directional Template Relationship.                                  | Target                  |
| **Target**                      | The destination participant of a directional Template Relationship.                                  | Source                  |
| **Cardinality**                 | The permitted number of participants in a relationship.                                              | Cardinality Constraint  |
| **Relationship Type**           | The semantic category assigned to a Template Relationship.                                           | Relationship            |

---

# 7. Constraint Terms

| Term                          | Definition                                                                           | Related Terms           |
| ----------------------------- | ------------------------------------------------------------------------------------ | ----------------------- |
| **Constraint**                | A defined restriction or condition governing a Template entity or relationship.      | Template Constraint     |
| **Structural Constraint**     | A constraint governing the organization of Template structures.                      | Template Structure      |
| **Element Constraint**        | A constraint governing the permitted use or characteristics of a Template Element.   | Template Element        |
| **Occurrence Constraint**     | A constraint governing the permitted number of occurrences of an entity.             | Occurrence              |
| **Cardinality Constraint**    | A constraint governing the permitted cardinality of a relationship.                  | Cardinality             |
| **Parameter Constraint**      | A constraint governing the definition or use of a Template Parameter.                | Template Parameter      |
| **Relationship Constraint**   | A constraint governing the permitted characteristics of a Template Relationship.     | Template Relationship   |
| **Composition Constraint**    | A constraint governing Template Composition.                                         | Template Composition    |
| **Specialization Constraint** | A constraint governing Template Specialization.                                      | Template Specialization |
| **Applicability Constraint**  | A constraint governing the conditions under which an entity or relationship applies. | Applicability           |

---

# 8. Lifecycle Terms

| Term                   | Definition                                                                                                 | Related Terms      |
| ---------------------- | ---------------------------------------------------------------------------------------------------------- | ------------------ |
| **Template Lifecycle** | The controlled progression of a Template through defined lifecycle states.                                 | Template State     |
| **Draft**              | A lifecycle state in which a Template is under development and not yet defined as an established Template. | Defined            |
| **Defined**            | A lifecycle state in which the Template definition has been established but is not yet active.             | Draft, Active      |
| **Active**             | A lifecycle state in which the Template is approved for applicable use.                                    | Deprecated         |
| **Deprecated**         | A lifecycle state in which the Template remains identifiable but is no longer intended for new use.        | Retired            |
| **Retired**            | A lifecycle state in which the Template is no longer active or intended for normal use.                    | Deprecated         |
| **Template Evolution** | The controlled modification of a Template definition over time.                                            | Template Version   |
| **Template State**     | A defined lifecycle condition of a Template.                                                               | Template Lifecycle |

---

# 9. Validation Terms

| Term                          | Definition                                                                                     | Related Terms                               |
| ----------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------- |
| **Template Validation**       | The evaluation of a Template or related structure against applicable requirements.             | Conformance                                 |
| **Structural Validation**     | Validation of the structural organization of a Template.                                       | Structural Constraint                       |
| **Element Validation**        | Validation of Template Elements and their permitted use.                                       | Template Element                            |
| **Schema Validation**         | Validation against the defined Template Schema.                                                | Template Schema                             |
| **Compatibility Validation**  | Validation of compatibility between a Template and relevant external or related DF components. | Metadata, Document Identity, Classification |
| **Semantic Validation**       | Validation of the semantic correctness of a Template definition.                               | Template Semantics                          |
| **Cross-Template Validation** | Validation of relationships and dependencies involving multiple Templates.                     | Template Relationship                       |
| **Conformant**                | A validation result indicating that applicable requirements are satisfied.                     | Non-Conformant                              |
| **Non-Conformant**            | A validation result indicating that one or more applicable requirements are not satisfied.     | Conformant                                  |
| **Indeterminate**             | A validation result indicating that conformance cannot be conclusively determined.             | Template Validation                         |

---

# 10. Governance Terms

| Term                      | Definition                                                                                                  | Related Terms       |
| ------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------- |
| **Template Governance**   | The controlled management of Template authority, change, review, approval, preservation, and evolution.     | Template Governance |
| **Template Authority**    | The authority responsible for establishing or approving Template definitions.                               | Template Governance |
| **Template Ownership**    | The responsibility for maintaining and evolving a Template.                                                 | Template Governance |
| **Template Change**       | A controlled modification to a Template definition.                                                         | Template Evolution  |
| **Change Assessment**     | Evaluation of the impact and implications of a proposed Template change.                                    | Template Change     |
| **Template Review**       | Formal examination of a Template change or definition.                                                      | Template Governance |
| **Template Approval**     | A governance decision authorizing a Template definition or change.                                          | Template Governance |
| **Template Preservation** | Retention of Template definitions required for traceability, reproducibility, or historical interpretation. | Template Governance |

---

# 11. Extensibility Terms

| Term                       | Definition                                                                                                            | Related Terms                                 |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| **Template Extensibility** | The capability to adapt, reuse, specialize, compose, or parameterize Template definitions through defined mechanisms. | Template Specialization, Template Composition |
| **Specialization**         | The derivation of a more specific Template from an existing Template.                                                 | Template Specialization                       |
| **Composition**            | The combination of reusable Template structures into a Template.                                                      | Template Composition                          |
| **Parameterization**       | The use of Template Parameters to provide controlled Template variation.                                              | Template Parameter                            |
| **Element Reuse**          | The use of an existing Template Element by multiple Templates.                                                        | Reusable Element                              |
| **Structural Extension**   | The addition of explicitly defined structure to an existing Template through an applicable extensibility mechanism.   | Specialization, Composition                   |
| **Controlled Restriction** | The deliberate narrowing of permitted structure or applicability within an extensible Template definition.            | Specialization, Constraint                    |

---

# 12. Conformance Terms

| Term                        | Definition                                                                                                      | Related Terms                             |
| --------------------------- | --------------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| **Conformance**             | Satisfaction of the requirements applicable to a Template definition or Template Instance.                      | Template Validation                       |
| **Conformance Requirement** | A structural, semantic, relational, or constraint-based requirement against which conformance may be evaluated. | Template Constraint                       |
| **Conformance Evaluation**  | The process of determining whether applicable requirements are satisfied.                                       | Template Validation                       |
| **Conformance Result**      | The outcome of a conformance evaluation.                                                                        | Conformant, Non-Conformant, Indeterminate |

---

# 13. Terms That Must Remain Distinct

The following terms represent important semantic distinctions.

| Term A                     | Term B                            | Distinction                                                                                              |
| -------------------------- | --------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Template**               | **Template Instance**             | A Template defines reusable structure; an Instance applies that structure.                               |
| **Template**               | **Template Version**              | A Template is the conceptual definition; a Version represents a controlled stage of its evolution.       |
| **Template Version**       | **Document Revision**             | Template Version concerns Template evolution; Document Revision concerns a document.                     |
| **Template Structure**     | **Physical Repository Structure** | Template Structure is conceptual; repository organization is external to Templates.                      |
| **Template Schema**        | **Template Model**                | The Model defines conceptual relationships; the Schema represents the structure formally.                |
| **Constraint**             | **Validation**                    | A Constraint defines a restriction; Validation evaluates conformance.                                    |
| **Governance**             | **Validation**                    | Governance controls change and approval; Validation evaluates conformance.                               |
| **Composition**            | **Specialization**                | Composition combines reusable structures; Specialization derives a more specific Template.               |
| **Reference**              | **Composition**                   | A Reference links to another entity; Composition incorporates reusable structure.                        |
| **Dependency**             | **Specialization**                | Dependency expresses reliance; Specialization expresses derivation.                                      |
| **Metadata Element**       | **Metadata**                      | A Metadata Element provides structural placement; Metadata defines metadata semantics.                   |
| **Identity Element**       | **Document Identity**             | An Identity Element provides structural placement; Document Identity defines identity semantics.         |
| **Classification Element** | **Classification**                | A Classification Element provides structural placement; Classification defines classification semantics. |

---

# 14. Canonical Terminology

The following terms are the preferred canonical terms within the Templates component:

* **Template**
* **Template Type**
* **Template Structure**
* **Template Section**
* **Template Element**
* **Template Schema**
* **Template Instance**
* **Template Parameter**
* **Template Constraint**
* **Template Relationship**
* **Template Version**
* **Template Specialization**
* **Template Composition**
* **Template Conformance**
* **Template Lifecycle**
* **Template Validation**
* **Template Governance**
* **Template Extensibility**

Equivalent informal terms should not replace these terms in normative Template documentation when the canonical term is applicable.

---

# 15. Terminology Usage Rules

### 15.1. Rule 1 — Template

Use **Template** for the reusable structural definition.

Do not use **Template** to refer to a concrete document instance.

### 15.2. Rule 2 — Template Instance

Use **Template Instance** for a concrete application of a Template.

### 15.3. Rule 3 — Template Version

Use **Template Version** for controlled evolution of a Template definition.

Do not use **Revision**, **Edition**, or **Baseline** as synonyms.

### 15.4. Rule 4 — Constraint

Use **Constraint** for a restriction or condition.

Do not use **Validation** as a synonym.

### 15.5. Rule 5 — Relationship

Use the most specific relationship category available when the semantics are known.

### 15.6. Rule 6 — Composition

Use **Composition** only when one Template incorporates another reusable Template structure.

### 15.7. Rule 7 — Specialization

Use **Specialization** only when a Template is derived as a more specific definition from another Template.

### 15.8. Rule 8 — Reuse

Use **Reuse** for explicit reuse of existing Template definitions or Elements.

Do not infer reuse merely from similar structures.

### 15.9. Rule 9 — Extensibility

Use **Extensibility** for mechanisms that permit controlled adaptation or reuse.

### 15.10. Rule 10 — Conformance

Use **Conformance** for satisfaction of applicable Template requirements.

---

# 16. Terminology Governance

The Template Dictionary is the authoritative terminology reference for the Templates component.

Changes to canonical terminology should be:

1. explicitly proposed;
2. assessed for semantic impact;
3. evaluated against existing Template documentation;
4. reviewed for cross-document consistency;
5. approved through the applicable governance process;
6. propagated to affected documentation.

Terminology changes must preserve semantic traceability.

---

# 17. Terminology Independence

The Template Dictionary is independent of:

* programming languages;
* serialization formats;
* database technologies;
* document editors;
* repository structures;
* source-control systems;
* implementation frameworks.

Technical implementations may introduce implementation-specific terms, but those terms must not silently replace the canonical conceptual terminology.

---

# 18. Dictionary Invariants

The following invariants apply to Template terminology.

### 18.1. Invariant 1 — Canonical Meaning

Each canonical Template term must have a defined meaning.

### 18.2. Invariant 2 — Semantic Distinction

Distinct concepts must not be represented as synonyms when their semantics differ.

### 18.3. Invariant 3 — Consistent Usage

Canonical terms should be used consistently throughout Template documentation.

### 18.4. Invariant 4 — No Responsibility Leakage

Template terminology must not redefine concepts owned by other Documentation Framework components.

### 18.5. Invariant 5 — Traceable Evolution

Changes to canonical terminology must remain traceable.

### 18.6. Invariant 6 — Architectural Consistency

Terminology must remain consistent with the Templates architecture and model.

### 18.7. Invariant 7 — Technology Independence

Canonical terminology must remain independent of implementation technology.

---

# 19. Related Documents

* DF-ARC-007 — Component Documentation Structure
* DF-TPL-001 — Templates Architecture
* DF-TPL-002 — Template Concepts
* DF-TPL-003 — Template Model
* DF-TPL-004 — Template Elements
* DF-TPL-005 — Template Schema
* DF-TPL-006 — Template Lifecycle
* DF-TPL-007 — Template Validation
* DF-TPL-008 — Template Governance
* DF-TPL-009 — Template Relationships
* DF-TPL-010 — Template Constraints
* DF-TPL-011 — Template Extensibility
* DF-RDM-040 — Templates Roadmap

---

# 20. Change History

| Version | Revision | Date       | Change                                     |
| ------- | -------: | ---------- | ------------------------------------------ |
| 1.0     |        0 | 2026-09-23 | Initial definition of Template terminology |
