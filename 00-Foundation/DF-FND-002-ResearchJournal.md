# Documentation Framework

# Research Journal


| Metadata | Value |
|----------|-------|
| **Document ID** | DF-FND-002 |
| **Title** | Research Journal |
| **Author** | Arnaldo Figueira |
| **Status** | Approved |
| **Version** | 1.0 |
| **Baseline** | 1.0 |
| **Language** | English |



---

# 1. The Origin of the Need

---

## 1.1. Introduction

This document constitutes the chronological record of the research that led to the emergence of the **Documentation Framework**.

Unlike a technical specification, this journal is not intended to describe the final architecture of the system.

Its purpose is to preserve the discovery process.

The questions.

The hypotheses.

The experiments.

The decisions.

And, above all, the reasoning that led to the architecture currently proposed.

As happened with the VisualEngine, most of the solutions described here were not designed in advance.

They were discovered progressively.

---

## 1.2. The Context

The Documentation Framework did not originate as an independent project.

It was born during the development of the **VisualEngine**.

Initially, there was only the need to organize some technical documentation.

Nothing more.

The first documents were relatively simple.

* README;
* personal notes;
* task lists;
* small architecture documents.

Each document was created independently.

Without any common structure.

---

## 1.3. The Initial Problem

As the number of documents increased, difficulties began to emerge.

For example.

* duplicated documents;
* different formats;
* lack of conventions;
* inconsistent versions;
* contradictory information;
* difficulty locating knowledge.

The problem still seemed small.

But it was beginning to repeat itself.

---

## 1.4. The First Observation

It quickly became apparent that writing documentation was very different from maintaining documentation.

Creating a document is relatively simple.

Keeping it up to date for months or years proved to be significantly more difficult.

A question then began to emerge.

**Why does documentation degrade so quickly?**

---

## 1.5. Documentation as Code

One of the first ideas was to treat documentation in a manner similar to source code.

Source code has.

* structure;
* conventions;
* organization;
* review;
* evolution.

Why not apply the same principles to documentation?

This question would accompany the entire research process.

---

## 1.6. The Problem Was Not Markdown

Initially, it was believed that the main limitation lay in the language being used.

Perhaps Markdown was too simple.

Perhaps another technology was required.

However.

After several experiments, it became evident that the problem was not the syntax.

Markdown proved to be sufficiently expressive.

The difficulty existed at another level.

---

## 1.7. The Lack of Structure

After analysing several projects, a common pattern became evident.

Most documentation was organised solely through directories.

For example.

```text
docs/

README.md

Architecture.md

Design.md

Notes.md

Todo.md
```

Although functional.

This organisation did not explain.

* the role of each document;
* the existing relationships;
* the relative importance;
* the approval status;
* the historical evolution.

The documents were merely files.

---

## 1.8. A Fundamental Question

During this phase, a particularly important question emerged.

**What is a document, really?**

Is it merely a Markdown file?

Or does it represent something more?

At the time, there was still no clear answer.

But this question would eventually transform the entire project.

---

## 1.9. The Value of Knowledge

Another important observation was the realization that different documents had very different values.

Some contained simple temporary notes.

Others described fundamental architectural decisions.

However.

They were all treated in exactly the same way.

This lack of distinction was beginning to become problematic.

---

## 1.10. The Need for Identity

As the documentation grew, it also became difficult to reference documents consistently.

Names varied.

Titles changed.

Files were frequently reorganised.

The idea then began to emerge of assigning each document its own identity.

Not merely a name.

But a stable identifier.

This idea would be developed later.

---

## 1.11. The Natural Evolution

Up to this point, the evolution can be summarised as follows.

```text

				  Notes

					↓

				Documents

					↓

		    Document Collection

					↓

			Need for Organization

```

Although simple.

This sequence represented the true birth of the Documentation Framework.

---

## 1.12.  An Important Discovery

During this phase, it became evident that the problem was not writing documentation.

The real problem was managing knowledge.

Documentation was merely the physical representation of that knowledge.

This distinction proved to be extremely important.

---

## 1.13.  Initial Hypotheses

Several possibilities were then considered.

* standardising file names;
* creating templates;
* defining conventions;
* organising directories;
* creating indexes.

All these solutions helped.

But none completely solved the problem.

---

## 1.14.  The First Framework Idea

It was precisely at this point that a different hypothesis emerged.

Instead of producing documents alone.

Perhaps it would be possible to build an infrastructure for documentation.

An infrastructure that defined.

* rules;
* conventions;
* structure;
* evolution.

The concept of a Documentation Framework did not yet exist.

But the idea was beginning to take shape.

---

## 1.15.  Research Status

At the end of this first phase, several important conclusions had already been reached.

* Markdown was adequate.
* The problem was not technological.
* The problem was structural.
* Documentation represents knowledge.
* Knowledge requires organisation.
* Documents should possess identity.

These observations would serve as the foundation for all subsequent research.

---

## 1.16.  Next Steps

The next stage would consist of finding a way to standardise documents.

Not merely through rules.

But through a common structure.

This research would lead to the emergence of the first **Templates**, marking the true beginning of document standardisation.

---

## 1.17.  Conclusion

The Documentation Framework was born from an extremely simple problem.

The difficulty of maintaining coherent documentation throughout the evolution of a project.

However, it quickly became clear that the issue went far beyond the organisation of Markdown files.

The real challenge was understanding how to structure knowledge in a consistent, evolutionary and reusable manner.

It was this change in perspective that gave rise to the research described in the following parts of this journal.

---

# 2. The First Templates

---

## 2.1. Introduction

After recognising that the main problem with documentation was not Markdown itself, but rather the lack of structure, the first attempt at standardisation naturally emerged.

This attempt consisted of creating **Templates**.

At the time, the idea was extremely simple.

If every document follows the same format, the documentation will automatically become more consistent.

It quickly became apparent that reality was considerably more complex.

---

## 2.2.  The Problem

The project's first documents were written according to the immediate needs of the moment.

Each document had.

* different titles;
* different sections;
* different organisation;
* different styles.

Even documents with similar objectives had completely different structures.

This diversity made.

* reading;
* maintenance;
* comparison;
* evolution.

more difficult.

---

## 2.3.  The First Solution

The initial solution seemed obvious.

Create a base document.

Whenever it became necessary to write a new document.

That document would simply be copied.

Only its content would then be modified.

Conceptually.

```text id="tpl1"

				 Template

					↓

			   New Document

```

This approach immediately revealed several advantages.

---

## 2.4. The First Benefits

Templates introduced an initial level of standardisation.

All documents began to include.

* a title;
* an introduction;
* chapters;
* a conclusion.

The documentation became significantly more homogeneous.

However.

New problems quickly emerged.

---

## 2.5. The Limitations of Templates

After a few months of use, it became apparent that different types of documents required completely different structures.

For example.

An architecture document.

Does not have the same organisation as a research document.

Nor as a technical manual.

Nor as a specification.

Consequently.

A single Template proved to be insufficient.

---

## 2.6. The Emergence of Multiple Templates

The research then evolved towards a new model.

Instead of having only one Template.

There would now be several.

For example.

```text id="tpl2"

				Architecture Template

				Research Template

				Specification Template

				Reference Template

				README Template

```

Each Template came to reflect a specific purpose.

---

## 2.7. The Discovery of Categories

It was precisely during this phase that an important observation emerged.

Templates were not selected randomly.

Each Template corresponded to a particular document category.

For example.

An architecture document frequently requires.

* an overview;
* diagrams;
* components;
* relationships;
* decisions.

Whereas a research document focuses on.

* context;
* hypotheses;
* experiments;
* results;
* conclusions.

This difference gradually became structural.

---

## 2.8. A Template Does Not Define a Document

Another particularly interesting discovery was the realisation that a Template only defines an initial structure.

It does not define the meaning of the document.

Two documents produced from the same Template may represent completely different knowledge.

