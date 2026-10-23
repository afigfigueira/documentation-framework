# Documentation Framework

# DF-CLS-013 — Classification Dictionary

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-013 |
| **Title** | Classification Dictionary |
| **Family** | Classification |
| **Type** | Reference |
| **Component** | Classification |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Introduction

The Classification Dictionary defines the canonical terminology used by the Classification component of the Documentation Framework.

Classification provides the semantic organization through which documents are grouped into meaningful categories.

The Dictionary establishes a common vocabulary for the concepts, elements, relationships and supporting terms used by Classification.

Its purpose is to ensure that the same terminology is used consistently across:

- Classification documents;
- document metadata;
- validation;
- governance;
- relationships;
- extensions;
- specifications;
- examples;
- automation.

The Classification Dictionary is therefore a terminology reference.

It does not replace the Classification Model, Schema, Constraints or Specification.

**Current sourced scope.**

Actual primary responsibility is terminology consultation with scoped working authoritative semantic definitions. Type Reference/current04-Reference remains correct under ReviewPolicy3.1/ARC00710. This Draft and canonical wording neither approve/publish definitions nor establish a complete populated vocabulary. Actual source/definition editions,scope,authority/applicability and owner conditions matter;adopted working correction is not actual canonical adoption.

---

# 2. Purpose

The purpose of this document is to provide a single authoritative vocabulary for Classification.

The Dictionary supports:

- semantic consistency;
- terminology normalization;
- unambiguous communication;
- documentation consistency;
- validation;
- governance;
- Classification maintenance;
- controlled evolution.

The Dictionary follows the Single Source of Truth principle.

A term defined here should not acquire a competing definition elsewhere in the Classification documentation.

**Current sourced scope.**

One authoritative meaning in actual context does not prohibit explicit necessary assessed definition/mandate revision. Preserve actual earlier definition/source editions and pinned history;do not retain contradictory same-context current rules or infer approval from an entry/name. Actual domain/common/Metadata/Identity owners remain distinct.

---

# 3. Scope

The Dictionary covers terminology associated with:

- Classification;
- Classification structure;
- Classification elements;
- Classification relationships;
- Classification schema;
- Classification lifecycle;
- Classification validation;
- Classification governance;
- Classification constraints;
- Classification extensibility.

It also defines the terminology necessary to describe the use and maintenance of Classification.

The Dictionary does not define the complete normative behavior of Classification.

That responsibility belongs to the applicable architectural and specification documents.

**Current sourced scope.**

Actual terminology authority is scoped,not complete behavioral/representation/implementation certification. Definition,concept,category/value,assignment/association/assertion,term/name/label,record and document K/local R/exact edition differ. Functional README/CHANGELOG/ArchitecturalMilestones remain non-normalized with applicable content/reference effects,no DF IDs allocated to them or every glossary entity.

---

# 4. Dictionary Conventions

Each dictionary entry contains:

| Field | Received purpose | Current representation / authority scope |
|---|---|---|
| **Term** | Canonical terminology  | Term is actual entry heading,not an allocated identity/Metadata field. |
| **Definition** | Authoritative meaning  | Actual working definition/source edition/scope under responsible owner authority,not canonical adoption from presence. |
| **Context** | Classification context in which the term is used  | Actual semantic/applicability/source-edition context,not universal physical field or arbitrary document-specific redefinition. |
| **Related Terms** | Closely related concepts  | Actual201 occurrence-level related references below;exact local/contextual/external/genuine-limit dispositions,no automatic alias or dependency. |
| **Notes** | Additional clarification where required  | Conditional entry clarification now supplies actual scope/history/owner/reference limits;not universally allocated required Notes field. |

Definitions should be:

- concise;
- semantic;
- unambiguous;
- independent of implementation technology;
- consistent with the Classification architecture.

**Current sourced scope.**

All five original convention rows retain received purposes beside current interpretation. Actual73 entry terms are headings;Definition/Context/Related Terms are actual blocks,Notes conditional and now used for needed scope. No mandatory literal Term field,complete Metadata schema or missing-field finding from original absent optional Notes is invented.

---

# 5. Core Classification Terms

## 5.1. Classification

**Definition**

A semantic mechanism used to organize documents according to meaningful categories and characteristics defined by the Documentation Framework.

**Context**

Classification component.

**Related Terms**

- Classification Element
- Classification Model
- Classification Schema
- Classification Type

**Notes**

Actual Classification domain conceptual/structural responsibility and current source-edition context remain distinct from common architectural concepts/components and Metadata representation. Definitions do not allocate components,approved populations or document/field IDs;actual Model provenance is reconstruction,not authentic recovered history.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Model | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Model definition/context in§5.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Type | Explicit contextual local phrase,not an allocated canonical alias: Contextual qualified phrase for primary document Type in5.1;uniform four-value responsibility,not additional primary kind or an approved alias registry. | Actual local entry§6.3 in this occurrence context;original literal retained,no independently allocated entry/alias. |

---

## 5.2. Classification Component

**Definition**

The Documentation Framework component responsible for defining and governing the semantic classification of documents.

**Context**

Documentation Layer.

**Related Terms**

- Classification
- Documentation Component
- Metadata Component

**Notes**

Actual Classification domain conceptual/structural responsibility and current source-edition context remain distinct from common architectural concepts/components and Metadata representation. Definitions do not allocate components,approved populations or document/field IDs;actual Model provenance is reconstruction,not authentic recovered history.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification definition/context in§5.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Documentation Component | External architectural grouping,not new component: ARC0055 actually groups the supplied documentation components;this related phrase is that context,not an allocated fifth component or new local term entry. | DF-ARC-005 V2.0 R2 §5;actual current owner context,not new local canonical entry. |
| Metadata Component | External actual component owner: ARC0055.1 actually identifies Metadata and responsibilities. This is a related external owner reference,not a new Classification component or transferred definition authority. | DF-ARC-005 V2.0 R2 §5.1;actual current owner context,not new local canonical entry. |

---

## 5.3. Classification Architecture

**Definition**

The architectural definition of the Classification component, including its purpose, responsibilities, boundaries and relationships with other Framework concepts.

**Context**

Classification architecture.

**Related Terms**

- Classification Model
- Classification Schema
- Classification Specification

**Notes**

Actual Classification domain conceptual/structural responsibility and current source-edition context remain distinct from common architectural concepts/components and Metadata representation. Definitions do not allocate components,approved populations or document/field IDs;actual Model provenance is reconstruction,not authentic recovered history.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Model | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Model definition/context in§5.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Specification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Specification definition/context in§19.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 5.4. Classification Concept

**Definition**

A conceptual entity representing a meaningful idea required to understand or define Classification.

**Context**

Classification conceptual model.

**Related Terms**

- Concept
- Classification Element
- Classification Model

**Notes**

Actual Classification domain conceptual/structural responsibility and current source-edition context remain distinct from common architectural concepts/components and Metadata representation. Definitions do not allocate components,approved populations or document/field IDs;actual Model provenance is reconstruction,not authentic recovered history.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Concept | External conceptual context,not an allocated local synonym: Generic architectural concept context under ARC0034/5;Classification Concept5.4 remains the local domain concept. No distinct local Concept entry or complete external concept registry is invented. | DF-ARC-003 V2.0 R2 §4;actual current owner context,not new local canonical entry. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Model | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Model definition/context in§5.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 5.5. Classification Model

**Definition**

The conceptual and structural model describing the entities and relationships that constitute Classification.

**Context**

Classification model.

**Related Terms**

- Classification Concept
- Classification Element
- Classification Schema

**Notes**

Actual Classification domain conceptual/structural responsibility and current source-edition context remain distinct from common architectural concepts/components and Metadata representation. Definitions do not allocate components,approved populations or document/field IDs;actual Model provenance is reconstruction,not authentic recovered history.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Concept | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Concept definition/context in§5.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 6. Classification Element Terms

## 6.1. Classification Element

**Definition**

A defined domain semantic unit,category or role/value definition used in Classification within actual responsible scope;the definition,an assigned value or association and its physical record/document are distinct subjects.

**Context**

Classification model.

**Related Terms**

- Family
- Type
- Class
- Classification Value

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Value | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Value definition/context in§6.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.6 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.2. Family

**Definition**

The actual canonical component membership or explicitly admitted documentary-area membership of an applicable normalized document;Family does not own or specialize the uniform primary Type vocabulary.

**Context**

Actual component/admitted documentary-area membership,not universal role hierarchy.

**Related Terms**

- Type
- Class
- Classification Element

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

Current Family identifies actual canonical component/admitted documentary-area membership. It does not create an area/component by listing it or own primary Type;valid identity/series is not recalculated.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.3. Type

**Definition**

Exactly one primary documentary responsibility selected uniformly from Architecture,Structure,Behavior or Reference for each applicable normalized document,independent of Family-owned specialization.

**Context**

Uniform primary documentary responsibility and actual applicable context.

**Related Terms**

- Family
- Class
- Classification Element

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

Exactly one uniform primary documentary responsibility is known. Actual Family-context valid-use restrictions do not specialize that vocabulary;relationship Type is kind,not primary document Type. Necessary mandate revision requires real prior/new authority,no routine fifth value.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.4. Class

**Definition**

A separate optional explicitly defined non-conflicting semantic distinction used in actual context,not a universal Type-child level or mandatory third Classification field/value.

**Context**

Optional explicitly defined semantic dimension and actual scheme/context.

**Related Terms**

- Family
- Type
- Classification Element

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

Class is optional,not unrestricted. Any used meaning needs explicit nonconflicting definition/context,no mandatory third field/value,universal Type parent,complete population or known general maximum.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.5. Classification Category

**Definition**

A semantic grouping represented by a Classification Element.

**Context**

General Classification terminology.

**Related Terms**

- Classification Element
- Family
- Type
- Class

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.6. Classification Value

**Definition**

A value assigned to a document or classification context according to the applicable Classification Schema.

**Context**

Classification assignment.

**Related Terms**

- Classification Element
- Classification Assignment
- Classification Schema

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Assignment | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Assignment definition/context in§6.7;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.7 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 6.7. Classification Assignment

**Definition**

An actual association or assertion connecting an identified document/entity/edition subject with applicable Classification definitions or values under responsible rules;definition,assigned value,assertion and record identity remain distinct.

**Context**

Classification usage.

**Related Terms**

- Classification Element
- Classification Value
- Document

**Notes**

Actual role/category/value/definition/assignment subjects differ. Membership Family,exactly one uniform Architecture/Structure/Behavior/Reference primary Type and optional explicitly defined nonconflicting Class apply under current Model/Elements/Schema34. General relation/assignment/population/field detail remains genuinely incomplete;known duties are not deferred and arbitrary counts/strings/all-pairs permission are not supplied.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Value | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Value definition/context in§6.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.6 plus its current sourced notes;working definition is not proof canonical adoption. |
| Document | External actual owner context: Actual Document concept under ARC0035.3;document K/exact edition/local R is separately governed by Identity. This related label does not turn every domain entity into a DF document. | DF-ARC-003 V2.0 R2 §5.3;actual current owner context,not new local canonical entry. |

---

# 7. Structural Terms

## 7.1. Classification Hierarchy

**Definition**

An actually defined scheme-specific arrangement of Classification subjects with responsible hierarchical relation/position semantics;documentary Family,primary Type and optional Class do not impose a universal specialization tree.

**Context**

Actual explicitly defined Classification scheme/relationship structure.

**Related Terms**

- Family
- Type
- Class
- Parent Element
- Child Element

**Notes**

Hierarchy/parent/child/level/specialization applies only to actual explicitly defined scheme/kind/endpoint semantics and responsible properties/cardinality constraints. Current complementary documentary roles impose no universal Family-owned tree. Real hierarchical/prohibited-cycle/ancestor duties remain;semantic/inverse/navigation/record/projection and indispensable provider graphs differ,no global DAG or renamed-away required cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Parent Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Parent Element definition/context in§7.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Child Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Child Element definition/context in§7.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 7.2. Parent Element

**Definition**

An actual broader or source-side hierarchical subject under a responsible scheme/relation definition and scope,not automatically the owner of documentary Type or Class.

**Context**

Actual scheme-specific hierarchical relation/endpoint context.

**Related Terms**

- Child Element
- Classification Hierarchy

**Notes**

Hierarchy/parent/child/level/specialization applies only to actual explicitly defined scheme/kind/endpoint semantics and responsible properties/cardinality constraints. Current complementary documentary roles impose no universal Family-owned tree. Real hierarchical/prohibited-cycle/ancestor duties remain;semantic/inverse/navigation/record/projection and indispensable provider graphs differ,no global DAG or renamed-away required cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Child Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Child Element definition/context in§7.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Hierarchy | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Hierarchy definition/context in§7.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 7.3. Child Element

**Definition**

An actual narrower or target-side hierarchical subject under a responsible scheme/relation definition and scope,not a mandatory documentary Class child.

**Context**

Actual scheme-specific hierarchical relation/endpoint context.

**Related Terms**

- Parent Element
- Classification Hierarchy

**Notes**

Hierarchy/parent/child/level/specialization applies only to actual explicitly defined scheme/kind/endpoint semantics and responsible properties/cardinality constraints. Current complementary documentary roles impose no universal Family-owned tree. Real hierarchical/prohibited-cycle/ancestor duties remain;semantic/inverse/navigation/record/projection and indispensable provider graphs differ,no global DAG or renamed-away required cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Parent Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Parent Element definition/context in§7.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Hierarchy | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Hierarchy definition/context in§7.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 7.4. Classification Level

**Definition**

An actual defined position in a responsible Classification scheme/hierarchical relation context,not a compulsory universal Family–Type–Class level or physical field.

**Context**

Actual defined scheme position,not universal documentary roles.

**Related Terms**

- Classification Hierarchy
- Family
- Type
- Class

**Notes**

Hierarchy/parent/child/level/specialization applies only to actual explicitly defined scheme/kind/endpoint semantics and responsible properties/cardinality constraints. Current complementary documentary roles impose no universal Family-owned tree. Real hierarchical/prohibited-cycle/ancestor duties remain;semantic/inverse/navigation/record/projection and indispensable provider graphs differ,no global DAG or renamed-away required cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Hierarchy | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Hierarchy definition/context in§7.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Family | Exact original local entry title,actual current definition/context qualified: Related to the actual current Family definition/context in§6.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Type definition/context in§6.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Class | Exact original local entry title,actual current definition/context qualified: Related to the actual current Class definition/context in§6.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 7.5. Semantic Specialization

