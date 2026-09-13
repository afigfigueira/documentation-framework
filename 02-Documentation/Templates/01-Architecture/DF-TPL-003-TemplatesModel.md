# Documentation Framework

# DF-TPL-003 — Template Model

| Metadata        | Value                           |
| --------------- | ------------------------------- |
| **Document ID** | DF-TPL-003                      |
| **Title**       | Template Model                  |
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

This document defines the structural model of the **Templates** component of the Documentation Framework.

It formalizes the relationships and structural dependencies between the concepts defined in **DF-TPL-002 — Template Concepts**, establishing a coherent model for representing templates, their structures, elements, schemas, parameters, constraints, versions, instances, specialization, composition, and conformance.

The model provides the structural foundation for the subsequent Template documentation documents.

## 1.2. Scope

This document defines:

* the Template model entities;
* the structural relationships between Template concepts;
* entity composition and containment;
* template specialization and composition;
* parameterization;
* constraints;
* template versions;
* template instances;
* conformance;
* model invariants;
* cross-component boundaries;
* model independence and evolution.

This document does not define:

* the detailed definition of individual template elements;
* the complete template schema;
* operational validation procedures;
* governance procedures;
* workflow management;
* document identity;
* document metadata;
* document classification;
* repository organization;
* physical storage formats.

Those concerns are addressed by the appropriate Templates documents or by other Documentation Framework components.

---

# 2. Model Position

The Template Model belongs to the **Documentation Layer** of the Documentation Framework.

Templates operate as reusable structural definitions for documentation.

The model establishes the relationship between a template and the structural artifacts required to apply that template to documentation.

At a high level:

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
            ├── Template Version
            │
            ├── Template Relationship
            │
            ├── Template Specialization
            │
            ├── Template Composition
            │
            └── Template Instance

```

The model describes conceptual structures and relationships. It does not prescribe a physical repository, file format, programming language, serialization mechanism, or storage technology.

---

# 3. Model Objectives

The Template Model has the following objectives:

1. provide a coherent structural representation of Templates;
2. establish explicit relationships between Template concepts;
3. support reusable documentation structures;
4. separate template definition from template application;
5. separate structural definition from metadata, identity, and classification;
6. support controlled template variation;
7. support template specialization and composition;
8. support parameterized templates;
9. support structural constraints;
10. support controlled template evolution through versions;
11. provide a basis for conformance and validation;
12. preserve technology and repository independence.

---

# 4. Template Model Overview

The model consists of several related structural areas.

```text

                                      ┌───────────────────┐
                                      │   Template Type   │
                                      └─────────┬─────────┘
                                                │
                                            classifies
                                                │
                                                ▼

                ┌────────────────┐      ┌──────────────┐
                │ Template       ├──────┤              │
                │ Relationship   │      │   Template   │
                └────────────────┘      │              │
                                        └──────┬───────┘
                                               │
                        ┌──────────────────────┼──────────────────────┐
                        │                      │                      │
                        ▼                      ▼                      ▼

                Template Structure      Template Schema        Template Version
                        │
                        │
             ┌──────────┴──────────┐
             │                     │
             ▼                     ▼

      Template Section     Template Element
             │
             │
             └──────────────────────┐
                                    │
                                    ▼

                            Template Parameter
                                    │
                                    ▼

                           Template Constraint

                 Template
                    │
                    ▼

         Template Specialization
                    │
                    ▼

           Template Composition

                 Template
                    │
                    ▼

            Template Instance
                    │
                    ▼

               Conformance

```

This overview represents conceptual relationships rather than implementation structures.

---

# 5. Core Model Entities

## 5.1. Template

The **Template** is the central entity of the model.

A Template represents a reusable definition of documentation structure.

Conceptually:

```text

            Template
            │
            ├── Type
            │
            ├── Structure
            │
            ├── Schema
            │
            ├── Parameters
            │
            ├── Constraints
            │
            ├── Versions
            │
            ├── Relationships
            │
            ├── Specializations
            │
            ├── Composition
            │
            └── Instances

