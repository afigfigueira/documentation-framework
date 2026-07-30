# Roadmaps

## Overview

The **Roadmaps** directory contains the planning documentation that guides the future evolution of the **Documentation Framework**.

Unlike the numbered directories that represent the framework's architectural layers, this directory is **not part of the architecture itself**.

Its purpose is to organise, coordinate and document the planned evolution of every architectural component while preserving the stability of the framework.

---

# Purpose

The Roadmaps directory provides a structured planning environment for the Documentation Framework.

Its objectives are to:

- define the evolution strategy for each architectural layer;
- document planned capabilities and future milestones;
- organise development priorities;
- preserve the long-term vision of the framework;
- support incremental and independent evolution of each component.

Roadmaps describe **where the framework is going**, not **how the framework is built**.

---

# Relationship with the Layered Architecture

The Documentation Framework is organised into a layered architecture.

Each layer has its own architectural responsibility.

The Roadmaps directory mirrors this organisation without belonging to it.

Conceptually.

```text

					Architecture
							│
							├── 00-Foundation
							├── 01-Architecture
							├── 02-Documentation
							├── 03-Governance
							├── 04-Discovery
							├── 05-Automation
							└── 06-Integration


						Roadmaps
							│
							├── 00-Foundation
							├── 01-Architecture
							├── 02-Documentation
							├── 03-Governance
							├── 04-Discovery
							├── 05-Automation
							└── 06-Integration

```

The architectural layers define the structure of the framework.

The Roadmaps directory defines the evolution strategy for that structure.

---

# Directory Structure

```text

					Roadmaps
					│
					├── 00-Foundation
					├── 01-Architecture
					├── 02-Documentation
					├── 03-Governance
					├── 04-Discovery
					├── 05-Automation
					└── 06-Integration

```

Each subdirectory contains the roadmap documents for the corresponding architectural layer.

---

# Component Roadmaps

Each architectural component may maintain its own independent roadmap.

For example.

```text

					Roadmaps
					│
					├── 02-Documentation
					│   ├── Metadata
					│   │   └── DF-MTD-RDM-001.md
					│   │
					│   ├── DocumentIdentity
					│   │   └── DF-DID-RDM-001.md
					│   │
					│   ├── Classification
					│   │   └── DF-CLS-RDM-001.md
					│   │
					│   └── Templates
					│       └── DF-TPL-RDM-001.md

```

This organisation allows every component to evolve independently while remaining aligned with the overall framework strategy.

---

# Architectural Principles

The Roadmaps directory follows the same principles adopted throughout the Documentation Framework.

- Separation of Concerns
- Layered Organisation
- Modularity
- Independence
- Scalability
- Traceability

These principles ensure that planning activities remain consistent with the architectural philosophy of the framework.

---

# Why Roadmaps Are Not Numbered

Unlike the architectural layers, the **Roadmaps** directory intentionally has **no ordinal prefix**.

This reflects an important architectural decision.

The numbered directories describe the framework itself.

The Roadmaps directory describes the evolution of the framework.

It is therefore a management structure rather than an architectural layer.

Maintaining this distinction preserves the separation between architecture and planning.

---

# Evolution

As the Documentation Framework evolves, new roadmap documents may be added for:

- new architectural components;
- new services;
- future integrations;
- automation initiatives;
- governance improvements.

The organisation of the Roadmaps directory is expected to evolve together with the framework while preserving its layered structure.

---

# Related Documents

- DF-RDM-001 — Documentation Framework Roadmap
- DF-FND-004 — Architectural Blueprint
- DF-FND-005 — Framework Evolution
- DF-FND-006 — Design Rationale

---

# Summary

The **Roadmaps** directory centralises all planning documentation for the Documentation Framework.

Although its internal organisation mirrors the framework's layered architecture, it intentionally remains outside the architectural hierarchy.

This separation ensures that the framework's architecture remains stable while its evolution can be planned, managed and extended independently.