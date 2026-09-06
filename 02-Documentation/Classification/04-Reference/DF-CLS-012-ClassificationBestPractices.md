# Documentation Framework

# DF-CLS-012 — Classification Best Practices

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-012 |
| **Title** | Classification Best Practices |
| **Family** | Classification |
| **Type** | Reference |
| **Component** | Classification |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

Classification provides the semantic organization through which documents are grouped into meaningful categories.

Within the Documentation Framework, Classification supports:

- organization;
- navigation;
- governance;
- discovery.

Classification is independent of the physical location of documents.

The Classification architecture therefore requires more than a formal model.

It also requires practices that preserve semantic clarity, structural consistency, maintainability and long-term architectural integrity.

Classification Best Practices defines recommended practices for designing, using, maintaining and evolving the Classification component.

This document is **informative**.

It provides guidance rather than introducing additional normative requirements beyond those established by the Classification architecture, constraints and specification.

---

# 2. Purpose

The purpose of Classification Best Practices is to provide practical guidance for maintaining a high-quality Classification architecture.

The practices defined here aim to:

- preserve semantic clarity;
- reduce unnecessary complexity;
- prevent semantic duplication;
- maintain structural coherence;
- improve discoverability;
- support governance;
- facilitate validation;
- support controlled evolution;
- preserve long-term maintainability.

---

# 3. Scope

This document applies to:

- Classification Families;
- Classification Types;
- Classification Classes;
- Classification Relationships;
- Classification Schema;
- Classification Dictionary;
- Classification Extensions;
- Classification maintenance;
- Classification evolution.

It does not replace:

- Classification Constraints;
- Classification Validation;
- Classification Governance;
- Classification Specification.

Where this document conflicts with a normative Classification document, the normative document takes precedence.

---

# 4. Nature of Best Practices

Best practices provide recommendations rather than independent architectural requirements.

The distinction is:

```text

       Classification Architecture
                    │
                    ▼

             Normative Rules
             │
             ├── Schema
             ├── Constraints
             ├── Lifecycle
             └── Specification
          
              Best Practices
                    │
                    ▼

       Recommended Ways of Applying
               Those Rules

```

Best practices should therefore guide decisions without creating an alternative Classification model.

---

# 5. Fundamental Principles

Classification should follow the architectural principles of the Documentation Framework.

In particular:

- Single Source of Truth;
- Semantic Consistency;
- Separation of Responsibilities;
- Modular Design;
- Explicit Relationships;
- Traceability;
- Incremental Evolution;
- Backward Compatibility;
- Technology Independence.

These principles apply to Classification because the architectural principles explicitly apply to all Framework components, including Classification.

---

# 6. Treat Classification as Knowledge Structure

Classification should be treated as a semantic structure rather than merely a filing mechanism.

A document's Classification should communicate something meaningful about the knowledge represented by that document.

The Framework defines documentation as a structured representation of knowledge and documents as coherent units of knowledge.

Therefore, Classification should answer questions such as:

- What kind of knowledge does this document represent?
- What role does the document play?
- What architectural context does it belong to?
- How does it relate to other classified knowledge?

---

# 7. Classify by Meaning

Classification should be based on semantic meaning rather than physical organization.

A document should not be classified according to:

- directory location;
- filename;
- repository;
- file extension;
- implementation technology.

The same principle that separates Classification from document location should be preserved in its application.

---

# 8. Avoid Classification by Appearance

Classification should not be based solely on superficial characteristics.

For example, documents should not be classified differently merely because they are:

- Markdown files;
- PDF files;
- source files;
- generated files.

The relevant question is what the document represents, not how it is physically represented.

---

# 9. Define Before Classifying

A Classification Element should be defined before it is broadly used.

The definition should establish its intended meaning and context.

A useful sequence is:

```text

               Requirement
                    │
                    ▼

                 Concept
                    │
                    ▼

                Definition
                    │
                    ▼

          Classification Element
                    │
                    ▼

                  Usage

```

This reduces the risk of Classification emerging implicitly from usage.

---

# 10. Prefer Existing Concepts

Before creating a new Classification Element, determine whether an existing element already represents the intended concept.

The preferred decision process is:

