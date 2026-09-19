# Documentation Framework

# DF-TPL-006 — Template Lifecycle

| Metadata        | Value                       |
| --------------- | --------------------------- |
| **Document ID** | DF-TPL-006                  |
| **Title**       | Template Lifecycle          |
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

This document defines the lifecycle of Templates within the Documentation Framework.

The Template Lifecycle establishes the conceptual states through which a Template may progress during its existence and the transitions between those states.

The lifecycle provides a controlled behavioral model for the evolution of Template definitions while preserving the separation between Template definition, Template usage, Template validation, and Template governance.

### 1.2. Scope

This document defines:

* the Template lifecycle model;
* Template lifecycle states;
* lifecycle transitions;
* state transition conditions;
* lifecycle termination;
* Template Version interaction with lifecycle;
* lifecycle relationship with Template Instances;
* lifecycle invariants.

This document does not define:

* validation algorithms;
* governance policies;
* approval workflows;
* repository operations;
* publication mechanisms;
* detailed constraint semantics;
* detailed relationship semantics;
* Template extensibility mechanisms.

Those concerns are addressed by the corresponding Templates component documents.

---

## 2. Lifecycle Position

The Template Lifecycle operates on the Template definition.

The primary distinction is:

```text

            Template Definition
            │
            ├── Lifecycle
            │
            ├── Version
            │
            ├── Structure
            │
            ├── Parameters
            │
            ├── Constraints
            │
            └── Relationships

```

The lifecycle therefore concerns the existence and evolution of a Template definition.

It does not represent the lifecycle of a document created from that Template.

```text

            Template Lifecycle
                    │
                    ▼

           Template Definition
                    │
                    ▼

            Template Instance
                    │
                    ▼

            Document Instance

```

The lifecycle of a Document Instance belongs to the appropriate document management and workflow responsibilities.

---

## 3. Lifecycle Objectives

The Template Lifecycle has the following objectives:

1. provide an explicit lifecycle model for Templates;
2. distinguish Templates at different stages of maturity;
3. control the transition of Templates between lifecycle states;
4. support controlled Template evolution;
5. distinguish active Templates from historical Templates;
6. preserve the relationship between Template Versions and lifecycle states;
7. prevent ambiguous interpretation of Template status;
8. provide a basis for governance and validation;
9. preserve Template traceability throughout its lifecycle;
10. remain independent of implementation technology.

---

## 4. Lifecycle Model

The abstract Template Lifecycle is:

```text

                  ┌─────────────┐
                  │    Draft    │
                  └──────┬──────┘
                         │
                         ▼

                  ┌─────────────┐
                  │   Defined   │
                  └──────┬──────┘
                         │
                         ▼

                  ┌─────────────┐
                  │    Active   │
                  └──────┬──────┘
                         │
               ┌─────────┴─────────┐
               │                   │
               ▼                   ▼

        ┌─────────────┐     ┌─────────────┐
        │  Deprecated │     │   Retired   │
        └──────┬──────┘     └─────────────┘
               │
               ▼

        ┌─────────────┐
        │   Retired   │
        └─────────────┘
```

The lifecycle represents conceptual states.

Concrete governance rules may impose additional conditions on transitions.

---

## 5. Lifecycle States

### 5.1. Draft

A Template is in the **Draft** state while its definition is under development.

A Draft Template may be incomplete.

Typical characteristics include:

* structure under development;
* elements under definition;
* parameters under definition;
* relationships under development;
* constraints under development;
* incomplete documentation.

A Draft Template is not assumed to be generally available for production use.

### 5.2. Defined

A Template is **Defined** when its structural definition has been established sufficiently to constitute a recognizable Template.

The Defined state indicates that the Template has progressed beyond initial drafting.

A Defined Template may still be subject to formal validation or governance activities.

The Defined state therefore does not, by itself, imply operational availability.

### 5.3. Active

A Template is **Active** when it is approved for its intended use within the applicable documentation context.

An Active Template may be used as the basis for Template Instances and document creation where the applicable policies permit such use.

The Active state represents the normal operational state of a Template.

### 5.4. Deprecated

A Template is **Deprecated** when it remains historically or technically relevant but is no longer the preferred Template for new use.

