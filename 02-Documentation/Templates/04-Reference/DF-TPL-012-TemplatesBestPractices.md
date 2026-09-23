# Documentation Framework

# DF-TPL-012 — Template Best Practices

| Metadata        | Value                        |
| --------------- | ---------------------------- |
| **Document ID** | DF-TPL-012                   |
| **Title**       | Template Best Practices      |
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

This document defines recommended practices for designing, maintaining, extending, validating, and governing Templates within the Documentation Framework.

The purpose of these practices is to promote:

* consistency;
* reuse;
* clarity;
* explicit semantics;
* maintainability;
* traceability;
* controlled evolution.

### 1.2. Scope

This document provides guidance for:

* Template design;
* Template structure;
* Template Elements;
* Template Relationships;
* Template Constraints;
* Template extensibility;
* Template versioning;
* Template validation;
* Template governance;
* Template reuse;
* Template maintenance.

These practices are recommendations rather than replacements for normative definitions established by the Templates component.

### 1.3. Position

Best practices complement the normative Template architecture and model.

They do not redefine:

* Template Concepts;
* Template Model;
* Template Schema;
* Template Lifecycle;
* Template Validation;
* Template Governance;
* Template Relationships;
* Template Constraints;
* Template Extensibility.

---

# 2. General Principles

Template design should follow the following principles:

1. Prefer reuse over duplication.
2. Keep semantics explicit.
3. Keep structure predictable.
4. Separate structural concerns from operational concerns.
5. Use the simplest mechanism that satisfies the requirement.
6. Avoid unnecessary specialization.
7. Avoid unnecessary composition.
8. Keep constraints explicit.
9. Preserve traceability.
10. Evolve Templates in a controlled manner.

---

# 3. Template Design Practices

## 3.1. Define the Purpose First

Every Template should have a clearly defined purpose.

The purpose should identify:

* what kind of documentation structure the Template supports;
* the intended scope;
* the expected users or consumers;
* the structural problem it solves.

A Template should not exist merely because a document happens to require a different layout.

## 3.2. Define Clear Boundaries

A Template should have an explicit responsibility boundary.

It should not attempt to define responsibilities belonging to:

* Metadata;
* Document Identity;
* Classification;
* Workflow;
* Governance;
* Registry;
* Validation.

## 3.3. Prefer Conceptual Simplicity

A Template should use the minimum structural complexity required to satisfy its purpose.

Unnecessary:

* nesting;
* parameters;
* relationships;
* specialization;
* composition;
* constraints

should be avoided.

---

# 4. Structural Practices

## 4.1. Use Consistent Section Organization

Sections should have predictable purposes.

Related Elements should be grouped into meaningful Sections rather than distributed arbitrarily throughout a Template.

## 4.2. Keep Structural Hierarchies Shallow

Deep nesting should be avoided unless it provides meaningful structural semantics.

For example:

```text

            Template
            │
            └── Section
                │
                └── Subsection
                    │
                    └── Element

```

should not be extended unnecessarily merely to represent formatting preferences.

## 4.3. Make Ordering Explicit

When Element or Section order has semantic significance, that ordering should be explicitly represented.

Ordering should not depend on accidental implementation behavior.

## 4.4. Distinguish Required and Optional Structure

Required and optional Elements should be explicitly distinguishable.

For example:

```text

            Section
            │
            ├── Required Element
            │
            └── Optional Element

```

Optionality should not be inferred from the absence of a constraint.

---

# 5. Element Practices

## 5.1. Reuse Existing Elements

Existing reusable Template Elements should be preferred over creating equivalent new Elements.

Before creating a new Element, determine whether an existing Element already provides the required semantics.

## 5.2. Avoid Overloaded Elements

An Element should have a clear purpose.

An Element that represents several unrelated concepts should normally be decomposed.

## 5.3. Preserve Element Semantics

When reusing an Element, its established semantics should be preserved.

A Template may constrain its use without silently redefining the Element itself.

## 5.4. Keep Element Names Consistent

Equivalent Elements should use consistent terminology throughout the Template ecosystem.

Different names should not be introduced for semantically identical Elements without justification.

---

# 6. Relationship Practices

## 6.1. Use the Most Specific Relationship

When defining a relationship, select the relationship type that most accurately represents its semantics.

For example:

```text

    Reference
    Dependency
    Composition
    Specialization
    Association

```

should not be used interchangeably.

## 6.2. Avoid Implicit Relationships

Relationships should be explicitly represented when they are relevant to Template semantics.

Do not rely on:

* naming conventions;
* physical location;
* file ordering;
* implementation-specific behavior

to establish semantic relationships.

## 6.3. Avoid Unnecessary Relationships

Not every connection between Template entities needs to become a formal relationship.

A relationship should be defined when its semantics provide meaningful structural, reuse, dependency, or traceability value.

---

# 7. Constraint Practices

## 7.1. Make Constraints Explicit

Constraints should clearly identify:

* their target;
* their semantic purpose;
* their scope;
* their applicability.

## 7.2. Prefer Simple Constraints

A simple constraint is preferable to a complex combination of interacting constraints when both achieve the same result.

## 7.3. Avoid Conflicting Constraints

Constraints applying to the same structural context should have a deterministic combined interpretation.

Conflicting constraints should be resolved before a Template is considered conformant.

## 7.4. Do Not Use Constraints as Documentation

A constraint should express an actual restriction or condition.

Descriptive information that does not restrict Template behavior should not be represented as a constraint.

---

# 8. Extensibility Practices

## 8.1. Prefer Reuse Before Specialization

When a Template can satisfy a requirement through reuse or composition, unnecessary specialization should be avoided.

## 8.2. Specialize for Meaningful Semantic Differences

Specialization should be used when the derived Template represents a meaningful specialization of an existing Template.

It should not be used merely to create a slightly different arrangement.

## 8.3. Compose Reusable Structures

Composition should be preferred when independently reusable structures can be combined without establishing a specialization relationship.

## 8.4. Parameterize Controlled Variation

Parameters should be used when variation is:

* predictable;
* explicitly definable;
* reusable;
* structurally meaningful.

Parameters should not be introduced merely to avoid creating a clear Template structure.

---

# 9. Versioning Practices

## 9.1. Distinguish Template Version from Document Version

Template Version must not be confused with:

* Document Edition;
* Document Revision;
* Document Baseline.

A Template Version identifies the evolution of the Template definition.

## 9.2. Minimize Breaking Changes

When evolving a Template, prefer changes that preserve existing conformance and usage where practical.

Potentially disruptive changes should receive explicit impact assessment.

## 9.3. Preserve Historical Definitions

Historical Template definitions should be preserved when required for:

* traceability;
* reproducibility;
* interpretation of existing documents;
* governance;
* historical analysis.

---

# 10. Validation Practices

## 10.1. Validate Structural Conformance

Templates should be validated against their defined structure.

Validation should consider, as applicable:

* Elements;
* Sections;
* ordering;
* occurrences;
* parameters;
* relationships;
* constraints.

## 10.2. Validate Cross-Template Dependencies

Where Templates depend on or compose other Templates, their relationships should be evaluated for conformance.

## 10.3. Treat Indeterminate Results Explicitly

An inability to determine conformance should not automatically be interpreted as conformance.

The validation result should explicitly distinguish:

```text

    Conformant
    Non-Conformant
    Indeterminate

```

---

# 11. Governance Practices

## 11.1. Record Significant Changes

Significant Template changes should be traceable.

Records should identify, as applicable:

* what changed;
* why it changed;
* affected Template Version;
* impact;
* validation evidence;
* governance decision.

## 11.2. Review Structural Impact

Changes affecting:

* relationships;
* constraints;
* specialization;
* composition;
* parameters

should receive appropriate impact assessment.

## 11.3. Separate Review from Validation

Validation evidence should support governance decisions, but validation and governance remain separate responsibilities.

---

# 12. Reuse Practices

Template reuse should be evaluated before introducing a new Template.

A useful decision sequence is:

```text

                    Required Structure
                            │
                            ▼

                    Existing Template?
                            │
                ┌───────────┴───────────┐
                │                       │
               Yes                      No
                │                       │
                ▼                       ▼

              Reuse             Existing reusable
                                    Elements?
                                        │
                                    Yes / No
                                        │
                                        ▼

                                Compose or create

```

The objective is to minimize unnecessary duplication while preserving semantic clarity.

---

# 13. Documentation Practices

Every Template should have sufficient documentation to make its intended use understandable.