```

A Template defines what structural organization a conforming document should follow.

A Template does not itself constitute a Document Instance.

### 5.1.1. Template Model Responsibilities

The Template entity provides the structural root for:

* template organization;
* structural definition;
* schema association;
* parameter definition;
* constraint association;
* version management;
* template relationships;
* specialization;
* composition;
* template instantiation.

---

## 5.2. Template Type

A **Template Type** provides the conceptual classification of a Template within the Templates component.

The relationship is:

```text

              Template Type
                    │
                classifies
                    │
                    ▼

                 Template

```

A Template Type does not replace or redefine the Documentation Framework's document classification mechanisms.

It describes the type of template rather than the classification of a document instance.

---

## 5.3. Template Structure

A **Template Structure** represents the conceptual organization of a Template.

It provides the structural container for template sections and their elements.

```text

            Template
            │
            └── Template Structure
                │
                └── Template Section
                    │
                    └── Template Element

```

Template Structure represents conceptual organization.

It does not represent:

* directories;
* files;
* repositories;
* storage containers;
* physical paths.

---

## 5.4. Template Section

A **Template Section** represents a logical subdivision of a Template Structure.

Sections organize template elements into meaningful structural units.

```text

            Template Structure
            │
            ├── Section
            │   │
            │   └── Element
            │
            └── Section
                │
                └── Element

```

A Template Structure may contain multiple Template Sections.

A Template Section belongs to a Template Structure.

---

## 5.5. Template Element

A **Template Element** represents a structural unit within a Template Section.

```text

            Template Section
            │
            ├── Template Element
            │
            ├── Template Element
            │
            └── Template Element

```

Elements represent the atomic or logically indivisible structural components required by a template.

The detailed taxonomy and semantics of Template Elements are deferred to **DF-TPL-004 — Template Elements**.

---

## 5.6. Template Schema

A **Template Schema** represents the formal structural definition of a Template.

The schema describes the structure sufficiently to establish structural conformance.

```text

            Template
            │
            ├── Structure
            │
            └── Schema

```

The Template Schema is associated with the Template rather than with a particular storage or serialization technology.

Detailed schema rules are defined in **DF-TPL-005 — Template Schema**.

---

## 5.7. Template Parameter

A **Template Parameter** represents a defined point of controlled variation within a Template.

```text

            Template
            │
            ├── Parameter
            │   │
            │   └── Value supplied during application
            │
            └── Structure

```

Parameters allow a reusable Template to accommodate controlled differences without requiring a separate Template definition for every variation.

A parameter belongs to the Template definition.

A supplied parameter value belongs to a particular application of that Template.

---

## 5.8. Template Constraint

A **Template Constraint** represents a restriction applied to a Template, its structure, elements, parameters, or relationships.

```text

            Template
            │
            └── Constraint
                │
                └── applies to Template Model component

```

Constraints establish conditions that must be respected for a Template or Template Instance to conform to the applicable Template definition.

Detailed constraint types and rules are defined in **DF-TPL-010 — Template Constraints**.

---

## 5.9. Template Version

A **Template Version** represents a controlled state in the evolution of a Template definition.

```text

            Template
            │
            ├── Version 1
            │
            ├── Version 2
            │
            └── Version 3

```

A Template Version belongs to the evolution of a Template.

Template Version is distinct from:

* Document Identity;
* document revision;
* document baseline;
* document instance state.

Template versioning describes the evolution of the reusable template definition, not the identity or lifecycle of documents created from it.

---

## 5.10. Template Instance

A **Template Instance** represents the concrete application of a Template to a particular documentation creation context.

```text

                 Template
                    │
                applied to
                    │
                    ▼

            Template Instance
            │
            ├── resolved structure
            │
            ├── resolved parameters
            │
            └── applicable constraints

