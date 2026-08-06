# Documentation Framework

# DF-MTD-012 — Metadata Best Practices

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-MTD-012 |
| **Title** | Metadata Best Practices |
| **Family** | Metadata |
| **Type** | Best Practices |
| **Component** | Metadata |
| **Author** | Arnaldo Figueira |
| **Status** | Draft |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Introduction

The Documentation Framework defines the architecture of Metadata through principles, concepts, models, schemas and specifications.

This document complements those normative specifications by providing architectural recommendations that promote consistency, maintainability and long-term interoperability.

The practices described herein are advisory rather than normative.

They represent recommended approaches for designing, extending and managing Metadata within the Documentation Framework.

---

# 2. Purpose

The purpose of this document is to provide architectural guidance for the effective use of the Metadata component.

It promotes:

- architectural consistency;
- semantic clarity;
- maintainability;
- interoperability;
- long-term stability.

---

# 3. Scope

This document provides recommendations for:

- Metadata design;
- Metadata evolution;
- Metadata organization;
- Metadata governance;
- Metadata maintenance.

It does not define mandatory architectural requirements.

Normative requirements are defined by the Metadata Specification and related architectural documents.

---

# 4. Guiding Principles

The following principles should guide every Metadata design decision.

## 4.1. Prefer Simplicity

Metadata should remain as simple as possible while fulfilling its intended purpose.

Avoid unnecessary complexity.

---

## 4.2. Preserve Semantic Clarity

Every Metadata Element should possess one explicit and easily understandable meaning.

Avoid ambiguous terminology.

---

## 4.3. Promote Reuse

Existing Metadata Elements should be reused whenever possible.

Introducing new Metadata should always be justified.

---

## 4.4. Maintain Consistency

Metadata should remain consistent throughout the Documentation Framework.

Similar concepts should be described in similar ways.

---

## 4.5. Design for Evolution

Metadata should be designed with future extension in mind.

Avoid designs that unnecessarily restrict future architectural evolution.

---

# 5. Metadata Design Practices

## 5.1. BP-001 — Design Around Concepts

Design Metadata around architectural concepts rather than implementation requirements.

Metadata should describe information, not software.

---

## 5.2. BP-002 — Prefer Atomic Elements

Each Metadata Element should represent one concept only.

Atomic Metadata is easier to understand, validate and reuse.

---

## 5.3. BP-003 — Avoid Composite Semantics

Do not combine multiple concepts within a single Metadata Element.

Instead, define multiple independent Metadata Elements.

---

## 5.4. BP-004 — Use Stable Terminology

Metadata names should remain stable over time.

Frequent renaming should be avoided.

---

## 5.5. BP-005 — Document Every Metadata Element

Every Metadata Element should be documented within the Metadata Dictionary.

Undocumented Metadata should not become part of the canonical architecture.

---

# 6. Metadata Organization Practices

## 6.1. BP-006 — Group Related Metadata

Organize Metadata Elements into logical Metadata Groups.

Groups improve readability without changing semantics.

---

## 6.2. BP-007 — Avoid Redundant Metadata

Do not define Metadata that duplicates existing architectural concepts.

---

## 6.3. BP-008 — Prefer Canonical Metadata

Always use canonical Metadata Elements whenever they satisfy the required purpose.

Extensions should only be introduced when necessary.

---

## 6.4. BP-009 — Keep Profiles Focused

Metadata Profiles should contain only the Metadata required for their intended document category.

Avoid overly generic profiles.

---

# 7. Metadata Evolution Practices

## 7.1. BP-010 — Prefer Extension over Modification

Introduce new Metadata through controlled extensions instead of modifying existing Metadata.

---

## 7.2. BP-011 — Preserve Compatibility

Whenever possible, Metadata evolution should preserve compatibility with existing Metadata Profiles and Metadata Instances.

---

## 7.3. BP-012 — Deprecate Before Removal

Metadata should be deprecated before being retired.

Immediate removal should be avoided.

---

## 7.4. BP-013 — Preserve Historical Information

Historical Metadata should remain documented to support long-term traceability.

---

# 8. Metadata Governance Practices

## 8.1. BP-014 — Review Architectural Impact

Every Metadata change should be evaluated for its architectural impact before approval.

---

## 8.2. BP-015 — Avoid Responsibility Creep

Metadata should not absorb responsibilities belonging to other Documentation Framework components.

---