**Definition**

An explicitly defined scheme-specific refinement between broader and more-specific meanings under responsible authority,not an automatic inheritance relation among the current documentary roles.

**Context**

Actual responsible scheme-specific semantic refinement.

**Related Terms**

- Parent Element
- Child Element
- Classification Hierarchy

**Notes**

Hierarchy/parent/child/level/specialization applies only to actual explicitly defined scheme/kind/endpoint semantics and responsible properties/cardinality constraints. Current complementary documentary roles impose no universal Family-owned tree. Real hierarchical/prohibited-cycle/ancestor duties remain;semantic/inverse/navigation/record/projection and indispensable provider graphs differ,no global DAG or renamed-away required cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Parent Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Parent Element definition/context in§7.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Child Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Child Element definition/context in§7.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Hierarchy | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Hierarchy definition/context in§7.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 8. Identity and Naming Terms

## 8.1. Classification Identifier

**Definition**

A stable identifier used to uniquely identify a Classification Element.

**Context**

Classification identity.

**Related Terms**

- Classification Element
- Classification Name

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Name | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Name definition/context in§8.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.2. Classification Name

**Definition**

The canonical human-readable name assigned to a Classification Element.

**Context**

Classification terminology.

**Related Terms**

- Classification Identifier
- Classification Label

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Identifier | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Identifier definition/context in§8.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Label | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Label definition/context in§8.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.3. Classification Label

**Definition**

A human-readable representation of a Classification Element intended for presentation or user interaction.

**Context**

Classification presentation.

**Related Terms**

- Classification Name
- Classification Identifier

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Name | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Name definition/context in§8.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Identifier | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Identifier definition/context in§8.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.4. Canonical Term

**Definition**

The authoritative term selected to represent a Classification concept within the Documentation Framework.

**Context**

Classification Dictionary.

**Related Terms**

- Preferred Term
- Synonym
- Classification Name

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Preferred Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Preferred Term definition/context in§8.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Synonym | Exact original local entry title,actual current definition/context qualified: Related to the actual current Synonym definition/context in§8.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.6 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Name | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Name definition/context in§8.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.5. Preferred Term

**Definition**

The term recommended for normal use when referring to a Classification concept.

**Context**

Classification terminology.

**Related Terms**

- Canonical Term
- Synonym

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Synonym | Exact original local entry title,actual current definition/context qualified: Related to the actual current Synonym definition/context in§8.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.6 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.6. Synonym

**Definition**

An alternative term that refers to the same Classification concept as a canonical term.

**Context**

Classification vocabulary.

**Related Terms**

- Canonical Term
- Preferred Term

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Preferred Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Preferred Term definition/context in§8.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 8.7. Deprecated Term

**Definition**

A previously accepted term retained for historical interpretation and ordinarily discouraged for new canonical naming in its actual deprecated scope;legitimate historical,quoted or pinned-edition references remain governed by their actual reference/use/retention contracts.

**Context**

Actual term-use authority,definition/source edition and historical reference scope.

**Related Terms**

- Deprecated Element
- Retired Term

**Notes**

Actual concept/term/name/label/definition/source edition/alias scope and authority differ from entity/assignment/assertion/record/document K/local complete R/exact edition. Identity/naming obligations do not populate a universal registry or allocate DF/Metadata keys/fields. Synonyms require actual same-meaning/context evidence;names or physical copies alone prove no collision,merge,canonical adoption or pinned-target retargeting.

Normal new canonical naming versus actual legitimate historical/quoted/pinned reference is distinguished. Deprecated Term and Deprecated Element11.4 are different subjects;Retired Term is contextual§24 status,no separately allocated entry or complete universal term machine.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Deprecated Element | Explicit contextual local phrase,not an allocated canonical alias: Contextual Element/definition state subject in8.7;not an alias of Deprecated Term or a separately allocated local canonical term. Actual state/use/history duties apply. | Actual local entry§11.4 in this occurrence context;original literal retained,no independently allocated entry/alias. |
| Retired Term | Explicit contextual term-use status reference;no exact standalone local entry: This8.7 related phrase concerns actual Retired term-use status in§24,not Element Retired11.5. No separate canonical Retired Term entry or universal retirement definition/transition is fabricated. Required history/pinned references and actual owner authority remain. | Actual received§24 Retired term-status row,qualified current term-state/use matrix;Constraints67/74/75 and Lifecycle/Extensibility owner duties. |

---

# 9. Definition Terms

## 9.1. Classification Definition

**Definition**

The authoritative semantic description of a Classification Element.

**Context**

Classification Dictionary.

**Related Terms**

- Classification Element
- Canonical Term

**Notes**

Actual definition/source edition,stable meaning,explicit scope/applicability/contextual valid use and responsible authority/evidence differ. Unknown applicability/checks is no NotApplicable/Satisfied/Violated/permission;no invented scope tag conceals a real same-context conflict. Meaning independence retains actual descriptor/Profile/physical/reference/interface/access/retrieval/history duties,not universal context fields.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 9.2. Semantic Meaning

**Definition**

The conceptual meaning represented by a Classification Element independently of its physical representation or implementation.

**Context**

Classification semantics.

**Related Terms**

- Classification Definition
- Classification Concept

**Notes**

Actual definition/source edition,stable meaning,explicit scope/applicability/contextual valid use and responsible authority/evidence differ. Unknown applicability/checks is no NotApplicable/Satisfied/Violated/permission;no invented scope tag conceals a real same-context conflict. Meaning independence retains actual descriptor/Profile/physical/reference/interface/access/retrieval/history duties,not universal context fields.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Concept | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Concept definition/context in§5.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 9.3. Classification Scope

**Definition**

The semantic boundary within which a Classification Element is applicable.

**Context**

Classification definition.

**Related Terms**

- Classification Definition
- Classification Constraint

**Notes**

Actual definition/source edition,stable meaning,explicit scope/applicability/contextual valid use and responsible authority/evidence differ. Unknown applicability/checks is no NotApplicable/Satisfied/Violated/permission;no invented scope tag conceals a real same-context conflict. Meaning independence retains actual descriptor/Profile/physical/reference/interface/access/retrieval/history duties,not universal context fields.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 9.4. Classification Context

**Definition**

The conceptual environment in which a Classification term or element is interpreted.

**Context**

Classification terminology.

**Related Terms**

- Classification Scope
- Classification Definition

**Notes**

Actual definition/source edition,stable meaning,explicit scope/applicability/contextual valid use and responsible authority/evidence differ. Unknown applicability/checks is no NotApplicable/Satisfied/Violated/permission;no invented scope tag conceals a real same-context conflict. Meaning independence retains actual descriptor/Profile/physical/reference/interface/access/retrieval/history duties,not universal context fields.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Scope | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Scope definition/context in§9.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 10. Schema Terms

## 10.1. Classification Schema

**Definition**

The formal structural definition governing the representation and organization of Classification.

**Context**

Classification schema.

**Related Terms**

- Classification Model
- Classification Element
- Classification Constraint

**Notes**

Domain structural definition/attribute/cardinality concerns differ from mandatory physical Metadata fields or complete represented Schema/Profile/Instance. Known Schema34/current roles and actual defined endpoint/property/count/constraint rules remain alongside genuine general multiplicity/population/representation gaps,no arbitrary maxima,all-pairs permission or blanket known-duty deferral.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Model | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Model definition/context in§5.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§5.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 10.2. Schema Element

**Definition**

A structural component defined by the Classification Schema.

**Context**

Classification schema.

**Related Terms**

- Classification Element
- Schema

**Notes**

Domain structural definition/attribute/cardinality concerns differ from mandatory physical Metadata fields or complete represented Schema/Profile/Instance. Known Schema34/current roles and actual defined endpoint/property/count/constraint rules remain alongside genuine general multiplicity/population/representation gaps,no arbitrary maxima,all-pairs permission or blanket known-duty deferral.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Schema | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Schema shorthand in10.2,not an unqualified Metadata/physical representation schema or complete fields. | Actual local entry§10.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |

---

## 10.3. Classification Attribute

**Definition**

A defined property associated with a Classification Element or Classification structure.

**Context**

Classification schema.

**Related Terms**

- Classification Element
- Classification Schema

**Notes**

Domain structural definition/attribute/cardinality concerns differ from mandatory physical Metadata fields or complete represented Schema/Profile/Instance. Known Schema34/current roles and actual defined endpoint/property/count/constraint rules remain alongside genuine general multiplicity/population/representation gaps,no arbitrary maxima,all-pairs permission or blanket known-duty deferral.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 10.4. Classification Cardinality

**Definition**

A constraint describing the permitted number of occurrences or associations of a Classification element or relationship.

**Context**

Classification schema and constraints.

**Related Terms**

- Classification Constraint
- Relationship
- Multiplicity

**Notes**

Domain structural definition/attribute/cardinality concerns differ from mandatory physical Metadata fields or complete represented Schema/Profile/Instance. Known Schema34/current roles and actual defined endpoint/property/count/constraint rules remain alongside genuine general multiplicity/population/representation gaps,no arbitrary maxima,all-pairs permission or blanket known-duty deferral.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Relationship concern in10.4;actual kind/definition/association/assertion/endpoints and common record/providers remain separately typed. | Actual local entry§14.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |
| Multiplicity | Contextual concern with genuine general-detail gap: Related occurrence10.4 concerns cardinality/association counts under current Relationships20/Constraints28. No separate universal Multiplicity term definition,complete general minima/maxima or registered global synonym is supplied;known duties and actual missing count/representation detail remain. | DF-CLS-009 V2.0 R1 §20;actual current owner context,not new local canonical entry. |

---

# 11. Lifecycle Terms

## 11.1. Classification Lifecycle

**Definition**

The actual subject-specific state/use/transition/history contract for Classification Elements or definitions and their relevant assignments under responsible rules,not a universal lifecycle of every term,document,decision or extension.

**Context**

Classification lifecycle.

**Related Terms**

- Lifecycle State
- Active
- Deprecated
- Retired

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Lifecycle State | Exact original local entry title,actual current definition/context qualified: Related to the actual current Lifecycle State definition/context in§11.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Active | Exact original local entry title,actual current definition/context qualified: Related to the actual current Active definition/context in§11.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Deprecated | Exact original local entry title,actual current definition/context qualified: Related to the actual current Deprecated definition/context in§11.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Retired | Exact original local entry title,actual current definition/context qualified: Related to the actual current Retired definition/context in§11.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 11.2. Lifecycle State

**Definition**

A defined state representing the current lifecycle condition of a Classification Element.

**Context**

Classification lifecycle.

**Related Terms**

- Classification Lifecycle
- Active
- Deprecated
- Retired

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Lifecycle | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Lifecycle definition/context in§11.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Active | Exact original local entry title,actual current definition/context qualified: Related to the actual current Active definition/context in§11.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Deprecated | Exact original local entry title,actual current definition/context qualified: Related to the actual current Deprecated definition/context in§11.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Retired | Exact original local entry title,actual current definition/context qualified: Related to the actual current Retired definition/context in§11.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 11.3. Active

**Definition**

A bounded Element-definition/use state of eligibility for ordinary use in an admitted scope under actual valid/authorized definition rules and required decision/evidence;it proves neither every assignment valid/permitted nor live availability.

**Context**

Actual bounded Element/definition state and ordinary-use eligibility.

**Related Terms**

- Lifecycle State
- Deprecated

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

Active eligibility under actual scope does not mean every assignment satisfies all rules,operations are authorized,or a current endpoint is live retrievable. Supported invalidity/current-use requirements remain separately checked.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Lifecycle State | Exact original local entry title,actual current definition/context qualified: Related to the actual current Lifecycle State definition/context in§11.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Deprecated | Exact original local entry title,actual current definition/context qualified: Related to the actual current Deprecated definition/context in§11.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 11.4. Deprecated

**Definition**

A lifecycle state indicating that a Classification Element remains recognized but should not normally be used for new Classification assignments.

**Context**

Classification lifecycle.

**Related Terms**

- Active
- Retired
- Deprecated Term

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

Actual ordinary new-use restrictions and permitted historical context apply under owner rules. Deprecated Element differs from Deprecated Term;no automatic assignment/document/term retirement,warning/grandfathering or live availability guarantee.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Active | Exact original local entry title,actual current definition/context qualified: Related to the actual current Active definition/context in§11.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Retired | Exact original local entry title,actual current definition/context qualified: Related to the actual current Retired definition/context in§11.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Deprecated Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Deprecated Term definition/context in§8.7;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.7 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 11.5. Retired

**Definition**

A bounded Element-definition/use state in which ordinary new use is not admitted in the actual retired scope,while required historical meaning and existence remain preserved under responsible rules.

**Context**

Actual scoped Element/definition retirement and required historical use.

**Related Terms**

- Deprecated
- Historical Classification

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

Actual retired subject/source edition/effective scope and separate decision/conditions/effects matter. Required historical meaning remains;retired current-use eligibility is no all-context deletion or blanket prohibition of legitimate pinned historical references.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Deprecated | Exact original local entry title,actual current definition/context qualified: Related to the actual current Deprecated definition/context in§11.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Historical Classification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Historical Classification definition/context in§11.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.6 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 11.6. Historical Classification

**Definition**

A Classification assignment or element preserved to maintain the interpretation of previously established documentation.

**Context**

Classification evolution and Baselines.

**Related Terms**

- Retired
- Baseline
- Traceability

**Notes**

Actual Element/definition/assignment state/use/transition/history under Lifecycle19/20/48/53 differs from term naming/authority/use,extension/proposal/decision/activation,kind/association/constraint-set,document Workflow,term/local R/result/finding/Milestone states. Known mandates and genuine exact actors/guards/routes/records gaps remain;selected labels create no aliases,universal machine,automatic event/severity/permission or grandfathering.

Required historical interpretation is not proof original conformity,current permission or live retrieval. Preserve actual source/definition/rule/assignment/context and original observations,no backdated new rules or automatic reassignment.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Retired | Exact original local entry title,actual current definition/context qualified: Related to the actual current Retired definition/context in§11.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.5 plus its current sourced notes;working definition is not proof canonical adoption. |
| Baseline | Exact original local entry title,actual current definition/context qualified: Related to the actual current Baseline definition/context in§18.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Traceability | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Traceability concern in11.6/18.3;actual common AP012 and responsible history/source-edition requirements retain independent scope. | Actual local entry§18.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |

---

# 12. Validation Terms

## 12.1. Classification Validation

**Definition**

Actual nonmutating comparison of an identified Classification subject/structure/assignment and relevant context against applicable responsible rules,with source/definition/rule-set editions,authority,observations and required coverage supporting the asserted breadth.

**Context**

Classification validation.

**Related Terms**

- Classification Constraint
- Validation Rule
- Conformance

**Notes**

Actual Validation16/39/67 and Constraints46/56 distinguish supported criterion observations from three rule-dependent aggregate results with actual rule/definition/set/source/subject editions,scope/applicability/authority,observations/executor and performed/unperformed mandatory coverage. Known violations remain;missing support withholds unsupported breadth without fabricated Invalid/Violation/NotApplicable/outcome/severity/waiver. Evaluation is nonmutating,separate from recording,correction,decision and authorized operation;subset/local PASS proves no complete Core/implementation/global acceptance or permission.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Validation Rule | Exact original local entry title,actual current definition/context qualified: Related to the actual current Validation Rule definition/context in§12.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Conformance | Exact original local entry title,actual current definition/context qualified: Related to the actual current Conformance definition/context in§12.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 12.2. Validation Rule

**Definition**

A defined condition used to determine whether a Classification structure or assignment is valid.

**Context**

Classification validation.

**Related Terms**

- Classification Validation
- Classification Constraint

**Notes**

Actual Validation16/39/67 and Constraints46/56 distinguish supported criterion observations from three rule-dependent aggregate results with actual rule/definition/set/source/subject editions,scope/applicability/authority,observations/executor and performed/unperformed mandatory coverage. Known violations remain;missing support withholds unsupported breadth without fabricated Invalid/Violation/NotApplicable/outcome/severity/waiver. Evaluation is nonmutating,separate from recording,correction,decision and authorized operation;subset/local PASS proves no complete Core/implementation/global acceptance or permission.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Validation | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Validation definition/context in§12.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 12.3. Validation Result

**Definition**

An actual supported evaluation outcome within identified subject/rule/source/definition/set editions,scope/applicability,authority,observations and coverage;criterion observations differ from the three rule-dependent aggregate results Valid,Valid with Warnings and Invalid.

**Context**

Actual criterion/aggregate evaluation result and supported breadth.

**Related Terms**

- Validation Rule
- Classification Validation

**Notes**

Actual Validation16/39/67 and Constraints46/56 distinguish supported criterion observations from three rule-dependent aggregate results with actual rule/definition/set/source/subject editions,scope/applicability/authority,observations/executor and performed/unperformed mandatory coverage. Known violations remain;missing support withholds unsupported breadth without fabricated Invalid/Violation/NotApplicable/outcome/severity/waiver. Evaluation is nonmutating,separate from recording,correction,decision and authorized operation;subset/local PASS proves no complete Core/implementation/global acceptance or permission.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Validation Rule | Exact original local entry title,actual current definition/context qualified: Related to the actual current Validation Rule definition/context in§12.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Validation | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Validation definition/context in§12.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 12.4. Conformance

**Definition**

Satisfaction of all actually applicable normative requirements for an identified claim and scope,substantiated by responsible source/rule/definition editions,authority,conditions,observations and adequate mandatory coverage;source presence or successful subsets do not prove broad conformance.

**Context**

Classification validation and specification.

**Related Terms**

- Validation
- Constraint
- Specification

**Notes**

Actual Validation16/39/67 and Constraints46/56 distinguish supported criterion observations from three rule-dependent aggregate results with actual rule/definition/set/source/subject editions,scope/applicability/authority,observations/executor and performed/unperformed mandatory coverage. Known violations remain;missing support withholds unsupported breadth without fabricated Invalid/Violation/NotApplicable/outcome/severity/waiver. Evaluation is nonmutating,separate from recording,correction,decision and authorized operation;subset/local PASS proves no complete Core/implementation/global acceptance or permission.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Validation | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Validation shorthand in12.4,not a universal engine/result/approval or completed implementation. | Actual local entry§12.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |
| Constraint | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Constraint shorthand in12.4,not every external constraint or an independently allocated rule/set/field. | Actual local entry§15.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |
| Specification | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Specification shorthand in12.4;actual declared normative scope/sourced owners govern,not title alone. | Actual local entry§19.2 in this occurrence context;original literal retained,no independently allocated entry/alias. |

---

# 13. Governance Terms

## 13.1. Classification Governance

**Definition**

The set of processes and responsibilities used to control the definition, approval, maintenance and evolution of Classification.

**Context**

Classification governance.

**Related Terms**

- Classification Change
- Classification Decision
- Classification Review

**Notes**

Actual domain Governance19/43/51/53/55/56 and Extensibility33/35/37/39/50/51 own scoped decisions,proposal/subject/source editions,authority,criteria/evidence,rationale/conditions/fulfillment and separate effective adoption/activation/publication/availability/Baseline. Common Workflow/Policies/Reviews/Baselines,Metadata representation and authorized DMS/CMS/tool/manual executor differ. No actor/delegation/outcome/permission or condition fulfillment is invented from source presence/phase command.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Decision | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Decision definition/context in§13.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Review | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Review definition/context in§13.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 13.2. Classification Change

**Definition**

A controlled modification to an existing Classification structure, element, relationship, constraint or definition.

**Context**

Classification evolution.

**Related Terms**

- Classification Extension
- Classification Decision
- Classification Governance

**Notes**

Actual domain Governance19/43/51/53/55/56 and Extensibility33/35/37/39/50/51 own scoped decisions,proposal/subject/source editions,authority,criteria/evidence,rationale/conditions/fulfillment and separate effective adoption/activation/publication/availability/Baseline. Common Workflow/Policies/Reviews/Baselines,Metadata representation and authorized DMS/CMS/tool/manual executor differ. No actor/delegation/outcome/permission or condition fulfillment is invented from source presence/phase command.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Extension | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Extension definition/context in§16.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Decision | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Decision definition/context in§13.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Governance | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Governance definition/context in§13.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 13.3. Classification Decision

**Definition**

An explicit decision concerning the definition, modification, acceptance, rejection or retirement of a Classification concept or structure.

**Context**

Classification governance.

**Related Terms**

- Classification Change
- Governance
- Decision Record

**Notes**

Actual domain Governance19/43/51/53/55/56 and Extensibility33/35/37/39/50/51 own scoped decisions,proposal/subject/source editions,authority,criteria/evidence,rationale/conditions/fulfillment and separate effective adoption/activation/publication/availability/Baseline. Common Workflow/Policies/Reviews/Baselines,Metadata representation and authorized DMS/CMS/tool/manual executor differ. No actor/delegation/outcome/permission or condition fulfillment is invented from source presence/phase command.

Retain/Rename/Deprecate/Retire in§31 are selected actions,not a universal closed decision enum or actual outcomes. Real Governance43 labels and extension-specific Request modification retain scope;missing evidence invents no rejection or permission.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Governance | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Governance shorthand in13.3;common process/Metadata/authorized executor remain separate,no universal actor/outcome allocation. | Actual local entry§13.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |
| Decision Record | External actual domain record contract: CLS00851 actual Governance Decision Record supplies required scope/evidence/rationale/conditions context. Decision entity/record identity is not automatically document K or a complete mandatory physical field schema. | DF-CLS-008 V2.0 R1 §51;actual current owner context,not new local canonical entry. |

---

## 13.4. Classification Review

**Definition**

A formal or controlled examination of a proposed or existing Classification structure or change.

**Context**

Classification governance.

**Related Terms**

- Classification Governance
- Classification Validation
- Classification Decision

**Notes**

Actual domain Governance19/43/51/53/55/56 and Extensibility33/35/37/39/50/51 own scoped decisions,proposal/subject/source editions,authority,criteria/evidence,rationale/conditions/fulfillment and separate effective adoption/activation/publication/availability/Baseline. Common Workflow/Policies/Reviews/Baselines,Metadata representation and authorized DMS/CMS/tool/manual executor differ. No actor/delegation/outcome/permission or condition fulfillment is invented from source presence/phase command.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Governance | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Governance definition/context in§13.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Validation | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Validation definition/context in§12.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Decision | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Decision definition/context in§13.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 13.5. Classification Approval

**Definition**

An actual responsible scoped decision authorizing an identified proposal/definition/source edition toward adoption under applicable conditions;approval is necessary where required but alone proves no fulfillment,effective canonical adoption,activation,publication or exact Baseline membership.

**Context**

Actual scoped decision,conditions/fulfillment and separate effective adoption.

**Related Terms**

- Classification Decision
- Classification Review

**Notes**

Actual domain Governance19/43/51/53/55/56 and Extensibility33/35/37/39/50/51 own scoped decisions,proposal/subject/source editions,authority,criteria/evidence,rationale/conditions/fulfillment and separate effective adoption/activation/publication/availability/Baseline. Common Workflow/Policies/Reviews/Baselines,Metadata representation and authorized DMS/CMS/tool/manual executor differ. No actor/delegation/outcome/permission or condition fulfillment is invented from source presence/phase command.

Necessary approval is not sufficient proof required conditions are fulfilled,effective adoption/activation/publication occurred or exact Baseline selected. Source35 checklist/working correction authorizes no canonical decision.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Decision | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Decision definition/context in§13.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Review | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Review definition/context in§13.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 14. Relationship Terms

## 14.1. Classification Relationship

**Definition**

An actual explicit semantic association between responsibly typed Classification subjects/endpoints under an identified kind/definition and scope;the semantic association,its assertion and common represented record are distinct.

**Context**

Classification relationships.

**Related Terms**

- Relationship Type
- Relationship Target
- Relationship Source

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Relationship Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Type definition/context in§14.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Target | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Target definition/context in§14.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Source | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Source definition/context in§14.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 14.2. Relationship Type

**Definition**

An actual semantic relationship kind with its responsible definition/source edition,allowed endpoint/property/cardinality/constraint/lifecycle context;kind,definition,association/assertion and represented record are distinct.

**Context**

Classification relationships.

**Related Terms**

- Classification Relationship
- Relationship Source
- Relationship Target

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

Relationship kind owns actual semantic definition context,not the primary four-value documentary Type. Definition,kind,association/assertion and common typed record differ,no generated edge/fields or registered complete kind vocabulary.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Relationship | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Relationship definition/context in§14.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Source | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Source definition/context in§14.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Target | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Target definition/context in§14.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 14.3. Relationship Source

**Definition**

The actual responsibly typed source endpoint from which a directed Classification association is asserted under its kind/definition/source-edition context;not automatically a DF document or physical field.

**Context**

Classification relationships.

**Related Terms**

- Relationship Target
- Relationship Type

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Relationship Target | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Target definition/context in§14.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Type definition/context in§14.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 14.4. Relationship Target

**Definition**

The actual responsibly typed target endpoint to which a directed Classification association is asserted under its kind/definition/source-edition context;not automatically a valid/live-available DF document or physical field.

**Context**

Classification relationships.

**Related Terms**

- Relationship Source
- Relationship Type

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Relationship Source | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Source definition/context in§14.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Type definition/context in§14.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 14.5. Hierarchical Relationship

**Definition**

A Classification Relationship expressing semantic specialization between a broader and a more specific Classification Element.

**Context**

Classification hierarchy.

**Related Terms**

- Parent Element
- Child Element
- Semantic Specialization

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Parent Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Parent Element definition/context in§7.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Child Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Child Element definition/context in§7.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Semantic Specialization | Exact original local entry title,actual current definition/context qualified: Related to the actual current Semantic Specialization definition/context in§7.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 14.6. Non-Hierarchical Relationship

**Definition**

A Classification Relationship that expresses a semantic association other than hierarchical specialization.

**Context**

Classification relationships.

**Related Terms**

- Classification Relationship
- Relationship Type

**Notes**

Actual Relationships20/23/34/43/46/49–54/71 governs kind/definition/source edition,association/assertion,typed endpoints/properties/cardinality/integrity/state/use/uniqueness and record/projection/provider distinctions. Possible endpoint+kind tuple is no universal key/field schema;not every endpoint is a DF document. No automatic inverse/reverse record,arbitrary properties/all-pairs admission,complete kind population or hidden required-provider cycle.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Relationship | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Relationship definition/context in§14.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Relationship Type | Exact original local entry title,actual current definition/context qualified: Related to the actual current Relationship Type definition/context in§14.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 15. Constraint Terms

## 15.1. Classification Constraint

**Definition**

A normative condition restricting the valid structure, usage or relationships of Classification.

**Context**

Classification constraints.

**Related Terms**

- Validation Rule
- Classification Schema
- Conformance

**Notes**

Actual constraint definition/rule/effective set/source edition/applicability/authority differs from criterion observation/result/finding/decision/document identity. Constraints28/46/48/54/56/59/91 and SpecificationR014/13/Core16.1 retain known mandatory breadth and actual precedence/resolution authority with genuine complete-catalog/count/priority gaps. Unknown support invents no priority/result/violation,temporary blanket waiver or success across mandatory conflict.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Validation Rule | Exact original local entry title,actual current definition/context qualified: Related to the actual current Validation Rule definition/context in§12.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Conformance | Exact original local entry title,actual current definition/context qualified: Related to the actual current Conformance definition/context in§12.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§12.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 15.2. Structural Constraint

**Definition**

A Classification Constraint governing the permitted structure of Classification Elements and their organization.

**Context**

Classification structure.

**Related Terms**

- Classification Constraint
- Classification Schema

**Notes**

Actual constraint definition/rule/effective set/source edition/applicability/authority differs from criterion observation/result/finding/decision/document identity. Constraints28/46/48/54/56/59/91 and SpecificationR014/13/Core16.1 retain known mandatory breadth and actual precedence/resolution authority with genuine complete-catalog/count/priority gaps. Unknown support invents no priority/result/violation,temporary blanket waiver or success across mandatory conflict.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 15.3. Semantic Constraint

**Definition**

A Classification Constraint governing the permitted meaning or semantic relationships of Classification Elements.

**Context**

