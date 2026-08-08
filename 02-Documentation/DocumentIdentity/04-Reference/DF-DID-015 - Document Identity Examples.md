# Documentation Framework

# DF-DID-015 – Document Identity Examples

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-DID-015 |
| **Title** | Document Identity Examples |
| **Family** | Documentation |
| **Type** | Reference |
| **Component** | Document Identity |
| **Author** | Arnaldo Figueira |
| **Status** | Canonical |
| **Version** | 1.0 |
| **Revision** | 0 |
| **Baseline** | 1.0 |
| **Language** | English |

---

# 1. Purpose

This document provides canonical examples illustrating the concepts defined by the **Document Identity** component.

Its purpose is purely educational.

The examples contained herein demonstrate the application of the architectural principles defined by the Document Identity specifications.

They are informative rather than normative.

---

# 2. Introduction

The previous specifications define the architecture, concepts, model, schema, lifecycle, validation, governance, relationships, constraints and extensibility of Document Identity.

This document complements those specifications by presenting representative examples of correct architectural usage.

The examples are intentionally technology independent and should not be interpreted as implementation models.

---

# 3. Example 1 — Minimal Document Identity

The simplest valid Document Identity consists of the canonical architectural elements.

```text

                    Document Identity
                    │
                    ├── Identifier
                    ├── Identity Domain
                    ├── Lifecycle State
                    └── Canonical Reference

```

This represents the minimum architectural information required to identify a document.

---

# 4. Example 2 — Conceptual Identity Model

```text

                              Document
                                  │
                                  ▼

                          Document Identity
                                  │
            ┌─────────────────────┼─────────────────────┐
            │                     │                     │
            ▼                     ▼                     ▼

       Identifier          Identity Domain       Lifecycle State

```

The document owns one Document Identity.

The identity contains its canonical architectural elements.

---

# 5. Example 3 — Identity Assignment

```text

              New Document
                    │
                    ▼

           Identity Assignment
                    │
                    ▼

       Document Identity Created
                    │
                    ▼

          Permanent Association

```

Once assigned, the identity becomes permanently associated with the document.

---

# 6. Example 4 — Document Evolution

```text

               Version 1.0
                    │
                    ▼

               Version 1.1
                    │
                    ▼

               Version 2.0
                    │
                    ▼

               Version 3.0

                    │
                    │
                    └───────────────► Same Document Identity

```

Document revisions preserve the same Document Identity.

Only the document evolves.

---

# 7. Example 5 — Metadata Relationship

```text

                                 ┌─────────────────────┐
                                 │  Document Identity  │
                                 └─────────────────────┘

                                            ▲
                                            │
                                       references
                                            │
                                 ┌─────────────────────┐
                                 │      Metadata       │
                                 └─────────────────────┘

```

Metadata references an existing Document Identity.

Metadata does not define identity.

---

# 8. Example 6 — Classification Relationship

```text

                                 ┌─────────────────────┐
                                 │  Document Identity  │
                                 └─────────────────────┘

                                            ▲
                                            │
                                       classifies
                                            │
                                 ┌─────────────────────┐
                                 │   Classification    │
                                 └─────────────────────┘

```

Classification categorises documents already identified.

---

# 9. Example 7 — Registry Relationship

```text

                 Registry
                    │
                    ▼

            Document Identity
                    │
                    ▼

                 Document

```

Registry stores references to Document Identities.

Registry does not own identity.

---

# 10. Example 8 — Relationships Component

```text

                Document A
                    │
                    ▼

                Identity A
                    │
                    │

               Relationship
                    │
                    ▼

                Identity B
                    
                    ▲
                    │
                Document B

```

Relationships connect Document Identities rather than documents directly.

---

# 11. Example 9 — Knowledge Graph

```text

                          ┌─────────────────────┐
                          │     Identity A      │
                          └─────────────────────┘
                                    │
                                    ▼

                          ┌─────────────────────┐
                          │     Identity B      │
                          └─────────────────────┘

```

The Knowledge Graph represents Document Identities as graph nodes.

Identity semantics remain defined by the Document Identity component.

---

# 12. Example 10 — Repository Migration

```text

               Repository A
                    │
                    ▼
                 Document
                    │
                    ▼

               Repository B

            Document Identity
                    │
                    └────────────── Unchanged

```

Repository migration does not affect Document Identity.

---

# 13. Example 11 — Publication Formats