```text

             New Requirement
                    │
                    ▼

            Existing Element?
                    │
             ┌──────┴──────┐
             │             │
            Yes            No
             │             │
             ▼             ▼

           Reuse       Define New

```

This supports the Single Source of Truth principle, which requires each architectural concept to have one authoritative definition and discourages duplicated definitions.

---

# 11. Avoid Semantic Duplication

Do not introduce multiple Classification Elements merely because different authors use different terminology.

For example:

```text

    Architectural Decision
    Architecture Decision
    Architecture Design Decision

```

should not automatically become three distinct Classification Elements.

First determine whether they represent:

- the same concept;
- related concepts;
- genuinely distinct concepts.

---

# 12. Distinguish Synonyms from Concepts

Different names may refer to the same concept.

Where this occurs, the Classification Dictionary should identify the canonical terminology.

Classification should not encode vocabulary variation as semantic variation unless the concepts are genuinely different.

---

# 13. Prefer Precise Definitions

Classification definitions should be precise enough to distinguish the concept from neighboring concepts.

A useful definition should establish:

- what the concept represents;
- what it does not represent;
- its scope;
- its relationship to parent concepts.

---

# 14. Avoid Overly Broad Categories

A Classification Element should not become a generic container for unrelated concepts.

For example:

```text

    Miscellaneous
    Other
    General
    Various

```

should be avoided as canonical categories unless their semantic purpose is explicitly justified.

Broad categories reduce the information value of Classification.

---

# 15. Avoid Overly Narrow Categories

The opposite problem is excessive specialization.

A new Classification Element should provide meaningful semantic value.

Do not introduce a new category merely because two documents differ in a minor detail.

The goal is a useful semantic structure rather than maximum fragmentation.

---

# 16. Maintain Appropriate Granularity

Classification granularity should be consistent.

Conceptually:

```text

                Too Broad
                    │
                    ▼

            Useful Granularity
                    │
                    ▼

              Too Fragmented

```

The appropriate level depends on:

- the purpose of Classification;
- the information being represented;
- discovery requirements;
- governance requirements;
- maintenance cost.

---

# 17. Keep Hierarchy Meaningful

The hierarchy should communicate a meaningful specialization relationship.

For example:

```text

            Family
            │
            └── Type
                │
                └── Class

```

should represent meaningful semantic refinement.

A hierarchy should not exist merely because a tree structure is convenient.

---

# 18. Avoid Artificial Hierarchies

Do not create intermediate Classification Elements solely to make a tree deeper.

For example:

```text

            Family
            │
            └── Group
                │
                └── Category
                    │
                    └── Type
                        │
                        └── Class

```

is undesirable if the intermediate concepts have no independent semantic purpose.

---

# 19. Use Relationships Explicitly

When two concepts have a meaningful relationship that is not hierarchical, represent that relationship explicitly.

The Framework favors explicit relationships over implicit conventions.

For example:

```text

            Classification A
            │
            └── relatedTo  ─────►  Classification B

```

is preferable to encoding the relationship indirectly through:

- directory names;
- naming conventions;
- ordering;
- textual assumptions.

---

# 20. Do Not Abuse Hierarchy

Not every relationship should be represented through parent-child Classification.

A hierarchy implies structural semantics.

If two concepts are merely related, use an explicit relationship instead.

---

# 21. Keep Relationship Semantics Clear

Each relationship should have a clear meaning.

Avoid generic relationship names such as:

- linkedTo;
- associatedWith;
- connectedTo;

when a more precise semantic relationship is available.

---

# 22. Use Direction Consistently

Where relationships are directional, maintain a consistent direction.

For example:

```text

            Type
            │
            └── belongsTo  ─────►  Family

```

should not arbitrarily alternate with:

```text

            Family
            │
            └── belongsTo  ─────►  Type

```

unless both relationships have independently defined meanings.

---

# 23. Respect Cardinality

Classification usage should respect the cardinality defined by the Schema and Constraints.

If a Type belongs to exactly one Family, Classification assignments should not introduce multiple Families merely for convenience.

---

# 24. Preserve Identity

Classification Element identity should remain stable.

Renaming a Classification Element should not automatically imply the creation of a new conceptual element.

