# Documentation Framework

# DF-TPL-005 — Template Schema

| Metadata        | Value                        |
| --------------- | ---------------------------- |
| **Document ID** | DF-TPL-005                   |
| **Title**       | Template Schema              |
| **Family**      | Templates                    |
| **Type**        | Component Structure Document |
| **Component**   | Templates                    |
| **Author**      | Arnaldo Figueira             |
| **Status**      | Draft                        |
| **Version**     | 1.0                          |
| **Revision**    | 0                            |
| **Baseline**    | 1.0                          |
| **Language**    | English                      |
| **Date**        | 2026-09-18                   |

---

## 1. Introduction

### 1.1. Purpose

This document defines the **Template Schema** of the Documentation Framework.

The Template Schema provides the structural representation required to describe a Template according to the concepts and relationships defined by the Templates component.

It establishes how a Template, its structural components, and their associations are represented at schema level.

The Template Schema is technology-independent and does not prescribe a particular serialization format, implementation technology, storage mechanism, or repository structure.

### 1.2. Scope

This document defines the structural schema for:

* Templates;
* Template Types;
* Template Structures;
* Template Sections;
* Template Elements;
* Template Parameters;
* Template Constraints;
* Template Relationships;
* Template Versions;
* structural references between Template components;
* structural representation of Template composition;
* structural representation of Template specialization;
* structural representation of Template Instances.

This document does not define the detailed semantics of:

* Template lifecycle;
* Template validation;
* Template governance;
* Template relationships;
* Template constraints;
* Template extensibility.

Those concerns are defined by the corresponding Templates component documents.

### 1.3. Schema Position

The Template Schema is the structural representation of the Template Model.

The conceptual progression is:

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
            ├───▶  Template Lifecycle
            │
            ├───▶  Template Validation
            │
            ├───▶  Template Governance
            │
            ├───▶  Template Relationships
            │
            ├───▶  Template Constraints
            │
            └───▶  Template Extensibility

```

The distinction is therefore:

| Level             | Responsibility                                                  |
| ----------------- | --------------------------------------------------------------- |
| **Concepts**      | Defines what Template concepts mean                             |
| **Model**         | Defines conceptual entities and their relationships             |
| **Elements**      | Defines the categories and characteristics of Template Elements |
| **Schema**        | Defines their structural representation                         |
| **Validation**    | Determines whether representations conform                      |
| **Governance**    | Defines controlled management                                   |
| **Relationships** | Defines relationship semantics                                  |
| **Constraints**   | Defines constraint semantics                                    |
| **Extensibility** | Defines extension mechanisms                                    |

---

## 2. Schema Objectives

The Template Schema has the following objectives:

1. provide a consistent representation of Templates;
2. represent Template structures explicitly;
3. preserve the semantics defined by the Template Model;
4. provide explicit structural relationships between Template components;
5. support reusable Template structures;
6. support Template composition;
7. support Template specialization;
8. support parameterized Templates;
9. represent applicable constraints without defining their evaluation;
10. represent applicable relationships without defining their detailed semantics;
11. distinguish Template definitions from Template Instances;
12. distinguish Template Versions from document identity and revision;
13. remain independent of implementation technology;
14. provide a stable structural basis for validation and governance.

---

## 3. Template Schema Model

### 3.1. Root Structure

The Template Schema is rooted in the Template entity.

```text

            TemplateSchema
            │
            └── Template
                │
                ├── TemplateType
                │
                ├── TemplateStructure
                │
                ├── TemplateParameters
                │
                ├── TemplateConstraints
                │
                ├── TemplateRelationships
                │
                └── TemplateVersion

```

The Template Structure contains the structural organization of the Template.

```text

            Template
            │
            └── TemplateStructure
                │
                └── TemplateSection
                    │
                    └── TemplateElement

```

### 3.2. Abstract Schema

The complete abstract representation can be expressed as:

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
            └── Version

```

This representation describes the structural organization of a Template and does not prescribe a concrete implementation syntax.

---

## 4. Template Schema Components

### 4.1. Template

The Template is the root entity of the schema.

Its structural representation identifies the Template and associates it with:

* a Template Type;
* a Template Structure;
* zero or more Template Parameters;
* zero or more Template Constraints;
* zero or more Template Relationships;
* a Template Version.

```text

            Template
            │
            ├── Type
            │
            ├── Structure
            │
            ├── Parameters     [0..*]
            │
            ├── Constraints    [0..*]
            │
            ├── Relationships  [0..*]
            │
            └── Version

```

