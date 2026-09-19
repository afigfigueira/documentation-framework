# Documentation Framework

# DF-TPL-007 — Template Validation

| Metadata        | Value                       |
| --------------- | --------------------------- |
| **Document ID** | DF-TPL-007                  |
| **Title**       | Template Validation         |
| **Family**      | Templates                   |
| **Type**        | Component Behavior Document |
| **Component**   | Templates                   |
| **Author**      | Arnaldo Figueira            |
| **Status**      | Draft                       |
| **Version**     | 1.0                         |
| **Revision**    | 0                           |
| **Baseline**    | 1.0                         |
| **Language**    | English                     |
| **Date**        | 2026-09-19                  |

---

## 1. Introduction

### 1.1. Purpose

This document defines the validation behavior of Templates within the Documentation Framework.

Template Validation determines whether a Template, its schema, and applicable Template Instances conform to the structural and semantic requirements established by the Templates component.

Validation provides the mechanisms by which Template conformance can be evaluated without assuming responsibility for Template lifecycle, governance, storage, or document management.

### 1.2. Scope

This document defines:

* Template validation;
* validation targets;
* validation levels;
* validation categories;
* validation sequence;
* validation results;
* validation findings;
* validation conformance;
* validation invariants;
* relationships between validation and other Templates responsibilities.

This document does not define:

* Template lifecycle states;
* governance policies;
* detailed relationship semantics;
* detailed constraint semantics;
* Template extensibility mechanisms;
* repository validation;
* document workflow;
* implementation-specific validation tools.

---

## 2. Validation Position

Template Validation operates on the representations defined by the Templates component.

The principal relationship is:

```text

            Template Concepts
                    │
                    ▼

              Template Model
                    │
                    ▼

            Template Elements
                    │
                    ▼

             Template Schema
                    │
                    ▼

           Template Validation

```

Validation evaluates whether a concrete representation conforms to the applicable model, schema, constraints, and semantic requirements.

Validation therefore consumes definitions established by other Templates documents rather than redefining them.

---

## 3. Validation Objectives

Template Validation has the following objectives:

1. determine Template conformance;
2. detect structural inconsistencies;
3. detect invalid or unresolved references;
4. detect invalid element composition;
5. detect parameter inconsistencies;
6. evaluate applicable constraints;
7. detect semantic inconsistencies;
8. support cross-Template consistency verification;
9. provide explicit validation findings;
10. distinguish valid, invalid, and indeterminate results;
11. provide a basis for controlled Template evolution;
12. remain independent of implementation technology.

---

## 4. Validation Targets

Template Validation may operate on different levels of the Templates model.

```text

            Validation Target
            │
            ├── Template
            │
            ├── Template Schema
            │
            ├── Template Structure
            │
            ├── Template Section
            │
            ├── Template Element
            │
            ├── Template Parameter
            │
            ├── Template Relationship
            │
            └── Template Instance

```

A validation operation must identify the target against which validation is being performed.

### 4.1. Template Validation

Template validation evaluates the Template definition as a whole.

It may include:

* structural validation;
* element validation;
* schema validation;
* parameter validation;
* relationship validation;
* constraint validation;
* semantic validation.

### 4.2. Schema Validation

Schema validation evaluates whether the Template representation conforms to the Template Schema.

### 4.3. Template Instance Validation

Template Instance validation evaluates whether a concrete Template Instance conforms to the applicable Template definition.

---

## 5. Validation Levels

Template Validation is organized into progressively broader validation levels.

```text

                Structural
                    │
                    ▼

                 Element
                    │
                    ▼

                  Schema
                    │
                    ▼

              Compatibility
                    │
                    ▼

                 Semantic
                    │
                    ▼

              Cross-Template

```

Not every validation operation must execute every level.

The applicable levels depend on the validation target and validation context.

---

## 6. Structural Validation

Structural Validation verifies the fundamental organization of a Template representation.

It evaluates conditions such as:

* Template Structure existence;
* Section containment;
* Element containment;
* structural hierarchy;
* structural references;
* ordering representation;
* occurrence representation.

Example:

```text

            Template
            │
            └── Structure
                │
                └── Section
                    │
                    └── Element

```

Structural validation determines whether this organization is structurally valid.

---

## 7. Element Validation

Element Validation evaluates Template Elements against their applicable Element definitions.

It may evaluate:

* Element category;
* Element identity;
* Element position;
* Element occurrence;
* Element applicability;
* Element composition;
* Element references;
* Element parameters.

Element Validation must preserve the distinctions defined by DF-TPL-004 — Template Elements.

It must not redefine Element categories.

---

## 8. Schema Validation

Schema Validation determines whether the concrete Template representation conforms to the Template Schema.

It includes evaluation of:

* required schema components;
* structural containment;
* references;
* parameter definitions;
* relationship representations;
* version representation;
* schema invariants.

The distinction is:

```text

             Template Schema
                    │
                    ▼

               Schema Rules
                    │
                    ▼

                Validation
                    │
                    ▼

            Conformance Result

```