Identity and presentation should remain conceptually distinct.

---

# 25. Separate Name from Meaning

A Classification Element has a semantic identity that is broader than its displayed name.

A name may evolve for clarity while the underlying concept remains the same.

Conversely, changing the meaning of an element is an architectural change even if its name remains unchanged.

---

# 26. Use Stable Terminology

Canonical Classification terminology should be used consistently throughout:

- document metadata;
- Dictionary;
- Specification;
- validation;
- governance;
- examples.

The Framework explicitly requires architectural concepts to preserve their meaning and terminology to be used consistently.

---

# 27. Avoid Context-Dependent Meaning

A Classification Element should not mean different things depending on:

- the repository;
- the author;
- the directory;
- the tool;
- the document format.

Where contextual specialization is required, it should be explicitly represented.

---

# 28. Keep Classification Independent of Storage

Classification should remain valid if documents move between:

- directories;
- repositories;
- storage systems;
- documentation platforms.

The Classification model should describe the document's semantic role, not its physical location.

---

# 29. Keep Classification Independent of Format

A document should retain the same Classification when represented as:

```text

            Markdown
            │
            ├── PDF
            ├── HTML
            ├── YAML
            └── Other Representation

```

unless the represented knowledge itself has changed.

---

# 30. Avoid Tool-Driven Classification

Do not introduce Classification concepts merely because a particular tool requires them.

Tool limitations should be solved at the implementation or integration level whenever possible.

Classification should represent architectural knowledge.

---

# 31. Preserve Separation of Responsibilities

Classification should not assume responsibilities belonging to other components.

For example:

```text

            Classification
            │
            ├── defines semantic categories
            │
            └── does not define
                ├── permanent identity
                ├── physical storage
                ├── lifecycle workflow
                └── repository management

```

The Framework explicitly defines components as architectural building blocks with specific responsibilities.

---

# 32. Do Not Encode Lifecycle in Classification

Classification and lifecycle are different dimensions.

Avoid creating categories such as:

```text

    DraftDecision
    ApprovedDecision
    ArchivedDecision

```

when the distinction is actually lifecycle state.

Instead:

```text

            Classification
            │
            └── Decision

            Lifecycle
            │
            ├── Draft
            ├── Approved
            └── Archived

```

---

# 33. Do Not Encode Governance in Classification

Governance status should not normally become part of the Classification hierarchy.

For example:

```text

    ApprovedArchitecture
    RejectedArchitecture
    PendingArchitecture

```

may represent governance states rather than Classification concepts.

Such distinctions should be handled by Governance.

---

# 34. Do Not Encode Storage in Classification

Avoid categories based on physical storage:

```text

    GitDocuments
    DatabaseDocuments
    ArchiveDocuments
    LocalDocuments

```

unless storage itself is genuinely the semantic subject being classified.

---

# 35. Do Not Encode Ownership in Classification

Ownership and responsibility should not automatically become Classification categories.

For example:

```text

    TeamADocuments
    TeamBDocuments

```

should not replace semantic Classification where ownership is a separate concern.

---

# 36. Use Classification for Stable Semantic Dimensions

Classification is most useful when the classified dimension is relatively stable.

Good candidates include:

- document role;
- document kind;
- architectural purpose;
- knowledge category;
- specification type.

Transient attributes should normally remain outside Classification.

---

# 37. Keep Classification Small Enough to Understand

A Classification model should remain comprehensible.

The Framework favors modular architecture and independent components that can evolve separately.

A Classification model that cannot be understood by its maintainers becomes difficult to govern and validate.

---

# 38. Prefer Coherent Vocabulary

Classification terminology should form a coherent vocabulary.

Avoid mixing unrelated naming conventions such as:

```text

    ArchitectureDecision
    API-Doc
    DesignNotes
    TechnicalSpecificationDocument

```

without a clear semantic rationale.

Terminology should reflect the conceptual model rather than individual author preferences.

---

# 39. Use Consistent Naming

Classification Element names should follow a consistent naming convention.

Names should be:

- recognizable;
- unambiguous;
- stable;
- concise;
- semantically meaningful.

---

# 40. Avoid Abbreviations When Ambiguous