This distinction proved to be important.

The Template came to be understood as a tool.

Not as a semantic definition.

---

## 2.9. Evolution Becomes Difficult

As the number of Templates increased, a new problem emerged.

Whenever an improvement was introduced.

It became necessary to update all the Templates.

And frequently.

All the existing documents as well.

Maintenance was once again becoming complex.

---

## 2.10. The Search for Common Elements

A new phase of the research then began.

Instead of looking for similar documents.

The focus shifted to identifying elements common to all documents.

Regardless of their type.

For example.

They all have.

* an author;
* a date;
* a version;
* a status.

This observation proved to be extremely important.

---

## 2.11. The Birth of Metadata

It was precisely here that one of the fundamental discoveries of the Documentation Framework emerged.

A significant portion of the information contained in a document does not belong to its content.

It belongs to its identity.

This information includes.

* author;
* version;
* status;
* identifier;
* dates;
* language.

This collection of information came to be known as **Metadata**.

At the time, there was still no formal definition.

But the idea had been established.

---

## 2.12. Templates as Contracts

Another conceptual evolution consisted of no longer viewing Templates merely as text models.

They gradually came to be regarded as structural contracts.

A document was no longer organised freely.

It now had to comply with a specific structure.

This change significantly increased document consistency.

---

## 2.13. The First Conventions

During this phase, several small conventions also began to emerge.

For example.

* consistent use of headings;
* section ordering;
* uniform naming;
* hierarchical organisation.

Although simple.

These conventions considerably reduced the heterogeneity that had previously existed.

---

## 2.14. Remaining Limitations

Despite the improvements introduced.

Several difficulties still remained.

Templates.

* did not identify documents;
* did not establish relationships;
* did not define states;
* did not enable knowledge discovery.

They were still merely writing templates.

It was evident that a higher layer was missing.

---

## 2.15. Research Status

At the end of this phase, several conclusions had been established.

* A single Template is insufficient.
* Different documents require different structures.
* All documents share common information.
* That information does not belong to the content.
* Templates represent structural contracts.
* Consistency depends on both structure and conventions.

These conclusions would directly prepare the next stage.

---

## 2.16. Next Steps

The discovery of Metadata would profoundly transform the entire document architecture.

For the first time, it became evident that a document is not merely text.

It also possesses its own intrinsic properties.

These properties would prove to be far more important than initially expected.

The next phase of the research would be dedicated precisely to the formalisation of this concept.

---

## 2.17. Conclusion

The first Templates represented the first concrete step towards the systematic organisation of documentation.

Although they did not solve every problem, they demonstrated that structural standardisation produced significant improvements in the quality and maintainability of documents.

More importantly, they led to the discovery of a fundamental distinction.

The content of a document and its structural identity are different concepts.

It was precisely this distinction that led to the emergence of **Metadata**, one of the fundamental pillars of the Documentation Framework.

---

# 3. The Discovery of Metadata

---

## 3.1. Introduction

The research initiated with the first Templates naturally led to a new discovery.

Although Templates standardised the structure of documents, there was still a set of information that was not part of the actual content.

This information appeared repeatedly in virtually every document.

Initially, it seemed to be nothing more than a collection of small annotations.

Later, it became evident that it represented something far more important.

This information came to be known as **Metadata**.

---

## 3.2. The Problem

When comparing different documents, it became apparent that they all contained similar information.

For example.

* author;
* version;
* date;
* language;
* status;
* project.

This information was often entered manually.

In different locations.

Using different formats.

And, in some cases.

It did not even exist.

---

## 3.3. Information About the Document

An important observation quickly emerged.

Not all the information contained in a document belongs to the knowledge the document is intended to convey.

There is also information that describes the document itself.

For example.

A document may discuss architecture.

While simultaneously having.

* an author;
* a revision;
* an owner;
* an approval status.

These data describe the document.

Not its content.

---

## 3.4. The Natural Separation

A conceptual separation then began to emerge.

```text id="md1"

					Document
					│
					├── Content
					│
					└── Metadata

```

Although apparently simple.

This distinction proved to be one of the fundamental pillars of the Documentation Framework.

---

## 3.5. Metadata Is Not Optional

Initially, it was thought that these data could be optional.

However.

After several months of use, it became evident that documents without Metadata were significantly more difficult to manage.

For example.

It was difficult to answer simple questions.

* What is the current version?
* Who is responsible?
* Is this document still valid?
* When was it last updated?

Metadata therefore ceased to be regarded as an optional complement.

It became an integral part of the document.

---

## 3.6. The Search for Uniformity

Once the importance of Metadata had been recognised.

A new challenge emerged.

Should all documents use exactly the same fields?

Or should each document type have different Metadata?

After several experiments, the conclusion was that.

There is a common core.

And a set of specific extensions.

This distinction made it possible to reconcile consistency and flexibility.

---

## 3.7. The Document Header

It was during this phase that the idea of a standardised header began to emerge.

Conceptually.

```text id="md2"

					Document ID

					Title

					Version

					Status

					Project

					Language

```

This header progressively became the entry point of every document.

Readers could immediately understand the context to which the document belonged.

---

## 3.8. Metadata as a Contract

Another important conceptual change consisted of no longer considering Metadata merely as auxiliary information.

It came to function as a genuine document contract.

If two documents belong to the same family.

They must have compatible Metadata.

This principle enabled the automation of various tasks.

---

## 3.9. The First Identity

During practical use, another problem became apparent.

A document's title may change.

Its file name may change as well.

But it must still be possible to identify that document unambiguously.

The idea of a permanent identifier therefore began to emerge.

There was still no formal model.

But the need was evident.

---

## 3.10. Metadata and Automation

Another important discovery was the realisation that Metadata can be used by tools.

For example.

An application can.

* locate documents;
* verify versions;
* generate indexes;
* build references;
* validate consistency.

Without even analysing the content.

This capability opened new possibilities for the evolution of the framework.

---

## 3.11. The Content Remains Independent

Despite the growing importance of Metadata.

A principle was also established.

Metadata must never directly interfere with the content.

Knowledge remains separate from administrative information.

This separation made the document architecture much cleaner.

---

## 3.12. The Beginning of Classification

As the number of documents increased.

New requirements began to emerge.

It was no longer sufficient to identify documents.

It also became necessary to classify them.

For example.

* architecture;
* analysis;
* reference;
* research;
* standard.

This requirement would prepare the next stage of the research.

---

## 3.13. A New Perspective

During this phase, a particularly interesting idea also began to emerge.

Just as a class in programming has properties.

A document also has properties.

This analogy brought documentation significantly closer to software engineering.

Documents were no longer viewed merely as text.

They came to be regarded as entities.

---

## 3.14. Research Status

At the end of this phase, several conclusions had been established.

* Every document has Metadata.
* Metadata describes the document.
* Content describes the knowledge.
* Both must remain separate.
* There is a common Metadata core.
* Metadata supports automation.
* The document has its own identity.

These ideas profoundly changed the project's original vision.

---

## 3.15. Next Steps

The existence of Metadata naturally led to a new question.

If documents have identity.

How should they be identified?

Is it sufficient to use file names?

Or is it necessary to define a formal identification system?

The next phase of the research would be dedicated precisely to the creation of the first **Document Identifiers**, **Families**, **Types**, and **Classes**, establishing a permanent identity for every document.

---

## 3.16. Conclusion

The discovery of Metadata marked the transition from a simple collection of documents to a true documentation system.

For the first time, documents acquired their own properties, independent of the knowledge they contained.

This separation between content and identity proved to be one of the fundamental principles of the Documentation Framework and paved the way for the formalisation of document classification, traceability, and the future automation of the entire ecosystem.

---

# 4. Document Identity

---

## 4.1. Introduction

The discovery of **Metadata** solved an important problem.

Documents came to possess their own properties.

However, a new difficulty quickly emerged.

How can a document be permanently identified?

For some time, only file names were used.