Classification semantics.

**Related Terms**

- Classification Constraint
- Classification Definition
- Classification Relationship

**Notes**

Actual constraint definition/rule/effective set/source edition/applicability/authority differs from criterion observation/result/finding/decision/document identity. Constraints28/46/48/54/56/59/91 and SpecificationR014/13/Core16.1 retain known mandatory breadth and actual precedence/resolution authority with genuine complete-catalog/count/priority gaps. Unknown support invents no priority/result/violation,temporary blanket waiver or success across mandatory conflict.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Relationship | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Relationship definition/context in§14.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§14.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 15.4. Cardinality Constraint

**Definition**

A Classification Constraint defining the permitted number of occurrences or associations.

**Context**

Classification relationships and assignments.

**Related Terms**

- Classification Cardinality
- Classification Constraint

**Notes**

Actual constraint definition/rule/effective set/source edition/applicability/authority differs from criterion observation/result/finding/decision/document identity. Constraints28/46/48/54/56/59/91 and SpecificationR014/13/Core16.1 retain known mandatory breadth and actual precedence/resolution authority with genuine complete-catalog/count/priority gaps. Unknown support invents no priority/result/violation,temporary blanket waiver or success across mandatory conflict.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Cardinality | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Cardinality definition/context in§10.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 16. Extensibility Terms

## 16.1. Classification Extension

**Definition**

A controlled addition or explicitly assessed necessary revision of Classification capability,meaning or mandates under actual responsible authority;ordinary additions preserve applicable meaning,while necessary incompatible revision is honestly assessed and governed with prior/new continuity evidence.

**Context**

Classification extensibility.

**Related Terms**

- Classification Change
- Extension Point
- Classification Evolution

**Notes**

Ordinary compatible addition preserves applicable meaning/owners. Necessary assessed normative/foundational/role/interface/domain revision identifies and actually revises prior mandates under real authority,need,rationale/alternatives,concrete batch/interfaces,honest incompatibility,mappings/nonreuse/history,pinned continuity,authorized transition and later checks. No absolute freeze,arbitrary mutation or simultaneously contradictory same-context canonical demands;unchanged Metadata owner no-invalidating/no-redefinition/Profile restrictions remain real source-specific pending differences,not waived.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Extension Point | Exact original local entry title,actual current definition/context qualified: Related to the actual current Extension Point definition/context in§16.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Evolution | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Evolution definition/context in§16.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 16.2. Extension Point

**Definition**

An actual defined semantic/structural extension opportunity under responsible owner/interface contracts,not automatically a physical plugin mechanism or permission to transfer responsibilities;necessary assessed role/interface change requires explicit prior/new authority.

**Context**

Classification extensibility.

**Related Terms**

- Classification Extension
- Modularity

**Notes**

Ordinary compatible addition preserves applicable meaning/owners. Necessary assessed normative/foundational/role/interface/domain revision identifies and actually revises prior mandates under real authority,need,rationale/alternatives,concrete batch/interfaces,honest incompatibility,mappings/nonreuse/history,pinned continuity,authorized transition and later checks. No absolute freeze,arbitrary mutation or simultaneously contradictory same-context canonical demands;unchanged Metadata owner no-invalidating/no-redefinition/Profile restrictions remain real source-specific pending differences,not waived.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Extension | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Extension definition/context in§16.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Modularity | External actual architectural principle: ARC0026.3 AP008 is the responsible modular-design principle. Extension Point16.2 relates to that scope,not a complete plugin/physical mechanism or mandatory no-dependency claim. | DF-ARC-002 V2.0 R2 §6.3;actual current owner context,not new local canonical entry. |

---

## 16.3. Classification Evolution

**Definition**

Controlled actual change of Classification over time,distinguishing ordinary compatible preservation from necessary assessed normative/foundational/role/interface/domain revision with actual prior/new authority,need,compatibility/history and transition/check evidence.

**Context**

Classification lifecycle and extensibility.

**Related Terms**

- Classification Change
- Classification Extension
- Backward Compatibility

**Notes**

Ordinary compatible addition preserves applicable meaning/owners. Necessary assessed normative/foundational/role/interface/domain revision identifies and actually revises prior mandates under real authority,need,rationale/alternatives,concrete batch/interfaces,honest incompatibility,mappings/nonreuse/history,pinned continuity,authorized transition and later checks. No absolute freeze,arbitrary mutation or simultaneously contradictory same-context canonical demands;unchanged Metadata owner no-invalidating/no-redefinition/Profile restrictions remain real source-specific pending differences,not waived.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Extension | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Extension definition/context in§16.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Backward Compatibility | Exact original local entry title,actual current definition/context qualified: Related to the actual current Backward Compatibility definition/context in§16.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 16.4. Backward Compatibility

**Definition**

The property of a Classification change that preserves the interpretation and required usability of previously valid Classification structures.

**Context**

Classification evolution.

**Related Terms**

- Classification Evolution
- Historical Classification
- Baseline

**Notes**

Ordinary compatible addition preserves applicable meaning/owners. Necessary assessed normative/foundational/role/interface/domain revision identifies and actually revises prior mandates under real authority,need,rationale/alternatives,concrete batch/interfaces,honest incompatibility,mappings/nonreuse/history,pinned continuity,authorized transition and later checks. No absolute freeze,arbitrary mutation or simultaneously contradictory same-context canonical demands;unchanged Metadata owner no-invalidating/no-redefinition/Profile restrictions remain real source-specific pending differences,not waived.

Backward compatibility is an actual property to substantiate for claimed continuity,not proof every change is compatible or prohibition of necessary assessed incompatibility. Required historical meaning survives even when current mandates actually change.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Evolution | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Evolution definition/context in§16.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Historical Classification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Historical Classification definition/context in§11.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.6 plus its current sourced notes;working definition is not proof canonical adoption. |
| Baseline | Exact original local entry title,actual current definition/context qualified: Related to the actual current Baseline definition/context in§18.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 17. Best Practice Terms

## 17.1. Semantic Duplication

**Definition**

Competing Classification semantic concepts or definitions presented as independent canonical meanings for the same or substantially equivalent concept without justified distinction;legitimate explicitly scoped synonyms,labels or representation copies alone are not such duplication.

**Context**

Classification quality.

**Related Terms**

- Classification Element
- Canonical Term
- Semantic Consistency

**Notes**

Actual semantic equivalence/definition/source/context/authority distinguishes legitimate synonyms/labels/representation copies from competing concepts/definitions. Quality/granularity/inflation are scoped concepts,not measured system health,numeric thresholds,severity/outcome enums or permissions. Actual Best PracticesV1R1 is explicitly informative;recommendation omission alone is no constraint violation,actual sourced mandatory duties retain their own force.

Multiple actual synonyms can represent one concept without competing canonical concepts. Anti-pattern concerns unsupported duplicate semantic ownership/definitions,not word count,naming style or every physical copy.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Semantic Consistency | Exact original local entry title,actual current definition/context qualified: Related to the actual current Semantic Consistency definition/context in§17.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§17.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 17.2. Classification Granularity

**Definition**

The degree of semantic detail represented by the Classification structure.

**Context**

Classification design.

**Related Terms**

- Classification Hierarchy
- Classification Element
- Semantic Specialization

**Notes**

Actual semantic equivalence/definition/source/context/authority distinguishes legitimate synonyms/labels/representation copies from competing concepts/definitions. Quality/granularity/inflation are scoped concepts,not measured system health,numeric thresholds,severity/outcome enums or permissions. Actual Best PracticesV1R1 is explicitly informative;recommendation omission alone is no constraint violation,actual sourced mandatory duties retain their own force.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Hierarchy | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Hierarchy definition/context in§7.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Semantic Specialization | Exact original local entry title,actual current definition/context qualified: Related to the actual current Semantic Specialization definition/context in§7.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§7.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 17.3. Classification Inflation

**Definition**

The unnecessary growth of Classification through excessive specialization or creation of categories with insufficient independent semantic value.

**Context**

Classification best practices.

**Related Terms**

- Classification Granularity
- Semantic Duplication
- Classification Element

**Notes**

Actual semantic equivalence/definition/source/context/authority distinguishes legitimate synonyms/labels/representation copies from competing concepts/definitions. Quality/granularity/inflation are scoped concepts,not measured system health,numeric thresholds,severity/outcome enums or permissions. Actual Best PracticesV1R1 is explicitly informative;recommendation omission alone is no constraint violation,actual sourced mandatory duties retain their own force.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Granularity | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Granularity definition/context in§17.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§17.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Semantic Duplication | Exact original local entry title,actual current definition/context qualified: Related to the actual current Semantic Duplication definition/context in§17.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§17.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Element | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Element definition/context in§6.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§6.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 17.4. Semantic Consistency

**Definition**

The property of Classification whereby the same concept has a consistent meaning throughout the Framework.

**Context**

Classification architecture.

**Related Terms**

- Canonical Term
- Classification Definition
- Single Source of Truth

**Notes**

Actual semantic equivalence/definition/source/context/authority distinguishes legitimate synonyms/labels/representation copies from competing concepts/definitions. Quality/granularity/inflation are scoped concepts,not measured system health,numeric thresholds,severity/outcome enums or permissions. Actual Best PracticesV1R1 is explicitly informative;recommendation omission alone is no constraint violation,actual sourced mandatory duties retain their own force.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Single Source of Truth | Exact original local entry title,actual current definition/context qualified: Related to the actual current Single Source of Truth definition/context in§17.5;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§17.5 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 17.5. Single Source of Truth

**Definition**

The architectural principle that each authoritative Classification concept should have one canonical definition.

**Context**

Classification architecture and documentation.

**Related Terms**

- Canonical Term
- Classification Definition
- Semantic Consistency

**Notes**

Actual semantic equivalence/definition/source/context/authority distinguishes legitimate synonyms/labels/representation copies from competing concepts/definitions. Quality/granularity/inflation are scoped concepts,not measured system health,numeric thresholds,severity/outcome enums or permissions. Actual Best PracticesV1R1 is explicitly informative;recommendation omission alone is no constraint violation,actual sourced mandatory duties retain their own force.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Semantic Consistency | Exact original local entry title,actual current definition/context qualified: Related to the actual current Semantic Consistency definition/context in§17.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§17.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 18. Traceability Terms

## 18.1. Classification Traceability

**Definition**

The ability to determine the origin, history, relationships and evolution of Classification concepts and changes.

**Context**

Classification governance and evolution.

**Related Terms**

- Classification Change
- Classification Decision
- Baseline

**Notes**

Actual traceability/history retains earlier definitions/terms/rules/sets/relationships/assignments/states/decisions/conditions/results/source editions and needed pinned context wherever responsible owners require. Interpretation,original conformity,current compliance/use and live retrieval differ. New rules are not backdated;later actual evidence can justify traced earlier-contract reassessment preserving original observations. Baseline concept is not actual exact membership/selection;no automatic consumer revision,migration,deletion or permission to erase required meaning.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Decision | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Decision definition/context in§13.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Baseline | Exact original local entry title,actual current definition/context qualified: Related to the actual current Baseline definition/context in§18.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 18.2. Classification History

**Definition**

The recorded sequence of relevant changes and decisions affecting Classification.

**Context**

Classification governance.

**Related Terms**

- Classification Traceability
- Classification Change
- Baseline

**Notes**

Actual traceability/history retains earlier definitions/terms/rules/sets/relationships/assignments/states/decisions/conditions/results/source editions and needed pinned context wherever responsible owners require. Interpretation,original conformity,current compliance/use and live retrieval differ. New rules are not backdated;later actual evidence can justify traced earlier-contract reassessment preserving original observations. Baseline concept is not actual exact membership/selection;no automatic consumer revision,migration,deletion or permission to erase required meaning.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Traceability | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Traceability definition/context in§18.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Change | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Change definition/context in§13.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Baseline | Exact original local entry title,actual current definition/context qualified: Related to the actual current Baseline definition/context in§18.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.3 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 18.3. Baseline

**Definition**

An identified immutable architectural snapshot comprising explicitly selected exact editions/state within actual responsible Baseline scope;this definition alone provides no actual membership,approval or snapshot-selection evidence.

**Context**

Classification evolution and governance.

**Related Terms**

- Classification History
- Historical Classification
- Traceability

**Notes**

Actual traceability/history retains earlier definitions/terms/rules/sets/relationships/assignments/states/decisions/conditions/results/source editions and needed pinned context wherever responsible owners require. Interpretation,original conformity,current compliance/use and live retrieval differ. New rules are not backdated;later actual evidence can justify traced earlier-contract reassessment preserving original observations. Baseline concept is not actual exact membership/selection;no automatic consumer revision,migration,deletion or permission to erase required meaning.

Actual immutable snapshot needs identified exact constituent editions/state and real membership evidence under Baselines;publication/approval/review/adoption alone selects no snapshot. Current header Not assigned inherits no input1.0 membership.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification History | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification History definition/context in§18.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§18.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Historical Classification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Historical Classification definition/context in§11.6;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§11.6 plus its current sourced notes;working definition is not proof canonical adoption. |
| Traceability | Explicit contextual local phrase,not an allocated canonical alias: Contextual Classification Traceability concern in11.6/18.3;actual common AP012 and responsible history/source-edition requirements retain independent scope. | Actual local entry§18.1 in this occurrence context;original literal retained,no independently allocated entry/alias. |

---

# 19. Documentation Terms

## 19.1. Classification Dictionary

**Definition**

The authoritative terminology reference for the Classification component.

**Context**

Classification documentation.

**Related Terms**

- Classification Specification
- Classification Definition
- Canonical Term

**Notes**

These are actual consultation/documentary roles with declared owner/source-edition/scope authority,not normative force by title/Type/path. Dictionary defines actual scoped working terminology without replacing Model/Schema/Constraints/Specification;Examples illustrate and Best PracticesV1R1 recommends. Presence creates no actual canonical adoption,fulfilled conditions,complete implementation or global architecture acceptance.

Actual authoritative working terminology scope does not mean complete approved vocabulary,populated registry or adoption from a Draft source. Actual adopted review rules and current responsible owner clauses govern correction;no blanket title/approval precedence.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Specification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Specification definition/context in§19.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Definition | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Definition definition/context in§9.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§9.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Canonical Term | Exact original local entry title,actual current definition/context qualified: Related to the actual current Canonical Term definition/context in§8.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§8.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 19.2. Classification Specification