Abbreviations should be avoided when they reduce semantic clarity.

For example:

```text

    ADR
    ARC
    SPEC
    REF

```

may be useful in identifiers but should not automatically become ambiguous canonical Classification names.

---

# 41. Separate Identifier from Label

Where the architecture defines stable identifiers, distinguish:

```text

            Identifier
            │
            └── stable identity

            Label
            │
            └── human-readable name

```

This permits terminology improvements without unnecessarily changing identity.

---

# 42. Document Classification Intent

When introducing a new Classification Element, document why it exists.

The rationale should explain:

- the requirement;
- the semantic distinction;
- why existing elements are insufficient.

This improves future governance decisions.

---

# 43. Review Before Creating New Elements

Before introducing a new Family, Type or Class, review:

1. existing terminology;
2. existing definitions;
3. existing relationships;
4. existing hierarchy;
5. Classification Dictionary;
6. Classification Constraints.

This minimizes duplication and inconsistency.

---

# 44. Prefer Additive Evolution

When possible, extend Classification by adding new elements rather than redefining existing ones.

For example:

```text

            Existing Model
            │
            ├── Existing A
            ├── Existing B
            │
            └── New C

```

is generally preferable to changing the meaning of A or B.

This is consistent with the Framework's incremental evolution and backward compatibility principles.

---

# 45. Use Controlled Specialization

Specialization should be introduced when it improves semantic precision.

For example:

```text

            Document
            │
            └── Specification
            │
            └── Architecture Specification

```

may be appropriate if the specialized concept has an independently meaningful definition.

---

# 46. Avoid Premature Specialization

Do not create specialized categories merely because they might be useful in the future.

Classification should evolve in response to actual architectural requirements.

---

# 47. Evaluate Extension Impact

Before approving an extension, consider its impact on:

- Schema;
- Constraints;
- Relationships;
- Lifecycle;
- Validation;
- Governance;
- Dictionary;
- Specification;
- existing documents.

Classification Extensibility establishes controlled architectural review and impact analysis as part of extension evolution.

---

# 48. Preserve Backward Compatibility

Classification evolution should preserve existing interpretation whenever possible.

Conceptually:

```text

         Existing Classification
                    │
                    ▼

            New Classification
            │
            └── Existing Meaning Preserved

```

The Framework explicitly identifies backward compatibility as an architectural principle.

---

# 49. Deprecate Before Removing

When a Classification Element is no longer appropriate, prefer:

```text

                  Active
                    │
                    ▼

                Deprecated
                    │
                    ▼

                 Retired

```

rather than immediate deletion.

This preserves historical interpretation and supports controlled evolution.

---

# 50. Preserve Historical Meaning

Historical documents should remain understandable even after Classification evolves.

A newer Classification should not silently change the meaning of historical Classification assignments.

---

# 51. Maintain Traceability

Classification changes should remain traceable.

Traceability should allow maintainers to determine:

- what changed;
- why it changed;
- when it changed;
- which elements were affected;
- which governance decision authorized the change.

Traceability is an explicit architectural principle of the Framework.

---

# 52. Use Governance for Significant Changes

Significant Classification changes should pass through the Classification Governance process.

Examples include:

- new Family;
- structural hierarchy changes;
- new relationship types;
- changes to constraints;
- semantic redefinition;
- retirement of canonical concepts.

---

# 53. Validate Before Adoption

A proposed Classification change should be validated against:

- Schema;
- Constraints;
- Relationships;
- Lifecycle;
- existing Classification.

Validation verifies compliance with the Framework.

---

# 54. Keep Validation Deterministic

The same Classification structure should produce the same validation result under the same rules.

This improves:

- reproducibility;
- automation;
- governance;
- debugging;
- trust.

---

# 55. Use Automation Carefully

Automation should operate on the architectural Classification model rather than relying on accidental file characteristics.

The Framework explicitly defines Automation as operating on architectural concepts rather than individual files.

---

# 56. Do Not Let Automation Define Semantics

Automation may:

- validate;
- detect;
- generate;
- report;
- assist.

It should not silently create or redefine canonical Classification semantics.

Semantic decisions remain architectural decisions.

---

# 57. Keep Dictionary and Classification Aligned