Schema Validation evaluates representation.

It does not define the schema itself.

---

## 9. Metadata Compatibility Validation

Templates interact with the Metadata component.

Validation may therefore verify compatibility between a Template and applicable metadata requirements.

Examples include:

* required metadata locations being represented;
* metadata references resolving;
* metadata structures being compatible with the Template;
* metadata-related Template Elements being structurally consistent.

Template Validation does not redefine Metadata semantics.

Metadata remains the responsibility of the Metadata component.

---

## 10. Document Identity Compatibility Validation

Templates may contain Identity Elements that provide structural locations for document identity information.

Validation may verify that:

* required identity structures are represented;
* Identity Elements are structurally valid;
* identity-related references resolve.

Template Validation does not assign or manage Document Identity.

Document Identity remains the responsibility of the Document Identity component.

---

## 11. Classification Compatibility Validation

Templates may contain Classification Elements that provide structural locations for classification information.

Validation may verify:

* classification structures are represented;
* applicable references resolve;
* classification-related elements are structurally consistent.

Template Validation does not define document classification.

Classification remains the responsibility of the Classification component.

---

## 12. Parameter Validation

Parameter Validation evaluates the structural definition and use of Template Parameters.

It may verify:

* parameter definitions exist;
* parameter references resolve;
* required parameters are represented;
* parameter applicability is consistent;
* parameter-related constraints are satisfied.

The distinction between definition and value remains:

```text

            Template
            │
            └── Parameter Definition
                         │
                         ▼

                 Template Instance
                 │
                 └── Parameter Value

```

Validation of a concrete parameter value occurs in the context of the applicable Template Instance.

---

## 13. Constraint Validation

Constraints defined for a Template are subject to validation.

The relationship is:

```text

            Template
            │
            └── Constraint
                    │
                    ▼

                Validation

```

Validation evaluates whether applicable constraints are satisfied.

The detailed semantics of constraints are defined by DF-TPL-010 — Template Constraints.

Therefore, this document defines the validation behavior but does not redefine the meaning of individual constraint types.

---

## 14. Relationship Validation

Template Relationships may require validation to ensure that their structural representation is consistent.

Validation may verify:

* relationship source exists;
* relationship target exists;
* references resolve;
* relationship participants are compatible;
* required relationship information is present.

Detailed relationship semantics are defined by DF-TPL-009 — Template Relationships.

---

## 15. Semantic Validation

Semantic Validation evaluates whether a Template representation preserves the intended meaning established by the Templates conceptual model.

Semantic validation may detect situations where a structure is technically representable but conceptually inconsistent.

Examples include:

* incompatible Template components;
* contradictory structural meanings;
* inappropriate use of Element categories;
* inconsistent parameter applicability;
* semantic conflicts between composed structures.

Semantic validation is therefore distinct from simple structural validation.

```text

     Structural Validity
             !=
      Semantic Validity

```

A Template may be structurally well-formed while still being semantically invalid.

---

## 16. Cross-Template Validation

Templates may interact with other Templates through composition, specialization, reuse, or relationships.

Cross-Template Validation evaluates consistency across these boundaries.

It may identify:

* incompatible composed structures;
* invalid specialization;
* unresolved reusable components;
* conflicting definitions;
* inconsistent references;
* incompatible versions.

Cross-Template Validation must respect the semantics defined by DF-TPL-009 and DF-TPL-011.

---

## 17. Validation Sequence

A complete validation operation may follow the following conceptual sequence:

```text

      1. Identify Validation Target
                    │
                    ▼

         2. Structural Validation
                    │
                    ▼

          3. Element Validation
                    │
                    ▼

           4. Schema Validation
                    │
                    ▼

        5. Component Compatibility
                    │
                    ▼

         6. Parameter Validation
                    │
                    ▼

         7. Constraint Validation
                    │
                    ▼

        8. Relationship Validation
                    │
                    ▼

          9. Semantic Validation
                    │
                    ▼

      10. Cross-Template Validation
                    │
                    ▼

          11. Validation Result

```

The sequence is conceptual.

An implementation may optimize the execution order provided that the resulting validation semantics are preserved.

---

## 18. Validation Findings

A validation operation produces findings when one or more conditions are not satisfied.

A finding identifies, as applicable:

```text

            Validation Finding
            │
            ├── Target
            │
            ├── Category
            │
            ├── Severity
            │
            ├── Condition
            │
            ├── Description
            │
            └── Reference

```

### 18.1. Target

Identifies the Template component associated with the finding.

### 18.2. Category

Identifies the validation category that produced the finding.

Examples include:

* Structural;
* Element;
* Schema;
* Compatibility;
* Parameter;
* Constraint;
* Relationship;
* Semantic;
* Cross-Template.

### 18.3. Severity

Severity indicates the significance of the finding.

The detailed severity taxonomy may be defined by the applicable validation implementation or governance rules.

### 18.4. Condition