At minimum, documentation should make clear:

* purpose;
* scope;
* structural organization;
* relevant relationships;
* constraints;
* extensibility mechanisms;
* applicable version.

Template documentation should use the authoritative terminology established by the Templates component.

---

# 14. Naming Practices

Template names should:

* be explicit;
* be stable;
* use established terminology;
* avoid unnecessary abbreviations;
* distinguish semantically different Templates;
* remain consistent with the Documentation Framework naming conventions.

Names should describe semantic purpose rather than implementation technology.

---

# 15. Anti-Patterns

The following practices should generally be avoided.

### 15.1. Template Duplication

Creating a new Template when an existing Template can be reused or appropriately specialized.

### 15.2. Implicit Semantics

Relying on naming, ordering, or physical location to establish meaning that should be explicitly represented.

### 15.3. Over-Parameterization

Introducing large numbers of parameters to represent variations that would be clearer as separate Templates.

### 15.4. Over-Specialization

Creating deep specialization hierarchies without meaningful semantic distinctions.

### 15.5. Uncontrolled Composition

Composing Templates without clearly defined structural or semantic relationships.

### 15.6. Constraint Accumulation

Continuously adding constraints to compensate for an unclear Template structure.

### 15.7. Responsibility Leakage

Using Templates to define metadata, identity, classification, workflow, repository, or governance semantics.

### 15.8. Technology Coupling

Defining Template semantics in terms of a specific file format, database, programming language, or document editor.

---

# 16. Template Design Checklist

Before introducing or substantially modifying a Template, verify:

### 16.1. Purpose

* [ ] Is the purpose explicit?
* [ ] Is the scope clear?
* [ ] Is the Template genuinely necessary?1.

### 16.2. Structure

* [ ] Is the structure simple?
* [ ] Are Sections meaningful2.?
* [ ] Is ordering explicit where necessary?
* [ ] Are required and optional Elements clear?

### 16.3. Reuse

* [ ] Could an existing Template be reused3.?
* [ ] Could an existing Element be reused?
* [ ] Would Composition be more appropriate than duplication?
* [ ] Is Specialization semantically justified?

### 16.4. Relationships4.

* [ ] Are relevant relationships explici 16.t?
* [ ] Is the relationship type appropriate?
* [ ] Is direction clear where required?
* [ ] Is cardinality appropriate?

### 16.5. Constraint 16.s

* [ ] Are restrictions explicit?
* [ ] Are constraints necessary?
* [ ] Are conflicting constraints avoided?
* [ ] Is applicability clear 16.?

### 16.6. Evolution

* [ ] Is the change compatible with existing usage?
* [ ] Is the Template Version appropriately updated?
* [ ] Is historical information preserved where necessary 16.?
* [ ] Is governance required?

### 16.7. Validation

* [ ] Can the Template be validated?
* [ ] Are applicable constraints evaluabl 16.e?
* [ ] Are cross-template dependencies identifiable?

---

# 17. Best Practices Summary

The principal Template best practices can be summarized as:

```text

            Design
            │
            ├── Define purpose
            │
            ├── Keep boundaries clear
            │
            └── Prefer simplicity

            Structure
            │
            ├── Organize consistently
            │
            ├── Make ordering explicit
            │
            └── Distinguish required/optional structure

            Reuse
            │
            ├── Reuse Elements
            │
            ├── Reuse Templates
            │
            ├── Compose when appropriate
            │
            └── Specialize when semantically justified

            Constraints
            │
            ├── Keep restrictions explicit
            │
            ├── Avoid conflicts
            │
            └── Avoid unnecessary complexity

            Evolution
            │
            ├── Version explicitly
            │
            ├── Preserve traceability
            │
            ├── Assess impact
            │
            └── Govern significant changes

            Validation
            │
            ├── Validate conformance
            │
            ├── Validate relationships
            │
            └── Treat indeterminate results explicitly

```

The central principle is:

> **Prefer explicit, reusable, simple, and semantically stable Template structures over duplicated, implicit, or unnecessarily complex structures.**

---

# 18. Related Documents

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

# 19. Change History

| Version | Revision | Date       | Change                                        |
| ------- | -------: | ---------- | --------------------------------------------- |
| 1.0     |        0 | 2026-09-23 | Initial definition of Template Best Practices |