The Classification Dictionary should reflect the authoritative vocabulary.

When a Classification Element changes, determine whether the Dictionary requires an update.

Avoid situations where:

```text

            Classification
                  ≠
              Dictionary

```

---

# 58. Keep Specification and Classification Aligned

The Classification Specification should describe the normative Classification architecture.

An approved Classification change should therefore be evaluated for its effect on the Specification.

---

# 59. Use Examples as Verification Aids

Examples should demonstrate:

- valid Classification;
- relationships;
- hierarchy;
- lifecycle;
- extension;
- common usage patterns.

Examples should not become an alternative source of normative definitions.

---

# 60. Distinguish Examples from Rules

A document example illustrates a rule.

It does not redefine the rule.

Therefore:

```text

            Specification
            │
            └── defines requirement

            Examples
            │
            └── demonstrate requirement

```

---

# 61. Review Classification Regularly

Classification should be periodically reviewed for:

- unused elements;
- duplicated concepts;
- ambiguous definitions;
- excessive fragmentation;
- obsolete categories;
- relationship inconsistencies.

Review supports long-term maintainability.

---

# 62. Monitor Classification Growth

Classification should evolve incrementally.

Rapid growth in the number of categories may indicate:

- inadequate conceptual boundaries;
- duplication;
- over-specialization;
- missing relationships;
- unclear responsibilities.

Growth should therefore be evaluated semantically rather than numerically alone.

---

# 63. Avoid Classification Inflation

Classification inflation occurs when increasingly small distinctions become independent canonical categories.

For example:

```text

            Document
            ├── TypeA
            ├── TypeA-1
            ├── TypeA-1a
            ├── TypeA-1a-v2
            └── TypeA-1a-v2-final

```

Such structures often represent lifecycle, versioning or implementation concerns rather than genuine semantic Classification.

---

# 64. Avoid Classification as a General Tagging System

Classification should not become an unrestricted collection of arbitrary labels.

Where the Framework requires independent dimensions, those dimensions should be represented through their appropriate architectural mechanisms.

Classification should remain coherent and governed.

---

# 65. Prefer Explicit Dimensions

If different semantic dimensions are required, do not force them into a single hierarchy.

For example:

```text

            Document
            ├── Classification
            │   │
            │   └── Specification
            │
            ├── Lifecycle
            │   │
            │   └── Approved
            │
            └── Relationship
                │
                └── Implements  ─────►  Architecture

```

Each mechanism expresses a different architectural dimension.

---

# 66. Keep Cross-Component Boundaries Clear

Classification interacts with other components but should not absorb their responsibilities.

The Framework architecture explicitly defines components as having distinct responsibilities and interacting through explicit architectural relationships.

---

# 67. Consider Discovery Requirements

Classification should support the ways in which knowledge needs to be discovered.

Useful Classification should help answer:

- What documents belong to this category?
- What documents serve this role?
- What documents represent this kind of knowledge?

---

# 68. Consider Navigation Requirements

Classification should make navigation meaningful.

Users should be able to move from a general Classification context toward more specific contexts without encountering arbitrary or unexplained branches.

---

# 69. Consider Governance Requirements

Classification should provide sufficient semantic distinction to support governance where necessary.

However, Governance state itself should not automatically become Classification.

---

# 70. Consider Knowledge Graph Integration

Classification relationships may contribute to the semantic network represented by the Knowledge Graph.

The Knowledge Graph supports navigation, dependency analysis, impact analysis and semantic discovery.

Classification should therefore avoid structures that obscure semantic relationships.

---

# 71. Prefer Explicit Semantics for Graph Integration

When Classification relationships are intended to participate in semantic discovery, their meanings should be explicit.

Ambiguous relationships reduce the quality of the resulting knowledge graph.

---

# 72. Preserve Component Independence

Classification should remain independently understandable.

It should not require knowledge of a specific:

- repository;
- implementation;
- automation tool;
- documentation platform.

This follows the Framework's layered and technology-independent architecture.

---

# 73. Use Modular Classification Design

Classification should be organized so that coherent areas can evolve without requiring unrelated changes elsewhere.

Modularity is an explicit architectural principle of the Framework.

---