But this approach quickly revealed several limitations.

It was precisely from this need that the concept of **Document Identity** was born.

---

## 4.2. The Problem

The first documents were identified solely by their file names.

For example.

```text id="id1"

					Architecture.md

					Design.md

					README.md

					Notes.md

```

This solution appeared to be sufficient.

But difficulties soon emerged.

---

## 4.3. Names Change

Throughout the evolution of a project, it is perfectly normal to change.

* titles;
* file names;
* directory locations.

Consequently.

A document could completely change its name.

While continuing to represent exactly the same knowledge.

Identity could not depend on the name.

---

## 4.4. The Document as an Entity

During this phase, an important analogy began to emerge.

In programming.

An object has identity.

Even if its state changes.

A document should likewise have a permanent identity.

Regardless of.

* its version;
* its title;
* its location;
* its content.

This idea profoundly changed the document architecture.

---

## 4.5. The First Identifier

The first proposal consisted of assigning a simple code to each document.

For example.

```text id="id2"

					DOC-001

					DOC-002

					DOC-003

```

Although this partially solved the problem.

It quickly revealed a limitation.

The identifier conveyed no meaning.

---

## 4.6. The Search for Semantics

A new question then emerged.

Could the identifier itself contain information?

For example.

* family;
* type;
* number.

In this way.

The identifier would no longer be just a number.

It would also communicate context.

---

## 4.7. The Emergence of Families

The first evolution consisted of grouping documents into broad areas.

For example.

```text id="id3"

					META

					ARC

					ANL

					REF

					STD

					RFC

```

Each Family came to represent a category of knowledge.

This organisation proved to be extremely useful.

---

## 4.8. The Concept of Type

It quickly became apparent that Family alone was still too generic.

Within the same Family there were very different documents.

A second level of classification then began to emerge.

The **Type**.

For example.

```text id="id4"

					META-DCL

					META-WFL

					META-CON

					META-REF

```

The combination of Family + Type made identifiers much more expressive.

---

## 4.9. Numbering

Once Family and Type had been defined.

Only one element remained.

Distinguishing documents belonging to the same category.

Sequential numbering was therefore introduced.

Conceptually.

```text id="id5"

					META-DCL-001

					META-DCL-002

					META-DCL-003

```

This convention made it possible to identify every document uniquely.

---

## 4.10. The Discovery of Classes

During practical use, another need emerged.

Not all documents fulfil the same role.

Some define standards.

Others merely record research.

Others describe architecture.

This observation led to the emergence of **Document Classes**.

A Class came to represent the nature of the document.

Regardless of its Family.

---

## 4.11. Identity Becomes Permanent

A particularly important decision was made during this phase.

The identifier must never change.

Even if.

* the title is modified;
* the content evolves;
* the document is reorganised.

The identity remains constant.

This principle brought documents significantly closer to software entities.

---

## 4.12. The Separation Between Identity and Location

Another important conclusion was to completely separate.

Identity.

From physical location.

A document may be moved between directories.

It may even be moved to another repository.

Yet it continues to represent exactly the same document.

This separation proved essential for the future evolution of the framework.

---

## 4.13. Metadata Evolves

With the introduction of identifiers.

Metadata also became richer.

For example.

```text id="id6"

					Document ID

					Family

					Type

					Class

					Version

					Revision

					Status

					Baseline

```

Metadata was no longer merely administrative.

It progressively came to represent the document structure itself.

---

## 4.14. The Document as an Architectural Object

At this stage, one particularly important idea became evident.

A document was no longer considered merely a file.

It came to represent an architectural object.

With.

* identity;
* properties;
* state;
* lifecycle.

This conceptual change laid the foundation for almost all subsequent evolution of the Documentation Framework.

---

## 4.15. Research Status

At the end of this phase, several fundamental principles had been established.

* Every document has a permanent identity.
* Identity does not depend on the name.
* Identity does not depend on the location.
* Family organises knowledge.
* Type specialises the Family.
* Class defines the nature of the document.
* The identifier must remain stable throughout the entire lifecycle.

These decisions would remain virtually unchanged until the current architecture.

---

## 4.16. Next Steps

As identifiers matured, an unexpected observation emerged.

Some documents did not describe the project.

They described the documentation itself.

In other words.

There were documents whose domain was the Documentation Framework itself.

This discovery would lead directly to the emergence of a new document category.

The **META Documents**.

---

## 4.17. Conclusion

The formalisation of document identity represented one of the most important milestones in the evolution of the Documentation Framework.

By definitively separating identity, content, and location, documents came to possess an existence of their own within the architecture.

This decision made it possible to introduce mechanisms for traceability, automation, and controlled evolution that would have been impossible using file names alone.

It was precisely upon this foundation that the next stage of the research emerged: the creation of **META Documents**, whose purpose was no longer to describe a project, but to describe the documentation system itself.

---

# 5. The Birth of META Documents

---

## 5.1. Introduction

The formalisation of document identity led to an unexpected discovery.

As the number of documents increased, a very particular type of documentation began to emerge.

These documents did not describe the VisualEngine.

Nor algorithms.

Nor components.

Nor architecture.

They described the documentation itself.

It was precisely at this point that the concept of **META Documents** was born.

---

## 5.2. A Different Problem

Up to this stage, all documents had a relatively clear purpose.

They described.

* components;
* decisions;
* research;
* references.

However.

Questions of a completely different nature began to emerge.

For example.

* How should a document be identified?
* How should a Template evolve?
* Which Metadata is mandatory?
* How are two documents related?

These questions no longer belonged to the project domain.

They belonged to the documentation domain.

---

## 5.3. Documentation Becomes a Domain

A new hypothesis was then formulated.

Documentation should be considered a domain in its own right.

Just like.

* Finance;
* Artificial Intelligence;
* Robotics.

Documentation also has.

* entities;
* rules;
* concepts;
* processes.

This change in perspective proved to be decisive.

---

## 5.4. The First META Document

The initial solution consisted of creating a document dedicated exclusively to documentation rules.

Conceptually.

```text id="meta1"

				  META

					↓

			Documentation Rules

```

This document did not describe the project.

It described how the project should be documented.

---

## 5.5. A New Document Category

The need to distinguish these documents from all others quickly emerged.

A new Family was created.

```text id="meta2"

					META

```

This Family came to represent documents whose domain is the Documentation Framework itself.

It became one of the first Families to span the entire project.

---

## 5.6. Self-Reference

During this phase, an interesting question emerged.

Can a system document itself?

Initially, this idea seemed paradoxical.

But it quickly became apparent that there was no contradiction.

Provided that clear levels of abstraction were established.

META Documents do not document a specific document.

They document the rules used by all documents.

---

## 5.7. The Emergence of the First META Documents

Specialised documents then began to appear.

For example.

```text id="meta3"

					META-DCL

					META-REF

					META-CON

					META-WFL

```

Each had clearly defined responsibilities.

Together, they began to form a true documentation architecture.

---

## 5.8. From Convention to Specification

Until this point, many decisions were merely conventions.

With the introduction of META Documents, they became formalised.

For example.

A convention.

"All documents must have a version."

Became a formal rule.

Defined.

Documented.

Versioned.

And subject to evolution.

This change significantly increased the consistency of the framework.

---

## 5.9. Knowledge About Knowledge

A particularly interesting consequence was the realisation that META Documents represent a higher level of knowledge.

While an architecture document describes a system.

A META Document describes how that document should exist.

This level of abstraction brought the Documentation Framework closer to metamodeling.

---

## 5.10. Internal Organisation

As the number of META Documents grew, it became evident that they too required organisation.

Relationships between them then began to emerge.

For example.

```text id="meta4"

				META-DCL

					↓

				 Defines

					↓

				META-REF

					↓

				  Uses

					↓

				META-CON

					↓

				Related to

					↓

				META-WFL

```

For the first time, the documentation itself had its own architecture.

---