**Definition**

The actual explicitly scoped normative integration reference for Classification requirements,incorporating responsible definitions/rules and conformance duties under real source/edition/scope authority;title or Type alone supplies no complete approved requirement catalog.

**Context**

Classification documentation.

**Related Terms**

- Classification Dictionary
- Classification Schema
- Classification Constraint

**Notes**

These are actual consultation/documentary roles with declared owner/source-edition/scope authority,not normative force by title/Type/path. Dictionary defines actual scoped working terminology without replacing Model/Schema/Constraints/Specification;Examples illustrate and Best PracticesV1R1 recommends. Presence creates no actual canonical adoption,fulfilled conditions,complete implementation or global architecture acceptance.

Actual explicit normative integration and independently applicable source/definition requirements remain. Dictionary terminology and Specification mandates are complementary,not all other owner requirements optional or a complete supplied precedence catalog.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Dictionary | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Dictionary definition/context in§19.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Schema | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Schema definition/context in§10.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§10.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Constraint | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Constraint definition/context in§15.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§15.1 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 19.3. Classification Example

**Definition**

A documented instance demonstrating the application of Classification concepts or rules.

**Context**

Classification documentation.

**Related Terms**

- Classification Specification
- Classification Best Practice

**Notes**

These are actual consultation/documentary roles with declared owner/source-edition/scope authority,not normative force by title/Type/path. Dictionary defines actual scoped working terminology without replacing Model/Schema/Constraints/Specification;Examples illustrate and Best PracticesV1R1 recommends. Presence creates no actual canonical adoption,fulfilled conditions,complete implementation or global architecture acceptance.

A documented illustration is not necessarily a performed domain assignment/Metadata Instance,accepted vocabulary member or complete validation result. Actual intended identity/edition/context and declared example limits remain.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Specification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Specification definition/context in§19.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.2 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Best Practice | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Best Practice definition/context in§19.4;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.4 plus its current sourced notes;working definition is not proof canonical adoption. |

---

## 19.4. Classification Best Practice

**Definition**

A recommended practice for designing, applying, maintaining or evolving Classification.

**Context**

Classification documentation.

**Related Terms**

- Classification Governance
- Classification Evolution
- Classification Specification

**Notes**

These are actual consultation/documentary roles with declared owner/source-edition/scope authority,not normative force by title/Type/path. Dictionary defines actual scoped working terminology without replacing Model/Schema/Constraints/Specification;Examples illustrate and Best PracticesV1R1 recommends. Presence creates no actual canonical adoption,fulfilled conditions,complete implementation or global architecture acceptance.

Current Best PracticesV1R1 informative status and omission-alone-no-violation remain;this term definition does not convert its advice into mandatory requirements,completed checks or independent approval authority.

| Received Related Terms occurrence | Actual scoped interpretation | Existing target / owner evidence |
|---|---|---|
| Classification Governance | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Governance definition/context in§13.1;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§13.1 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Evolution | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Evolution definition/context in§16.3;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§16.3 plus its current sourced notes;working definition is not proof canonical adoption. |
| Classification Specification | Exact original local entry title,actual current definition/context qualified: Related to the actual current Classification Specification definition/context in§19.2;this relation is not semantic identity,inheritance,approval,provider dependency or automatic assignment. Preserve actual subject/source edition/owner requirements. | Actual local entry§19.2 plus its current sourced notes;working definition is not proof canonical adoption. |

---

# 20. Relationship Between Dictionary Terms

The principal terminology relationships can be summarized as follows:

```text

            Classification
            │
            ├── Architecture
            │
            ├── Concepts
            │
            ├── Model
            │   │
            │   └── Elements
            │       ├── Family
            │       ├── Type
            │       └── Class
            │
            ├── Schema
            │
            ├── Lifecycle
            │
            ├── Validation
            │
            ├── Governance
            │
            ├── Relationships
            │
            ├── Constraints
            │
            └── Extensibility

```

**Current relation scope.** Received document/role consultation view,not current universal Family-owned Type/Class hierarchy,complete integration or provider graph. Actual current roles/owners and interfaces govern.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Classification | Actual component/domain context,not additional component or complete implemented system. |
| Architecture | Architectural responsibility/source context,not inherent normative priority. |
| Concepts | Actual domain conceptual definitions and responsible sources. |
| Model | Actual reconstructed current model source,not recovered authentic historical edition. |
| Elements | Actual domain definitions/categories/values,not automatically a complete populated registry. |
| Family | Actual component/admitted documentary-area membership,not owner of primary Type. |
| Type | Exactly one uniform primary Architecture/Structure/Behavior/Reference responsibility. |
| Class | Separate optional explicitly defined nonconflicting semantic distinction. |
| Schema | Actual Classification structural contract,distinct from broader Metadata Schema/effective Profile/Instance. |
| Lifecycle | Actual typed subject state/use/history contracts,not universal state enum. |
| Validation | Actual scoped nonmutating rule/evidence comparison,not implementation or permission. |
| Governance | Actual responsible decision/conditions/fulfillment/adoption scope,not performed approval. |
| Relationships | Actual responsible kinds/definitions/assertions/endpoint/property/count context,not provider DAG. |
| Constraints | Actual responsible definitions/rules/effective sets,not all counts/precedence supplied. |
| Extensibility | Ordinary preservation versus necessary assessed responsible revision,not arbitrary change/absolute freeze. |


The terminology forms a coherent vocabulary rather than a collection of independent terms.

**Current sourced scope.**

This exact terminology-organization view does not impose old Family-owned Type/Class hierarchy or allocate new components/accepted population. Current roles are complementary;actual defined scheme/property/cardinality/identity/state/use and indispensable provider graphs remain separate,no complete DAG/runtime or ownership transfer from adjacency.

---

# 21. Canonical Terminology Rules

The following rules apply to the Dictionary.

**Current sourced scope.**

Actual terminology consistency and no-silent-change duties retain scope;necessary explicitly assessed semantic/mandate revision needs actual prior/new authority,need,alternatives,batch/interfaces,honest compatibility/mappings/history,pinned continuity,authorized transition and later checks. Canonical term label alone does not establish actual adoption or waive independently applicable owners.

---

## 21.1. Use the Canonical Term

When referring to a defined Classification concept, use its canonical term.

**Current sourced scope.**

Use actual authoritative term/definition/source edition and context;earlier/historical/quoted/pinned or proposed terminology can be referenced with explicit scope rather than prohibited or silently retargeted.

---

## 21.2. Avoid Uncontrolled Synonyms

Alternative terminology should not be introduced as though it represented a different concept unless a semantic distinction exists.

**Current sourced scope.**

Genuine synonyms/labels are not automatically different concepts. Actual definition/edition/context/equivalence and responsible naming authority support any alias claim,no approved complete registry or automatic merge/key allocation.

---

## 21.3. Preserve Defined Meaning

Ordinary use retains the actual defined source-edition/context meaning;necessary assessed semantic or mandate revision explicitly identifies and revises prior authority with compatibility/history and transition evidence rather than silently changing earlier definitions.

**Current sourced scope.**

Ordinary preservation and necessary assessed revision differ. Actual unchanged external owner restrictions remain source-specific pending differences,not silently edited/waived by Dictionary correction.

---

## 21.4. Prefer Existing Vocabulary

New documents should reuse existing Classification terminology whenever applicable.

**Current sourced scope.**

Reusing vocabulary needs actual meaning/source edition/context and authority,not string equality or absent lookup alone. No additional mandatory field,universal namespace or approval is created.

---

## 21.5. Update the Dictionary When Terminology Changes

A change to canonical terminology should result in a corresponding Dictionary update.

**Current sourced scope.**

Actual required source/consumer/term/definition editions,authority/conditions,compatibility/history and later evidence govern updates;entry changes are not automatic consumer revisions or completed global propagation.

---

# 22. Naming Conventions

Classification terminology should generally use:

- descriptive nouns;
- established architectural vocabulary;
- singular terms for concepts;
- consistent capitalization;
- stable terminology.

Names should avoid:

- unnecessary abbreviations;
- implementation-specific terminology;
- temporary terminology;
- ambiguous generic terms.

**Current sourced scope.**

All five recommended naming and four avoided-name subjects remain advice under actual semantic purpose/context/authority. No universal reserved/forbidden names,severity/outcome thresholds or physical field registry;real imported owner mandates retain force independently.

---

# 23. Singular and Plural Usage

Canonical Classification terms representing concepts should normally use singular form.

For example:

```text

    Family
    Type
    Class
    Element
    Relationship
    Constraint

```

**Current relation scope.** Received selected singular/plural terminology forms,not semantic equivalence registry,canonical population,mandatory field allocation or universal hierarchy. Actual current entry definitions and responsible counts/scope govern.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Family | Actual component/admitted documentary-area membership,not owner of primary Type. |
| Type | Exactly one uniform primary Architecture/Structure/Behavior/Reference responsibility. |
| Class | Separate optional explicitly defined nonconflicting semantic distinction. |
| Element | Actual domain definition/category/value subject distinct from assignment/record/document. |
| Relationship | Actual relationship concern;kind/definition/association/assertion/endpoints differ. |
| Constraint | Actual responsible restriction/rule/set concern,not result or complete allocated registry. |


Plural forms should be used when referring to collections of those concepts.

For example:

```text

    Families
    Types
    Classes
    Elements
    Relationships
    Constraints

```

**Current relation scope.** Received selected singular/plural terminology forms,not semantic equivalence registry,canonical population,mandatory field allocation or universal hierarchy. Actual current entry definitions and responsible counts/scope govern.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Families | Actual membership contexts,not primary-Type-owning hierarchies. |
| Types | Uniform four primary responsibilities,not Family-owned vocabulary. |
| Classes | Optional explicitly defined meanings,not universal third fields/Type children. |
| Elements | Actual domain definitions/categories/values,not automatically a complete populated registry. |
| Relationships | Actual responsible kinds/definitions/assertions/endpoint/property/count context,not provider DAG. |
| Constraints | Actual responsible definitions/rules/effective sets,not all counts/precedence supplied. |

**Current sourced scope.**

Both exact singular/plural examples retain original spelling/order as grammatical illustrations,not allocated Types/Class vocabulary,complete term population or automatic identity equivalence. Actual current definitions/context and authority govern use.

---

# 24. Term Status

Dictionary terminology may have one of the following conceptual statuses:

| Status | Received meaning | Current bounded term-use / authority interpretation |
|---|---|---|
| **Canonical** | Current authoritative terminology  | Actual term authority designation for identified meaning/edition/scope under real responsible decision/fulfilled conditions/effective adoption where required;Draft presence proves none. |
| **Preferred** | Recommended terminology  | Actual preferred naming recommendation;not automatically canonical approval,Element Active state or exclusive global status. |
| **Synonym** | Alternative terminology referring to the same concept  | Actual alternative terminology relationship needs supported same concept/definition/context;not a separate competing concept or automatic approved alias registry. |
| **Deprecated** | Terminology retained for historical compatibility but no longer recommended  | Actual term-use context retains historical meaning;ordinary new canonical naming differs from legitimate historical/quoted/pinned references and Element/document state. |
| **Retired** | Terminology no longer valid for current use  | Actual scoped term-use retirement with required historical reference/interpretation retained;not Element Retired state or all-context invalidity/deletion/automatic transition. |

**Current sourced scope.**

Five original status/meaning pairs are received evidence with current qualified column,not competing current rules. Naming authority/preference/synonym relation and deprecated/retired term-use are not one universal exclusive lifecycle/decision enum. Actual term/source edition/use scope,authority/conditions/history and legitimate historical references differ from Element/document/extension/local R/result/finding states. No actual transition,canonicality,default outcome or permission from row presence.

---

# 25. Dictionary Maintenance

The Dictionary should be maintained whenever:

- a new Classification concept is introduced;
- a canonical term is renamed;
- a definition changes;
- a term is deprecated;
- a term is retired;
- a new relationship type is introduced;
- a new architectural distinction requires terminology.

Dictionary maintenance should be coordinated with the Classification Governance process.

**Current sourced scope.**

All seven maintenance triggers remain. Actual responsible definition/source/term editions,need,rationale/alternatives,criteria/evidence,authority/conditions/fulfillment,affected owners/interfaces,compatibility/history and authorized effects matter. Domain Governance/common documentary process/Metadata representation/actual executor differ;no actor/outcome schema,performed adoption or consumer successor inferred.

---

# 26. Dictionary Integrity

The Dictionary should maintain:

- one canonical definition per concept;
- consistent terminology;
- stable references;
- explicit relationships between related terms;
- traceable terminology changes.

Duplicate definitions should be avoided.

**Current sourced scope.**

All five integrity subjects remain. Actual canonical concept/definition/source edition/context,term/name/label/synonym/record copies and responsible identity/uniqueness/history differ;multiple terms can be legitimate synonyms rather than competing definitions. Real owner mandates and genuine missing external detail are explicit,no invented complete registry or deletion.

---

# 27. Dictionary and Specification

The Dictionary and Specification have different responsibilities.

```text

            Classification Dictionary
            │
            └── defines terminology

            Classification Specification
            │
            └── defines normative requirements

```

**Current relation scope.** Complementary terminology and normative integration responsibilities,not title-derived precedence,exclusive authority or proof complete approved contents.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Classification Dictionary | This actual authoritative scoped terminology reference;Draft presence is not canonical adoption. |
| defines terminology | Working meaning/source edition/scope under real owners,not all domain normative rules. |
| Classification Specification | Actual explicitly scoped normative integration source with independent responsible owner duties. |
| defines normative requirements | Actual declaration/incorporation/source-edition/scope authority,not title-only exclusive authority. |


The Dictionary explains what Classification terms mean.

The Specification defines what Classification must satisfy.

**Current sourced scope.**

Dictionary/Specification are actual semantic consultation/integration roles,not authority by Type/title/path alone. Explicit source declarations/incorporation,edition/scope and actual owner mandates determine normative force. Dictionary does not replace independent Model/Schema/Constraints/Lifecycle/Profile/Identity duties or establish full implementation from definitions.

---

# 28. Dictionary and Examples

Examples should use Dictionary terminology consistently.

Examples should not introduce undocumented Classification concepts without corresponding architectural definition.