# 74. Minimize Coupling

A Classification Element should depend only on concepts necessary to express its meaning.

Unnecessary dependencies increase the cost of evolution.

---

# 75. Preserve Cohesion

Related Classification concepts should remain conceptually coherent.

Unrelated concepts should not be grouped simply to reduce the number of categories.

---

# 76. Prefer Explicit Architecture

Classification decisions should be documented explicitly.

Avoid relying on conventions that are known only by maintainers.

The Framework explicitly requires architecture to be defined and documented rather than relying on implicit conventions.

---

# 77. Use a Single Authoritative Definition

A Classification concept should have one authoritative definition.

Other documents should reference that definition rather than reproducing competing definitions.

This directly follows the Single Source of Truth principle.

---

# 78. Keep Supporting Documentation Consistent

When a Classification Element changes, review:

- README;
- Dictionary;
- Specification;
- Examples;
- Validation rules;
- Constraints;
- related documents.

This avoids partial architectural evolution.

---

# 79. Review Before Baseline

Classification changes should be reviewed before becoming part of an architectural Baseline.

A Baseline represents an immutable snapshot and preserves architectural history.

---

# 80. Preserve Baseline Interpretation

Changes made after a Baseline should not retroactively alter the meaning of the Baseline.

Historical Classification should remain interpretable in the context in which the Baseline was created.

---

# 81. Recommended Classification Design Workflow

A practical workflow is:

```text

                     Requirement
                          │
                          ▼

                  Semantic Analysis
                          │
                          ▼

               Existing Concept Review
               │
               ├── Existing → Reuse
               │
               └── New
                    │
                    ▼

                Definition
                    │
                    ▼

           Structural Placement
                    │
                    ▼

            Relationship Analysis
                    │
                    ▼

           Constraint Analysis
                    │
                    ▼

                Validation
                    │
                    ▼

                Governance
                    │
                    ▼

         Canonical Classification

```

---

# 82. Recommended Review Questions

Before approving a Classification change, ask:

1. Does the concept already exist?
2. Is the semantic distinction clear?
3. Is the proposed name unambiguous?
4. Is the hierarchy meaningful?
5. Are the relationships explicit?
6. Are the cardinalities appropriate?
7. Does the change respect constraints?
8. Does it preserve existing meaning?
9. Does it affect lifecycle?
10. Does it affect validation?
11. Does it affect governance?
12. Does it affect the Dictionary?
13. Does it affect the Specification?
14. Does it preserve historical interpretation?
15. Is the extension necessary?

---

# 83. Common Anti-Patterns

The following patterns should generally be avoided.

## 83.1. Classification by Folder

Using directory structure as the semantic Classification.

## 83.2. Classification by File Type

Using file extension as Classification.

## 83.3. Classification by Lifecycle

Using lifecycle states as Classification categories.

## 83.4. Classification by Ownership

Using team or author ownership as the primary Classification.

## 83.5. Classification Duplication

Creating multiple elements for the same concept.

## 83.6. Classification Inflation

Creating excessive categories for minor distinctions.

## 83.7. Implicit Relationships

Encoding relationships only through naming or physical organization.

## 83.8. Tool-Driven Classification

Allowing implementation limitations to define semantic categories.

## 83.9. Silent Redefinition

Changing the meaning of an existing Classification Element without governance.

---

# 84. Classification Quality Indicators

A healthy Classification architecture should exhibit:

- clear definitions;
- consistent terminology;
- meaningful hierarchy;
- explicit relationships;
- low semantic duplication;
- controlled growth;
- stable identity;
- predictable validation;
- traceable evolution;
- clear governance.

---

# 85. Classification Smell Indicators

The following may indicate Classification degradation:

- many near-duplicate categories;
- categories with unclear definitions;
- frequent renaming without semantic rationale;
- hierarchy branches with no clear meaning;
- relationships encoded through filenames;
- categories representing lifecycle states;
- categories representing repositories;
- categories created solely for tooling;
- frequent exceptions to constraints;
- undocumented Classification decisions.

---

# 86. Maintenance Practices

Classification maintainers should periodically:

- review definitions;
- detect duplication;
- review relationships;
- verify constraints;
- review deprecated elements;
- inspect Classification growth;
- update Dictionary references;
- update Specification references;
- review examples.