```

A Template Instance is not itself equivalent to a Document Instance.

It represents the application of the template definition from which documentation may be created or structured.

The Template Instance therefore provides the bridge between reusable template definition and concrete template application without transferring document-management responsibilities into Templates.

---

# 6. Entity Relationships

The primary relationships can be represented as follows:

```text

              Template Type
                    │
                  1 : N
                    │
                    ▼

                 Template
                 │
                 ├────  1 : 1  ────  Template Structure
                 │
                 ├────  1 : 1  ────  Template Schema
                 │
                 ├────  1 : N  ────  Template Parameter
                 │
                 ├────  1 : N  ────  Template Constraint
                 │
                 ├────  1 : N  ────  Template Version
                 │
                 ├────  1 : N  ────  Template Relationship
                 │
                 ├────  1 : N  ────  Template Instance
                 │
                 └────  N : N  ────  Template

                            ▲
                            │
    specialization / composition / other relationships

```

The cardinalities represent the conceptual model and are not implementation requirements.

---

# 7. Structural Model

## 7.1. Template Structural Hierarchy

The fundamental structural hierarchy is:

```text

            Template
            │
            └── Template Structure
                │
                └── Template Section
                    │
                    └── Template Element

```

This hierarchy establishes the primary organization of template content.

The hierarchy is structural rather than physical.

## 7.2. Structural Containment

The containment relationships are:

```text

    Template
        contains Template Structure

    Template Structure
        contains Template Sections

    Template Section
        contains Template Elements

```

Containment expresses structural membership.

It does not imply:

* filesystem containment;
* database containment;
* ownership by a repository;
* storage dependency.

## 7.3. Structural Ordering

Template Sections and Template Elements may have an explicitly defined structural order when ordering is significant to the Template.

The model therefore permits:

```text

            Template Structure
            │
            ├── Section [1]
            │
            ├── Section [2]
            │
            └── Section [3]

```

and:

```text

            Section [1]
            │
            ├── Element [1]
            │
            ├── Element [2]
            │
            └── Element [3]

```

Ordering is a property of the template structure and must not be inferred from physical storage order.

---

# 8. Template Composition Model

Template composition allows a Template to be constructed from reusable structural definitions.

Conceptually:

```text

            Template A
            │
            ├── Component Structure A
            │
            ├── Component Structure B
            │
            └── Component Structure C

```

Composition establishes that a Template may incorporate structures defined by other Templates or reusable template structures where permitted by the applicable model rules.

Composition must preserve:

* structural clarity;
* semantic consistency;
* explicit dependencies;
* conformance;
* responsibility boundaries.

Composition must not create implicit dependencies that cannot be represented by the Template Model.

Detailed composition rules are part of the subsequent Templates specification.

---

# 9. Specialization Model

Template specialization represents the derivation of a more specific Template from an existing Template.

```text

              Base Template
                    │
               specializes
                    │
                    ▼

           Specialized Template

```

A specialized Template retains the applicable structural semantics of its base Template while introducing permitted specialization.

The relationship can be represented as:

```text

            Template A
            │
            └── specialization  ─────►  Template B

```

Specialization must be explicit.

It must not be inferred solely from similarity between Templates.

A specialized Template remains a distinct Template definition.

---

# 10. Parameterization Model

Parameterization provides controlled variation within a Template.

```text

            Template
            │
            ├── Parameter A
            │
            ├── Parameter B
            │
            └── Parameter C

```

A parameter consists conceptually of:

```text

            Parameter
            │
            ├── Definition
            │
            ├── Expected value characteristics
            │
            ├── Structural or semantic applicability
            │
            └── Constraint association

```

During template application:

```text

           Template Definition
                    │
                    ├── Parameter Definitions
                    │
                    ▼

            Template Instance
            │
            └── Parameter Values