A Deprecated Template may remain available for:

* interpretation of existing documents;
* maintenance of existing Template Instances;
* historical reference;
* controlled migration;
* compatibility purposes.

Deprecation does not imply immediate removal.

### 5.5. Retired

A Template is **Retired** when it is no longer intended for normal use.

A Retired Template remains part of the historical Template record where preservation is required.

Retirement does not imply deletion.

A Retired Template may remain necessary to interpret documents or Template Instances created while it was Active.

---

## 6. Lifecycle Transitions

### 6.1. Draft to Defined

The transition:

```text

                  Draft
                    │
                    ▼

                 Defined

```

occurs when the Template definition has reached the level required to constitute a defined Template.

The transition does not itself imply approval for operational use.

### 6.2. Defined to Active

The transition:

```text

                 Defined
                    │
                    ▼

                 Active

```

occurs when the Template has satisfied the applicable requirements for operational use.

The detailed approval and governance conditions are defined outside the lifecycle model.

### 6.3. Active to Deprecated

The transition:

```text

                  Active
                    │
                    ▼

                Deprecated

```

occurs when a Template remains relevant but should no longer be selected as the preferred Template for new use.

Typical causes include:

* replacement by a newer Template;
* architectural evolution;
* improved Template design;
* changed documentation requirements;
* controlled migration to another Template.

### 6.4. Deprecated to Retired

The transition:

```text

                Deprecated
                    │
                    ▼

                 Retired

```

occurs when the Template is no longer intended for normal use and its operational role has ended.

Historical preservation may still be required.

### 6.5. Active to Retired

An Active Template may transition directly to Retired when circumstances require immediate termination of normal use.

Such a transition is expected to be exceptional and subject to applicable governance.

### 6.6. Deprecated to Active

A Deprecated Template may be restored to Active when it becomes appropriate for normal use again.

```text

                Deprecated
                    │
                    ▼

                  Active

```

This transition must preserve Template Version traceability.

### 6.7. Defined to Draft

A Defined Template may return to Draft when substantial changes are required before it can continue progressing through the lifecycle.

```text

                 Defined
                    │
                    ▼

                  Draft

```

This transition represents renewed development rather than lifecycle loss.

---

## 7. Lifecycle State Semantics

Lifecycle state and Template Version are related but distinct concepts.

```text

            Template
            │
            ├── Lifecycle State
            │
            └── Template Version

```

A Template Version identifies the version of the Template definition.

The lifecycle state identifies the current lifecycle condition of that definition.

For example:

```text

            Template A
            │
            ├── Version 1.0
            │
            └── State: Retired

            Template A
            │
            ├── Version 2.0
            │
            └── State: Active

```

A new Template Version does not automatically imply a lifecycle transition.

Likewise, a lifecycle transition does not inherently create a new Template Version.

The applicable versioning rules belong to the Template Version model.

---

## 8. Template Evolution

Template evolution may result in new Template Versions.

Conceptually:

```text

            Template
            │
            ├── Version 1
            │
            ├── Version 2
            │
            └── Version 3

```

Lifecycle states may apply to the evolving Template definition.

A common evolution pattern is:

```text

              Version 1
              │
              └── Active
                    │
                    ▼

                Deprecated

              Version 2
              │
              └── Draft
                    │
                    ▼

                 Defined
                    │
                    ▼

                  Active

```

This allows a newer Template Version to become Active while an earlier Version becomes Deprecated.

The lifecycle therefore supports controlled Template evolution without conflating versions with lifecycle states.

---

## 9. Template Lifecycle and Template Instances

A Template Instance may remain associated with a Template Version after that Template has changed lifecycle state.

For example:

```text

            Template Version 1
            │
            ├── Deprecated
            │
            └── Template Instances created previously

```

Deprecating or retiring a Template does not inherently invalidate existing Template Instances.

This distinction is important for historical documents and traceability.

An existing document may therefore remain associated with:

```text

            Document
            │
            └── Template
                │
                └── Template Version
                    │
                    └── Historical lifecycle state

```

The Templates component preserves the structural relationship.

Document management and preservation policies determine how such historical instances are handled operationally.

---

## 10. Lifecycle and Validation

Lifecycle and validation are separate responsibilities.