### 4.2. Template Type

A Template Type identifies the conceptual type of a Template.

The schema references the applicable Template Type.

It does not redefine Template Type semantics.

```text

            Template
            │
            └── TemplateType

```

### 4.3. Template Structure

Template Structure defines the organization of the Template.

```text

            Template
            │
            └── TemplateStructure
                │
                └── TemplateSections

```

Template Structure is conceptual.

It does not represent:

* a directory;
* a file-system hierarchy;
* a repository;
* a database schema;
* a storage structure.

### 4.4. Template Section

A Template Section represents a logical subdivision of a Template Structure.

```text

            TemplateSection
            │
            ├── Identifier
            │
            ├── Name
            │
            ├── Position
            │
            ├── Applicability
            │
            └── Elements

```

A Section may contain zero or more Template Elements according to the applicable Template definition.

### 4.5. Template Element

A Template Element represents an individual component of a Template Structure.

The Element categories established by DF-TPL-004 are:

```text

            TemplateElement
            │
            ├── StructuralElement
            │
            ├── ContentElement
            │
            ├── ReferenceElement
            │
            ├── MetadataElement
            │
            ├── IdentityElement
            │
            ├── ClassificationElement
            │
            ├── ParameterizedElement
            │
            └── ReusableElement

```

The schema identifies the applicable Element category and represents the properties required for its structural position.

The schema does not redefine the semantics of these categories.

---

## 5. Structural Representation

### 5.1. Containment

The principal structural containment hierarchy is:

```text

            Template
            │
            └── Structure
                │
                └── Section
                    │
                    └── Element

```

Containment establishes structural membership.

It does not imply:

* physical containment;
* storage ownership;
* repository ownership;
* document ownership.

### 5.2. Structural References

Not every relationship between Template entities is represented through containment.

Entities may therefore be connected through explicit references.

```text

Template
    │
    ├── Structure
    │
    └── References
          │
          └── Target Entity

```

References must identify the intended schema entity without depending on physical storage location.

---

## 6. Template Section Schema

A Section is represented by a structural definition containing the information necessary to identify and position the Section.

Abstract representation:

```text

            TemplateSection
            │
            ├── Identifier
            │
            ├── Name
            │
            ├── Position
            │
            ├── Applicability
            │
            └── Elements

```

### 6.1. Identifier

The Section Identifier distinguishes the Section within its applicable Template Structure.

### 6.2. Name

The Section Name provides the human-readable name of the Section.

### 6.3. Position

Position represents the Section's structural ordering when ordering applies.

### 6.4. Applicability

Applicability identifies whether and under which conditions the Section participates in the Template structure.

Detailed applicability semantics are outside the scope of this schema document.

### 6.5. Elements

Elements represent the components contained by the Section.

---

## 7. Template Element Schema

A Template Element is structurally represented according to its category and applicable properties.

Abstract representation:

```text

            TemplateElement
            │
            ├── Category
            │
            ├── Identifier
            │
            ├── Name
            │
            ├── Position
            │
            ├── Occurrence
            │
            ├── Applicability
            │
            ├── Content
            │
            ├── Parameters
            │
            ├── Constraints
            │
            └── Relationships

```

Not every property is applicable to every Element.

The applicable representation is determined by the Element category and Template definition.

### 7.1. Element Category

The category identifies the structural role of the Element.

### 7.2. Identifier

The Element Identifier provides a stable reference within the Template Schema.

### 7.3. Name

The Element Name provides the human-readable name of the Element.

### 7.4. Position

Position represents the Element's structural order within its parent structure when ordering applies.

### 7.5. Occurrence

Occurrence represents the permitted number of occurrences of the Element.

### 7.6. Applicability

Applicability identifies whether the Element participates in the Template Structure and, where applicable, the conditions under which it applies.

### 7.7. Content

Content represents the content definition associated with a Content Element or another Element for which content is applicable.

The schema does not prescribe a concrete content format.

---

## 8. Ordering Representation

Ordering represents the relative structural position of Sections and Elements.

Example:

```text

            Template Structure
            │
            ├── Section A  [Position 1]
            │
            ├── Section B  [Position 2]
            │
            └── Section C  [Position 3]

```

Within a Section:

```text

            Section
            │
            ├── Element A  [Position 1]
            │
            ├── Element B  [Position 2]
            │
            └── Element C  [Position 3]

```