## 5.11. The Evolution of Rules

Another important observation was the realisation that documentation rules also evolve.

Consequently.

META Documents also came to have.

* versions;
* revisions;
* history;
* states.

The framework thus began to document the evolution of its own rules.

---

## 5.12. A Self-Describing Architecture

It was precisely during this phase that an ambitious objective emerged.

The Documentation Framework should be capable of explaining itself.

Every documentation decision should be understandable by consulting the META Documents.

This objective would strongly influence all subsequent evolution.

---

## 5.13. The Limits of META

Despite the enormous progress achieved.

A philosophical question also began to emerge.

META Documents explain the rules.

But who explains why those rules change?

This question remained unanswered for some time.

It would later lead directly to integration with the **Change Management System**.

---

## 5.14. Research Status

At the end of this phase, several conclusions had been established.

* Documentation constitutes a domain in its own right.
* META Documents document that domain.
* Documentation rules must be formalised.
* META Documents have identity and a lifecycle.
* Documentation requires its own architecture.
* The framework must be capable of explaining its own rules.

These ideas marked an important turning point in the research.

---

## 5.15. Next Steps

With the META Documents consolidated, a new need emerged.

The documentation rules already existed.

But one essential problem remained unresolved.

How can the simultaneous evolution of dozens or hundreds of documents be controlled?

How can it be ensured that a collection of documents represents a coherent state of the documentation?

The answer would begin to emerge through the concepts of **Baseline**, **Document Versioning**, and **Controlled Revision**, which would become the subject of the next stage of the research.

---

## 5.16. Conclusion

The emergence of **META Documents** represented the definitive transition from an organised collection of documents to a true documentation framework.

Documentation ceased to be merely a means of communication.

It came to possess its own rules, its own architecture, and a formal set of documents responsible for defining its structure and evolution.

This was the moment when the Documentation Framework acquired its identity as an independent project, rather than remaining merely a collection of conventions associated with the VisualEngine.

---

# 6. Baselines and Document Versioning

---

## 6.1. Introduction

The creation of **META Documents** solved an important problem.

The documentation rules became formally defined.

However, a new difficulty quickly emerged.

Even with well-established rules, documentation continued to evolve continuously.

New documents were created.

Others were modified.

Some were removed.

The question therefore became different.

**How can it be ensured that a collection of documents represents a coherent state of the documentation?**

It was from this need that the concepts of **Baseline** and **Document Versioning** were born.

---

## 6.2. The Problem

For some time, each document evolved independently.

For example.

```text id="bl1"

					Architecture

					Version 2.1

					Documentation

					Version 1.4

					Reference

					Version 3.0

					Workflow

					Version 1.2

```

Individually.

Each document made sense.

Together.

They did not always represent the same architecture.

---

## 6.3. The Discovery of Consistency

It quickly became apparent that the real problem was not the version of an individual document.

It was the consistency between multiple documents.

A significant change in one document could require updates to many others.

Evolution was no longer local.

It became systemic.

---

## 6.4. The Concept of Baseline

A new idea was then introduced.

Instead of considering documents individually.

A consistent collection of documents came to be considered.

This collection was named a **Baseline**.

Conceptually.

```text id="bl2"

					Baseline
					│
					├── Architecture
					│
					├── Reference
					│
					├── Workflow
					│
					├── Templates
					│
					└── Standards

```

A Baseline represents a coherent state of knowledge.

---

## 6.5. Baseline Is Not a Version

Initially, there was some tendency to confuse a Baseline with a version.

It quickly became clear that they are different concepts.

A version describes a document.

A Baseline describes a collection of documents.

This distinction became a fundamental principle.

---

## 6.6. The Role of Revisions

During this phase, it also became evident that not all changes have the same significance.

Some correct errors.

Others fundamentally change the architecture.

A distinction therefore began to emerge between.

* Version;
* Revision.

A Version identifies a significant evolution.

A Revision represents small, backward-compatible changes.

---

## 6.7. Document Status

Another important discovery was the realisation that document evolution does not depend solely on the version.

It also depends on the status.

For example.

```text id="bl3"

				   Draft

					↓

				  Review

					↓

				 Approved

					↓

				Deprecated

					↓

				 Archived

```

The status came to represent the point in the lifecycle at which a document currently exists.

---

## 6.8. The Collection Must Remain Consistent

An immediate consequence of this approach was the need to validate the entire documentation.

Whenever a document evolves.

A new question arises.

Is it still compatible with the current Baseline?

If not.

The Baseline must evolve.

Or the change must be postponed.

---

## 6.9. The First Baseline

It was precisely during this phase that the project's first formal Baseline emerged.

Its objective was simple.

To represent a stable state of the documentation.

From that moment onwards.

New changes no longer modified that state directly.

Instead, they first passed through an evolution process.

---

## 6.10. The Concept of Freezing

Another important idea emerged naturally.

An approved Baseline must remain immutable.

New changes do not modify the existing Baseline.

They create a new Baseline.

This principle made it possible to preserve historical traceability.

---

## 6.11. Incremental Evolution

The research also demonstrated that large changes are more difficult to control.

Consequently.

Baselines began to evolve incrementally.

Each new Baseline represents a small evolution relative to the previous one.

This model significantly simplified documentation management.

---

## 6.12. The Impact on Metadata

Metadata evolved once again.

New fields became part of the document header.

For example.

```text id="bl4"

					Baseline

					Version

					Revision

					Status

					Last Updated

```

The document now explicitly indicates the Baseline to which it belongs.

---

## 6.13. Preparing for Automation

As Baselines and versions became established, a new possibility began to emerge.

Documentation validation could be automated.

For example.

A tool could verify.

* incompatible documents;
* inconsistent versions;
* invalid references;
* outdated documents.

This possibility brought the Documentation Framework closer to configuration engineering.

---

## 6.14. Research Status

At the end of this phase, several principles had been established.

* A Baseline represents a coherent state of the documentation.
* Baseline and Version are distinct concepts.
* Documents have their own lifecycle.
* Significant changes create new Baselines.
* Approved Baselines remain immutable.
* Documentation consistency became an architectural objective.

These decisions remained virtually unchanged throughout the subsequent phases.

---

## 6.15. Next Steps

The introduction of Baselines resolved the temporal consistency of the documentation.

However.

Another question still remained unanswered.

How can a document be located quickly?

How can all related documents be discovered?

How can the existing knowledge be navigated?

These questions would lead directly to the emergence of the **Document Registry**, responsible for the organisation, discovery, and traceability of the entire documentation asset.

---

## 6.16. Conclusion

The introduction of the concepts of **Baseline** and **Document Versioning** represented one of the greatest advances of the Documentation Framework.

Documentation ceased to be regarded as a collection of independent files and came to be treated as a coherent system capable of representing stable states of knowledge over time.

This evolution naturally prepared the next stage of the research, where the focus would shift from the individual evolution of documents to the integrated management of the entire documentation collection through the **Document Registry**.

---

# 7. The Document Registry and Knowledge Discovery

---

## 7.1. Introduction

The introduction of **Baselines** solved an important problem.

Documents could now evolve coherently.

However.

As the documentation grew, a new difficulty emerged.

The documents existed.

But finding them was becoming increasingly difficult.

Even with a good understanding of the project's architecture, locating a specific document was not always straightforward.

It was precisely from this need that the concept of the **Document Registry** was born.

---

## 7.2. The Problem

In the early stages, documentation organisation depended exclusively on the directory structure.

For example.

```text id="reg1"

					docs/

					architecture/

					meta/

					analysis/

					templates/

					research/

```

This approach was sufficient for a few dozen documents.

But it quickly began to reveal its limitations.

---

## 7.3. The Limitation of Directories

Directories organise files.

They do not organise knowledge.

A single document may be related to several topics.

But it can exist in only one directory.

This limitation became increasingly evident.

---

## 7.4. Search Was Not Enough