---

# 87. Change Management Practices

Classification changes should be:

- explicit;
- justified;
- reviewed;
- validated;
- governed;
- documented;
- traceable.

Avoid making architectural Classification changes as incidental edits to unrelated documentation.

---

# 88. Extension Practices

When extending Classification:

1. Prefer additive changes.
2. Reuse existing concepts where possible.
3. Define the new concept explicitly.
4. Evaluate semantic duplication.
5. Evaluate structural impact.
6. Evaluate relationship impact.
7. Evaluate constraint impact.
8. Evaluate validation impact.
9. Preserve compatibility.
10. Obtain governance approval.

These practices complement the formal extension architecture defined by DF-CLS-011.

---

# 89. Deprecation Practices

When deprecating a Classification Element:

1. Record the reason.
2. Preserve the original definition.
3. Identify replacement concepts where applicable.
4. Preserve historical references.
5. Update the Dictionary.
6. Update the Specification where required.
7. Update examples.
8. Ensure validation handles the deprecated state correctly.

---

# 90. Retirement Practices

When retiring a Classification Element:

1. Verify that it is no longer required.
2. Identify historical dependencies.
3. Identify replacement concepts.
4. Preserve historical interpretation.
5. Record the governance decision.
6. Update affected documentation.
7. Update validation.
8. Update Dictionary and Specification where required.

---

# 91. Documentation Practices

Classification documentation should distinguish clearly between:

```text

            Architecture
            │
            └── what Classification is

            Specification
            │
            └── what Classification requires

            Best Practices
            │
            └── how Classification should preferably be applied

            Examples
            │
            └── how Classification may be used

```

This preserves the role of each document in the Classification documentation sequence.

---

# 92. Recommended Separation of Concerns

The Classification component should maintain the following separation:

```text

                 Concepts
                    │
                    ▼

                  Model
                    │
                    ▼

                 Elements
                    │
                    ▼

                  Schema
                    │
                    ▼

                Lifecycle
                    │
                    ▼

                Validation
                    │
                    ▼

                Governance
                    │
                    ▼

              Relationships
                    │
                    ▼

               Constraints
                    │
                    ▼

              Extensibility
                    │
                    ▼

              Best Practices
                    │
                    ▼

                Dictionary
                    │
                    ▼

              Specification
                    │
                    ▼

                 Examples

```

Each document addresses a different architectural concern rather than repeating the same material.

---

# 93. Recommended Decision Hierarchy

When making a Classification decision, use the following order:

```text

         Architectural Principles
                    │
                    ▼

       Classification Architecture
                    │
                    ▼

           Classification Model
                    │
                    ▼

          Classification Schema
                    │
                    ▼

        Classification Constraints
                    │
                    ▼

       Classification Specification
                    │
                    ▼

              Best Practices

```

Best Practices should support the architecture rather than override it.

---

# 94. Long-Term Maintainability

Classification should be designed for long-term maintenance.

This requires:

- stable terminology;
- stable identities;
- explicit semantics;
- controlled growth;
- traceable evolution;
- limited coupling;
- clear responsibility boundaries.

The Framework's conceptual model explicitly characterizes architectural concepts as clearly defined, independent, stable, reusable and explicit.

---

# 95. Simplicity

Classification should remain as simple as possible while satisfying its architectural purpose.

Simplicity does not mean minimizing the number of elements.

It means avoiding unnecessary concepts, relationships and structural complexity.

---

# 96. Reuse

Existing Classification concepts should be reused where their semantics already satisfy the requirement.

Reuse reduces:

- duplication;
- governance overhead;
- validation complexity;
- documentation complexity.

---

# 97. Explicitness

Important Classification semantics should be explicit.

Avoid requiring maintainers to infer meaning from:

- ordering;
- directory structure;
- naming conventions;
- historical knowledge.

---

# 98. Stability

Classification definitions should evolve slowly.

Frequent semantic changes reduce the reliability of:

- document metadata;
- discovery;
- governance;
- historical interpretation.

---

# 99. Evolution

Classification should nevertheless remain capable of controlled evolution.

The objective is:

```text

            Stable Core
            │
            ├── Controlled Extensions
            │
            ├── Controlled Deprecation
            │
            └── Controlled Refinement

```

rather than either uncontrolled change or architectural stagnation.

---

# 100. Best Practices Checklist

Before introducing or modifying Classification, verify:

### 100.1. Semantics

- [ ] The concept has a clear meaning.
- [ ] Existing concepts were reviewed.
- [ ] Semantic duplication was considered.
- [ ] The terminology is consistent.

### 100.2. Structure

- [ ] The hierarchy is meaningful.
- [ ] The structural position is appropriate.
- [ ] Artificial hierarchy was avoided.
- [ ] Granularity is appropriate.

### 100.3. Relationships

- [ ] Relationships are explicit.
- [ ] Relationship semantics are clear.
- [ ] Direction is consistent.
- [ ] Cardinality is respected.

### 100.4. Constraints

- [ ] Applicable constraints were reviewed.
- [ ] No constraint is silently overridden.
- [ ] New constraints are identified where necessary.

### 100.5. Lifecycle

- [ ] Lifecycle is kept separate from Classification.
- [ ] Deprecation is handled explicitly.
- [ ] Historical meaning is preserved.

### 100.6. Governance

- [ ] The change has an architectural rationale.
- [ ] Impact was considered.
- [ ] Governance requirements were identified.
- [ ] The change is traceable.

### 100.7. Documentation

- [ ] Dictionary impact was considered.
- [ ] Specification impact was considered.
- [ ] Examples remain valid.
- [ ] Related documents were reviewed.

### 100.8. Architecture

- [ ] Component responsibilities remain separated.
- [ ] Technology independence is preserved.
- [ ] Existing Classification remains compatible.
- [ ] The canonical Classification model remains coherent.

---

# 101. Summary

Classification Best Practices provides guidance for maintaining a coherent and useful Classification architecture.

The central principles are:

```text

             Clear Semantics
                    │
                    ▼

           Meaningful Structure
                    │
                    ▼

          Explicit Relationships
                    │
                    ▼

          Controlled Constraints
                    │
                    ▼

         Validated Classification
                    │
                    ▼

            Governed Evolution
                    │
                    ▼

        Stable Knowledge Structure

```

The most important practical rule is:

> Prefer the simplest Classification structure that clearly represents the intended semantics while preserving the architectural principles of the Documentation Framework.

Classification should therefore be:

- semantic rather than physical;
- explicit rather than implicit;
- coherent rather than fragmented;
- stable rather than volatile;
- reusable rather than duplicated;
- governed rather than arbitrary;
- extensible rather than rigid;
- technology independent.

---

# 102. Conformance

This document is informative.

Conformance to DF-CLS-012 means following its recommendations where appropriate.

Failure to follow a recommendation does not, by itself, constitute a Classification constraint violation.

Normative conformance is determined by the applicable:

- Classification Architecture;
- Classification Schema;
- Classification Constraints;
- Classification Lifecycle;
- Classification Specification;
- Governance decisions.

---

# 103. Related Documents

## 103.1. Foundation

- DF-FND-001 — Framework Manifest
- DF-FND-002 — Research Journal
- DF-FND-003 — Evolution Timeline
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

## 103.2. Architecture

- DF-ARC-001 — Architecture Overview
- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-004 — Architectural Layers
- DF-ARC-007 — Component Documentation Structure

## 103.3. Classification

- DF-CLS-001 — Classification Architecture
- DF-CLS-002 — Classification Concepts
- DF-CLS-003 — Classification Model
- DF-CLS-004 — Classification Elements
- DF-CLS-005 — Classification Schema
- DF-CLS-006 — Classification Lifecycle
- DF-CLS-007 — Classification Validation
- DF-CLS-008 — Classification Governance
- DF-CLS-009 — Classification Relationships
- DF-CLS-010 — Classification Constraints
- DF-CLS-011 — Classification Extensibility
- **DF-CLS-012 — Classification Best Practices**
- DF-CLS-013 — Classification Dictionary
- DF-CLS-014 — Classification Specification
- DF-CLS-015 — Classification Examples

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of Classification Best Practices. |

---

**End of Document**