```

Parameter definitions belong to the Template.

Parameter values belong to a particular Template Instance or application context.

This distinction prevents mutable application values from altering the Template definition itself.

---

# 11. Constraint Model

Constraints may apply at different structural levels.

```text

            Template
            │
            ├── Template-level constraint
            │
            ├── Structure-level constraint
            │
            ├── Section-level constraint
            │
            ├── Element-level constraint
            │
            ├── Parameter-level constraint
            │
            └── Relationship-level constraint

```

The model therefore treats constraints as associated structural restrictions rather than as independent document-management policies.

Constraints may define conditions such as:

* required structural components;
* permitted structural relationships;
* cardinality;
* ordering;
* parameter applicability;
* composition restrictions;
* specialization restrictions;
* conformance conditions.

Detailed constraint semantics are defined in **DF-TPL-010 — Template Constraints**.

---

# 12. Version Model

Template evolution is represented through Template Versions.

```text

            Template
            │
            ├── Version 1
            │
            ├── Version 2
            │
            └── Version 3

```

A Template Version represents a controlled state of the Template definition.

A version may affect:

* Template Structure;
* Template Schema;
* Template Elements;
* Parameters;
* Constraints;
* Relationships;
* Composition;
* Specialization rules.

Version changes must preserve the distinction between:

```text

            Template Version
            │
            └── evolution of Template definition

            Document Revision
            │
            └── evolution of Document Instance

```

These are separate concepts belonging to different responsibilities.

Detailed lifecycle semantics are defined in **DF-TPL-006 — Template Lifecycle**.

---

# 13. Instance Model

Template application produces a Template Instance.

```text

                 Template
                    │
               instantiate
                    │
                    ▼
   
            Template Instance
            │
            │
            ├── Template Version
            │
            ├── resolved Structure
            │
            ├── resolved Parameters
            │
            └── applicable Constraints

```

A Template Instance is associated with the Template definition from which it was produced.

The instance may resolve:

* the applicable Template Version;
* parameter values;
* structural composition;
* specialization;
* applicable constraints.

The instance does not acquire responsibility for:

* assigning document identity;
* managing document metadata;
* classifying documents;
* approving documents;
* publishing documents;
* storing documents.

Those responsibilities belong to other Documentation Framework components or systems.

---

# 14. Conformance Model

Conformance expresses whether a Template Instance satisfies the structural requirements of the applicable Template definition.

Conceptually:

```text

                 Template
                    │
                 defines
                    │
                    ▼

             Template Schema
                    │
                constrains
                    │
                    ▼

            Template Instance
                    │
              evaluated for
                    │
                    ▼

               Conformance

```

Conformance may consider:

* required structure;
* permitted structure;
* element presence;
* structural relationships;
* parameter validity;
* applicable constraints;
* composition;
* specialization;
* Template Version compatibility.

Conformance is a property of the relationship between an applied template structure and its defining template.

Operational validation procedures are defined separately in **DF-TPL-007 — Template Validation**.

---

# 15. Cross-Component Model Boundaries

The Template Model interacts with other Documentation Framework components without absorbing their responsibilities.

| Component                      | Relationship with Template Model                                                                                                        |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Metadata**                   | Templates may define structures in which metadata is represented or expected, but Templates do not define the Metadata component        |
| **Document Identity**          | Templates may provide structural locations for identity information, but Templates do not assign or govern document identity            |
| **Classification**             | Templates may be associated with structural expectations related to document classification, but Templates do not define classification |
| **Workflow**                   | Templates may be used by workflow activities, but Templates do not define workflow                                                      |
| **Policies**                   | Template constraints are structural constraints and are distinct from governance policies                                               |
| **Registry**                   | Templates may be referenced by registry mechanisms, but Templates do not manage registration                                            |
| **Validation**                 | Templates provide conformance requirements; validation mechanisms determine whether those requirements are satisfied                    |
| **Automation**                 | Templates may be consumed by automated generation or validation mechanisms, but do not define automation                                |
| **Document Management System** | A DMS may apply Templates when managing document instances, but Template Model remains independent of operational document management   |

The central boundary is:

```text

            Templates
            │
            ├──────  define reusable documentation structure
            │
            X  ────  do not manage documentation operations