Ordering is semantic structural information.

It must not be interpreted as:

* file-system order;
* directory order;
* serialization order;
* database record order.

A concrete implementation may serialize components in another order provided that the defined structural ordering remains recoverable.

---

## 9. Occurrence Representation

Occurrence defines the allowed number of instances of a structural component.

Abstract representation:

```text

            Occurrence
            │
            ├── Minimum
            │
            └── Maximum

```

Occurrence may represent:

* mandatory components;
* optional components;
* repeated components;
* bounded repetition;
* unbounded repetition.

Examples:

```text

    Required:
        Minimum = 1
        Maximum = 1

    Optional:
        Minimum = 0
        Maximum = 1

    Repeated:
        Minimum = 0
        Maximum = *

```

These examples illustrate structural representation only.

Detailed occurrence constraint semantics belong to the Template Constraints documentation.

---

## 10. Parameter Schema

A Template Parameter represents controlled variation within a Template.

The schema represents the parameter definition.

```text

            Template
            │
            └── TemplateParameter
                │
                ├── Name
                │
                ├── Definition
                │
                ├── Applicability
                │
                └── Constraints

```

The distinction between definition and value is maintained:

```text

            Template Schema
            │
            └── Parameter Definition
                        │
                        ▼

                Template Instance
                │
                └── Parameter Value

```

The Template Schema therefore defines what may vary without defining the concrete value selected for a particular Template Instance.

The schema does not prescribe a programming-language type system or parameter implementation.

---

## 11. Constraint Representation

The Template Schema represents constraints as associations between a constraint definition and its target.

Abstract representation:

```text

            TemplateConstraint
            │
            ├── Target
            │
            └── Definition

```

Possible targets include:

```text

Template
Section
Element
Parameter
Relationship

```

The schema establishes where a constraint applies.

It does not define:

* constraint semantics;
* constraint evaluation;
* validation algorithms;
* validation results;
* enforcement mechanisms.

Those concerns are defined by DF-TPL-010 and DF-TPL-007.

---

## 12. Relationship Representation

The Template Schema represents relationships independently from structural containment.

Abstract representation:

```text

            TemplateRelationship
            │
            ├── Source
            │
            ├── Target
            │
            └── Definition

```

This permits a relationship to connect entities that do not have a parent-child relationship.

For example:

```text

            Template A
            │
            └── relationship  ─────►  Template B

```

or:

```text

            Element A
            │
            └── relationship  ─────►  Element B

```

The schema defines the structural representation of the association.

Detailed relationship semantics and relationship categories are defined by DF-TPL-009.

---

## 13. Template Composition Representation

Template Composition permits a Template Structure to incorporate reusable structures from another Template or reusable Template component.

Abstract representation:

```text

            Template A
            │
            └── Structure
                │
                └── Composition Reference
                              │
                              ▼

                     Template B Structure

```

The schema represents the composition reference and its structural position.

It does not define:

* composition resolution algorithms;
* composition conflict resolution;
* composition precedence;
* implementation mechanisms.

Those concerns belong to the applicable Templates behavior and extensibility documentation.

---

## 14. Template Specialization Representation

Template Specialization represents a Template derived from another Template while preserving the conceptual relationship between them.

Abstract representation:

```text

              Base Template

                    ▲
                    │
               specializes
                    │
           Specialized Template

```

The schema represents the reference to the specialized Template's source Template.

Specialization does not imply that the specialized Template is a new unrelated Template.

Detailed specialization rules are addressed by the Templates component's extensibility model.

---

## 15. Template Version Representation

The schema identifies the Template Version associated with the represented Template definition.

Abstract representation:

```text

            Template
            │
            └── TemplateVersion
                │
                └── VersionIdentifier

```

Template Version represents the evolution state of the Template definition.

It is distinct from:

```text

    Template Version
           !=
    Document Identity

    Template Version
           !=
    Document Revision

    Template Version
           !=
    Document Edition

    Template Version
           !=
        Baseline

```

A document created using a particular Template Version retains its own Document Identity independently of the Template Version.

---

## 16. Template Instance Representation

A Template Instance represents a concrete application of a Template.

The structural relationship is:

```text

                 Template
                    │
                    ▼

             Template Schema
                    │
                    ▼

            Template Instance

```

A Template Instance may contain concrete:

* content;
* parameter values;
* structural occurrences;
* applicable sections;
* applicable elements.

The Template Instance must remain distinguishable from the Template definition.