```text

                       Document
                          │
            ┌─────────────┼─────────────┐
            ▼             ▼             ▼

           PDF           HTML        Markdown

            ────────────────────────────
                          │
                          ▼

               Same Document Identity

```

Different document representations share the same canonical identity.

---

# 14. Example 12 — Lifecycle

```text

                Unassigned
                    │
                    ▼

                 Assigned
                    │
                    ▼

                Preserved
                    │
                    ▼

                 Retired

```

The identity lifecycle is independent of the document lifecycle.

---

# 15. Example 13 — Validation

```text

            Document Identity
                    │
                    ▼

          Structural Validation
                    │
                    ▼

           Semantic Validation
                    │
                    ▼

          Consistency Validation
                    │
                    ▼

              Valid Identity

```

Validation confirms compliance with the canonical specification.

---

# 16. Example 14 — Governance

```text

            Document Changes
                    │
                    ▼

            Metadata Changes
                    │
                    ▼

          Classification Changes
                    │
                    ▼

            Repository Changes
                    │
                    ▼

            Document Identity
                    │
                    ▼

                Unchanged

```

Governance preserves identity regardless of document evolution.

---

# 17. Example 15 — Identity Uniqueness

Valid example

```text

                    Document A  →  Identity A

                    Document B  →  Identity B

                    Identity A  ≠  Identity B

```

Each document possesses a different identity.

---

# 18. Example 16 — Invalid Identity Reuse

Invalid example

```text

                    Document A  →  Identity A

                    Document B  →  Identity A

```

Violation:

- uniqueness;
- identity ownership;
- canonical specification.

---

# 19. Example 17 — Invalid Identifier Modification

```text

           Assigned Identifier
                    │
                    ▼

           Modified Identifier

```

This situation is invalid.

Document Identities are immutable after assignment.

---

# 20. Example 18 — Invalid Identity Replacement

```text

                 Document
                    │
                    ▼

               Identity A
                    │
                    ▼

               Identity B

```

Replacing an existing identity violates the permanence principle.

---

# 21. Example 19 — Cross-Component Overview

```text

                                   Document Identity
                                           │
            ┌───────────────┬──────────────┼───────────────┬──────────────────┐
            ▼               ▼              ▼               ▼                  ▼

        Metadata     Classification     Registry     Relationships     Knowledge Graph

```

Every collaborating component references the canonical Document Identity.

Only the Document Identity component owns identity semantics.

---

# 22. Example 20 — Complete Conceptual View

```text

                              Document
                                 │
                                 ▼

                         Document Identity
                                 │
        ┌────────────────────────┼────────────────────────┐
        ▼                        ▼                        ▼

   Identifier             Identity Domain          Lifecycle State
                                 │
                                 ▼

                        Canonical Reference
                                 │
        ┌───────────────┬────────────────┬─────────────────┐
        ▼               ▼                ▼                 ▼

    Metadata      Classification      Registry       Relationships

```

This example illustrates the complete architectural role of Document Identity within the Documentation Framework.

---

# 23. Relationship with Other Specifications

The examples presented in this document illustrate concepts defined by the following specifications.

| Specification | Contribution |
|--------------|--------------|
| DF-DID-001 — Document Identity Architecture | Overall architecture |
| DF-DID-002 — Document Identity Concepts | Core concepts |
| DF-DID-003 — Document Identity Model | Conceptual model |
| DF-DID-004 — Document Identity Elements | Identity elements |
| DF-DID-005 — Document Identity Schema | Canonical structure |
| DF-DID-006 — Document Identity Lifecycle | Lifecycle examples |
| DF-DID-007 — Document Identity Validation | Validation examples |
| DF-DID-008 — Document Identity Governance | Governance examples |
| DF-DID-009 — Document Identity Relationships | Component interactions |
| DF-DID-010 — Document Identity Constraints | Valid and invalid scenarios |
| DF-DID-011 — Document Identity Extensibility | Extension examples |
| DF-DID-012 — Document Identity Best Practices | Recommended usage |
| DF-DID-013 — Document Identity Dictionary | Canonical terminology |
| DF-DID-014 — Document Identity Specification | Normative reference |

---

# 24. Summary

This document provides representative examples demonstrating the application of the Document Identity architecture within the Documentation Framework.

The examples illustrate both correct and incorrect architectural scenarios, reinforcing the principles of permanence, uniqueness, immutability, canonical representation, and implementation independence.

Together with the normative specifications, these examples provide practical guidance for architects, framework implementers, and documentation engineers while preserving the conceptual integrity of the Document Identity component.

---

**End of Document**

---