```

---

# 16. Model Invariants

The Template Model establishes the following invariants.

## 16.1. Template Identity Independence

A Template is conceptually independent of:

* filenames;
* directory paths;
* repositories;
* storage systems;
* serialization formats.

## 16.2. Structural Independence

Template Structure represents conceptual organization and must not depend on a particular physical representation.

## 16.3. Definition/Application Separation

A Template definition and a Template Instance are distinct entities.

```text

         Template

            !=

     Template Instance

```

## 16.4. Template/Document Separation

A Template is not a Document Instance.

```text

         Template

            !=

     Document Instance

```

## 16.5. Version Separation

Template Version is distinct from document revision and document baseline.

## 16.6. Parameter Separation

Parameter definitions belong to the Template definition, while parameter values belong to a specific application context.

## 16.7. Explicit Relationships

Specialization, composition, and other Template relationships must be explicitly represented.

## 16.8. Responsibility Separation

The Template Model must not absorb responsibilities belonging to Metadata, Document Identity, Classification, Workflow, Registry, or other components.

## 16.9. Structural Consistency

A Template Structure must remain consistent with the Template definition and applicable Template Schema.

## 16.10. Conformance Determinability

The model must provide sufficient structural information for conformance to be determinable.

---

# 17. Model Independence

The Template Model is technology-independent.

It does not require:

* a specific programming language;
* a specific database;
* a specific markup language;
* a specific serialization format;
* a specific repository;
* a specific document editor;
* a specific automation platform.

Possible implementations may represent the model using different physical technologies while preserving the same conceptual semantics.

The implementation must therefore conform to the model rather than redefine the model according to implementation limitations.

---

# 18. Model Evolution

The Template Model is intended to support controlled evolution.

Future extensions may include:

* richer composition mechanisms;
* template inheritance;
* template specialization rules;
* parameterized structural generation;
* conditional structures;
* semantic template relationships;
* automated template derivation;
* template quality metrics;
* interoperability models;
* semantic impact analysis.

Such extensions must preserve the established model invariants and responsibility boundaries.

New concepts should be introduced only when existing concepts cannot adequately represent the required semantics.

---

# 19. Relationship to Subsequent Templates Documents

The Template Model provides the structural basis for the remaining Templates documentation sequence.

```text

            DF-TPL-003 Template Model
            │
            ├──────►  DF-TPL-004 Template Elements
            │
            ├──────►  DF-TPL-005 Template Schema
            │
            ├──────►  DF-TPL-006 Template Lifecycle
            │
            ├──────►  DF-TPL-007 Template Validation
            │
            ├──────►  DF-TPL-008 Template Governance
            │
            ├──────►  DF-TPL-009 Template Relationships
            │
            ├──────►  DF-TPL-010 Template Constraints
            │
            ├──────►  DF-TPL-011 Template Extensibility
            │
            ├──────►  DF-TPL-012 Template Best Practices
            │
            ├──────►  DF-TPL-013 Template Dictionary
            │
            ├──────►  DF-TPL-014 Template Specification
            │
            └──────►  DF-TPL-015 Template Examples

```

The subsequent documents refine the model without redefining its fundamental concepts.

---

# 20. Related Documents

* DF-RDM-040 — Templates Roadmap
* DF-ARC-007 — Component Documentation Structure
* DF-TPL-001 — Templates Architecture
* DF-TPL-002 — Template Concepts
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

---

# 21. Change History

| # | Date       | Author           | Type            | Document   | Description                           |
| - | ---------- | ---------------- | --------------- | ---------- | ------------------------------------- |
| 1 | 13/09/2026 | Arnaldo Figueira | Add New Content | DF-TPL-003 | Initial definition of Template Model. |

---

**End of Document**

---