Another attempt was to rely on text search.

Although useful.

Search only provides answers when we already know what we are looking for.

It cannot answer questions such as.

* Which documents define this architecture?
* Which standards affect this component?
* Which documents depend on this one?
* Which decisions led to this specification?

A different mechanism was required.

---

## 7.5. The Concept of a Registry

A new hypothesis was then formulated.

Perhaps every document should have a central registry.

Containing not the content.

But information about each document.

Thus, the concept of the **Document Registry** was born.

Conceptually.

```text id="reg2"

			 Document Registry

					↓

				  Knows

					↓

			  All Documents

```

---

## 7.6. The Registry as a Catalogue

Initially, the Registry was understood as a catalogue.

Each document came to have an entry.

For example.

* Document ID
* Title
* Family
* Type
* Class
* Status
* Baseline

The Registry came to represent a formal index of the available knowledge.

---

## 7.7. Much More Than an Index

It quickly became apparent that the Registry could play a much more important role.

Not only locating documents.

But understanding the documentation.

For example.

It could automatically answer.

* Which documents belong to the same Family?
* Which documents are obsolete?
* Which documents are part of the current Baseline?

This capability profoundly changed the value of the Registry.

---

## 7.8. The Separation Between the Document and the Registry Entry

Another important decision was to clearly separate.

The document.

From its registry entry.

Conceptually.

```text id="reg3"

				 Document

					↓

			   Represented by

					↓

			   Registry Entry

```

The Registry does not replace the document.

It represents it.

This separation made it possible to keep both independent.

---

## 7.9. The Registry as a Knowledge Discovery Mechanism

Until this stage, documentation was primarily accessed by navigating directories.

With the Registry, a new paradigm emerged.

Knowledge discovery.

Users no longer search for files.

They explore relationships.

This change proved to be extremely important.

---

## 7.10. Knowledge Begins to Form a Network

During practical use, an interesting phenomenon became apparent.

Each new document established connections with several others.

For example.

```text id="reg4"

			   Architecture

					↓

				Reference

					↓

				 Workflow

					↓

				  META
				  
```

Documents progressively ceased to form a tree.

They began to form a network.

---

## 7.11. The Need for Explicit Relationships

Initially, these relationships were only implicit.

They existed through references within the text.

However.

It quickly became apparent that they should become explicit.

A tool should be able to answer automatically.

* Which documents depend on this one?
* Which documents replace it?
* Which documents complement it?

This idea prepared the next phase of the research.

---

## 7.12. The Registry as a Service

Another important conceptual evolution was to stop viewing the Registry merely as a file.

It came to be understood as a service.

Responsible for.

* registering;
* locating;
* validating;
* discovering.

This perspective brought the Documentation Framework significantly closer to software architecture.

---

## 7.13. Scalability

As the number of documents increased, it became evident that the Registry would enable the documentation to scale.

Without it.

Maintenance would become progressively more difficult.

With it.

The size of the project would no longer represent a significant limitation.

---

## 7.14. A New Perspective

During this phase, another particularly interesting idea also emerged.

The Registry does not manage documents.

It manages knowledge about documents.

This distinction proved subtle.

But extremely important.

The Registry became a metadata layer.

---

## 7.15. Research Status

At the end of this phase, several conclusions had been established.

* Directories organise files.
* The Registry organises documentation knowledge.
* A Document and a Registry Entry are distinct concepts.
* The Registry supports knowledge discovery.
* Documentation begins to take the form of a network.
* Relationships should become explicit.
* The Registry is an architectural service.

These observations directly prepared the next stage.

---

## 7.16. Next Steps

The existence of a Registry made it possible to locate documents.

However, one important limitation still remained.

Relationships between documents were still insufficiently formalised.

It became necessary to understand.

How are two documents related?

What types of dependencies can exist?

How should those relationships be represented?

These questions would lead directly to the emergence of the formal **Document Relationships** model, bringing the Documentation Framework closer to a true **Knowledge Graph**.

---

## 7.17. Conclusion

The introduction of the **Document Registry** marked the transition from organised documentation to a true knowledge discovery system.

For the first time, it became possible to treat documentation as a structured, searchable, and navigable knowledge asset, independent of the physical organisation of files.

This evolution paved the way for the formalisation of relationships between documents, progressively transforming the documentation into a knowledge graph capable of representing not only information, but also the dependencies and evolution of the project itself.

---

# 8. Document Relationships and the Knowledge Graph

---

## 8.1 Introduction

The creation of the **Document Registry** solved an important problem.

Documents could now be located consistently.

However.

A new question quickly emerged.

Finding a document is only the first step.

The real challenge is understanding that document's relationship with the rest of the available knowledge.

It was precisely from this need that the concept of **Document Relationships** emerged, followed by the vision of documentation as a **Knowledge Graph**.

---

## 8.2. The Problem

For some time, relationships between documents existed only implicitly.

For example.

A document referenced another through its text.

Or mentioned its identifier.

Although functional.

This approach had several limitations.

Relationships.

* could not be verified;
* could not be searched;
* could not be navigated;
* could not be automatically validated.

---

## 8.3. The First Observation

An analysis of the existing documentation revealed that almost no document is completely independent.

Each document.

* depends on others;
* complements others;
* defines concepts used by others.

The documentation proved to be far more interconnected than initially expected.

---

## 8.4. A Change in Perspective

Until this point, the focus had been on documents.

Gradually.

The focus shifted towards the connections between documents.

This change closely resembled the evolution that had occurred in the VisualEngine.

Initially, the emphasis was on entities.

Later.

It shifted to relationships.

Documentation appeared to be following exactly the same path.

---

## 8.5. The First Model

Several simple relationship types then began to emerge.

For example.

```text id="rel1"

					Defines

					References

					Depends On

					Replaces

					Extends

					Implements

```

Although limited.

This set was sufficient to describe most existing dependencies.

---

## 8.6. Relationships as Objects

Another important discovery was the realisation that a relationship also possesses properties.

For example.

A relationship may have.

* source;
* target;
* type;
* date;
* justification.

Consequently.

Relationships ceased to be simple hyperlinks.

They became architectural objects.

---

## 8.7. The Network Begins to Emerge

Once all relationships were represented explicitly.

A new structure became evident.

Conceptually.

```text id="rel2"

				 Document

					↓

				Related To

					↓

				 Document

					↓

				Related To

					↓

				 Document

```

Documents definitively ceased to form a hierarchy.

They became a network.

---

## 8.8. The Discovery of the Knowledge Graph

It was during this phase that a particularly important idea emerged.

The Documentation Framework was not merely managing documents.

It was constructing a **Knowledge Graph**.

Each document became a node.

Each relationship became an edge.

This perspective profoundly changed the way documentation was understood.

---

## 8.9. Knowledge Navigation

Until this point, navigation was based on directories.

Or on text search.

With the Knowledge Graph, it became possible to navigate in an entirely different way.

For example.

```text id="rel3"

			   Architecture

					↓

				 Defines

					↓

				Component

					↓

			  Implemented By

					↓

			   Specification

					↓

			   Referenced By

					↓

				 Research

```

Users no longer navigate directories.

They navigate knowledge.

---

## 8.10. The Value of Relationships

Another important conclusion was the realisation that.

In many cases.

Relationships are just as valuable as the documents themselves.

Knowing that a document exists is useful.

Knowing why it exists and what it depends on is far more valuable.

---

## 8.11. Knowledge Becomes Discoverable

An unexpected consequence was the indirect discovery of knowledge.

By navigating relationships.

Users began to encounter documents they had not initially been searching for.

The system began to support exploration.

Not merely search.

---

## 8.12. Relationships and Consistency

Another important benefit was automatic validation.

For example.

A tool could detect.

* references to non-existent documents;
* circular dependencies;
* superseded documents;
* incomplete relationships.

The graph also began to support documentation consistency mechanisms.

---

## 8.13. The Registry Evolves