## 8.3. BP-016 — Preserve Architectural Boundaries

Maintain clear separation between:

- Metadata;
- Validation;
- Governance;
- Workflow;
- Relationships;
- Document Identity.

---

## 8.4. BP-017 — Record Architectural Decisions

Significant Metadata decisions should be documented to preserve architectural rationale.

---

# 9. Metadata Validation Practices

## 9.1. BP-018 — Validate Early

Metadata should be validated as early as practical during document creation.

---

## 9.2. BP-019 — Separate Validation from Governance

Validation should determine architectural compliance.

Governance should determine architectural acceptance.

The two responsibilities should remain independent.

---

## 9.3. BP-020 — Validate Against Profiles

Metadata should always be validated against the applicable Metadata Profile.

---

# 10. Metadata Documentation Practices

## 10.1. BP-021 — Maintain a Complete Dictionary

Every canonical Metadata Element should appear in the Metadata Dictionary.

---

## 10.2. BP-022 — Keep Documentation Synchronized

Metadata documentation should evolve together with the Metadata architecture.

---

## 10.3. BP-023 — Document Deprecation

Deprecation should include:

- reason;
- replacement;
- compatibility considerations.

---

## 10.4. BP-024 — Preserve Traceability

Changes to Metadata should remain traceable throughout the Metadata Lifecycle.

---

# 11. Architectural Anti-Patterns

The following practices should be avoided.

## 11.1. AP-001 — Semantic Overloading

One Metadata Element representing multiple concepts.

---

## 11.2. AP-002 — Duplicate Metadata

Different Metadata Elements representing the same concept.

---

## 11.3. AP-003 — Technology-Driven Metadata

Metadata designed around implementation technologies instead of architectural concepts.

---

## 11.4. AP-004 — Profile Fragmentation

Creating numerous Metadata Profiles with insignificant differences.

---

## 11.5. AP-005 — Uncontrolled Extensions

Introducing Metadata outside the governance process.

---

## 11.6. AP-006 — Hidden Semantics

Embedding architectural meaning in naming conventions or implementation details instead of explicit Metadata definitions.

---

# 12. Relationship with Other Metadata Documents

This document complements the normative Metadata specifications.

| Document | Relationship |
|----------|--------------|
| Metadata Architecture | Defines architectural vision. |
| Metadata Concepts | Defines conceptual foundations. |
| Metadata Model | Defines conceptual organization. |
| Metadata Schema | Defines structural organization. |
| Metadata Validation | Defines validation principles. |
| Metadata Governance | Defines governance responsibilities. |
| Metadata Extensibility | Defines controlled evolution. |
| Metadata Specification | Defines normative requirements. |

Best Practices provide guidance for applying these specifications effectively.

---

# 13. Architectural Characteristics

Metadata Best Practices possess the following characteristics.

## 13.1. Advisory

Recommendations rather than mandatory rules.

---

## 13.2. Architecture-Oriented

Focused on preserving architectural quality.

---

## 13.3. Technology Independent

Applicable regardless of implementation technologies.

---

## 13.4. Evolvable

May evolve as the Documentation Framework matures.

---

## 13.5. Complementary

Support, but do not replace, normative specifications.

---

## 13.6. Reusable

Applicable across all Metadata implementations.

---

# 14. Conformance

Conformance with the Documentation Framework does not require adherence to every Best Practice.

However, implementations following these recommendations are more likely to achieve:

- higher architectural consistency;
- improved maintainability;
- better interoperability;
- greater long-term stability.

---

# 15. Related Documents

## 15.1. Architecture

- DF-ARC-002 — Architectural Principles
- DF-ARC-003 — Architectural Concepts
- DF-ARC-005 — Architectural Components

## 15.2. Metadata

- DF-MTD-001 — Metadata Architecture
- DF-MTD-002 — Metadata Concepts
- DF-MTD-003 — Metadata Model
- DF-MTD-004 — Metadata Elements
- DF-MTD-005 — Metadata Schema
- DF-MTD-006 — Metadata Lifecycle
- DF-MTD-007 — Metadata Validation
- DF-MTD-008 — Metadata Governance
- DF-MTD-009 — Metadata Relationships
- DF-MTD-010 — Metadata Constraints
- DF-MTD-011 — Metadata Extensibility
- DF-MTD-013 — Metadata Dictionary
- DF-MTD-014 — Metadata Specification

---

**End of Document**

---