Where an example introduces a new concept for illustrative purposes, that concept should not be interpreted as automatically becoming canonical Classification terminology.

**Current sourced scope.**

Illustrations do not allocate actual canonical term/definition/field/key or demonstrate completed assignment/state/decision/permission. Hypothetical labels require declared scope and responsible definitions for actual use;no automatic adoption from example presence.

---

# 29. Dictionary and Best Practices

Best Practices should use the canonical terminology established by this Dictionary.

Conversely, terminology introduced by Best Practices that represents a genuine Classification concept should be evaluated for inclusion in the Dictionary.

**Current sourced scope.**

Actual corrected Best PracticesV1R1 remains explicitly informative:recommendation omission alone is no constraint violation. A candidate term can be evaluated under actual authority/need/evidence without assuming approval or creating a mandatory new local entry merely from advice.

---

# 30. Dictionary and Governance

Terminology changes should be governed when they affect the canonical Classification vocabulary.

A terminology change may require review of:

- Classification Elements;
- relationships;
- constraints;
- validation;
- Dictionary;
- Specification;
- Examples.

**Current sourced scope.**

All seven actual impact subjects remain. Substantive terminology/meaning change needs actual prior/new source/definition/term/consumer editions,authority,rationale/alternatives,batch/interfaces,honest compatibility/mappings/history,pinned context,authorized transition and later checks. Working source-phase command is no canonical approval/condition fulfillment/operation.

---

# 31. Dictionary and Evolution

The Dictionary must support controlled terminology evolution.

When terminology changes:

```text

              Existing Term
                    │
                    ▼

                  Review
                    │
                    ▼

                 Decision
                 │
                 ├── Retain
                 ├── Rename
                 ├── Deprecate
                 └── Retire

```

**Current relation scope.** Selected term maintenance options,not complete universal transition machine,authorized actor/guard/record/outcome or performed rename/deprecation/retirement.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Existing Term | Identified actual term/meaning/definition/source edition,not merely same string. |
| Review | Actual responsible assessment/evidence and criteria,not automatically approval. |
| Decision | Actual authorized scoped decision/conditions/evidence,not universal actor/outcome field. |
| Retain | Possible justified maintenance disposition;no performed operation. |
| Rename | Possible actual name change under identity/reference/history authority,not automatic semantic rekey. |
| Deprecate | Possible scoped term-use discouragement,not Element/document transition or historical invalidity. |
| Retire | Possible scoped ordinary-use withdrawal retaining required history,not automatic deletion. |


The historical terminology should remain traceable where required.

**Current sourced scope.**

Required traceability/history is mandatory where actual owners require,not optionalized by should-where-required shorthand. Retain/Rename/Deprecate/Retire are selected actions under actual subject/edition/authority/conditions/evidence,not universal decision enum,actual outcomes or source-version algorithm. Preserve original observations/meaning;no automatic migration/deletion/consumer transition or blanket waiver.

---

# 32. Recommended Dictionary Entry Lifecycle

A terminology entry should normally follow:

```text

              Proposed Term
                    │
                    ▼

             Semantic Review
                    │
                    ▼

                Definition
                    │
                    ▼

                Governance
                    │
                    ▼

              Canonical Term
              │
              ├── Active
              ├── Deprecated
              └── Retired

```

**Current relation scope.** Selected term proposal/use-state consultation,not sufficient approval,condition fulfillment,effective adoption,activation or universal Element/document/term state machine.

| Received literal label / relation | Actual current interpretation |
|---|---|
| Proposed Term | Actual identified proposal/definition/source edition and intended scope,not accepted population. |
| Semantic Review | Actual meaning/owner/context/evidence assessment,not full implementation validation. |
| Definition | Actual identified meaning/source edition under responsible scope,not allocated physical schema. |
| Governance | Actual responsible decision/conditions/fulfillment/adoption scope,not performed approval. |
| Canonical Term | Actual term authority requires responsible decision,fulfilled conditions/effective adoption;Draft presence proves none. |
| Active | Bounded term-use context here,not proof all assignments valid/permitted/available or Element-state alias. |
| Deprecated | Actual scoped term-use context,not blocked legitimate historical/pinned references. |
| Retired | Actual scoped ordinary-term-use withdrawal retaining required historical meaning,not automatic Element/document transition. |

**Current sourced scope.**

Selected entry proposal/review/definition/Governance/canonical/state path is not a complete workflow or approval sufficiency. Actual scoped approval,required fulfilled conditions and effective adoption/activation evidence remain under Governance43/51/53 and Extensibility33/35/37/39/50/51. Proposed terms/working Draft correction can exist without false canonicality. Term naming/use status,Element/document/extension/decision/local R/result/finding/Milestone states are not aliases;known duties/genuine exact actor/guard/record/route gaps remain.

---

# 33. Quality Criteria

A good Dictionary entry should be:

**Current sourced scope.**

All five quality subjects remain bounded criteria/advice under actual source authority,not measured health,mandatory numeric thresholds,state/outcome enums or permission. Definition consistency does not prohibit necessary explicit assessed revision or legitimate related synonyms. Actual evidence/source/context supports each claim.

---

### 33.1. Clear

The meaning should be understandable without relying on undocumented assumptions.

**Current sourced scope.**

Clarity depends on actual declared meaning/context/owner rather than undocumented convention. It is not proof full implementation or complete registered vocabulary.

---

### 33.2. Precise

The definition should distinguish the concept from related concepts.

**Current sourced scope.**

Precision distinguishes actual concepts with definition/source edition/scope/evidence;names alone prove neither duplicate meaning nor new canonical allocation.

---

### 33.3. Consistent

The terminology should agree with the rest of the Classification architecture.

**Current sourced scope.**

Consistency follows actual adopted current owner contracts and explicit necessary revision;prior incompatible source meanings retain event-time evidence,not simultaneous current alternative rules.

---

### 33.4. Stable

The definition should not depend on implementation details.

**Current sourced scope.**

Representation-independent meaning preserves actual descriptor/Profile/physical/reference/interface/access/retrieval/history duties. Stable does not mean no necessary assessed change or every instance valid/available.

---

### 33.5. Traceable

Changes to the definition should be attributable to an explicit architectural decision.

**Current sourced scope.**

Actual mandatory rationale/decision/history follows responsible change scope. Record source/definition/term editions,authority/evidence/conditions/effects without inventing organization actors or treating editorial working correction as actual canonical architecture approval.

---

# 34. Anti-Patterns

The following practices should be avoided.

**Current sourced scope.**

All six anti-patterns remain scoped concerns,not universal forbidden labels or measured violations. Actual source/definition/context/authority evidence matters;legitimate synonyms/copies/related-term cross-references are not competing concepts or circular definitions solely by count/graph.

---

## 34.1. Multiple Canonical Names

Different names representing the same concept as though they were distinct.

**Current sourced scope.**

Actual same concept may have supported synonyms/readable labels without multiple competing canonical concepts. Spelling alone establishes no collision or alias merge.

---

## 34.2. Multiple Definitions

Different documents providing competing definitions for the same term.

**Current sourced scope.**

Actual competing same-context definitions differ from earlier pinned editions,legitimate scoped context and actual representation copies. Necessary revised meaning retains prior evidence rather than erasing history.

---

## 34.3. Implementation Vocabulary

Using tool-specific terminology as canonical architectural terminology.

**Current sourced scope.**

Tool preference alone owns no semantic definition,but actual representation/descriptor/Profile/interface contracts remain real;independence does not waive them.

---

## 34.4. Undefined Terms

Using important Classification concepts without defining them.

**Current sourced scope.**

All201 actual related-term occurrences have exact-local/contextual/import/genuine-limit dispositions;no exact title match is not automatically undefined concept or a reason to invent definitions/fields/keys.

---

## 34.5. Circular Definitions

Defining one term exclusively through another term that ultimately depends on the first.

**Current sourced scope.**

Exclusive circular definition can be a real issue;mutual Related Terms/navigation links are not automatically circular semantic definitions or required-provider cycles. Actual definition text/authority and indispensable provider graph need separate evidence.

---

## 34.6. Context Switching

Changing the meaning of a term depending on the document in which it appears.

**Current sourced scope.**

Stable canonical meaning differs from actual explicit applicability/contextual valid use or historical source-edition scope. Unknown applicability is not NotApplicable,permission or fabricated violation;invented context tags cannot conceal real conflict.

---

# 35. Dictionary Review Checklist

Before approving a Dictionary change:

- [ ] Is the term genuinely required?
- [ ] Does the concept already exist?
- [ ] Is there an existing synonym?
- [ ] Is the definition unambiguous?
- [ ] Is the scope clear?
- [ ] Are related terms identified?
- [ ] Does the terminology agree with the Classification Model?
- [ ] Does it agree with the Schema?
- [ ] Does it affect Constraints?
- [ ] Does it affect Validation?
- [ ] Does it affect Governance?
- [ ] Does it affect the Specification?
- [ ] Does it affect Examples?
- [ ] Is the terminology change traceable?

**Current sourced scope.**

All14 original checklist labels remain unchanged and unchecked. Prompts are not completed observations,mandatory physical fields,approval/condition fulfillment or full conformance. Actual rule/source/definition/subject editions,authority/applicability/evidence and mandatory coverage govern any real claim;recommendation omission alone is no constraint violation.

---

# 36. Canonical Classification Vocabulary

The following terms constitute the principal canonical vocabulary of the Classification component:

| Term | Received primary meaning | Actual current working meaning / scope |
|---|---|---|
| Classification | Semantic organization mechanism  | Actual§5.1: A semantic mechanism used to organize documents according to meaningful categories and characteristics defined by the Documentation Framework. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Component | Framework component responsible for Classification  | Actual§5.2: The Documentation Framework component responsible for defining and governing the semantic classification of documents. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Concept | Conceptual entity used to define Classification  | Actual§5.4: A conceptual entity representing a meaningful idea required to understand or define Classification. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Model | Conceptual and structural model  | Actual§5.5: The conceptual and structural model describing the entities and relationships that constitute Classification. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Element | Semantic classification unit  | Actual§6.1: A defined domain semantic unit,category or role/value definition used in Classification within actual responsible scope;the definition,an assigned value or association and its physical record/document are distinct subjects. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Family | Top-level classification grouping  | Actual§6.2: The actual canonical component membership or explicitly admitted documentary-area membership of an applicable normalized document;Family does not own or specialize the uniform primary Type vocabulary. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Type | Specialization within a Family  | Actual§6.3: Exactly one primary documentary responsibility selected uniformly from Architecture,Structure,Behavior or Reference for each applicable normalized document,independent of Family-owned specialization. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Class | Further semantic specialization  | Actual§6.4: A separate optional explicitly defined non-conflicting semantic distinction used in actual context,not a universal Type-child level or mandatory third Classification field/value. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Hierarchy | Structured arrangement of elements  | Actual§7.1: An actually defined scheme-specific arrangement of Classification subjects with responsible hierarchical relation/position semantics;documentary Family,primary Type and optional Class do not impose a universal specialization tree. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Relationship | Explicit semantic association  | Actual§14.1: An actual explicit semantic association between responsibly typed Classification subjects/endpoints under an identified kind/definition and scope;the semantic association,its assertion and common represented record are distinct. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Schema | Formal structural definition  | Actual§10.1: The formal structural definition governing the representation and organization of Classification. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Lifecycle | Controlled evolution of element state  | Actual§11.1: The actual subject-specific state/use/transition/history contract for Classification Elements or definitions and their relevant assignments under responsible rules,not a universal lifecycle of every term,document,decision or extension. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Validation | Verification of Classification conformance  | Actual§12.1: Actual nonmutating comparison of an identified Classification subject/structure/assignment and relevant context against applicable responsible rules,with source/definition/rule-set editions,authority,observations and required coverage supporting the asserted breadth. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Governance | Control of Classification definition and evolution  | Actual§13.1: The set of processes and responsibilities used to control the definition, approval, maintenance and evolution of Classification. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Constraint | Normative restriction on Classification  | Actual§15.1: A normative condition restricting the valid structure, usage or relationships of Classification. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Extension | Controlled addition to Classification  | Actual§16.1: A controlled addition or explicitly assessed necessary revision of Classification capability,meaning or mandates under actual responsible authority;ordinary additions preserve applicable meaning,while necessary incompatible revision is honestly assessed and governed with prior/new continuity evidence. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Dictionary | Authoritative Classification terminology reference  | Actual§19.1: The authoritative terminology reference for the Classification component. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Specification | Normative Classification requirements  | Actual§19.2: The actual explicitly scoped normative integration reference for Classification requirements,incorporating responsible definitions/rules and conformance duties under real source/edition/scope authority;title or Type alone supplies no complete approved requirement catalog. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |
| Classification Example | Demonstration of Classification usage  | Actual§19.3: A documented instance demonstrating the application of Classification concepts or rules. Consult its actual notes/source-edition authority;selected summary is not complete approved vocabulary. |

**Current sourced scope.**

All19 original selected term/primary-meaning pairs remain received evidence beside actual current definition/scope. Current column governs working role/authority/state/evolution meanings,not a simultaneous old rule. This principal subset is neither all73 entries nor a complete populated approved canonical registry,field catalog or actual adoption.

---

# 37. Summary

The Classification Dictionary establishes the canonical vocabulary required to describe and maintain the Classification component.

Its primary objectives are:

- semantic consistency;
- terminology stability;
- authoritative definitions;
- controlled vocabulary;
- traceability;
- architectural coherence.

The Dictionary should be treated as the authoritative terminology reference for Classification.

It evolves with actual responsible Classification contracts:ordinary compatible preservation differs from necessary explicitly assessed meaning/mandate revision,with actual prior/new authority,need,compatibility/history,pinned continuity and later checks.

**Current sourced scope.**

All six objectives remain. Actual working terminology authority is scoped with known duties and genuine owner/population/precedence/transition/record/interface gaps;authoritative word/entry presence proves no canonical adoption,publication,Baseline or globally accepted implementation. Required historical meaning and actual necessary assessed revision coexist.

---

# 38. Conformance

This document defines terminology rather than the complete normative behavior of Classification.