The lifecycle may define that a Template must satisfy applicable conditions before entering the Active state.

However, the lifecycle does not define how those conditions are evaluated.

The separation is:

```text

            Template Lifecycle
                    │
        defines transition context
                    │
                    ▼

           Template Validation
                    │
          evaluates conformance
                    │
                    ▼

            Validation Result

```

DF-TPL-007 — Template Validation defines validation behavior.

---

## 11. Lifecycle and Governance

Lifecycle states provide the behavioral structure required for governance, but they do not define governance policies.

For example:

```text

                 Defined
                    │
           governance decision
                    │
                    ▼

                  Active

```

The lifecycle identifies the transition.

Governance defines:

* who may authorize it;
* what evidence is required;
* what approvals are necessary;
* what records must be preserved.

These responsibilities belong to DF-TPL-008 — Template Governance.

---

## 12. Lifecycle and Constraints

Template constraints may influence whether a Template can transition to a subsequent lifecycle state.

However, constraint semantics remain separate from lifecycle behavior.

```text

            Template
            │
            ├── Constraints
            │
            └── Lifecycle

```

DF-TPL-010 — Template Constraints defines constraint semantics.

The lifecycle only consumes the applicable result or condition; it does not redefine constraint meaning.

---

## 13. Lifecycle and Relationships

A Template may have relationships with other Templates during its lifecycle.

Examples include:

```text

            Template A
            │
            └── specializes  ─────►  Template B

            Template A
            │
            └── replaces  ─────►  Template B

```

The lifecycle does not define the semantics of these relationships.

Relationship semantics belong to DF-TPL-009 — Template Relationships.

---

## 14. Lifecycle Invariants

The following invariants apply to the Template Lifecycle.

### 14.1. State Invariant

A Template has one applicable lifecycle state at a given point in its lifecycle.

### 14.2. Transition Invariant

A lifecycle state change occurs through a defined lifecycle transition.

### 14.3. Traceability Invariant

Lifecycle transitions must not destroy the historical identity of the Template or its Versions.

### 14.4. Version Separation Invariant

Lifecycle state and Template Version remain distinct concepts.

### 14.5. Instance Preservation Invariant

Changing the lifecycle state of a Template does not inherently invalidate existing Template Instances.

### 14.6. Historical Preservation Invariant

Retired Templates remain preservable when required for historical interpretation or traceability.

### 14.7. Responsibility Invariant

The lifecycle does not assume responsibility for validation, governance, storage, workflow, or document management.

### 14.8. Technology Independence Invariant

The lifecycle model remains independent of implementation technology.

---

## 15. Lifecycle Termination

Retirement represents the normal terminal state of a Template lifecycle.

```text

         Retired
            │
            ✘

```

A Retired Template is not normally returned to operational use.

If a previously Retired Template becomes necessary again, the preferred approach is normally to create or derive an appropriate new Template Version or Template definition rather than silently reversing its historical retirement.

Any exceptional reactivation must preserve historical traceability.

---

## 16. Lifecycle Independence

The Template Lifecycle is independent of:

* file-system organization;
* repository organization;
* storage technology;
* serialization format;
* programming language;
* document publication mechanism;
* document workflow implementation.

The lifecycle defines conceptual Template behavior only.

---

## 17. Lifecycle Summary

The Template Lifecycle can be summarized as:

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

With controlled alternative transitions:

```text

    Defined     ─────►  Draft

    Deprecated  ─────►  Active

    Active      ─────►  Retired

```

The lifecycle provides:

* explicit Template states;
* controlled state transitions;
* distinction between operational and historical Templates;
* separation between lifecycle and version;
* preservation of historical Template usage;
* a behavioral basis for validation and governance.

---

## 18. Related Documents

### 18.1. Templates Component

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

### 18.2. Related Components

* Metadata
* Document Identity
* Classification
* Workflow
* Baselines

---

## 19. Change History

| # | Date       | Author           | Type            | Document   | Description                            |
| - | ---------- | ---------------- | --------------- | ---------- | -------------------------------------- |
| 1 | 2026-09-19 | Arnaldo Figueira | Add New Content | DF-TPL-006 | Initial Template Lifecycle definition. |

---

**End of Document**

---