```text

           Template Definition
                    │
            defines structure
                    │
                    ▼

            Template Instance
                    │
          represents application
                    │
                    ▼

            Document Instance

```

The Templates component does not assign Document Identity to the resulting Document Instance.

---

## 17. Schema Conformance Representation

The Template Schema provides the structural basis against which a Template Instance may be evaluated for conformance.

At schema level, conformance concerns include:

* structural components corresponding to the Template definition;
* references resolving to defined entities;
* Sections occurring within their applicable structures;
* Elements occurring within their applicable Sections;
* ordering information being structurally consistent;
* occurrence information being represented;
* parameter references resolving to defined parameters;
* relationship references identifying their participants.

These are structural conditions.

The determination of whether a concrete Template Instance conforms is the responsibility of Template Validation.

---

## 18. Schema Invariants

The following invariants apply to the Template Schema.

### 18.1. Template Root Invariant

Every Template Schema has one Template as its root conceptual entity.

### 18.2. Structure Invariant

Every represented Section belongs to a Template Structure.

### 18.3. Element Context Invariant

Every represented Element has a defined structural context.

### 18.4. Reference Resolution Invariant

Every schema reference identifies a resolvable schema entity.

### 18.5. Parameter Resolution Invariant

Every parameter reference corresponds to a defined Template Parameter.

### 18.6. Relationship Invariant

Every represented relationship identifies its participating entities.

### 18.7. Occurrence Invariant

Occurrence information is associated with the structural component to which it applies.

### 18.8. Version Invariant

Every Template Schema identifies the Template Version represented by the schema.

### 18.9. Semantic Preservation Invariant

The schema representation must preserve the semantics established by the Template Model.

### 18.10. Responsibility Invariant

The Template Schema must not assume responsibility for concepts owned by other Documentation Framework components.

### 18.11. Technology Independence Invariant

The schema must remain independent of any particular implementation technology, serialization format, repository, or storage mechanism.

---

## 19. Schema and Other Templates Documents

The Template Schema has a defined boundary with the other Templates component documents.

| Document                                | Relationship with Template Schema                        |
| --------------------------------------- | -------------------------------------------------------- |
| **DF-TPL-002 — Template Concepts**      | Provides the concepts represented by the schema          |
| **DF-TPL-003 — Template Model**         | Provides the conceptual model represented by the schema  |
| **DF-TPL-004 — Template Elements**      | Defines the Element categories represented by the schema |
| **DF-TPL-006 — Template Lifecycle**     | Defines lifecycle behavior of Templates                  |
| **DF-TPL-007 — Template Validation**    | Defines conformance evaluation                           |
| **DF-TPL-008 — Template Governance**    | Defines governance                                       |
| **DF-TPL-009 — Template Relationships** | Defines relationship semantics                           |
| **DF-TPL-010 — Template Constraints**   | Defines constraint semantics                             |
| **DF-TPL-011 — Template Extensibility** | Defines extension mechanisms                             |
| **DF-TPL-014 — Template Specification** | Provides the complete normative specification            |

This separation prevents the Template Schema from becoming a substitute for the other component documents.

---

## 20. Schema Independence

The Template Schema is independent of physical documentation organization.

It does not define:

* component directories;
* document directories;
* repository locations;
* file names;
* storage systems;
* publication locations;
* synchronization mechanisms.

It is also independent of document representation formats.

A Template Schema may therefore be mapped to different technical representations without changing the conceptual Template Model.

---

## 21. Schema Evolution

Template Schema evolution must preserve the established Template concepts and model.

Schema evolution may introduce:

* additional structural properties;
* additional Element representations;
* additional reusable structures;
* additional parameter representations;
* additional relationship representations;
* additional composition representations.

Evolution must not silently redefine established concepts.

Changes affecting lifecycle, validation, governance, relationships, constraints, or extensibility must remain within their respective architectural responsibilities.

---

## 22. Related Documents

### 22.1. Templates Component

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

### 22.2. Framework Architecture

* DF-ARC-007 — Component Documentation Structure

### 22.3. Related Components

* Metadata
* Document Identity
* Classification

---

## 23. Change History

| # | Date       | Author           | Type            | Document   | Description                         |
| - | ---------- | ---------------- | --------------- | ---------- | ----------------------------------- |
| 1 | 2026-09-18 | Arnaldo Figueira | Add New Content | DF-TPL-005 | Initial Template Schema definition. |