Actual source/definition editions,scope,applicability,authority and responsible precedence/decision contracts govern any conflict. This working Dictionary follows the user-adopted ReviewPolicy and actual responsible sources without claiming completed canonical adoption;approved-source wording or a title alone supplies no universal priority or waiver. A real required reconciliation needs an actual traced successor and later checks.

**Current sourced scope.**

Actual adopted ReviewPolicy governs this authorized working correction. Normative source authority follows real declaration/incorporation,edition,scope/applicability and responsible contracts,not only approved label/title. Actual Constraints54/56/59 Specification-owned precedence and Governance/necessary revision apply;unknown mandatory conflict/authority withholds unsupported success without invented priority,violation or waiver. Local documentary results are no architecture acceptance.

---

# 39. Related Documents

**Current sourced scope.**

All26 original related-document subjects retain original order/self-reference with actual intended local targets. Current working source link is not inherited approval,full peer validation or rewrite of earlier snapshot;actual owner clauses and independent historical scope remain.

---

## 39.1. Foundation

- [DF-FND-001 — Framework Manifest](../../../00-Foundation/DF-FND-001-FrameworkManifest.md)
- [DF-FND-002 — Research Journal](../../../00-Foundation/DF-FND-002-ResearchJournal.md)
- [DF-FND-003 — Evolution Timeline](../../../00-Foundation/DF-FND-003-EvolutionTimeline.md)
- [DF-FND-004 — Architectural Blueprint](../../../00-Foundation/DF-FND-004-ArchitecturalBlueprint.md)
- [DF-FND-005 — Framework Evolution](../../../00-Foundation/DF-FND-005-FrameworkEvolution.md)
- [DF-FND-006 — Design Rationale](../../../00-Foundation/DF-FND-006-DesignRationale.md)

## 39.2. Architecture

- [DF-ARC-001 — Architecture Overview](../../../01-Architecture/DF-ARC-001-ArchitectureOverview.md)
- [DF-ARC-002 — Architectural Principles](../../../01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md)
- [DF-ARC-003 — Architectural Concepts](../../../01-Architecture/DF-ARC-003-ArchitecturalConcepts.md)
- [DF-ARC-004 — Architectural Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md)
- [DF-ARC-007 — Component Documentation Structure](../../../01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md)

## 39.3. Classification

- [DF-CLS-001 — Classification Architecture](../01-Architecture/DF-CLS-001-ClassificationArchitecture.md)
- [DF-CLS-002 — Classification Concepts](../01-Architecture/DF-CLS-002-ClassificationConcepts.md)
- [DF-CLS-003 — Classification Model](../01-Architecture/DF-CLS-003-ClassificationModel.md)
- [DF-CLS-004 — Classification Elements](../02-Structure/DF-CLS-004-ClassificationElements.md)
- [DF-CLS-005 — Classification Schema](../02-Structure/DF-CLS-005-ClassificationSchema.md)
- [DF-CLS-006 — Classification Lifecycle](../03-Behavior/DF-CLS-006-ClassificationLifecycle.md)
- [DF-CLS-007 — Classification Validation](../03-Behavior/DF-CLS-007-ClassificationValidation.md)
- [DF-CLS-008 — Classification Governance](../03-Behavior/DF-CLS-008-ClassificationGovernance.md)
- [DF-CLS-009 — Classification Relationships](../02-Structure/DF-CLS-009-ClassificationRelationships.md)
- [DF-CLS-010 — Classification Constraints](../03-Behavior/DF-CLS-010-ClassificationConstraints.md)
- [DF-CLS-011 — Classification Extensibility](../03-Behavior/DF-CLS-011-ClassificationExtensibility.md)
- [DF-CLS-012 — Classification Best Practices](DF-CLS-012-ClassificationBestPractices.md)
- **[DF-CLS-013 — Classification Dictionary](DF-CLS-013-ClassificationDictionary.md)**
- [DF-CLS-014 — Classification Specification](DF-CLS-014-ClassificationSpecification.md)
- [DF-CLS-015 — Classification Examples](DF-CLS-015-ClassificationExamples.md)

---

# 40. Working terminology decisions, scoped references, affected sources and provenance

This is the actual authorized working Dictionary successor,not proof canonical approval,fulfilled conditions,effective adoption,activation,publication or exact Baseline membership. Reference/current04-Reference responsibility remains correct. Actual working meaning follows source/definition editions,scope,applicability and real owner authority;entry presence is not complete approved population. Current role/definition columns and sourced notes qualify received old meanings;earlier exact text remains historical evidence,not simultaneous contradictory current authority.

| Actual decision | Received meaning / risk | Current working choice | Actual authority | Need, rationale and alternatives |
|---|---|---|---|---|
| Authoritative current roles and typed domain subjects | Canonical Family top-level grouping,TypeFamily specialization,Class further hierarchy;Element/value/assignment and table36 collapse subject context | Membership Family,one uniform four-value primary Type,optional defined Class;actual definition/category/value/assignment/kind/constraint/record/document/context and known role duties/general-count gaps separated | ReviewPolicy3/4,current Elements5–8,Model11–14,Schema34,Relationships20/23/34/43/46/71,Constraints28/48 and Identity | Keeping old authoritative definitions contradicts actual adopted roles;header-only/label repair cannot reconcile semantics. Deleting entries loses full source. Selected actual term replacements preserve all73 headings/subjects/related strings,original exact before-evidence and tables with explicit current columns,no field/key/component population allocation. |
| Terminology authority,related names and actual owner references | Canonical vocabulary/approved-source fallback and201 related-term occurrences with17 distinct nonexact local labels can imply complete approval,population or unqualified imports | Actual working authoritative meaning under identified source/definition editions/scope,not actual canonical adoption;201 occurrence-level local/contextual/imported/limited dispositions and actual owner clauses,73 original entries retained | ARC00710,ReviewPolicy1/5/6,current Architecture/Classification/Specification/Identity owners,actual external ARC0034/5.3,ARC0055/5.1,ARC0026.3,Governance51/Relationships20 | Inventing17 new entries or treating names as approved aliases fabricates authority;marking every nonmatch undefined discards real owners. Selected exact references/qualified shorthand/contextual gaps preserve literal strings and explicitly admit no exact local RetiredTerm/Multiplicity entry or complete imported registry. |
| Term state,domain lifecycle,identity and required history | Activevalid-and-available,DeprecatedTermno-new-reference,status24 mixed naming/authority/use and selected term-state path can imply global validity,blocked historical references or universal machine | Actual scoped term/definition naming/authority/use versus Element/assignment/extension/decision/document/term/R/result/finding states;eligibility not full validity/access;required historical definitions/editions/pinned context and separate authorized effects | Lifecycle19/20/48/53,Governance43/51,Relationships34/46/61,Constraints31/48/67/68/74/75/86.7,Extensibility38/41–44/69/70,DID014 | Universal enums/keys/availability or automatic history invalidity invent consequences. Selected bounded definitions preserve known duties and legitimate historical/pinned references,with genuine exact actor/guard/route/record gaps and traced earlier-contract reassessment rather than backdated new rules or erased observations. |
| Actual rule/result/decision authority and necessary assessed revision | Validation/conformance/approval/extension meanings underspecify evidence/coverage/conditions/effects and can freeze all meaningful revision or manufacture precedence | Actual criterion versus aggregate outcomes,applicability/authority/observations/coverage/nonmutation;actual scoped decisions/fulfilled conditions/effective adoption distinct from activation/publication/Baseline;ordinary preservation versus necessary assessed prior/new mandate revision | Validation16/39/67,Constraints46/50/54/56/59/69/71/91,Governance19/43/51/53/55/56,ExtensibilityV2R2 33/35/37/39/50/51/79,SpecificationR029/R030/13/14/Core16.1 | Unknown support is not result/violation/permission,approval does not fulfill itself,and absolute freeze blocks necessary justified correction. Selected actual owner meanings retain independent mandatory breadth/gaps and prior/new authority/need/alternatives/batch/compatibility-history/transition/checks,not arbitrary changes or waived Metadata restrictions. |
| Entry/table preservation,interfaces and honest successor scope | Five-field convention/principal table/status table/quality/checklist and semantic independence can be mistaken for complete mandatory physical schema,approved population or no provider/physical effects | 73 actual entry/201 reference/29 table-pair maps with current scope,14 unchecked prompts,actual domain/common/Metadata/Identity/capability/executor/provider duties and independent placement/global limits. Actual incompatible authoritative meaning replacement justifiesV2R1 | ReviewPolicy5–7,ARC005/007,actual current responsible Classification/Metadata/Profile/Identity sources and concrete36-path pre-mutation batch | Replacing dictionary with a summary or turning conventions into allocated fields loses scope;renamed graph/Local labels cannot erase required providers/cycles. Selected complete preserved subjects/current maps and actual provenance allow reviewable local correction without peer rewrite,canonical adoption,physical migration or global acceptance. |

All73 original entry headings/subjects and201 Related Terms literal strings/order remain. The original Term representation is its heading;Notes was conditional,not a missing universally required field. Current Notes supplies actual owner/context/history/reference limits without physical Metadata field allocation. All17 distinct nonexact labels have occurrence-specific dispositions:9 contextual local phrases,Retired Term referring to the actual qualified term-status row,and7 external/contextual owner concerns. These are no allocated alias registry,new canonical entries or full imported population. Multiplicity retains genuine complete general-count/representation gaps;Retired Term has no separate standalone canonical entry. Same-string/exact-local navigation is neither semantic identity,inheritance,approval nor indispensable provider dependency.

Actual Family membership,uniform four-value primary Type and optional defined Class replace incompatible authoritative role meanings and derived hierarchy/state/authority/evolution interpretations. Therefore actual V1.0 R0→V2.0 R1 is a major semantic successor under ReviewPolicy5.2,not a major increment caused by format,title,Type Reference,links or peer edition numbers. Dictionary is an authoritative scoped terminology reference;the informative Best Practices correction is not its authority model. Revision remains monotonic;Draft/Baseline Not assigned and cumulative real contributors remain. Original meaning/earlier source-edition observations are retained;new rules are not backdated. Current conformity/use/retrieval,original conformity,historical interpretation and traced earlier-contract reassessment are distinct.

Actual known owner duties and genuine general-rule/population/actor/guard/route/record/precedence/field/count/implementation gaps remain. Eligibility is not complete assignment validity,permission or live availability. Term authority/naming/use states differ from domain Element/definition/assignment,document Workflow,extension/proposal/decision/activation,relationship/constraint-set,local R,result/finding and Milestone states. Legitimate historical/quoted/pinned references and required prior definitions,rules,sets,relations,assignments,states,decisions,conditions,results/source editions remain;deprecation or retirement neither destroys required history nor automatically migrates,invalidates or deletes consumers.

Actual Validation16/39/67 and Constraints46/50/54/56/59 retain criterion versus three rule-dependent aggregate results,identified applicable source/definition/rule-set editions,authority,observations/context/mandatory coverage and nonmutation. Unknown is not NotApplicable,permission,success,fabricated violation,fourth result or waiver;known violations persist. Actual Governance/Extensibility authority,conditions/fulfillment,effective adoption/activation and separate publication/Baseline remain necessary in real scope. Approval alone fulfills none. Ordinary preservation and necessary explicitly assessed normative/foundational/role/interface/domain revision differ;actual prior/new mandates,authority,need,alternatives,batch,interfaces,honest compatibility,mappings/history,pinned continuity,authorized transition and later checks are needed. No arbitrary mutation or blanket freeze;unchanged Metadata no-invalidating/no-redefinition/Profile/owner restrictions are not silently waived.

Actual domain/common typed records/process/projections,Metadata broader Concepts/Values/Dictionary/Schema/Profile/Instance/effective representation,Identity K/local R/exact edition,Automation capability and authorized DMS/CMS/tool/manual executor retain separate ownership. Meaning independence waives no physical/representation/reference/index/interface/access/retrieval/freshness/use/history duties. Actual indispensable Classification→Metadata/Identity,conditional Templates and reciprocal Metadata↔Identity descriptor/provider/core/source-edition/interface/cycle claims remain pending responsible work. Renaming semantic edges or Local labels erases no required provider/cycle;this Dictionary is no accepted merged schema,DAG,runtime or operational permission.

The concrete prospective36-path source/owner/consumer/interface batch below was established against actual source coordinates/hashes/clauses before mutation. All peers remain byte-identical;this is coordination evidence,not completed cross-source propagation or knowledge of every external consumer. Fifty received inbound occurrences across19 input-of-REVIEW sources and29 actual prior-note contexts remain source-qualified/event-time evidence. Their old DictionaryV1R0 observations are not rewritten into current approval or silently revalidated. Model reconstruction/prior factual qualifications and CLS011 initial failedV2R1/later correctedV2R2 result history remain intact;completed cycles are not reopened.