With the introduction of relationships.

The Document Registry ceased to be merely a catalogue.

It became a knowledge repository.

Each entry came to contain.

* Metadata;
* status;
* relationships;
* history.

The Registry progressively assumed a central role within the framework architecture.

---

## 8.14. An Architecture Increasingly Similar to Software

Interestingly.

As the research progressed.

Documentation began to exhibit characteristics remarkably similar to those of a software system.

There were.

* entities;
* properties;
* relationships;
* lifecycles;
* validation.

Documentation definitively ceased to be merely text.

It became a structured system.

---

## 8.15. Research Status

At the end of this phase, several principles had been established.

* Every document can establish formal relationships.
* Relationships have their own identity.
* The documentation collection forms a Knowledge Graph.
* Navigation should prioritise knowledge rather than directories.
* The Registry represents a catalogue of knowledge.
* Documentation consistency can be automatically validated.

These ideas significantly reshaped the architecture of the Documentation Framework.

---

## 8.16. Next Steps

Despite the existence of a Knowledge Graph.

One essential element was still missing.

Documents evolved.

But that evolution did not yet follow a formal process.

New questions needed to be answered.

* Who approves a document?
* When may it be published?
* How does it transition between states?
* Who is responsible for each stage?

These questions would naturally lead to the emergence of the **Documentation Workflow**, responsible for formalising the entire document lifecycle.

---

## 8.17. Conclusion

The formalisation of **Document Relationships** represented one of the most significant milestones in the evolution of the Documentation Framework.

Documentation definitively ceased to be a collection of files connected by occasional references.

It became an explicit network of knowledge, where both documents and relationships possess their own identity, properties, and meaning.

It was this transformation that made it possible to understand documentation as a true **Knowledge Graph**, preparing the way for the formal definition of its lifecycle through the **Documentation Workflow**.

---

# 9. The Documentation Workflow and the Document Lifecycle

---

## 9.1. Introduction

The formalisation of relationships between documents made it possible to represent knowledge in a structured manner.

However.

One fundamental question still remained unresolved.

Documents evolve.

But how should that evolution occur?

Up to this point.

Changes had been made freely.

Without a clearly defined process.

It was precisely from this need that the concept of the **Documentation Workflow** emerged.

---

## 9.2. The Problem

For some time.

The evolution of a document depended entirely on its author.

A document could move directly from an initial idea to what was considered its final version.

Without review.

Without validation.

Without any formal mechanism.

Although adequate for small projects.

This approach proved insufficient.

---

## 9.3. Documents Also Have a Lifecycle

An important observation quickly emerged.

Documents behave in much the same way as software components.

They too.

* are created;
* evolve;
* stabilise;
* become obsolete;
* are archived.

Consequently.

Documents also require a formal lifecycle.

---

## 9.4. The First Model

Initially, an extremely simple workflow was proposed.

```text id="wf1"

				  Draft

					↓

				 Approved

```

This approach solved the problem only partially.

Between an initial idea and final approval, there were several important stages.

---

## 9.5. The Review Process

A new intermediate stage quickly emerged.

```text id="wf2"

				  Draft

					↓

				 Review

					↓

				Approved

```

The introduction of the review stage significantly improved the quality of the documentation.

For the first time.

The document no longer depended exclusively on its author.

---

## 9.6. The Discovery of States

As the research progressed, it became evident that a document does not change only in terms of its content.

It also changes its state.

For example.

```text id="wf3"

					Draft

					Review

					Approved

					Deprecated

					Archived

```

The state came to represent the document's position within its lifecycle.

---

## 9.7. State and Version Are Different Concepts

Initially, there was some confusion between these concepts.

It was soon concluded that.

The version describes the evolution of the content.

The state describes the maturity of the document.

This distinction proved to be extremely important.

---

## 9.8. Workflow as a Contract

Another conceptual evolution consisted of no longer considering the Workflow merely as a sequence of states.

It came to represent an organizational contract.

Each transition became governed by rules.

For example.

A document.

* cannot be approved without review;
* cannot be archived directly from the Draft state;
* should not arbitrarily return to previous states.

These rules significantly increased document consistency.

---

## 9.9. The Role of Responsibilities

During this phase, another question also emerged.

Who is allowed to change the state of a document?

Not every transition should be available to every user.

Responsibilities associated with the Workflow then began to emerge.

For example.

* author;
* reviewer;
* technical owner;
* approver.

This separation brought the Documentation Framework closer to software engineering processes.

---

## 9.10. Workflow as a Process

Another important discovery was the realization that the Workflow does not belong to the document.

It belongs to the documentation process.

The document progresses through the Workflow.

But it does not define it.

This distinction made it possible to reuse the same Workflow for different document types.

---

## 9.11. Knowledge Evolves Formally

A particularly interesting consequence was the realization that.

In reality.

It is not only the document that evolves.

It is the knowledge.

The document merely provides the medium for that evolution.

This observation brought the Workflow significantly closer to the future Change Management System.

---

## 9.12. Workflow and Baselines

The introduction of the Workflow also brought an important benefit to Baselines.

Only approved documents became eligible to be included in an official Baseline.

As a result.

Consistency no longer depended solely on the version.

It also depended on the state.

---

## 9.13. Process Automation

Another natural consequence was the possibility of automating several validations.

For example.

A tool could prevent.

* approval without review;
* inclusion of Draft documents in a Baseline;
* publication of Deprecated documents.

The Workflow ceased to be merely a concept.

It became something that could be executed automatically.

---

## 9.14. A New Perspective

During this phase, another particularly important idea began to emerge.

Documents do not evolve in isolation.

The evolution of one document frequently triggers the evolution of others.

The Workflow therefore began to reveal its limitations.

It became necessary to understand not only the evolution of a single document.

But the coordinated evolution of knowledge.

---

## 9.15. Research Status

At the end of this phase, several principles had been established.

* Every document has a lifecycle.
* State and version represent distinct concepts.
* The Workflow constitutes a process contract.
* Transitions are governed by rules.
* Responsibilities are part of the Workflow.
* Only approved documents may belong to a Baseline.
* The Workflow supports automation.

These decisions definitively consolidated the document evolution model.

---

## 9.16. Next Steps

The Workflow solved the individual evolution of documents.

However.

A broader question still remained.

How can this documentation system be integrated with the rest of the VisualEngine ecosystem?

How can architecture, code, documentation, and knowledge evolve in a coordinated manner?

These questions would lead directly to the integration of the Documentation Framework with the **VisualEngine**, the subject of the next stage of the research.

---

## 9.17. Conclusion

The creation of the **Document Workflow** represented a decisive step in the maturity of the Documentation Framework.

Documentation ceased to evolve informally and began to follow a clearly defined process, supported by states, rules, responsibilities, and validation mechanisms.

This formalization made it possible to treat documentation as an engineering process and naturally prepared the integration of the framework with the overall architecture of the VisualEngine, where documentation and development would evolve in a coordinated manner.

---

# 10. Integration with the VisualEngine

---

## 10.1. Introduction

Up to this point, the research had focused exclusively on the evolution of the Documentation Framework.

The main concepts had already been established.

* Templates;
* Metadata;
* Document Identity;
* META Documents;
* Baselines;
* Registry;
* Relationships;
* Workflow.

However, one fundamental question remained.

**How can this framework be integrated with the VisualEngine?**

It was precisely this question that led to a significant shift in perspective.

---

## 10.2. The Problem

Initially, the Documentation Framework was viewed as a collection of supporting documents.

The VisualEngine remained the primary project.

Documentation played only a supporting role.

However, as both evolved, it became evident that this view was too limited.

---

## 10.3. Documentation as Part of the Architecture

An important observation began to repeat itself.

Whenever an architectural decision was made.

The documentation had to be updated.

Whenever the documentation evolved.

It influenced new architectural decisions.

Code and documentation no longer evolved independently.

They became part of a single system.

---