Identifies the condition that was not satisfied.

### 18.5. Description

Provides a human-readable explanation of the finding.

### 18.6. Reference

Identifies the applicable Template definition, schema component, constraint, relationship, or other authoritative source.

---

## 19. Validation Results

A validation operation produces a Validation Result.

The conceptual result states are:

```text

            Validation Result
            │
            ├── Conformant
            │
            ├── Non-Conformant
            │
            └── Indeterminate

```

### 19.1. Conformant

The validated target satisfies the applicable validation requirements.

### 19.2. Non-Conformant

One or more applicable requirements are not satisfied.

The result includes the associated validation findings.

### 19.3. Indeterminate

A conformance determination cannot be completed because required information or evaluation conditions are unavailable.

An Indeterminate result must not be interpreted as Conformant.

---

## 20. Validation Scope

Validation may be performed at different scopes.

### 20.1. Component Scope

Validation applies to one Template component.

```text

            Template
            │
            └── Element

```

### 20.2. Template Scope

Validation applies to a complete Template definition.

```text

            Template
            │
            ├── Structure
            │
            ├── Parameters
            │
            ├── Constraints
            │
            ├── Relationships
            │
            └── Version

```

### 20.3. Template Instance Scope

Validation applies to a concrete Template Instance.

### 20.4. Cross-Template Scope

Validation applies to multiple related Templates.

The selected scope must be explicit for a validation operation.

---

## 21. Validation and Lifecycle

Validation and lifecycle are separate concerns.

The lifecycle determines the behavioral state of a Template.

Validation determines conformance.

```text

            Template
            │
            ├── Lifecycle State
            │
            └── Validation Result

```

A validation result does not itself constitute a lifecycle transition.

Conversely, a lifecycle transition may require validation according to applicable governance rules.

---

## 22. Validation and Governance

Governance determines how validation results may be used for lifecycle decisions.

For example:

```text

                Validation
                    │
                    ▼

            Validation Result
                    │
                    ▼

           Governance Decision
                    │
                    ▼

           Lifecycle Transition

```

Validation does not define who may approve a Template or which governance process must be followed.

Those responsibilities belong to DF-TPL-008 — Template Governance.

---

## 23. Validation and Template Version

Validation applies to a specific Template definition and therefore to a specific Template Version where versioning is applicable.

```text

            Template
            │
            └── Version
                │
                ├── Schema
                │
                └── Validation

```

A validation result must therefore be traceable to the Template Version against which validation was performed.

A validation result for one Template Version must not automatically be interpreted as a validation result for another Version.

---

## 24. Validation Invariants

The following invariants apply to Template Validation.

### 24.1. Target Invariant

Every validation operation identifies a validation target.

### 24.2. Context Invariant

Validation is performed against an explicitly applicable Template definition, schema, or validation context.

### 24.3. Traceability Invariant

Validation findings remain traceable to the validated target and applicable requirement.

### 24.4. Version Invariant

Validation results are associated with the Template Version against which validation was performed.

### 24.5. Result Invariant

Indeterminate validation must not be interpreted as conformance.

### 24.6. Responsibility Invariant

Validation does not assume responsibility for lifecycle, governance, storage, repository management, or document identity.

### 24.7. Semantic Invariant

Validation must preserve the semantics defined by the Templates component.

### 24.8. Technology Independence Invariant

The validation model remains independent of a particular implementation technology.

---

## 25. Validation Independence

Template Validation is independent of:

* programming language;
* storage technology;
* repository implementation;
* serialization format;
* file-system organization;
* document editor;
* publication mechanism.

An implementation may provide automated validation, manual validation, or a combination of both, provided that the resulting behavior conforms to the Templates architecture.

---

## 26. Validation Summary

Template Validation provides a structured mechanism for determining Template conformance.

Its principal validation dimensions are:

```text

                Structural
                    │
                    │
                 Element
                    │
                    │
                  Schema
                    │
                    │
              Compatibility
                    │
                    │
                Parameter
                    │
                    │
                Constraint
                    │
                    │
               Relationship
                    │
                    │
                 Semantic
                    │
                    │
              Cross-Template

```

The resulting determination is:

```text

    Conformant
    Non-Conformant
    Indeterminate

```

Validation therefore provides the behavioral bridge between the structural definitions of Templates and their controlled use.

---

## 27. Related Documents

### 27.1. Templates Component

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
* DF-TPL-012 — Template Best Practices
* DF-TPL-013 — Template Dictionary
* DF-TPL-014 — Template Specification
* DF-TPL-015 — Template Examples

### 27.2. Related Components

* Metadata
* Document Identity
* Classification
* Workflow
* Baselines

---

## 28. Change History

| # | Date       | Author           | Type            | Document   | Description                             |
| - | ---------- | ---------------- | --------------- | ---------- | --------------------------------------- |
| 1 | 2026-09-19 | Arnaldo Figueira | Add New Content | DF-TPL-007 | Initial Template Validation definition. |

---

**End of Document**

---