| Actual path | Received edition / raw SHA-256 | Coordinated concern / proposed disposition | Authority / interfaces / compatibility and history |
|---|---|---|---|
| /01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md | V2.0 R2;3993411c226cccd1b67059c97b09ef39646afc8021d9b55470ddbc6c737bfe16 | Keep actual principles/necessary assessed revision,semantic continuity/quality authority and compatibility/history;Dictionary vocabulary does not freeze all necessary mandate change or prove approved adoption. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /01-Architecture/DF-ARC-005-ArchitecturalComponents.md | V2.0 R2;0329a1ad17f95108fe9ef770e5e1de779efd1f0f8fce18cab0f28fecfcca4a6b | Actual Classification semantic owner,common typed records/process/projections/Automation,Metadata-Identity and authorized executor remain distinct. Common/external Related Terms need actual owner clauses,not new Classification fields/components or a complete provider DAG. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md | V2.0 R2;0fdc12e1d096c61152a2eeef175b2bd61b23970a6842f0d9e680780538e9aea5 | Terminology reference remains Reference/current04-Reference;authority follows explicit actual scope/definitions/incorporation,not Type/title. Both Elements/Constraints actual placement residuals remain unmet/M13. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/01-Architecture/DF-CLS-001-ClassificationArchitecture.md | V2.0 R1;6eb5fe3d98319b15ec487a13aaf705bc6e4d399974aec0f72d3f33b2d583e7d4 | Actual membership/uniform Type/optional defined Class and owner interfaces remain;earlier DictionaryV1R0 observations retain event-time/source-qualified scope,not current canonical old hierarchy or successor acceptance. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md | V2.0 R1;640b3e6ad7ed850d45a4eaee97403810915402342c39c5cbd024421a912a23e4 | Actual concept/Element/definition/category/value/assignment/identity contexts remain;Dictionary terms should distinguish them without transferring owner responsibility or populating a complete approved registry. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md | V2.0 R1;82e5cace5d9bc7b05f2f591c25462a7adcf0a2253a751fdeca36ea9392045039 | Actual reconstructed Model11–14 role/cardinality and23 state/use/26 necessary revision retain source scope. Old Family-owned Type/Class glossary definitions do not replace actual current working mandates or authentic recovered history. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/02-Structure/DF-CLS-004-ClassificationElements.md | V2.0 R1;c64b43036aa8d9950a6ad792166f67d1113e789264ff37edc7a6f4c9e14d68d8 | Actual5/6/7/8 roles/definition/value/assignment and real identity/lifecycle duties remain;Elements known Architecture/02-Structure placement unmet/M13 independent of semantic Dictionary correction. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/02-Structure/DF-CLS-005-ClassificationSchema.md | V2.0 R1;e618b7c98ee5c416a1e6187441c94694fa16492d703d5788c122aedbaafe61a1 | Actual34 known role duties and general multiplicity/field/population gaps,representation/conformance remain;Dictionary cardinality/multiplicity/attribute labels allocate no arbitrary counts/fields or blanket unknown-duty deferral. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md | V2.0 R1;f52b83ab5ed3b65bd9a22d15a2ab3ab5ad44a22e74edd0c49e61c9c3e5b80a8b | Actual19/20/48/53 definition/state/use/transition/history and genuine exact actor/guard/route/record gaps remain. Active eligibility is not every assignment valid/permitted/live-available;term/document/extension/R states differ. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/03-Behavior/DF-CLS-007-ClassificationValidation.md | V2.0 R1;3db6e857f5c4e017e11cba345a327eba11ab200e09c6cb3a1e4fb1feadefef01 | Actual16/39/67 criterion/aggregate results,rule/applicability/authority/observations/mandatory coverage/nonmutation/equivalence remain;glossary/result/checklist presence does not produce full conformance or permission. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/04-Reference/DF-CLS-014-ClassificationSpecification.md | V1.0 R0;e3edf0047a9cf3dcdbc5c3f69f1c64ad2b7872dc792b0d9641bf8999ccc2f663 | Actual normative requirements/incorporation/R014/13,R023–025,R027,R029/R030,14/16.1/28 retain source scope. Dictionary role/approved-source fallback grants no blanket priority,complete catalog,condition fulfillment or implemented Core acceptance. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/04-Reference/DF-CLS-015-ClassificationExamples.md | V1.0 R0;204db601fc644f2fb799905beb8e03676ecf258a9a7dad7a4f509be0cf6e0603 | Examples remain scoped illustrations,not accepted terms/aliases,allocated keys/fields,actual assignment/state/decision/operation or performed full conformance evidence. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/README.md | V? R?;452c9910cdb26654cf475c21f6c4b3bf13f624d1c4b3bfd88538d818a1474c18 | Non-normalized index retains Dictionary Reference/current path. Future intended term/source-edition/reference coordination needs actual scoped batch/history,not silent propagation/reopened peer cycle. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/DocumentIdentity/02-Structure/DF-DID-009 - Document Identity Relationships.md | V2.0 R1;892dab07966a3a6e49ebcd2e97afeb9898c8022f7889d6538a24b8260cac4566 | Actual typed entity/document/record/edition/reference/projection/provider scopes remain;glossary identity/hierarchy/name labels cannot remove actual reciprocal Metadata↔Identity core/descriptor/interface/cycle duties. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/DocumentIdentity/04-Reference/DF-DID-014 - Document Identity Specification.md | V2.0 R1;972291275ecb10e8a2ae17f9071e4ca3fa5d45eb5958fd202372aaf228f56dec | Actual document K/local complete R/exact edition/reference versus term/concept/definition/assignment/record identity and nonreuse/history apply. Canonical name/identifier/synonym is no universal DF allocation/rekey/consumer revision or pinned-history retargeting. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/01-Architecture/DF-MTD-001-MetadataArchitecture.md | V1.0 R0;7a757a7e72d108bf307d1a71f323ff54aea0a2e20e9541cb86558731ec0a4747 | Actual Metadata→Identity and reciprocal supplied descriptor/provider/source-edition duties remain;terminology coherence creates no global provider consistency or waived indispensable edge/cycle. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/01-Architecture/DF-MTD-002-MetadataConcepts.md | V1.0 R0;1abf7b1d0c2b80b14bff6d49c902f9ba8f951889daf833522e33e2e08fe5e19c | Actual Metadata descriptive/representation meaning differs from domain Classification role/definition/term/assignment;Dictionary conventions/context fields allocate no mandatory Metadata Elements or owner takeover. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md | V1.0 R0;0eb29cbb5dda1c85d88f90cf01a06df7a2d34258cfe183347e00364740661746 | Actual broader Schema/Profile/Instance/effective representation model remains;glossary Entry Field/Attribute/Context/Status are conceptual requirements in actual scope,not universal physical record fields or complete merged representation. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/01-Architecture/DF-MTD-004-MetadataElements.md | V1.0 R0;60dc7aa35153410b7bfacb774163d62959c3c830b6fa15948a82f913c0657568 | Metadata Element/definition identity differs from Classification concept/term/definition/assignment and document identity. Related Terms lists/headings/status/summary rows allocate no DF or Metadata IDs. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/02-Structure/DF-MTD-005-MetadataSchema.md | V1.0 R0;1ed13b4f94564703e5b5af1268941e21a329cfc62b9c67e3f69cc63b8c2fa302 | Actual Schema/effective Profile/Instance field/value/representation conformance remains independently mandatory;Dictionary semantic independence supplies no complete structural compliance or waived physical/reference obligations. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/02-Structure/DF-MTD-009-MetadataRelationships.md | V1.0 R0;ed847e8f5e9026159ac119432c9b77cbaf6f790cd771296b99809a96759a74dc | Actual Metadata relation categories/known Profile-Instance providers/no-owner-transfer/no-cycle restrictions remain;semantic terminology/inverse/projection cannot conceal mandatory reciprocal provider edges. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/02-Structure/DF-MTD-010-MetadataConstraints.md | V1.0 R0;466cc09d475f690779ea0f929dcafea150e643f9d2a622e47d87f519426142fa | Actual constraint/dependency/profile/stability/applicability/external enforcement duties remain;necessary assessed Classification terminology revision does not silently edit or waive unchanged Metadata restrictions. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md | V1.0 R0;3c0a07a8cf9e9ed4cd43fe70591e883e235fa3c5a11013fb9b651e72facc7206 | Actual Metadata descriptor/term/definition/source-edition authority remains;Dictionary Term/Definition/Context/Related Terms/Notes conventions are not complete canonical fields/registry or automatically imported aliases. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/03-Behavior/DF-MTD-006-MetadataLifecycle.md | V1.0 R0;ddb15d2cbffe7ec2d4c0f9903226f65f98d3a63f82afa3864433173e5cc86acc | Actual Metadata lifecycle states differ from Dictionary term-status roles,Classification Element/document/extension/term/localR/result/finding states;no name-based alias,automatic transition or universal machine. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/03-Behavior/DF-MTD-007-MetadataValidation.md | V1.0 R0;163c13b58acba33353e66d472649759ced513f6742d9231d3e60d7562ec632aa | Actual descriptor/Profile/Instance/rule/authority/coverage checks remain;Dictionary Validation/Conformance definitions alone establish no implemented Metadata validity or operation permission. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/03-Behavior/DF-MTD-008-MetadataGovernance.md | V1.0 R0;69112d8cce7fb5bb511c9d548bf64ab0e2a97c3b9bfd667d5225ccf626569c8d | Actual Metadata decision/outcome/rationale/conditions/process/owner restrictions retain scope;Dictionary Retain/Rename/Deprecate/Retire are selected actions,not universal closed decision enum or performed canonical adoption. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/03-Behavior/DF-MTD-011-MetadataExtensibility.md | V1.0 R0;044fc204c8b877e705902d3a7fbfe7c2bd5b40fa18aa32ea6602f38131e7ab26 | Actual no-invalidating/no-redefinition/Profile/semantic/owner restrictions remain real source-specific pending differences,not waived by Classification extension/evolution definitions or corrected role meanings. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/04-Reference/DF-MTD-012-MetadataBestPractices.md | V1.0 R0;324fd72a22bf6417d1f0a05f43ff1d01f7666c6f61916acf96c7730159935f61 | Explicit advice remains informative unless actual owner adoption states otherwise;Dictionary quality/smell/anti-pattern definitions create no new mandatory threshold,outcome,actor,field or permission. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/04-Reference/DF-MTD-014-MetadataSpecification.md | V1.0 R0;55cf09d6237304314d18e6e13d7cfd74e41e222ebae0779002d7d8e6ae7ddf2e | Actual independent Profile/Instance/descriptor/owner conformance remains;Dictionary authority/meaning/context/population claims supply no complete accepted representation schema or global implementation proof. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Metadata/04-Reference/DF-MTD-015-MetadataExamples.md | V1.0 R0;9de2984688ff67469ee6b0761aa445d0cc23b7075738e11277ece2462f24a7c8 | Informative examples supply no actual canonical term/field/status/precedence,allocated identity,decision/condition fulfillment or measured validation evidence. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md | V1.0 R2;8f6c3a967f076dfc3ddd4fef90b5901dbb780e0a8c7cda17c70039e2f581f9ef | Actual phase/evidence/edition/cumulative-author/stable-ID/functional-exclusion rules apply. Preserve correct Reference/path/valid identity and original author/history. ProposedV2R1 conditional on actual incompatible authoritative meaning replacement,not label/format alone;changed successor Draft/unassigned,no canonical/global approval. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/03-Behavior/DF-CLS-008-ClassificationGovernance.md | V2.0 R1;1d95ca2f294ea07b421270a39abe590fe97d237247b132f29fcaef55454ba04c | Actual19/43/51/53/55/56 domain decision/authority/evidence/rationale/conditions/fulfillment/effective adoption/publication/Baseline and genuine actor gaps remain;term status/action labels are not universal enums or approval sufficiency. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/02-Structure/DF-CLS-009-ClassificationRelationships.md | V2.0 R1;ff31f08fc6fb489172e6df335250ff5dbf0e77d90f4651e84f6e94fd414ecfce | Actual20/23/34/43/46/49–54/71 kind/definition/association/assertion/typed endpoints/properties/cardinality/integrity/identity/state/record/provider distinctions remain;Dictionary relation terms allocate no universal tuple key/fields or all-document endpoints. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/03-Behavior/DF-CLS-010-ClassificationConstraints.md | V2.0 R1;7a05118d2533f3cfa347e154f1844fe74de1cb08d224aa3a619742e0f60fa5c0 | Actual28/31/46/48/50/54/56/59/67/68/69/71/74/75/91 constraint/rule/set/edition/identity/applicability/precedence/authority/evaluation/history/necessary revision retain mandatory breadth and genuine gaps. Structure/current03-Behavior placement remains actual unmetM13. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/03-Behavior/DF-CLS-011-ClassificationExtensibility.md | V2.0 R2;2b9a1576001c0bd040a31d1bb6b374d241cb13ca8b1acbe48f3006d79d8209e8 | ActualV2R2 7.1–7.6/24/34/35/37/38/39/50/59/71/79 role/authority/condition/fulfillment/Dictionary incorporation/necessary-revision/history duties remain. InitialV2R1 FAIL and later exactV2R2 local PASS stay separate history,not glossary canonical approval. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |
| /02-Documentation/Classification/04-Reference/DF-CLS-012-ClassificationBestPractices.md | V1.0 R1;0ee4177757f0c774e95d5322488672653e2091cc23bf77de3439d5208f3ad4b0 | ActualV1R1 explicit informative advice/omission-alone-no-violation and4/23/53/54/93/102/104 boundaries remain. Best Practice/quality/synonym/inflation glossary definitions should not turn heuristics into new mandates,thresholds,completed checks or permission. | Actual adopted ReviewPolicy/current responsible Architecture/Classification/Specification/Identity/Metadata/common sources;REVIEW changes no term/source/owner requirement or canonical adoption. Actual term/concept/definition/value/assignment/kind/constraint-set/state/use/decision/result/document/record/source editions,common records/process/projections/capability/authorized executor,Metadata effective-Profile/Identity/provider interfaces and actual related-term imports. Actual prior/new definition/mandate,need,authority,alternatives,batch/interfaces,honest compatibility,mappings/nonreuse/history/pinned snapshots,authorized coordinated transition and later checks. No automatic field/key allocation,consumer revision,rekey or event rewrite. |

All39 original chapters/131 numbered bodies,73 entry blocks,29 original convention/status/principal row pairs,86 lists,six exact unnamed fenced spans/46 literal label-relation occurrences,26 related-document subjects/order/selflink and14 unchecked checklist labels remain mapped. Original undated initial history and Arnaldo authorship remain;actual later contribution is separate. Quality/examples/checklist prompts are not performed observations,thresholds,severities,mandatory fields or canonical allocation. New tables use separate headers;no diagram IDs or Author auxiliary are introduced.

Twenty-four source-local corrections remain Corrected—pending validation;none closes through construction. Separate VALIDATE must assess this exact V2.0 R1 edition and original criteria. M12 remains27 C/1 S/36 O In Progress,Dictionary S with no completion. EntireM13 Not Started is unchanged. Actual Elements Architecture under02-Structure and Constraints Structure under03-Behavior remain unmet ARC007 placement requirements,not compliant,waived or mere evidence gaps. M14/global19/actual owner/integration/implementation/permission/architectural acceptance remain independent. Local documentary results are not global architectural approval.

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of Classification Dictionary. |

---

## Actual later contribution

| Date | Version | Revision | Contributor | Actual contribution / scope |
|---|---|---|---|---|
| 2026-10-16 | 2.0 | 1 | Codex — AI assistant | Step4.41 UPDATE: actual incompatible authoritative terminology correction with full preserved subjects/reference/table/view/history maps and current owner scope;24 corrections pending separate VALIDATE. Draft;Baseline Not assigned;no canonical adoption or global approval. |

**End of Document**