## 10.4. A Bidirectional Relationship

Until then, it had been implicitly assumed that documentation followed the software.

However.

The research revealed a different model.

```text id="ve1"

			   VisualEngine

					↓

			   Documentation

					↓

			   VisualEngine

```

The architecture influences the documentation.

The documentation influences the architecture.

This relationship is bidirectional.

---

## 10.5. Documentation as a Component

A new hypothesis was then formulated.

Perhaps documentation should be considered a component of the architecture itself.

Not an external artifact.

But an integral part of the system.

This shift profoundly changed the role of the Documentation Framework.

---

## 10.6. Independence Is Preserved

Despite this integration.

An important principle was established.

The Documentation Framework must remain independent of the VisualEngine.

Conceptually.

```text id="ve2"

					VisualEngine

					Documentation Framework

```

Both collaborate.

But neither depends structurally on the other.

This independence would allow the framework to be reused in other projects.

---

## 10.7. Knowledge as the Interface

Another important discovery was the realization that the point of contact between the two is not the code.

It is the knowledge.

The VisualEngine produces knowledge.

The Documentation Framework organizes that knowledge.

This separation made the architecture much clearer.

---

## 10.8. The Architecture Becomes Documentable

Up to this stage.

The documentation described the architecture.

With the integration.

The architecture itself explicitly began to provide documentation mechanisms.

For example.

* documentable components;
* architectural decisions;
* contracts;
* interfaces.

Documentation ceased to be a subsequent reflection.

It became part of the architectural design itself.

---

## 10.9. The Role of META Documents

During this integration.

META Documents assumed a new level of importance.

They began to define.

* how to document components;
* how to document services;
* how to document APIs;
* how to document decisions.

META Documents no longer served only the Documentation Framework.

They also began to serve the VisualEngine.

---

## 10.10. The Value of Consistency

Another important consequence was the consistency between implementation and documentation.

Ideally.

An architectural decision.

A component.

A specification.

And its corresponding documentation.

Should evolve together.

This synchronization became a permanent objective.

---

## 10.11. The Documentation Framework as Infrastructure

It gradually became evident that.

Just as there is infrastructure for persistence.

Or for communication.

There can also be infrastructure for documentation.

The Documentation Framework began to be viewed as a cross-cutting service.

Not merely as a collection of documents.

---

## 10.12. Integration with the Laboratory

A particularly interesting idea emerged during this phase.

The results produced by the Laboratory could be documented automatically.

Experiments.

Results.

Observations.

Hypotheses.

Everything could directly feed the documentation ecosystem.

The Documentation Framework was beginning to move closer to scientific research.

---

## 10.13. Integration with the Domain Packages

Another important evolution consisted of associating documentation directly with the Domain Packages.

Each domain could potentially have its own.

* documentation;
* references;
* standards;
* research.

Knowledge became distributed.

But organized according to a common model.

---

## 10.14. The Discovery of Circularity

At the end of this phase, a particularly interesting observation emerged.

The Documentation Framework documents the VisualEngine.

The VisualEngine supports the evolution of the Documentation Framework.

Both evolve together.

This circularity does not constitute a problem.

It represents a relationship of co-evolution.

---

## 10.15. Research Status

At the end of this stage, several principles had been established.

* The Documentation Framework integrates with the VisualEngine architecture.
* Both remain structurally independent.
* Knowledge constitutes the primary point of integration.
* Documentation must evolve alongside the architecture.
* META Documents also support the VisualEngine.
* The framework represents a cross-cutting infrastructure.
* Architecture and documentation evolve in a coordinated manner.

These ideas definitively consolidated the position of the Documentation Framework within the project's ecosystem.

---

## 10.16. Next Steps

The integration with the VisualEngine revealed a new question.

If architecture and documentation evolve together.

Who governs that evolution?

The Workflow governs documents.

But it does not explain why documents change.

That answer would emerge only with the discovery of the **Change Management System (CMS)**.

For the first time, it became evident that both the VisualEngine and the Documentation Framework are merely specializations of a more general principle.

The explicit management of change.

---

## 10.17. Conclusion

The integration of the Documentation Framework with the VisualEngine marked the moment when they ceased to be viewed as separate projects.

They became complementary components of the same ecosystem.

The VisualEngine provides the technological context and produces knowledge.

The Documentation Framework organizes, preserves, and structures that knowledge.

This integration naturally prepared the next stage of the research, where the focus would shift away from documents and toward the true origin of their evolution: **change**.

---

# 11. The Discovery of Integration with the Change Management System

---

## 11.1. Introduction

The integration of the Documentation Framework with the VisualEngine made it possible to understand that both evolved in a coordinated manner.

However.

One question remained unanswered.

The Workflow explained **how** a document evolves.

But it did not explain **why** that evolution occurs.

This distinction proved to be far more important than initially expected.

It was precisely from this reflection that the connection between the Documentation Framework and the **Change Management System (CMS)** emerged.

---

## 11.2. The Limit of the Workflow

For a long time, it was believed that the Workflow represented the complete mechanism for document evolution.

Documents progressed through states.

* Draft;
* Review;
* Approved;
* Deprecated;
* Archived.

The process appeared to be complete.

However.

One simple question remained unanswered.

**What initiates that process?**

---

## 11.3. Before the Document, There Is a Change

Looking retrospectively at the evolution of the documentation revealed a consistent pattern.

No document was ever created spontaneously.

Every document came into existence because some change had occurred.

Or because a change was intended to occur.

For example.

* a new architecture;
* a change in requirements;
* a new convention;
* a technical decision.

Documentation proved to be a consequence.

Never the cause.

---

## 11.4. A New Hierarchy

Until this point, evolution had been understood as follows.

```text id="cms1"

				 Document

					↓

				 Workflow

					↓

			   New Version

```

With the new perspective.

The hierarchy became different.

```text id="cms2"

				  Change

					↓

				 Document

					↓

				 Workflow

					↓

			   New Version
```

This inversion profoundly transformed the entire conceptual architecture.

---

## 11.5. The Document as Evidence

Another important observation emerged naturally.

The document does not represent the change.

It represents the evidence of that change.

For example.

An architectural decision.

↓

Produces documentation.

↓

Produces implementation.

↓

Produces tests.

The document is merely one manifestation of the change.

---

## 11.6. The CMS as an Upper Layer

A new hypothesis was then formulated.

The Workflow belongs to the Documentation Framework.

But the reason for evolution belongs to the CMS.

Conceptually.

```text id="cms3"

		  Change Management System

					↓

		  Documentation Framework

					↓

				 Workflow

					↓

				Documents

```

This organization proved to be much more consistent.

---

## 11.7. The Workflow Remains Important

An immediate consequence of this discovery was the clarification of responsibilities.

The CMS does not replace the Workflow.

The Workflow remains responsible for the document lifecycle.

The CMS merely explains why that lifecycle was initiated.

Both perform distinct.

Yet complementary.

Functions.

---

## 11.8. Change as an Entity

Another important idea began to consolidate.

Just as a document has an identity.

A change should also have.

* identifier;
* state;
* impact;
* history.

Change gradually came to be treated as an independent entity.

---

## 11.9. Complete Traceability

With the integration of the CMS, it became possible to establish a complete traceability chain.

For example.

```text id="cms4"

				  Change

					↓

				 Document

					↓

			   Architecture

					↓

				   Code

					↓

				 Behavior

```

For the first time, it became possible to understand the complete origin of a decision.

---

## 11.10. The Role of META Documents

META Documents also acquired a new function.

In addition to defining documentation rules.

They began to establish how changes should be documented.

Documentation ceased to describe only systems.

It also began to describe evolution processes.

---

## 11.11. Baselines and Change

Another important consequence was the redefinition of Baselines.

A Baseline no longer represented only a coherent set of documents.

It also came to represent a coherent set of approved changes.

This interpretation proved to be considerably more robust.

---

## 11.12. The Evolution of Knowledge

During this phase, a particularly interesting idea became evident.

Neither the CMS manages documents.

Nor does the Documentation Framework manage files.

Both manage knowledge.

The CMS governs evolution.

The Documentation Framework governs representation.

This distinction made the architecture much more elegant.

---

## 11.13. A New Perspective

Looking at the research as a whole revealed a recurring sequence.

```text id="cms5"

				  Change

					↓

				Knowledge

					↓

			  Documentation

					↓

			  Implementation

```

This sequence came to explain virtually the entire evolution of the project.

---

## 11.14. Research Status

At the end of this phase, several fundamental principles had been established.

* All documentation results from a change.
* The Workflow governs documents.
* The CMS governs changes.
* Document and change represent distinct entities.
* Traceability must begin with the change.
* Baselines represent stabilized knowledge.
* The Documentation Framework and the CMS are complementary.

These conclusions permanently transformed the conceptual architecture of the framework.

---

## 11.15. Next Steps

With the integration of the CMS, virtually all the fundamental components of the Documentation Framework had been defined.

Only one final task remained.

To reflect on the entire journey.

To identify the principles that remained constant.

The most important decisions.

The lessons learned.

And the future lines of research.

This synthesis will constitute the final part of this **Research Journal**.

---

## 11.16. Conclusion

The integration with the **Change Management System** marked the moment when the Documentation Framework definitively ceased to be regarded merely as a documentation system.

It became part of a broader architecture dedicated to managing the evolution of knowledge.

Documents ceased to be viewed as isolated objects and came to represent formal manifestations of changes that occurred within the system.

This discovery completed the conceptual architecture of the Documentation Framework and naturally prepared the conclusion of this research journal.

---

# 12. Research Summary, Lessons Learned, and Future Perspectives

---

## 12.1. Introduction

Throughout this journal, the conceptual evolution that led to the creation of the **Documentation Framework** has been recorded.

The objective was never simply to create a collection of document templates.

The real objective proved to be far more ambitious.

To build an infrastructure capable of organizing, preserving, relating, and supporting the evolution of knowledge throughout the lifecycle of a project.

This final part summarizes that journey and identifies the principal conclusions reached during the research.

---

## 12.2. An Unplanned Evolution

As happened with the VisualEngine.

The Documentation Framework was not created as a complete solution.

Each component emerged to solve a limitation identified during the previous stage.

The evolution can be summarized as follows.

```

				Documents

					↓

				Templates

					↓

				 Metadata

					↓

			Document Identity

					↓

			 META Documents

					↓

				Baselines

					↓

				Registry

					↓

			   Relationships

					↓

				 Workflow

					↓

			  CMS Integration

```

Each stage preserved the principles established by the previous one.

While introducing a new level of abstraction.

---

## 12.3. The Real Problem

Initially, it was believed that the problem was organizing documents.

Later, it became evident that the real problem was organizing knowledge.

Documents are merely the medium through which knowledge is represented.

Knowledge itself is the true object of interest.

This change in perspective influenced every subsequent architectural decision.

---

## 12.4. The Discovery of Structure

The first Templates demonstrated that documentation consistency does not depend solely on the quality of its content.

It also depends on the existence of a common structure.

That structure reduced heterogeneity.

Simplified maintenance.

And prepared the foundation for future automation.

---

## 12.5. The Importance of Metadata

One of the most significant discoveries was the separation between.

* content;
* identity;
* document properties.

Metadata ceased to be regarded as auxiliary information.

It became an integral part of the document model.

This decision made document classification, validation, and traceability possible.

---

## 12.6. Permanent Identity

Another fundamental conclusion was the definitive separation between.

* identity;
* name;
* location.

Documents acquired a permanent identity.

Just like entities in a software system.

This decision proved essential for every subsequent evolution of the framework.

---

## 12.7. META Documents

The introduction of META Documents represented a turning point.

For the first time.

Documentation began documenting itself.

Rules no longer existed merely as implicit conventions.

They became formal knowledge.

Versioned.

Documented.

And continuously evolving.

---

## 12.8. Baselines

Baselines introduced a new concept.

The stable state of knowledge.

Instead of managing documents individually.

The framework began managing coherent sets of documents.

This approach brought the Documentation Framework much closer to configuration engineering principles.

---

## 12.9. The Registry

The Document Registry completely changed the way documentation is navigated.

Documentation was no longer simply a collection of files.

It became a formal catalog of knowledge.

Documentation became searchable.

Discoverable.

And verifiable.

---

## 12.10. The Knowledge Graph

The formalization of document relationships revealed a new reality.

The complete document collection forms a network.

Each document represents a node.

Each relationship represents additional knowledge.

This perspective brought the Documentation Framework closer to modern knowledge management systems.

---

## 12.11. Workflow

Workflow introduced a temporal dimension.

Documents acquired.

* states;
* responsibilities;
* transitions;
* rules.

Documentation ceased to be static.

It became an entity with a formal lifecycle.

---

## 12.12. Integration with the VisualEngine

Another important discovery was understanding that documentation and architecture evolve together.

Neither completely describes the other.

Both are part of the same ecosystem.

This integration consolidated the role of the Documentation Framework as a cross-cutting infrastructure.

---

## 12.13. The Role of the CMS

Integration with the Change Management System finally answered the question that had remained unresolved from the beginning.

Why do documents evolve?

The answer proved to be simple.

Because knowledge evolves.

Documentation merely represents the consequence of that evolution.

This conclusion permanently transformed the conceptual architecture of the framework.

---

## 12.14. Fundamental Principles

Looking back over the entire research journey.

Several principles remained constant.

* Documentation represents knowledge.
* Knowledge requires structure.
* Every document possesses identity.
* Metadata is part of the document.
* Documentation should be treated as a system.
* Relationships are as valuable as the documents themselves.
* Knowledge evolves through change.

These principles now constitute the foundation of the Documentation Framework.

---

## 12.15. Lessons Learned

Throughout the development process, several engineering lessons were also learned.

Among them.

* Informal conventions deteriorate rapidly.
* Consistency should be defined through explicit rules.
* Documentation requires architecture.
* Automation depends on structure.
* Traceability should be designed from the beginning.
* Knowledge should remain independent of its representation.

These observations strongly influenced the final architecture.

---

## 12.16 Future Perspectives

Despite the level of maturity currently achieved.

Several research directions remain open.

For example.

* automatic validation of documentation consistency;
* automatic documentation generation;
* integration with development tools;
* semantic knowledge representation;
* visualization of the documentation graph;
* deeper integration with the CMS;
* the use of Artificial Intelligence for documentation analysis.

These areas represent natural opportunities for future evolution.

---

## 12.17. A New Way of Understanding Documentation

Perhaps the most important conclusion of this research is precisely this.

Documentation should not be regarded as a final deliverable.

Nor as an administrative obligation.

It should be considered a knowledge infrastructure.

Just as there is infrastructure for persistence.

Or for communication.

There can also be infrastructure for documentation.

It is precisely that infrastructure that this project set out to build.

---

## 12.18. Final Considerations

The Documentation Framework originated from the need to organize documents.

But ultimately evolved into an architecture dedicated to organizing knowledge.

Throughout this journey.

Documents ceased to be viewed as Markdown files.

They became entities with their own identity, properties, relationships, and lifecycle.

More importantly.

This research demonstrated that documentation can be designed with the same architectural rigor applied to software engineering.

---

## 12.19. Closing Remarks

This concludes the **Research Journal** of the Documentation Framework.

This document has recorded the evolution of the ideas that gave rise to the framework, preserving not only the solutions that were discovered but also the reasoning process that led to its current architecture.

As with the VisualEngine, this journal does not represent the end of the research.

It merely represents the current state of knowledge.

New discoveries will inevitably lead to new abstractions.

And those abstractions will, in turn, give rise to new ways of understanding, representing, and managing documentary knowledge.

---

**End of Document**