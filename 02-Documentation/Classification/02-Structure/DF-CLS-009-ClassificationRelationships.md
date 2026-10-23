# Documentation Framework

# DF-CLS-009 — Classification Relationships

| Metadata | Value |
|----------|-------|
| **Document ID** | DF-CLS-009 |
| **Title** | Classification Relationships |
| **Family** | Classification |
| **Type** | Structure |
| **Component** | Classification |
| **Author** | Arnaldo Figueira; Codex — AI assistant |
| **Status** | Draft |
| **Version** | 2.0 |
| **Revision** | 1 |
| **Baseline** | Not assigned |
| **Language** | English |

---

# 1. Introduction

Classification organizes documents through a structured semantic model.

The Classification model is not limited to isolated Classification Elements.

Classification Elements may be semantically related to one another.

These relationships provide the structural and semantic connections required to understand:

- how Classification Elements are organized;
- how Classification Elements specialize one another within an actually defined scheme, rather than a universal documentary-role hierarchy;
- how Classification Elements relate across the Classification model;
- how Classification evolves;
- how Classification Elements may be replaced or superseded.

Classification Relationships defines the architectural model governing these relationships.

**Current governing scope.** Current applicable Family denotes actual canonical component or admitted documentary-area membership. Type is exactly one uniform primary Architecture, Structure, Behavior or Reference responsibility; Class is separate optional additional explicitly defined non-conflicting meaning. A relationship kind, definition, actual association/assertion, role/category/value definition, assignment, logical document/exact edition and represented connection are different subjects. A semantic scheme can have real hierarchy without making the three documentary roles universally hierarchical.

---

# 2. Purpose

The purpose of Classification Relationships is to define how relationships between Classification Elements are represented and governed.

This document establishes:

- relationship concepts;
- relationship types;
- relationship semantics;
- relationship direction;
- relationship cardinality;
- relationship constraints;
- relationship integrity;
- relationship lifecycle;
- relationship governance.

It does not define the complete Classification vocabulary.

The vocabulary is defined through the Classification Dictionary and Classification Specification.

**Current governing scope.** These are domain structural contracts and required assessment concerns, not evidence of completed implementation or approved complete vocabulary. Actual Dictionary/Specification terminology, earlier role differences and genuine general-rule/population/record gaps remain visible. Definition, checking, decision, operation, canonical adoption, publication and exact Baseline selection are separate claims.

---

# 3. Scope

Classification Relationships applies to relationships involving:

- Families;
- Types;
- Classes;
- other formally defined Classification Elements.

The document covers relationships that form part of the Classification architecture.

It does not define:

- document-to-document relationships;
- Knowledge Graph implementation;
- Registry implementation;
- repository relationships;
- workflow relationships;
- implementation-specific relationship storage.

**Current governing scope.** The actual claim identifies endpoint kinds, relationship-kind/definition/assertion and source/definition/target edition/context where needed. Applicable normalized documents use current roles; excluded functional README/CHANGELOG/ArchitecturalMilestones files remain non-normalized at every location while content/reference effects still apply. A proposal may precede document allocation; not every entity receives a DF key. The exclusion of document-to-document relations here does not redefine all common Relationships endpoints as document-only. Authorized working Draft correction is not a canonical decision, operational permission or architectural approval.

---

# 4. Relationship Concept

A Classification Relationship establishes a semantic association between Classification Elements.

Conceptually:

**Received unnamed visual in §4 (span 1 in original order).** Exact text below is evidence,not a second governing rule.

```text

          Classification Element
                    │
               Relationship
                    │
                    ▼

          Classification Element

```

**Current relation scope:** Actual semantic association and three explanatory endpoint/kind subjects;domain kind/definition/assertion and common record/Metadata representation differ,no universal fields or automatic validity.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| Relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Classification Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |


A relationship therefore consists of at least:

**Received unnamed visual in §4 (span 2 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Relationship
            ├── Source
            ├── Relationship Type
            └── Target

```

**Current relation scope:** Actual semantic association and three explanatory endpoint/kind subjects;domain kind/definition/assertion and common record/Metadata representation differ,no universal fields or automatic validity.

| Received label / relation | Current typed interpretation |
|---|---|
| Relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| Relationship Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |


The relationship type determines the meaning of the association.

**Current governing scope.** Source, Relationship Type and Target are semantic subjects, not three newly allocated physical Metadata fields. Relationship Type means relationship kind, not primary document Type. Identify actual endpoint kinds and their responsible identity/definition editions, relationship meaning/applicability and actual association evidence; readable labels or the presence of a definition alone establish no valid assignment, current use or full connection conformity. Claim-dependent context is required evidence, not a universal stored tuple.

---

# 5. Relationship Model

The general model is:

**Received unnamed visual in §5 (span 3 in original order).** Exact text below is evidence,not a second governing rule.

```text

              Source Element
                    │
               Relationship
                    │
                    ▼

              Target Element

```

**Current relation scope:** General directed-association concern plus exact historical Family→Type and Type→Class containment examples;current roles are complementary,not universally hierarchical.

| Received label / relation | Current typed interpretation |
|---|---|
| Source Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| Relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Target Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |


The received role-hierarchy examples are retained as historical evidence:

**Received unnamed visual in §5 (span 4 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                 contains
                    │
                    ▼

                   Type

```

**Current relation scope:** General directed-association concern plus exact historical Family→Type and Type→Class containment examples;current roles are complementary,not universally hierarchical.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


and:

**Received unnamed visual in §5 (span 5 in original order).** Exact text below is evidence,not a second governing rule.

```text

                   Type
                    │
                 contains
                    │
                    ▼

                  Class

```

**Current relation scope:** General directed-association concern plus exact historical Family→Type and Type→Class containment examples;current roles are complementary,not universally hierarchical.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


The relationship itself has semantic meaning independent of its physical representation.

**Current governing scope.** The three received spans distinguish a general directed association concern from historical Family/Type/Class containment. Current roles are complementary, not a universal containment chain. Actual domain relationship semantics and common typed connection representation remain separate; a visual neither creates a provider edge nor performs an assignment.

---

# 6. Relationship Identity

A Classification Relationship shall be identifiable.

A conceptual relationship identity may be represented as:

**Received unnamed visual in §6 (span 6 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Relationship Identity
            ├── Source
            ├── Type
            └── Target

```

**Current relation scope:** Possible conceptual identity composition,with Type meaning relationship kind;actual uniqueness/context/definition/assertion/record/K/R distinctions in matrix46,no universal tuple key.

| Received label / relation | Current typed interpretation |
|---|---|
| Relationship Identity | Actual relationship/kind/definition/assertion identity versus endpoint,record/projection/lookup identity needs responsible scope. Source+kind+target may describe conceptual composition,not a proved universal key;document K/local R/exact edition are distinct. |
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. This exact Type position denotes the relationship kind,not documentary Type. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |


The physical representation of relationship identity is implementation independent.

**Current governing scope.** The possible Source/Type/Target conceptual composition is retained with its original may qualification. Type here means relationship kind. Relation-kind definition identity, actual association/assertion identity, endpoint identity and record/projection/lookup identity are different. The tuple alone proves no global unique key across actual schemes, definitions, source editions or historical/contextual records; actual responsible uniqueness/duplicate rules and precise claim context govern. Section46 supplies the identity/comparison matrix without inventing mandatory universal fields or DF allocations.

---

# 7. Relationship Direction

Classification Relationships are directional unless explicitly defined as symmetric.

A directional relationship has:

**Received unnamed visual in §7 (span 7 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Source  ─────  Relationship  ─────►  Target

```

**Current relation scope:** Actual direction and historical/conditional role inverse examples;source-target semantics differ,only defined inverse/symmetry applies,no generated reverse records or required dependency.

| Received label / relation | Current typed interpretation |
|---|---|
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| Relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |


The source and target have different semantic roles.

For example:

**Received unnamed visual in §7 (span 8 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family  ─────  contains  ─────►  Type

```

**Current relation scope:** Actual direction and historical/conditional role inverse examples;source-target semantics differ,only defined inverse/symmetry applies,no generated reverse records or required dependency.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


is not equivalent in representation to:

**Received unnamed visual in §7 (span 9 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type  ─────  contains  ─────►  Family

```

**Current relation scope:** Actual direction and historical/conditional role inverse examples;source-target semantics differ,only defined inverse/symmetry applies,no generated reverse records or required dependency.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


The inverse relationship may have a different relationship type:

**Received unnamed visual in §7 (span 10 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type  ─────  belongs to  ─────►  Family

```

**Current relation scope:** Actual direction and historical/conditional role inverse examples;source-target semantics differ,only defined inverse/symmetry applies,no generated reverse records or required dependency.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |

**Current governing scope.** Keep actual direction significant unless responsible semantics explicitly defines symmetry. Every received Family/Type contains/belongs-to example is historical or conditional, not current Family ownership. An inverse changes navigation perspective under an actual definition; it does not automatically reverse required provider direction, create records, perform a mutation or establish symmetry/transitivity. Actual Specification R012 and Constraints21 direction mandates remain.

---

# 8. Relationship Semantics

Every canonical Classification Relationship shall have a defined semantic meaning.

A relationship shall not exist merely because two Classification Elements happen to be associated.

The relationship type must explain the nature of the association.

Conceptually:

**Received unnamed visual in §8 (span 11 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Source
            │
            ├── relationship meaning
            │
            ▼

          Target

```

**Current relation scope:** Actual explicitly defined relationship meaning under responsible source/edition/context,not mere coincident labels,physical fields or full association validity.

| Received label / relation | Current typed interpretation |
|---|---|
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| relationship meaning | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |

**Current governing scope.** Defined semantic meaning and applicability must be evidenced for the actual kind/definition/association claim. A readable label, coincident connection, approved endpoint or diagram does not supply all owner requirements. Canonical name, display label, inverse kind, synonym and definition identity are distinct; §28 records the actual incomplete vocabulary/alias boundary.

---

# 9. Canonical Relationships

Only relationships that are part of the approved Classification architecture shall be considered canonical.

A relationship becomes canonical through the applicable governance process.

This preserves the principle established in Classification Governance that unauthorized Classification definitions and structural changes must not become part of the canonical architecture.

**Current governing scope.** Approval under actual scope/authority is necessary, not proof alone that required conditions, effective adoption, activation, publication or exact Baseline inclusion occurred. Use actual Governance V2.0 R1 matrices19/43/51 and §§53–56/72, not its older snapshot. Unknown decision/condition evidence supplies no automatic outcome or permission; authorized Draft work remains identifiable noncanonical material.

---

# 10. Primary Classification Relationships

The received earlier model illustrated a primary hierarchy, retained below as historical evidence:

**Received unnamed visual in §10 (span 12 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                    ▼

                   Type
                    │
                    ▼

                  Class

```

**Current relation scope:** Exact received universal role-hierarchy claim retained only as historical evidence;actual schemes may define their own hierarchy,not Family-owned document Type or mandatory Class.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


The corresponding semantic relationships are:

**Received unnamed visual in §10 (span 13 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family  ─────  contains  ─────►  Type
            Type    ─────  contains  ─────►  Class

```

**Current relation scope:** Exact received universal role-hierarchy claim retained only as historical evidence;actual schemes may define their own hierarchy,not Family-owned document Type or mandatory Class.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


These received relationships expressed the earlier Family-owned specialization. They are not the current governing documentary-role hierarchy; actual scheme-specific relationships require their own definitions and properties.

**Current governing scope.** Current Family membership, uniform Type responsibility and optional defined Class are not three mandatory hierarchical levels. Hierarchical and non-hierarchical relationships in an actual explicitly defined scheme remain possible under actual Model/Schema/Constraints/Specification rules. Correcting old universal role ownership does not waive genuine direction, structure, applicability or property requirements.

---

# 11. Family-to-Type Relationship

An applicable document Type expresses one uniform primary responsibility; Family identifies actual membership rather than ownership of a Type vocabulary.

Conceptually:

**Received unnamed visual in §11 (span 14 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family
            │
            └── contains  ─────►  Type

```

**Current relation scope:** Historical Family containment/inverse example,current membership Family and uniform Type use actual contextual restrictions without ownership/specialization.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


The inverse relationship may be expressed as:

**Received unnamed visual in §11 (span 15 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type
            │
            └── belongs to  ─────►  Family

```

**Current relation scope:** Historical Family containment/inverse example,current membership Family and uniform Type use actual contextual restrictions without ownership/specialization.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


Actual Family-context applicability shall be evaluated without redefining the uniform Type responsibility or imposing universal Family-owned specialization.

**Current governing scope.** Family context can constrain valid use without redefining the uniform four-value primary Type or creating a Family-owned vocabulary. Actual component/admitted-area membership, documentary directory, category option and new component existence differ; no complete Family population, new component or key is allocated. Exact contains/belongs-to visuals remain prior examples with individual current interpretations.

---

# 12. Type-to-Class Relationship

Class is a separate optional explicitly defined non-conflicting meaning; it is not universally a child of document Type.

    Conceptually:

**Received unnamed visual in §12 (span 16 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type
            │
            └── contains  ─────►  Class

```

**Current relation scope:** Historical/conditional Type/Class containment and inverse,current Class optional defined/non-conflicting;actual scheme hierarchy needs separate authority and no mandatory child/value/field.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


The inverse relationship may be expressed as:

**Received unnamed visual in §12 (span 17 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Class
            │
            └── belongs to  ─────►  Type

```

**Current relation scope:** Historical/conditional Type/Class containment and inverse,current Class optional defined/non-conflicting;actual scheme hierarchy needs separate authority and no mandatory child/value/field.

| Received label / relation | Current typed interpretation |
|---|---|
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


A Class shall have a defined Type context when the Classification model requires hierarchical Classification.

**Current governing scope.** A real hierarchical scheme must identify its actual semantics and permitted endpoints/context. The retained when-required qualification does not make Class universally mandatory, an unrestricted string, a physical third field, a Type duplicate or a known maximum population. Current Schema34 known duties and genuine general cardinality/representation gaps remain distinct.

---

# 13. Classification Hierarchy

The received earlier primary hierarchy is retained as historical evidence:

**Received unnamed visual in §13 (span 18 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family
            │
            ├── Type
            │   ├── Class
            │   ├── Class
            │   └── Class
            │
            ├── Type
            │   ├── Class
            │   └── Class
            │
            └── Type

```

**Current relation scope:** Historical role tree,not complete current vocabulary,cardinality,mandatory Class,population or universal tree structure.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


This received hierarchy is not the current universal organization of documentary roles. Actual structural organization follows current roles and any separately defined scheme-specific relationships.

**Current governing scope.** The exact received tree is an old role-hierarchy example. Its repeated Class/Type labels are not actual allocations, complete vocabulary, number of allowed values or proof every scheme is a tree. Any actual parent/child structure and endpoint multiplicities require responsible rules and evidence.

---

# 14. Hierarchical Relationship

A hierarchical relationship expresses that one Classification Element is structurally contained within another Classification Element.

The received earlier canonical-hierarchy claim is historical evidence:

**Received unnamed visual in §14 (span 19 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                    ▼

                   Type
                    │
                    ▼

                  Class

```

**Current relation scope:** Historical canonical-role chain,not current universal role hierarchy;actual defined hierarchical kind/scheme and real constraints retain their scope.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


An actual defined hierarchical relationship establishes its applicable scheme context; the drawing does not establish a universal Family→Type→Class hierarchy.

**Current governing scope.** Hierarchical meaning belongs to the actual defined relation and scheme; it is not inferred from Family/Type/Class labels, directory order or drawing position. Keep real structural/semantic hierarchy requirements and scoped acyclicity where actual owners require them, rather than declaring arbitrary associations hierarchical.

---

# 15. Parent and Child

Within a hierarchical relationship:

- the containing element is the **Parent**;
- the contained element is the **Child**.

For example:

**Received unnamed visual in §15 (span 20 in original order).** Exact text below is evidence,not a second governing rule.

```text

              Family
              │
              └── Parent
                    │
                    ▼

                   Type
                   │
                   └── Parent
                         │
                         ▼

                       Class

```

**Current relation scope:** Selected historical parent/child role example;Parent is a relation role,not new Element,record cardinality or component dependency.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Parent | Relation role in actual defined hierarchy,not another registered Classification Element,universal Family/Type/Class owner or provider dependency;actual permitted endpoints/properties/context remain. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Parent | Relation role in actual defined hierarchy,not another registered Classification Element,universal Family/Type/Class owner or provider dependency;actual permitted endpoints/properties/context remain. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


Parent and Child are relationship roles.

They do not constitute separate Classification Elements.

**Current governing scope.** Parent and Child remain relation roles, not newly registered Classification Elements. Apply them only to actual defined hierarchical semantics and permitted endpoints. The exact Family/Type/Class span is historical evidence; parent/child labels do not establish current normalized-role ownership, field cardinality or component dependencies.

---

# 16. Ancestor and Descendant

A Classification Element may have ancestors and descendants.

For example:

**Received unnamed visual in §16 (span 21 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family
            │
            └── Type
                │
                └── Class

```

**Current relation scope:** Historical selected ancestor/descendant example;actual ancestry requires defined kind/scheme/endpoint context,not current documentary-role inheritance or generated closure.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


For the Class:

- in the received earlier example, Type is its direct ancestor;
- in that received earlier example, Family is an indirect ancestor.

For the Family:

- in the received earlier example, Type is a direct descendant;
- in that received earlier example, Class is an indirect descendant.

**Current governing scope.** The four original ancestor/descendant subjects retain their received-example meaning. Actual ancestry needs the real hierarchical kind, endpoints, scheme and context; current document Type/Class does not inherit Family ancestry by label alone. Derived navigation does not require additional stored canonical associations or prove a provider path.

---

# 17. Relationship Transitivity

Hierarchical relationships may provide transitive structural context.

For example:

**Received unnamed visual in §17 (span 22 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                    ▼

                   Type
                    │
                    ▼

                  Class

```

**Current relation scope:** Historical selected role chain,only actual semantics supports transitive context;no arbitrary relationship transitivity or runtime/dependency closure.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


expressed the earlier hierarchical Class/Type/Family context. Current documentary roles do not inherit that universal hierarchy; actual scheme-specific transitivity requires explicit responsible semantics.

Transitivity shall not be assumed for arbitrary relationship types.

It applies only where the semantics of the relationship explicitly support it.

**Current governing scope.** The explicit no-arbitrary-transitivity rule remains. Establish the actual relation composition/meaning and responsible applicability; no general transitive closure, all-context ancestry, runtime edge generation or dependency propagation is inferred. Current normalized roles remain separate from this historical diagram.

---

# 18. Relationship Inverse

A relationship may have a defined inverse.

For example:

**Received unnamed visual in §18 (span 23 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family  ─────  contains  ─────►  Type

```

**Current relation scope:** Historical/conditional inverse semantic perspectives of an actual association,not automatic aliases,extra canonical record,operation or reverse provider direction.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


has the conceptual inverse:

**Received unnamed visual in §18 (span 24 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type  ─────  belongs to  ─────►  Family

```

**Current relation scope:** Historical/conditional inverse semantic perspectives of an actual association,not automatic aliases,extra canonical record,operation or reverse provider direction.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


Inverse relationships provide alternative navigation directions without introducing a different semantic association.

**Current governing scope.** An actual defined inverse is an alternative semantic perspective/navigation of the association within its scope. It is not required for every kind, a second independently authoritative meaning, a compulsory physical duplicate or a performed reverse operation. Preserve actual endpoint/direction/property restrictions; historical Family containment does not govern current Type responsibility.

---

# 19. Relationship Symmetry

A relationship is symmetric only when its semantics explicitly define it as symmetric.

For a symmetric relationship:

**Received unnamed visual in §19 (span 25 in original order).** Exact text below is evidence,not a second governing rule.

```text

            A  ─────  relates to  ─────►  B

```

**Current relation scope:** Generic A/B symmetry example only under actual explicitly symmetric semantics;no allocated kind/endpoints or automatic reverse record/required edge.

| Received label / relation | Current typed interpretation |
|---|---|
| A | Generic symmetry-example endpoint placeholder,not allocated category,document or complete vocabulary. Actual relationship definition supplies allowed endpoint kinds,scope and symmetric meaning. |
| relates to | Generic conditional symmetric-association example,not a registered kind or proof every relationship is symmetric. No generated reverse record,transitivity or reverse required dependency from the label. |
| B | Generic symmetry-example endpoint placeholder,not allocated category,document or complete vocabulary. Actual relationship definition supplies allowed endpoint kinds,scope and symmetric meaning. |


implies:

**Received unnamed visual in §19 (span 26 in original order).** Exact text below is evidence,not a second governing rule.

```text

            B  ─────  relates to  ─────►  A

```

**Current relation scope:** Generic A/B symmetry example only under actual explicitly symmetric semantics;no allocated kind/endpoints or automatic reverse record/required edge.

| Received label / relation | Current typed interpretation |
|---|---|
| B | Generic symmetry-example endpoint placeholder,not allocated category,document or complete vocabulary. Actual relationship definition supplies allowed endpoint kinds,scope and symmetric meaning. |
| relates to | Generic conditional symmetric-association example,not a registered kind or proof every relationship is symmetric. No generated reverse record,transitivity or reverse required dependency from the label. |
| A | Generic symmetry-example endpoint placeholder,not allocated category,document or complete vocabulary. Actual relationship definition supplies allowed endpoint kinds,scope and symmetric meaning. |


Hierarchical relationships such as `contains` are not symmetric.

**Current governing scope.** The A/B and relates-to names are generic example placeholders, not allocated identities or a registered symmetric kind. Only an actual responsible definition establishes the symmetry and allowed endpoints/context. Symmetry of a semantic association does not reverse an indispensable consumer→provider requirement or prove a globally cycle-free graph.

---

# 20. Relationship Cardinality

A Classification Relationship may impose cardinality constraints.

For example:

**Received unnamed visual in §20 (span 27 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family 1  ─────  * Type
            Type   1  ─────  * Class

```

**Current relation scope:** Exact historical/conditional1-to-many illustrations;actual known obligations versus genuine general relation-count gaps in matrix20,no invented universal counts.

| Received label / relation | Current typed interpretation |
|---|---|
| Family 1 | Exact received historical/conditional multiplicity notation. It neither establishes current documentary-role ownership nor a universal numerical bound,mandatory Class,tree or complete population. Actual applicable counts follow matrix20 and responsible rules. |
| * Type | Exact received historical/conditional multiplicity notation. It neither establishes current documentary-role ownership nor a universal numerical bound,mandatory Class,tree or complete population. Actual applicable counts follow matrix20 and responsible rules. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| 1 | Exact received historical/conditional multiplicity notation. It neither establishes current documentary-role ownership nor a universal numerical bound,mandatory Class,tree or complete population. Actual applicable counts follow matrix20 and responsible rules. |
| * Class | Exact received historical/conditional multiplicity notation. It neither establishes current documentary-role ownership nor a universal numerical bound,mandatory Class,tree or complete population. Actual applicable counts follow matrix20 and responsible rules. |


This represents the conceptual model in which:

- in the received earlier hierarchy, a Family may contain multiple Types;
- in that received earlier hierarchy, a Type belongs to a Family;
- in that received earlier hierarchy, a Type may contain multiple Classes;
- in that received earlier hierarchy, a Class belongs to a Type.

The exact cardinality constraints are subject to the Classification Schema and Classification Specification.

**Current governing scope.** The exact numeric example remains historical/conditional; it is not the current cardinality of primary Type or Class. Actual responsible Schema/Constraints/Specification rules govern each real relationship claim.

| Association / question | Known current obligation | Remaining boundary / authority |
|---|---|---|
| Applicable normalized document → Family | Actual canonical component or admitted documentary-area membership; no alias-derived multiple Families | Representation and further multiplicity need actual owner rules |
| Applicable normalized document → Type | Exactly one primary Architecture/Structure/Behavior/Reference responsibility, uniform across Families | Contextual valid-use rules do not redefine responsibility or add a fifth Type |
| Applicable normalized document → Class | Optional, explicitly defined and non-conflicting when used | No complete Class population, mandatory field, universal child hierarchy or unsupported maximum |
| Relationship kind / actual endpoints | Identify actual kind/definition, source/target kinds and applicable semantic properties | General endpoint populations, minimum/maximum associations, parents/children and complete multiplicities remain unestablished unless actual owners supply them |
| Mandatory / optional actual association | Respect actual responsible requirements/permissions; an actually required association must be evidenced | Absence of a universal rule is neither permission for every possible edge nor waiver of a known requirement |
| Scheme hierarchy / inverse / symmetry / transitivity / cycles | Apply only actual defined properties and real independent mandates | No universal tree, inverse record, transitive closure or all-relations DAG is established |
| Actual assignment / represented connection | Identify intended document/entity/edition and actual applicable representation/Profile/interface | Semantic role/kind lists allocate no universal physical field schema or one-to-one record |

Known Model14/Schema34 obligations remain; genuine general-rule gaps do not authorize arbitrary counts or blanket deferral. Constraints22/28–30 and Specification R013/§8 retain actual independent authority.

---

# 21. Relationship Optionality

A relationship may be:

- mandatory;
- optional.

For example, if every Type must belong to a Family:

**Received unnamed visual in §21 (span 28 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type  ─────  belongs to  ─────►  Family
                         mandatory

```

**Current relation scope:** Conditional historical mandatory-Type→Family and generic optional association examples;real applicable obligations/permissions need authority,no known duty waived or unrestricted edges.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| mandatory | Actual requirement/permission property under responsible scope,rules and evidence. Received Type→Family is old-hierarchy/conditional;optional is not unrestricted and general gaps waive no known mandatory obligation. |


If an optional relationship is permitted:

**Received unnamed visual in §21 (span 29 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Element  ─────  relationship  ─────►  Element
                              optional

```

**Current relation scope:** Conditional historical mandatory-Type→Family and generic optional association examples;real applicable obligations/permissions need authority,no known duty waived or unrestricted edges.

| Received label / relation | Current typed interpretation |
|---|---|
| Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| optional | Actual requirement/permission property under responsible scope,rules and evidence. Received Type→Family is old-hierarchy/conditional;optional is not unrestricted and general gaps waive no known mandatory obligation. |


Optionality shall be explicitly defined rather than inferred.

**Current governing scope.** The mandatory Type→Family span is received conditional/old-hierarchy evidence, not current Family-owned Type. Optionality must be explicit under actual applicable rules; optional does not mean unrestricted or that every possible edge is admitted. Conversely a known mandatory association cannot be skipped because general populations remain incomplete. The two words are properties, not observed operations or entity states.

---

# 22. Relationship Constraints

Relationships shall conform to applicable Classification Constraints.

Constraints may define:

- permitted source elements;
- permitted target elements;
- cardinality;
- direction;
- relationship type;
- lifecycle requirements.

Relationship validation shall verify conformance with these constraints.

**Current governing scope.** Identify actual source/target kinds and identities, relationship-kind definition/source edition, scope and applicable direction/cardinality/lifecycle/constraint authority. Constraint conflicts, scope and precedence remain actual Constraints53–56/Specification responsibilities; an implementation must not invent precedence or waive known rules. Checking itself does not change constraints or authorize correction.

---

# 23. Relationship Validity

The eight received validity subjects below are necessary within their actual applicability and responsible rules. Source presence alone does not establish complete validity or implementation conformance:

1. the source exists;
2. the target exists;
3. the relationship type is defined;
4. the source is permitted by the relationship;
5. the target is permitted by the relationship;
6. cardinality constraints are satisfied;
7. lifecycle constraints are satisfied;
8. no applicable Classification constraint is violated.

**Current governing scope.** The actual claim, applicable responsible rule/edition, authority, observed evidence and coverage determine each criterion. Existing endpoints alone are not full semantic, structural, lifecycle or permission success.

| Original validity subject | Actual bounded assessment | Evidence / limit |
|---|---|---|
| Source exists | Actual source identity/kind/definition/context is established under its governing contract | Missing catalog/live lookup is not automatically a proven undefined endpoint; a real supported undefined source remains a violation |
| Target exists | Actual intended target identity/kind/definition/edition/context is established | Logical/exact-edition reference and live retrieval differ; endpoint presence alone does not validate the association |
| Relationship type defined | Actual relationship kind and governing meaning/source edition are defined and applicable | Primary document Type, readable label, inverse/synonym and actual relation assertion differ; no full vocabulary from examples |
| Source permitted | Actual source kind/context satisfies the responsible relationship restrictions | Do not infer permission from existence or fabricate a required field/endpoint class |
| Target permitted | Actual target kind/context satisfies applicable restrictions | Historical interpretation and current ordinary use need distinct evidence |
| Cardinality satisfied | Actual applicable counts and known obligations are evaluated | Matrix20 retains genuine general-rule gaps without arbitrary maxima or waived known duties |
| Lifecycle satisfied | Actual relationship-kind/association/assertion/endpoint state/use subject, authority and rules are evaluated | Bounded Lifecycle19/20/48 and Governance19/43/51 apply; no automatic event, complete guards or default severity |
| No applicable constraint violation | Evaluate actual mandatory rules and record real observations and performed/unperformed coverage | Missing authority/checks withholds broader success, not a fabricated violation or permission; known violations stay real |

Actual Validation16/39/67 retains Valid, Valid with Warnings and Invalid under responsible rules. Success needs adequately evidenced coverage for the declared breadth; a successful subset is not complete implementation/Core or architectural acceptance. These are semantic criteria, not newly mandatory physical fields.

---

# 24. Relationship Integrity

Classification Relationship integrity requires that relationships do not reference undefined Classification Elements.

Therefore:

**Received unnamed visual in §24 (span 30 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Valid Relationship
            │
            ├── Valid Source
            ├── Valid Type
            └── Valid Target

```

**Current relation scope:** Actual validity subjects source/kind/target,not documentary Type or successful evaluation from labels;matrix23 applies evidence/coverage and historical/current context.

| Received label / relation | Current typed interpretation |
|---|---|
| Valid Relationship | Actual supported validity subject under responsible rule/source/definition/endpoint/context and adequate observations/coverage. Valid Type means relationship-kind validity,not primary document Type. Source presence or unknown lookup is not all criteria checked;no result or permission from a label. |
| Valid Source | Actual supported validity subject under responsible rule/source/definition/endpoint/context and adequate observations/coverage. Valid Type means relationship-kind validity,not primary document Type. Source presence or unknown lookup is not all criteria checked;no result or permission from a label. |
| Valid Type | Actual supported validity subject under responsible rule/source/definition/endpoint/context and adequate observations/coverage. Valid Type means relationship-kind validity,not primary document Type. Source presence or unknown lookup is not all criteria checked;no result or permission from a label. |
| Valid Target | Actual supported validity subject under responsible rule/source/definition/endpoint/context and adequate observations/coverage. Valid Type means relationship-kind validity,not primary document Type. Source presence or unknown lookup is not all criteria checked;no result or permission from a label. |


A relationship containing an invalid reference is not part of the valid Classification model.

**Current governing scope.** Source, relationship kind and target each need actual qualified meaning/identity/context and applicable validity observations. Valid Type in the received view is relationship-kind validity, not primary document Type. Keep no-undefined-reference requirements; source presence, approved endpoints, a well-formed key or a drawing alone do not establish a valid current connection or live target. Actual record/rule/definition editions and historical scope remain relevant.

---

# 25. Orphan Relationships

For an actual current relationship claim, an orphan concern is a source or target that is actually undefined or invalid under the applicable responsible rule; actual Constraints25 also identifies invalid relationship type. Historical associations and unresolved lookup need their own context and evidence.

For example:

**Received unnamed visual in §25 (span 31 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Unknown Element
            │
            └── relationship  ─────►  Class

```

**Current relation scope:** Selected unresolved/undefined endpoint example with actual known violation versus lookup/authority/retrieval gap distinction;no fabricated orphan/Invalid or waived real integrity.

| Received label / relation | Current typed interpretation |
|---|---|
| Unknown Element | Selected unresolved/undefined endpoint example must be distinguished by evidence:known actual undefined/invalid endpoint/type versus missing lookup/authority/live retrieval. Real integrity mandates remain;unknown observation is not automatically fabricated orphan/Invalid. |
| relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


An actually established undefined/invalid endpoint or type violates the applicable integrity requirement; an unsupported lookup inference is not a proven violation.

Orphan relationships shall be detected by Classification Validation.

**Current governing scope.** Distinguish supported actual undefined/invalid source, target or kind from unresolved lookup, absent authority, unperformed checks or a live endpoint outage. A retired/deprecated but historically identified endpoint is not automatically an orphan for historical interpretation. Real current-use/type/reference violations remain enforceable; historical orphan evidence can be retained under actual Constraints25 without treating it as a valid active relation. Checking reports real rule-dependent observations and coverage, not an invented result from absence alone.

---

# 26. Invalid Relationships

Examples of invalid relationships include:

**Received unnamed visual in §26 (span 32 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Class  ─────  contains──► Family

```

**Current relation scope:** Conditional prohibited-edge examples under actual responsible kind/endpoints/rules;old Family hierarchy premise is historical,not universal current role authority.

| Received label / relation | Current typed interpretation |
|---|---|
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


when `contains` is defined only for the Family-to-Type hierarchy.

Another example is:

**Received unnamed visual in §26 (span 33 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type  ─────  belongs to  ─────►  Type

```

**Current relation scope:** Conditional prohibited-edge examples under actual responsible kind/endpoints/rules;old Family hierarchy premise is historical,not universal current role authority.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongs to | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


when the relationship is restricted to Type-to-Family associations.

Relationship validity is determined by the Classification Schema and Constraints.

**Current governing scope.** Both exact examples are conditional on actual responsible permitted endpoint/kind rules. Their earlier Family-owned hierarchy premise is not the current normalized-role contract. Do not turn the example into an unconditional universal prohibition or admit arbitrary relationships: actual kind/definition/applicability/source-target, constraints and supporting observations decide the real claim.

---

# 27. Relationship Type

A Relationship Type defines the semantic nature of a Classification Relationship.

Conceptually:

**Received unnamed visual in §27 (span 34 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Relationship Type
                    │
                    ▼

          Relationship Semantics

```

**Current relation scope:** Relationship kind→meaning concern,not primary documentary Type,completed catalog,actual association or canonical/physical allocation.

| Received label / relation | Current typed interpretation |
|---|---|
| Relationship Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |
| Relationship Semantics | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |


A Relationship Type shall have:

- a defined name;
- a defined meaning;
- defined source constraints;
- defined target constraints;
- defined direction;
- defined lifecycle rules where applicable.

**Current governing scope.** Relationship Type means semantic relationship kind/definition, distinct from document Type, a value/name and an actual association or physical connection record. The six required semantic subjects identify responsible meaning/applicability, not universal Metadata fields. Inverse, symmetry, transitivity and exact lifecycle details apply only when actual owner definitions establish them. Naming/presence is not approval or performed creation.

---

# 28. Relationship Vocabulary

The Classification component shall maintain a controlled vocabulary of canonical relationship types.

The vocabulary may include:

- `contains`;
- `belongsTo`;
- `supersedes`;
- `replaces`;
- other formally approved relationships.

Only relationship types approved through Classification Governance become canonical.

**Current governing scope.** This is a controlled-vocabulary requirement with a may-include list, not proof a complete accepted relationship-kind population or alias register already exists. Actual Dictionary14/36 supplies general relationship terms and earlier roles; its broader terms/term statuses and incomplete specific kind evidence remain. Preserve exact contains/belongsTo/belongs to/supersedes/replaces/replaced by spelling as received evidence with actual current meaning/status; no synonym/inverse/alias is allocated or silently merged. Approval is necessary within actual scope and conditions, not proof of canonical adoption from this list.

---

# 29. Contains Relationship

`contains` expresses hierarchical containment.

Examples:

**Received unnamed visual in §29 (span 35 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family  ─────  contains  ─────►  Type
            Type    ─────  contains  ─────►  Class

```

**Current relation scope:** Historical/conditional hierarchical contains and inverse examples under actual defined scheme semantics;no universal current role containment or widened general association.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


The relationship is directional.

Its inverse is conceptually:

**Received unnamed visual in §29 (span 36 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type   ─────  belongsTo  ─────►  Family
            Class  ─────  belongsTo  ─────►  Type

```

**Current relation scope:** Historical/conditional hierarchical contains and inverse examples under actual defined scheme semantics;no universal current role containment or widened general association.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongsTo | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| belongsTo | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |

**Current governing scope.** The hierarchical-containment meaning is retained for an actual explicitly defined hierarchical kind/scheme; it is not silently widened to general association or used as current Family-owned Type. Every exact contains/belongsTo role example is historical/conditional. Actual inverse semantics/endpoint constraints need their own authority and do not generate records automatically (§§18/46/60).

---

# 30. Belongs-To Relationship

`belongsTo` expresses membership in an actually defined Classification hierarchy; it is not the governing relation of uniform documentary Type to Family or optional Class to Type.

Examples:

**Received unnamed visual in §30 (span 37 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type   ─────  belongsTo  ─────►  Family
            Class  ─────  belongsTo  ─────►  Type

```

**Current relation scope:** Historical/conditional inverse membership examples,not current Family-owned Type or universal Type-child Class;no merged aliases or generated inverse record.

| Received label / relation | Current typed interpretation |
|---|---|
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongsTo | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| belongsTo | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


The relationship is the inverse semantic perspective of `contains`.

**Current governing scope.** The received inverse perspective is conditional on actual kind/definition and matching context. The exact Type→Family/Class→Type labels remain historical examples, not a current documentary-role rule. Canonical kind, label with spaces, inverse and synonym must not be merged without actual owner definition; no required physical reverse record or fifth Type follows.

---

# 31. Supersession Relationship

A Classification Element may supersede another Classification Element.

Conceptually:

**Received unnamed visual in §31 (span 38 in original order).** Exact text below is evidence,not a second governing rule.

```text

            New Classification
                    │
                supersedes
                    │
                    ▼

            Old Classification

```

**Current relation scope:** Scoped directed supersession between actual old/new subjects/editions,not automatic equivalence,assignment migration,rekey or pinned-history retargeting.

| Received label / relation | Current typed interpretation |
|---|---|
| New Classification | Actual identified prior/new domain subject and definition/source edition/context. Supersession/replacement need actual authority,meaning/mapping/history and effects;no automatic equivalence,assignment migration,rekey or pinned-target retargeting. |
| supersedes | Received directed evolution/replacement wording;exact supersession/replacement/inverse distinction follows actual canonical owner definitions and remains unestablished where evidence is incomplete. Not automatic equivalence,migration,alias allocation,history deletion or current-use permission. |
| Old Classification | Actual identified prior/new domain subject and definition/source edition/context. Supersession/replacement need actual authority,meaning/mapping/history and effects;no automatic equivalence,assignment migration,rekey or pinned-target retargeting. |


This relationship is particularly relevant to Classification evolution.

It allows historical Classification meaning to remain traceable after a newer definition is introduced.

**Current governing scope.** Identify actual new/old relationship kind, definition or element subject and exact source/definition context. Supersession is a directed evolution relation, not automatically semantic equivalence, document-key reuse, migration or changed current assignments. Required historical meaning and earlier evidence remain; exact replacement distinction is not invented from name similarity.

---

# 32. Replacement Relationship

A replacement relationship expresses that one Classification Element is intended to replace another.

**Received unnamed visual in §32 (span 39 in original order).** Exact text below is evidence,not a second governing rule.

```text

               New Element
                    │
                 replaces
                    │
                    ▼

               Old Element

```

**Current relation scope:** Scoped intended replacement between actual subjects/editions;precise distinction from supersession remains actual owner authority,not automatic operation/equivalence.

| Received label / relation | Current typed interpretation |
|---|---|
| New Element | Actual identified prior/new domain subject and definition/source edition/context. Supersession/replacement need actual authority,meaning/mapping/history and effects;no automatic equivalence,assignment migration,rekey or pinned-target retargeting. |
| replaces | Received directed evolution/replacement wording;exact supersession/replacement/inverse distinction follows actual canonical owner definitions and remains unestablished where evidence is incomplete. Not automatic equivalence,migration,alias allocation,history deletion or current-use permission. |
| Old Element | Actual identified prior/new domain subject and definition/source edition/context. Supersession/replacement need actual authority,meaning/mapping/history and effects;no automatic equivalence,assignment migration,rekey or pinned-target retargeting. |


Replacement and supersession may be distinguished when the Classification Specification requires different semantics.

The precise distinction shall be defined by the canonical Classification vocabulary.

**Current governing scope.** The deferred precise distinction remains genuine. An intended replacement is not proof of semantic equivalence, performed reassignment, approved operation or retargeting prior references. Actual old/new subject/definition editions, authority, scope, compatibility and history need evidence; migration is separately governed (§62).

---

# 33. Deprecation Relationships

Deprecation may require relationships between:

- a deprecated Classification Element;
- its successor;
- its recommended replacement.

For example:

**Received unnamed visual in §33 (span 40 in original order).** Exact text below is evidence,not a second governing rule.

```text

             Deprecated Class
                    │
               replaced by
                    │
                    ▼

               Active Class

```

**Current relation scope:** Selected definition/category state/use and replacement concern with optional Class and required history;no actual transition,default severity or performed migration.

| Received label / relation | Current typed interpretation |
|---|---|
| Deprecated Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| replaced by | Received directed evolution/replacement wording;exact supersession/replacement/inverse distinction follows actual canonical owner definitions and remains unestablished where evidence is incomplete. Not automatic equivalence,migration,alias allocation,history deletion or current-use permission. |
| Active Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


Such relationships preserve the evolution history of Classification.

**Current governing scope.** The three original deprecation subjects and exact Class example remain selected concerns. Deprecated/Active Class here concerns actual category/definition/use context, not mandatory Class or automatic document Status/term/R aliases. A recommended replacement need not prove all historical assignments originally valid or permit current new use. Preserve actual rules and required history without default warnings, exceptions or migration.

---

# 34. Relationship Lifecycle

Relationships may have lifecycle states independently of the Classification Elements they connect.

Conceptually:

**Received unnamed visual in §34 (span 41 in original order).** Exact text below is evidence,not a second governing rule.

```text

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

**Current relation scope:** Selected bounded state labels interpreted for actual kind-definition/association/assertion/endpoint subject;matrix34 retains known duties and genuine exact-route/actor gaps,not aliases or engine.

| Received label / relation | Current typed interpretation |
|---|---|
| Defined | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |
| Active | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |
| Deprecated | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |
| Retired | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |


The lifecycle semantics are governed by Classification Lifecycle and Classification Governance.

**Current governing scope.** Use actual Lifecycle V2.0 R1 matrices19/20/48 and Governance V2.0 R1 matrices19/43/51. Exact received state labels are selected bounded concerns, not an approved exhaustive machine or actual transition.

| State / decision / action subject | Known requirement | Genuine detail / evidence boundary |
|---|---|---|
| Relationship kind / definition | Identify actual semantic definition identity, source edition and applicable state/use meaning | Not primary document Type, Dictionary term status or a universal physical state field |
| Actual association / assertion | Identify intended source/target kind/identity/edition/context and actual association evidence | Definition presence/state alone proves no association, validity or permission; complete event/record fields are not supplied |
| Endpoint state / historical use | Apply actual source/target definition and current/historical use rules independently | Deprecated/retired historical meaning, proven original validity, present permission and live retrieval differ |
| Defined / Active / Deprecated / Retired | Bounded Lifecycle meanings and actual known governed-transition/ordinary-use/history obligations remain | No complete actual guards/routes/actors/effective-time/conflict/bulk/record authority is inferred; missing detail neither waives mandates nor grants permission |
| Validation / domain decision / operation | Nonmutating evidence, actual responsible decision and separately authorized execution/effect evidence are distinct | Approved is a decision, not an added definition state; phase authorization is not actual canonical adoption or permission |
| Conditions / canonicality / publication / Baseline | Actual subject/edition/scope/authority, required conditions and fulfillment, effective adoption and independent event evidence | Conditional approval does not fulfill itself; CLS01137 retains real extension conditions before canonicality; publication and exact Baseline selection are separate |

Document Status, local supporting R assertion, definition/association state, Dictionary term/extension status, validation result/finding and Milestone state are not automatic aliases.

---

# 35. Relationship Activation

A proposed relationship becomes Active only after the applicable governance and validation requirements have been satisfied.

Conceptually:

**Received unnamed visual in §35 (span 42 in original order).** Exact text below is evidence,not a second governing rule.

```text

          Proposed Relationship
                    │
                    ▼

                Validation
                    │
                    ▼

                Governance
                    │
                    ▼

           Active Relationship

```

**Current relation scope:** Necessary validation/governance/activation concerns,not sufficient approval,fulfilled conditions,complete guards or performed activation;actual evidence/authority/execution remain separate.

| Received label / relation | Current typed interpretation |
|---|---|
| Proposed Relationship | Actual identified proposal/need/definition subject and governing source edition/scope/authority,not a universally registered lifecycle state,created kind,canonical adoption or performed operation from this view. |
| Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| Active Relationship | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |

**Current governing scope.** The only-after statement is necessary conditions, not proof that the selected arrows establish sufficiency or execute activation. Actual proposal/relationship subject/definition/source edition, authority, applicable checks/coverage, decision conditions/fulfillment and authorized operation/effect evidence govern any real activation. Current Governance43 retains five scoped outcomes; Deferred/Rejected or missing decision evidence is not approval, and Approved with Conditions does not fulfill unknown conditions.

---

# 36. Relationship Deprecation

A relationship may be deprecated when:

- its semantic meaning is obsolete;
- its relationship type has been replaced;
- the associated Classification structure has evolved;
- the relationship should no longer be used for new Classification definitions.

Deprecation shall preserve historical information wherever required for interpretation and traceability; additional preservation should be maintained where reasonably possible.

**Current governing scope.** Deprecation criteria are possible grounds, not automatic events or a fixed severity. Identify actual kind/definition/association subject and current/historical use scope. Real new-use restrictions and required history remain, without universal invalidation of original assignments, invented grandfathering, silent migration or aliasing document/term states.

---

# 37. Relationship Retirement

A retired relationship is no longer part of the active Classification architecture.

Retirement does not necessarily imply deletion.

Historical relationships may remain necessary to interpret previous Classification states.

**Current governing scope.** Actual retirement decision/state/action and scope require their own evidence; a retired kind/association is not automatically deletion of source/target definitions or invalidation of historical interpretation. Preserve actual prior relationship/endpoint/definition/assignment/decision/source editions and relevant pinned context where required. Current-use validity, original validity and live retrieval remain separately assessed.

---

# 38. Relationship Evolution

Classification Relationships shall evolve through controlled governance.

The general process is:

**Received unnamed visual in §38 (span 43 in original order).** Exact text below is evidence,not a second governing rule.

```text

          Relationship Proposal
                    │
                    ▼

           Architectural Review
                    │
                    ▼

          Consistency Assessment
                    │
                    ▼

             Impact Analysis
                    │
                    ▼

                Validation
                    │
                    ▼

           Governance Decision
                    │
                    ▼

          Canonical Relationship

```

**Current relation scope:** Conditional conceptual evolution under current GovernanceV2R1,not runtime/approval sufficiency or completed canonical adoption,publication or Baseline.

| Received label / relation | Current typed interpretation |
|---|---|
| Relationship Proposal | Actual identified proposal/need/definition subject and governing source edition/scope/authority,not a universally registered lifecycle state,created kind,canonical adoption or performed operation from this view. |
| Architectural Review | Actual evaluation concern needs responsible criteria/source editions,authority,observations and coverage,prior/new meaning and affected interfaces. Not a completed review/runtime,decision,condition fulfillment or direct mutation. |
| Consistency Assessment | Actual evaluation concern needs responsible criteria/source editions,authority,observations and coverage,prior/new meaning and affected interfaces. Not a completed review/runtime,decision,condition fulfillment or direct mutation. |
| Impact Analysis | Actual evaluation concern needs responsible criteria/source editions,authority,observations and coverage,prior/new meaning and affected interfaces. Not a completed review/runtime,decision,condition fulfillment or direct mutation. |
| Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Governance Decision | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| Canonical Relationship | Actual exact authorized/effectively adopted domain relationship kind/definition/association subject under applicable conditions and independent owner requirements. Necessary approval alone is not proof of fulfillment,activation,publication or Baseline selection;changed Draft inherits none. |


This follows the governance model established by DF-CLS-008.

**Current governing scope.** This follows current actual Governance V2.0 R1, not its original snapshot. The exact view is a conditional conceptual progression, not serial runtime or approval sufficiency. Actual scope/authority, performed checks/evidence/coverage, conditions/fulfillment, effective adoption and authorized execution remain distinct; no canonical relationship, transition, publication or Baseline is created by the arrows.

---

# 39. Relationship Governance

Classification Governance controls:

- introduction of relationship types;
- modification of relationship semantics;
- relationship constraints;
- relationship cardinality;
- relationship lifecycle transitions;
- relationship deprecation;
- relationship retirement.

Classification Relationships defines the semantics.

Classification Governance controls their evolution.

**Current governing scope.** Classification owns domain relationship semantic/change conditions; common Relationships owns typed connection-record mechanisms under ARC0057.2/Specification28. Metadata owns actual representation/Profile rules, common Workflow/Policies/Reviews/Baselines their documentary contracts, and an actual authorized executor performs operations. Actual actor/delegation/guard/record gaps remain explicit rather than invented. The seven original governance subjects retain these actual scopes.

---

# 40. Relationship Validation

Classification Validation evaluates whether identified relationships conform to the actual applicable model and responsible rules recorded for the claim.

Validation may verify:

- source validity;
- target validity;
- relationship type;
- direction;
- cardinality;
- constraints;
- lifecycle state;
- integrity.

Validation does not authorize new relationship semantics.

**Current governing scope.** Use actual Validation V2R1 matrices16/39/67. Identify intended claim/population/subject and exact source/definition/rule/Schema/Profile/Lifecycle/Constraints context, responsible authority/executor, actual observations and performed/unperformed coverage. Real blocking/nonblocking observations retain rule-dependent result meaning; missing/conflicting/unperformed mandatory evidence withholds broader success without fabricated Invalid, fourth universal result or Governance outcome. Evaluation is nonmutating; result recording, correction, assignment, transition, migration, permission, approval, publication and Baseline selection are separate. A local documentary PASS is not complete domain implementation or architectural acceptance.

---

# 41. Governance and Validation Separation

The distinction is:

**Received unnamed visual in §41 (span 44 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Classification Relationships
            │
            └── defines relationships

            Classification Validation
            │
            └── validates relationships

            Classification Governance
            │
            └── governs relationship evolution

```

**Current relation scope:** Domain semantic definition,nonmutating evidence and actual responsible evolution decision are separate;no owner transfer,engine or phase-command approval.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Relationships | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| defines relationships | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| Classification Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| validates relationships | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Classification Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| governs relationship evolution | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |


This preserves the separation of responsibilities established across the Classification component.

**Current governing scope.** The exact separation view describes domain semantics, actual nonmutating evidence and responsible change decisions. It is not implementation evidence, a required component/runtime pipeline or a transfer of common connection-record, Metadata or actual executor authority. Real independent source requirements remain; source existence or a task command proves no canonical approval.

---

# 42. Relationship Constraints

Relationship constraints may restrict:

**Received unnamed visual in §42 (span 45 in original order).** Exact text below is evidence,not a second governing rule.

```text

                    Source
                    │
                    ├── permitted element types
                    │
                    ▼

            Relationship Type
            │
            ├── permitted target types
            │
            ▼

          Target

```

**Current relation scope:** Actual permitted source/target kinds and relationship-kind restrictions,not primary document Type,physical fields or proof of enforced invalidity prevention.

| Received label / relation | Current typed interpretation |
|---|---|
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| permitted element types | Actual allowed source/target endpoint kinds and responsible applicability restrictions,not necessarily documentary Type values or a fabricated canonical field/endpoint enumeration. Actual rule observations and coverage required. |
| Relationship Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |
| permitted target types | Actual allowed source/target endpoint kinds and responsible applicability restrictions,not necessarily documentary Type values or a fabricated canonical field/endpoint enumeration. Actual rule observations and coverage required. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |


Constraints therefore prevent semantically invalid relationships.

**Current governing scope.** Source/target types here are actual allowed endpoint kinds under the relationship definition, not necessarily primary document Type. Constraint provision differs from actual enforcement: actual rules/applicability/authority/evidence and coverage must support the observed claim. No arbitrary endpoint enumeration, precedence, physical fields or automatic prevention is proven by this conceptual span.

---

# 43. Acyclicity

Hierarchical Classification relationships should preserve an acyclic structure.

For example:

**Received unnamed visual in §43 (span 46 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                    ▼

                   Type
                    │
                    ▼

                  Class

```

**Current relation scope:** Historical/conditional role-cycle examples under actual hierarchical/acyclic semantics and applicable Schema/Constraints prohibition;no global all-relations DAG or hidden real provider cycle.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


must not result in:

**Received unnamed visual in §43 (span 47 in original order).** Exact text below is evidence,not a second governing rule.

```text

                  Family
                    │
                    ▼

                   Type
                    │
                    ▼

                  Class
                  │
                  └────────► Family

```

**Current relation scope:** Historical/conditional role-cycle examples under actual hierarchical/acyclic semantics and applicable Schema/Constraints prohibition;no global all-relations DAG or hidden real provider cycle.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


when the relationship type is hierarchical and acyclic.

Cycles shall be treated as invalid where prohibited by the Classification Schema.

**Current governing scope.** Keep the received explicit when-hierarchical/acyclic and where-Schema-prohibited qualifications. The two exact Family/Type/Class spans are historical/conditional examples, not a universal role hierarchy or proof every relationship graph must be acyclic. Actual Constraints17 and Specification R007/§8 retain genuine applicable hierarchy prohibitions. Semantic hierarchy, inverse navigation/representation and required consumer→provider dependencies are distinct graphs; naming a projection erases no indispensable edge or real required cycle.

---

# 44. Hierarchical Consistency

A Classification hierarchy shall preserve the defined parent-child semantics.

For example:

**Received unnamed visual in §44 (span 48 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family
            │
            └── Type
                │
                └── Class

```

**Current relation scope:** Historical selected role chain and actual defined-hierarchy ancestor prohibition;no universal current role ancestry or arbitrary graph constraint.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


shall not contain a relationship that causes a Class to become a parent of its own ancestor.

**Current governing scope.** The actual parent-of-own-ancestor prohibition is preserved for an actually defined hierarchical kind/scheme. The exact earlier role chain is historical, not a current Family/Type/Class mandate. Establish actual relation composition and permitted endpoints before inferring ancestry or invalidity; no universal tree or all-relations DAG follows.

---

# 45. Relationship Consistency

Relationships must remain semantically consistent.

For example, if:

**Received unnamed visual in §45 (span 49 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family A   ─────  contains  ─────►  Type B

```

**Current relation scope:** Historical/conditional same-association inverse perspectives with placeholder endpoints/context;no contradictory meaning,Family-owned Type or compulsory duplicate stored records.

| Received label / relation | Current typed interpretation |
|---|---|
| Family A | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type B | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |


then the inverse semantic relationship must be consistent:

**Received unnamed visual in §45 (span 50 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Type B   ─────  belongsTo  ─────►  Family A

```

**Current relation scope:** Historical/conditional same-association inverse perspectives with placeholder endpoints/context;no contradictory meaning,Family-owned Type or compulsory duplicate stored records.

| Received label / relation | Current typed interpretation |
|---|---|
| Type B | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| belongsTo | Received inverse/membership wording in an actually defined hierarchical association and matching scope;exact spellings are evidence,not allocated synonyms/aliases or a current Family-owned Type rule. No compulsory second physical record or reverse provider edge. |
| Family A | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |


The two representations must not establish contradictory Classification contexts.

**Current governing scope.** Both exact views are historical/conditional inverse examples under actual same association/definition/context. A defined inverse must not contradict its original semantic perspective; it need not create a second authoritative definition or stored record. Family A/Type B are placeholders, not actual allocated categories or a Family-owned Type rule. Current record/projection freshness and endpoint/edition scope still matter.

---

# 46. Relationship Uniqueness

The Classification architecture should avoid duplicate canonical relationships.

For a given:

**Received unnamed visual in §46 (span 51 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Source  +  Relationship Type  +  Target

```

**Current relation scope:** Possible conceptual endpoint+kind tuple and normal uniqueness with actual Schema-supported exceptions;matrix46 separates semantic/record/projection/context identity,no universal key or dedup operation.

| Received label / relation | Current typed interpretation |
|---|---|
| Source | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |
| + | Received conceptual endpoint+kind composition,not a proved universal persistent identity key,automatic tuple allocation,serialized fields or deduplication/operation instruction. |
| Relationship Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |
| + | Received conceptual endpoint+kind composition,not a proved universal persistent identity key,automatic tuple allocation,serialized fields or deduplication/operation instruction. |
| Target | Actual typed endpoint with intended identity,definition/source edition and claim-dependent logical/exact-edition/context under its own responsible contract. Not automatically a DF document,physical field,valid association or available live endpoint. |


there should normally be one canonical relationship.

Duplicate relationships should not be introduced unless explicitly supported by the Classification Schema.

**Current governing scope.** The original normally-one and explicit Schema-supported duplicate qualifications remain. Actual canonical semantic identity is distinct from stored/projected copies and historical/contextual assertions.

| Identity / comparison concern | Actual interpretation | Boundary |
|---|---|---|
| Relationship kind / definition | Responsible semantic identity/name/meaning and exact governing definition/source context | Not primary document Type, display label, actual association or automatically allocated DF document |
| Source / Target | Actual typed endpoint identity and logical/exact-edition/definition/context needed by the claim | Not every endpoint is a document; canonical endpoints alone do not prove valid connection or live retrieval |
| Actual association / assertion | Identify actual relation under its allowed kind/endpoints/context and responsible uniqueness rules | Source+kind+target is possible conceptual composition, not proved universal key for all histories/records |
| Normal canonical uniqueness | Preserve actual one-authoritative-meaning and no-duplicate requirements plus explicit permitted Schema exceptions | Do not invent arbitrary duplicates, missing multiplicity rules or automatic deduplication/record deletion |
| Physical connection / inverse / projection | Common typed record and actual representation/source-edition/freshness provenance | Legitimate copies or derived inverse/navigation do not alone create competing semantic identity or mandatory duplicate records |
| Document K / exact edition / local R | Qualified stable document key and actual edition differ from complete supporting descriptor/assertions and intended reference | K alone is not full R; Canonical Reference is not mandatory incoming edge or guaranteed URL; no generic entity allocation/rekey |
| Change / historical continuity | Preserve actual old/new definition/association/record/endpoint mappings, authority, compatibility and pinned context | Same tuple/name/path proves no unchanged meaning; external decision alone revises no consumer or older approval |

Actual Constraints23/26/27 and responsible Schema/Specification scope govern real duplicates and stability; this matrix allocates no universal physical identity fields.

---

# 47. Relationship Identity Stability

Once a relationship becomes canonical, its identity should remain stable whenever possible.

Changing relationship identity unnecessarily can cause:

- broken references;
- loss of traceability;
- inconsistent historical records;
- migration complexity.

Evolution should therefore prefer controlled modification over unnecessary replacement.

**Current governing scope.** Keep stability whenever possible and preference rather than an absolute prohibition on replacement. Actual semantic/endpoint/identity/record change needs honest prior/new mapping, authority, need, alternatives/rationale, compatibility, consumer/interface effects and required history. Renaming/moving/serialization alone need not change semantic identity or document K, but actual references/Profile/index/access/retrieval/usage/history effects still require checks. Do not mutate earlier meaning or retarget pinned approvals silently.

---

# 48. Relationship Compatibility

Relationship changes shall consider compatibility with:

- existing Classification Elements;
- existing documents;
- Classification Validation;
- Classification Constraints;
- Classification Dictionary;
- Classification Specification;
- Registry;
- Knowledge Graph;
- automation.

**Current governing scope.** The nine original consumer subjects require concrete source-specific impact. The36-path batch in§71 was identified before normative mutation with actual coordinates/hashes/clauses/prior-new actions and authority/interfaces/history. Local/cross-component labels waive no real structural/role/domain/provider requirement. Unchanged IDs/path or labels prove no compatibility; any further substantive propagation needs its own authorized successor and later checks.

---

# 49. Cross-Component Relationships

Classification Relationships may have implications outside the Classification component.

For example:

**Received unnamed visual in §49 (span 52 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Classification
            │
            ├── Registry
            ├── Discovery
            ├── Knowledge Graph
            ├── Metadata
            └── Automation

```

**Current relation scope:** Selected actual domain consumers/structural-area/capability concerns,not complete component/provider graph,runtime or completed reciprocal interface/cycle resolution.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification | Actual Classification domain/component context with separate role/category/value/assignment/relationship/owner duties. A selected architecture view proves no complete population,required-provider direction,runtime or global acceptance. |
| Registry | Actual catalog/lookup/projection responsibility with authoritative source/edition,current-historical/snapshot and freshness/refresh context;not domain meaning owner,automatic registration,approval or mandatory intermediary for every component. |
| Discovery | Actual structural area containing discovery capabilities,not automatically an extra peer component or a new indispensable service/runtime from this selected view. |
| Knowledge Graph | Actual semantic-network projection and node/edge representation under authoritative domain/general typed-connection sources,editions and freshness. Not every node is a DF document;projection proves no valid current connection,live target,implemented engine,complete graph or erased provider cycle. |
| Metadata | Actual Concepts/Elements/Values/Schema/Profile/Instance and effective representation contracts remain broader than Element-only shorthand. No ownership transfer or field allocation;actual provider/no-cycle/Profile obligations remain independently applicable. |
| Automation | Actual common capability definitions consuming responsible contracts;authorized DMS/CMS/tool/manual implementation/execution supplies own inputs,editions/checks/observations/coverage/effects. No installed engine,performed generation,permission,approval or complete implementation from the view. |


These components may consume Classification relationships.

However, their internal relationship models remain outside the scope of this document.

**Current governing scope.** The exact view selects consumers/concerns, not a complete provider graph or runtime. Discovery is a structural area, not automatically an additional peer component; Metadata has broader actual Concepts/Element/Value/Schema/Profile/Instance contracts. Common Relationships typed records and actual Classification→Metadata/Document Identity requirements, conditional Templates and real reciprocal Metadata↔Identity claims remain visible. Actual core/descriptor/source-edition/interface/cycle reconciliation is not completed by projection labels.

---

# 50. Relationship and Metadata

Classification and Metadata are related but distinct concepts.

Classification Relationships describe relationships between Classification Elements.

Actual Metadata Relationships covers Metadata Concepts, Elements, Values, Schemas, Profiles and Instances; its own type categories, representation and provider mandates retain their scope.

The two models may interact, but one does not replace the other.

**Current governing scope.** Actual Metadata Relationships3/13/16 retains broader subjects, type categories, no ownership transfer, no architectural dependency cycles and real Profile/Instance provider rules. Classification owns domain semantic conditions; Metadata/Schema/effective Profile owns representation, and common Relationships owns typed connections/records. No domain role/kind/name or Source/Type/Target label automatically allocates a Metadata field or merges owner authority.

---

# 51. Relationship and Document Identity

Classification Relationships do not define Document Identity relationships.

A document may be classified using a Classification Element:

**Received unnamed visual in §51 (span 53 in original order).** Exact text below is evidence,not a second governing rule.

```text

                 Document
                    │
              classified as
                    │
                    ▼

          Classification Element

```

**Current relation scope:** Actual document-classification assignment concern versus internal domain relationships;qualified K/exact edition/local R/entity/record differ,no assignment or allocation from view.

| Received label / relation | Current typed interpretation |
|---|---|
| Document | Actual document-to-category/value assignment concern,distinct from internal domain relation. Use intended logical document K or explicit exact edition/context where applicable;local complete supporting R and domain entity identities differ. No automatic DF allocation,assignment or rekey. |
| classified as | Actual document-to-category/value assignment concern,distinct from internal domain relation. Use intended logical document K or explicit exact edition/context where applicable;local complete supporting R and domain entity identities differ. No automatic DF allocation,assignment or rekey. |
| Classification Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |


The relationship between a Document and a Classification Element belongs to the document classification mechanism.

The relationships defined in this document primarily concern Classification Elements themselves.

**Current governing scope.** Document→classified-as concerns actual assignment mechanism, not all internal domain relations. Identify intended logical document K or exact edition/bytes/context when a document is really an endpoint; category/definition/relationship/record identities follow their own kinds. DID0147/12 locally distinguishes stable K from complete supporting R with Document Identity, Identifier, Identity Domain, Identity State and Canonical Reference. R assertion is not automatic document Status or definition state; qualified reference/edition target differs from connection and live endpoint. Remaining field/interface/prior-restriction reconciliation is not a fully accepted merged schema. No entity is allocated/rekeyed by this view.

---

# 52. Relationship and Registry

The Registry may expose Classification Relationships for discovery.

However:

**Received unnamed visual in §52 (span 54 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Classification Relationships
            │
            └── defines semantic relationship

            Registry
            │
            └── exposes registered relationship information

```

**Current relation scope:** Domain semantics versus Registry exposed source-edition/freshness projection,not semantic takeover,automatic registration or canonical adoption.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Relationships | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| defines semantic relationship | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| Registry | Actual catalog/lookup/projection responsibility with authoritative source/edition,current-historical/snapshot and freshness/refresh context;not domain meaning owner,automatic registration,approval or mandatory intermediary for every component. |
| exposes registered relationship information | Actual catalog/lookup/projection responsibility with authoritative source/edition,current-historical/snapshot and freshness/refresh context;not domain meaning owner,automatic registration,approval or mandatory intermediary for every component. |


The Registry does not redefine Classification semantics.

**Current governing scope.** Registry catalog authority differs from domain meaning and general typed connection records. Actual authoritative source/edition, current/historical/snapshot scope and freshness/refresh must support a projection claim; stale entries do not silently retarget pinned evidence or make a changed definition canonical. A projection label removes no actual indispensable provider or real cycle and proves no automatic registration.

---

# 53. Relationship and Knowledge Graph

Classification Relationships may become edges in a Knowledge Graph.

Conceptually:

**Received unnamed visual in §53 (span 55 in original order).** Exact text below is evidence,not a second governing rule.

```text

          Classification Element
                    │
               relationship
                    │
                    ▼

          Classification Element

```

**Current relation scope:** Domain relation/definition/assertion versus common typed record and Node/Edge projection,with source editions/context/freshness;not implemented graph,all-document endpoints or complete network.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Classification Element | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |


may be represented as:

**Received unnamed visual in §53 (span 56 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Node  ─────  Edge  ─────►  Node

```

**Current relation scope:** Domain relation/definition/assertion versus common typed record and Node/Edge projection,with source editions/context/freshness;not implemented graph,all-document endpoints or complete network.

| Received label / relation | Current typed interpretation |
|---|---|
| Node | Actual semantic-network projection and node/edge representation under authoritative domain/general typed-connection sources,editions and freshness. Not every node is a DF document;projection proves no valid current connection,live target,implemented engine,complete graph or erased provider cycle. |
| Edge | Actual semantic-network projection and node/edge representation under authoritative domain/general typed-connection sources,editions and freshness. Not every node is a DF document;projection proves no valid current connection,live target,implemented engine,complete graph or erased provider cycle. |
| Node | Actual semantic-network projection and node/edge representation under authoritative domain/general typed-connection sources,editions and freshness. Not every node is a DF document;projection proves no valid current connection,live target,implemented engine,complete graph or erased provider cycle. |


The Knowledge Graph is an external representation and discovery mechanism.

The Classification Relationship remains the authoritative semantic definition.

**Current governing scope.** Domain relationship-kind definition remains responsible for semantic meaning; the actual association/assertion, common typed connection record and graph Node/Edge projection are distinct. Actual governing source/definition/endpoint/record editions, identity/context and freshness matter. Nodes/edges need not all be normalized documents; a valid-looking projection neither owns new semantics nor proves actual connection validity, current availability, complete network or an implemented graph engine.

---

# 54. Relationship and Automation

Automation may consume Classification Relationships to:

- validate Classification;
- generate registries;
- construct navigation;
- generate documentation;
- verify consistency.

Automation shall not introduce canonical relationships without the applicable governance process.

**Current governing scope.** Common Automation under ARC0058 defines these capability contracts consuming actual domain/representation rules. An actual authorized DMS/CMS/tool/manual implementation records inputs/editions/rules/checks/observations/coverage and generated effects; capability prose is not installed software. Generation/evaluation is separate from actual scoped decision, required condition fulfillment, effective canonical adoption, publication or Baseline selection. No five-item pipeline or automatic edge/allocation/registration operation is imposed.

---

# 55. Relationship Dictionary

The Classification Dictionary shall provide authoritative definitions for canonical relationship types.

A relationship definition should include:

- relationship name;
- semantic definition;
- source;
- target;
- inverse;
- cardinality;
- constraints;
- lifecycle semantics.

**Current governing scope.** These eight semantic definition subjects retain their meaning, not a universal physical entry schema or evidence every kind has an inverse/fully established numerical counts. Identify actual owner definitions/editions and applicable endpoint/property rules. Actual Dictionary14/36 general terms, earlier role meanings and specific kind/alias population limits remain; citation alone proves no completed accepted catalog. Metadata descriptor/Profile rules remain independent.

---

# 56. Relationship Specification

The Classification Specification shall define the normative representation and conformance requirements for Classification Relationships.

This document provides the architectural model.

The Classification Specification provides the normative specification.

**Current governing scope.** This is a real owner requirement, not proof a complete physical representation, general count catalog or all conformance rules already exist there. Actual Specification R011–014/§8/§12/§28/Core16.1, Constraints and common mechanism duties remain independently applicable. Primary Type Structure correctly describes this domain organization; architectural-model wording does not reclassify it automatically. No local source result proves complete implementation or global acceptance.

---

# 57. Extensibility

The Classification Relationship model may be extended when new semantic relationships are required.

Extensions shall:

- have explicit semantics;
- define source and target;
- define direction;
- define cardinality;
- define constraints;
- preserve existing semantics in ordinary extension, with necessary assessed semantic or mandate revision explicitly governed;
- receive governance approval.

This follows the Classification Extensibility model.

**Current governing scope.** Ordinary extension preserves existing meaning. Necessary assessed normative, foundational, role, interface or domain revision requires actual prior/new mandates, need, responsible authority, rationale/alternatives, concrete owners/consumers/indispensable interfaces, honest compatibility, mappings/nonreuse/reservation/history, pinned source/definition/endpoint/record/decision/result/target editions/context, authorized coordinated transition and later checks (§71). No arbitrary mutation, owner takeover or hidden compatibility by extension label. Actual Extensibility34 Request modification and37 conditions fulfilled before canonical extension remain; unchanged Metadata owner restrictions retain their real source-specific pending differences.

---

# 58. Relationship Extension

A new relationship type should follow:

**Received unnamed visual in §58 (span 57 in original order).** Exact text below is evidence,not a second governing rule.

```text

             Need Identified
                    │
                    ▼

          Relationship Proposal
                    │
                    ▼

           Semantic Evaluation
                    │
                    ▼

                Governance
                    │
                    ▼

            Relationship Type

```

**Current relation scope:** Conditional actual need/proposal/evaluation/decision/kind concern,not a created kind,allocated identity,fulfilled conditions or effective canonical adoption from arrows.

| Received label / relation | Current typed interpretation |
|---|---|
| Need Identified | Actual identified proposal/need/definition subject and governing source edition/scope/authority,not a universally registered lifecycle state,created kind,canonical adoption or performed operation from this view. |
| Relationship Proposal | Actual identified proposal/need/definition subject and governing source edition/scope/authority,not a universally registered lifecycle state,created kind,canonical adoption or performed operation from this view. |
| Semantic Evaluation | Actual evaluation concern needs responsible criteria/source editions,authority,observations and coverage,prior/new meaning and affected interfaces. Not a completed review/runtime,decision,condition fulfillment or direct mutation. |
| Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| Relationship Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. |


A new relationship type should not be introduced merely as an implementation convenience.

**Current governing scope.** Need is actual semantic/architectural need, not tool convenience or a completed decision from this conceptual chain. Actual proposal/subject/edition/authority, evaluation evidence/coverage, rationale/alternatives, conditions and effective adoption remain required. The view creates no kind, assigns no identity and performs no canonical or operational act.

---

# 59. Relationship Naming

Relationship names shall be:

- unambiguous;
- semantically meaningful;
- stable;
- consistent with the Classification vocabulary.

Equivalent concepts should not receive multiple canonical names without an explicit architectural reason.

**Current governing scope.** Distinguish canonical kind/name, readable label, inverse, synonym, entity identity and assertion/record. Preserve exact received spelling and actual definition status; equivalent-looking names do not prove equivalence or allocate an alias. An explicitly justified naming distinction needs actual authority/evidence and historical mapping, not uncontrolled vocabulary duplication or a fifth documentary Type.

---

# 60. Relationship Semantics Preservation

The meaning of a canonical relationship should remain stable.

Changing:

**Received unnamed visual in §60 (span 58 in original order).** Exact text below is evidence,not a second governing rule.

```text

    contains  =  hierarchical containment

```

**Current relation scope:** Exact before/after semantic meanings demonstrate noneditorial change;not equivalent concurrent current definitions,automatic authority or arbitrary widening of contains.

| Received label / relation | Current typed interpretation |
|---|---|
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| = | Received semantic-change comparison in§60:hierarchical containment→general association is actual meaning change requiring assessed responsible authority,not editorial equivalence,two current contains definitions or permission from the example. |
| hierarchical containment | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |


into:

**Received unnamed visual in §60 (span 59 in original order).** Exact text below is evidence,not a second governing rule.

```text

    contains  =  general association

```

**Current relation scope:** Exact before/after semantic meanings demonstrate noneditorial change;not equivalent concurrent current definitions,automatic authority or arbitrary widening of contains.

| Received label / relation | Current typed interpretation |
|---|---|
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| = | Received semantic-change comparison in§60:hierarchical containment→general association is actual meaning change requiring assessed responsible authority,not editorial equivalence,two current contains definitions or permission from the example. |
| general association | Received semantic-change comparison in§60:hierarchical containment→general association is actual meaning change requiring assessed responsible authority,not editorial equivalence,two current contains definitions or permission from the example. |


would represent a semantic change rather than a simple editorial modification.

Such changes require governance.

**Current governing scope.** This explicit semantic-change example remains valid: changing hierarchical containment into general association is not editorial correction. Both exact literal meanings remain received evidence, not two current governing definitions of contains. Any actual changed meaning needs its responsible prior/new mandate/authority/need/alternatives/impact/history/compatibility and later checks. Authorized working Draft reconciliation is distinct from formal canonical adoption; implementations cannot silently redefine owner meaning.

---

# 61. Relationship Historical Preservation

Historical relationships shall remain interpretable wherever actual responsible requirements require it; additional preservation should be maintained where possible.

When a relationship is deprecated or retired, its historical meaning shall remain preserved where necessary under the actual historical-interpretation requirements.

For example:

**Received unnamed visual in §61 (span 60 in original order).** Exact text below is evidence,not a second governing rule.

```text

                Old Class
                    │
               replaced by
                    │
                    ▼

                New Class

```

**Current relation scope:** Selected historical replacement example with required retained interpretation and actual identity/edition/context;not mandatory Class,equivalence,performed migration or live retrieval proof.

| Received label / relation | Current typed interpretation |
|---|---|
| Old Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| replaced by | Received directed evolution/replacement wording;exact supersession/replacement/inverse distinction follows actual canonical owner definitions and remains unestablished where evidence is incomplete. Not automatic equivalence,migration,alias allocation,history deletion or current-use permission. |
| New Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


preserves the evolution of the Classification model.

**Current governing scope.** Preserve actual prior relation/kind/endpoint/definition/assignment/decision/source editions and relevant pinned context where needed for required interpretation. The exact replacement view is selected evolution evidence, not compulsory Class, equivalence or executed migration. Historical interpretation, proven original validity, present use and live retrieval are separate. Retirement or a successor does not erase required meaning or silently retarget old snapshots.

---

# 62. Relationship Migration

When relationship semantics change, migration may be required.

Migration should identify:

- affected relationships;
- affected Classification Elements;
- affected documents;
- affected consumers;
- historical impact;
- compatibility requirements.

Migration is governed separately from the semantic definition of the relationship.

**Current governing scope.** The six migration subjects require a concrete actual affected-association/endpoint/document/consumer/source-edition batch, old/new mapping, authority/conditions, semantic-equivalence limits, compatibility/history and later target checks before separately authorized execution. Replacement/supersession and field/path changes alone perform no reassignment, rekeying, retargeting or migration. Real cross-owner/provider/cycle effects remain even when impact is labelled Local.

---

# 63. Relationship Impact

Relationship changes may have local or cross-component impact.

Examples:

| Change | Received potential impact | Current bounded assessment |
|---|---|---|
| New relationship | Local / Dictionary / Validation | Actual kind/definition/association admission;domain Dictionary,Schema/Constraints,Validation,Governance,common records and real consumers as applicable,not automatically Local. |
| Changed cardinality | Schema / Validation | Known obligations and actual responsible general multiplicities/endpoint/property scope;no arbitrary counts or waiver by missing general rules. |
| Changed relationship semantics | Entire Classification architecture | Actual prior/new semantics/authority and concrete owner/consumer/interface/compatibility/history batch;independent mandatory requirements remain. |
| Deprecated relationship | Existing Classification | Actual kind/association/endpoint state/use subject,conditions and required history;no default severity or automatic migration. |
| Retired relationship | Historical data | Actual explicit retirement/use constraints and required prior interpretation;not deletion or automatic invalidation of historical evidence. |
| New inverse | Navigation / Discovery | Actual inverse semantics/navigation versus stored record/projection and freshness;no automatic reverse edge or duplicate allocation. |
| New cross-component relationship | Registry / Knowledge Graph | Actual domain/common typed record/Metadata/Identity/Registry/Graph/provider interfaces and real cycles,not a complete network or implicit owner transfer. |


Impact shall be evaluated before approval.

**Current governing scope.** All seven original change/impact pairs remain exact received subjects with current assessment scope in the table. Actual36-path batch precedes this source mutation; its hashes/coordinates/clauses/prior-new reason/authority/interfaces/history remain central evidence. It is concrete coordination evidence, not proof all external consumers known or integrated. Actual significant structural/role/provider/domain effects require responsible authority regardless of local/cross-component labels.

---

# 64. Relationship Integrity Rules

The following rules apply to canonical relationships:

1. Every relationship shall have a valid source.
2. Every relationship shall have a valid target.
3. Every relationship shall have a defined relationship type.
4. The relationship type shall define its semantic meaning.
5. Source and target shall satisfy relationship constraints.
6. Direction shall be respected.
7. Cardinality shall be respected.
8. Hierarchical relationships shall respect hierarchy constraints.
9. Invalid cycles shall not exist.
10. Deprecated relationships shall not be used for new Classification definitions unless explicitly permitted.
11. Retired relationships shall not be used as active relationships.
12. Relationship evolution shall be governed.

**Current governing scope.** All twelve original integrity subjects retain actual scoped force: source/target/type must be actually valid under applicable rules; defined meaning, permitted endpoints, direction, cardinality and actual hierarchy/cycle requirements remain; deprecation needs actual explicit permission for a different use, retirement forbids ordinary active use and evolution is governed. Matrix23 distinguishes real violations from incomplete authority/check/lookup evidence; matrix34 separates state subjects/decisions/operations. No universal tree, automatic exception/severity, all-context valid history or field catalog follows; known mandates are not waived.

---

# 65. Conformance

A Classification implementation conforms to this document when:

- Classification Relationships are explicitly defined;
- canonical relationship types have defined semantics;
- source and target roles are defined;
- relationship direction is defined;
- relationship constraints are enforceable;
- hierarchical relationships preserve Classification structure;
- invalid relationships can be detected;
- relationship evolution is governed;
- historical relationships can remain traceable;
- conceptual relationship meaning remains independent of implementation technology, while implementations respect applicable owner contracts.

**Current governing scope.** Assess the ten criteria for actual intended subject/population/source/definition/endpoint/record editions, rules/authority, conditions, performed checks/observations/coverage and actual implementation/effect evidence where the claim needs it. Actual Specification R011–014/R018/§8/§12/§28/Core16.1, independent Constraints/Profile/Identity and known duties remain. Missing mandatory checks withholds broader success; source presence or a successful subset is not complete implementation or architectural acceptance. Technology independence preserves owner meaning rather than allowing implementations to ignore the conceptual contract.

---

# 66. Relationship Invariants

The following invariants define the architectural relationship model:

1. A relationship connects Classification Elements.
2. A relationship has semantic meaning.
3. A relationship type defines that meaning.
4. Direction is significant unless symmetry is explicitly defined.
5. Any actual scheme-specific hierarchy is explicitly defined and structurally ordered; documentary roles do not impose a universal Family–Type–Class hierarchy.
6. Document Type has one uniform primary responsibility; Family context can constrain use without owning its Type vocabulary.
7. Class is optional explicitly defined non-conflicting meaning; any actual hierarchical relation requires a separately defined applicable scheme context.
8. Hierarchical relationships must remain structurally consistent.
9. Invalid references are prohibited.
10. Relationship evolution requires governance.
11. Validation verifies relationship conformance.
12. Required historical relationship meaning shall remain interpretable; additional preservation should be maintained where possible.
13. Relationship semantics must remain stable unless explicitly changed through governance.

**Current governing scope.** The thirteen invariant subjects now use current roles and actual scheme-specific properties. Relationship kind/definition/assertion/record and endpoint state/context remain distinct; direction/symmetry, valid references and actual constraints keep responsible force. Known rule observations and genuine missing general-rule/authority/route/guard/record/evidence details coexist. Required history and explicit semantic-change authority remain; no source-local correction closes global19, M13/M14 or actual implementation/permission/architectural-acceptance criteria.

---

# 67. Architectural Model

Selected relationship-model concerns are summarized below; the received view is not a complete accepted implementation or provider graph:

**Received unnamed visual in §67 (span 61 in original order).** Exact text below is evidence,not a second governing rule.

```text

                                    Classification
                                          │
                    ┌─────────────────────┴─────────────────────┐
                    │                                           │
                 Elements                                 Relationships
                    │                                           │
         ┌──────────┼──────────┐                   ┌────────────┼────────────┐
         │          │          │                   │            │            │
       Family      Type      Class                Type      Direction   Constraints
         │          │          │                   │
         └──────────┴──────────┘                   │
                    │                              │
                    └──────────────┬───────────────┘
                                   │
                                 Schema
                                   │
                                   │
                               Validation
                                   │
                                   │
                               Governance

```

**Current relation scope:** Selected structural/owner concerns,not complete accepted model,components/provider DAG or runtime;first Type is document role,second Type is relationship kind.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification | Actual Classification domain/component context with separate role/category/value/assignment/relationship/owner duties. A selected architecture view proves no complete population,required-provider direction,runtime or global acceptance. |
| Elements | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| Relationships | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. This exact Type position denotes the relationship kind,not documentary Type. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |
| Type | Actual relationship kind and responsible semantic definition/edition/applicability,not primary documentary Type,a display label or actual assertion. Defined semantics is a real requirement;no complete accepted kind catalog or universal physical field inferred. This exact Type position denotes the relationship kind,not documentary Type. |
| Direction | Actual relationship property under defined responsible semantics and endpoint/context;not every edge is a dependency and inverse/symmetry do not reverse actual consumer→provider authority. |
| Constraints | Actual allowed kinds/endpoints/properties/count/state/context and responsible applicability/conflict/precedence duties. Known mandates remain;missing detail neither invents precedence/counts nor waives real requirements. |
| Schema | Actual responsible structural contract including known Schema34 normalized-role obligations and genuine general cardinality/population/record gaps;not complete physical fields,automatic provider/runtime or fully accepted integrated schema. |
| Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |


This model establishes the relationship between Classification Elements and the semantic relationships that connect them.

**Current governing scope.** The exact full-looking view is selected structural/evaluation/decision composition, not registered components, runtime order, indispensable-provider direction, complete vocabulary, field schema or accepted complete architecture. The two Type positions have different meanings: primary document role under Elements, relationship kind under Relationships. Actual Schema/Validation/Governance owners and real provider/representation interfaces remain, with known obligations and genuine integration gaps.

---

# 68. Relationship Governance Model

The overall governance model is:

**Received unnamed visual in §68 (span 62 in original order).** Exact text below is evidence,not a second governing rule.

```text

       Classification Relationship
                    │
                    ▼

                Definition
                    │
                    ▼

                Validation
                    │
                    ▼

                Governance
                    │
                    ▼

            Canonical Relationship
                    │
                    ▼

                Lifecycle
                │
                ├── Active
                ├── Deprecated
                └── Retired

```

**Current relation scope:** Selected definition/evidence/decision/canonical/lifecycle concerns with distinct actual kind/assertion/endpoint state subjects and authority/conditions/effect evidence,not automatic adoption or machine.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Relationship | Actual domain semantic association concern;identify kind/definition and actual association/assertion/endpoints/context separately from common typed connection record and projection. Presence of labels/definitions alone supplies no validity,permission or actual operation. |
| Definition | Actual identified proposal/need/definition subject and governing source edition/scope/authority,not a universally registered lifecycle state,created kind,canonical adoption or performed operation from this view. |
| Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| Canonical Relationship | Actual exact authorized/effectively adopted domain relationship kind/definition/association subject under applicable conditions and independent owner requirements. Necessary approval alone is not proof of fulfillment,activation,publication or Baseline selection;changed Draft inherits none. |
| Lifecycle | Actual bounded owner definition/state/use contract and independent decision/transition/history requirements. Relationship-kind definition,association/assertion and endpoints differ;selected path is not complete route/guard/actor/record authority or executed machine. |
| Active | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |
| Deprecated | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |
| Retired | Actual bounded kind-definition/association/assertion/endpoint state/use subject under LifecycleV2R1 and GovernanceV2R1. Document Status,term/extension/R assertion/result/finding/Milestone states differ;known decisions/use/history rules and genuine guard/route/actor gaps remain,not an executed event. |


This separates definition, validation, governance and lifecycle responsibilities.

**Current governing scope.** The exact view selects definition/evidence/decision/canonical/lifecycle concerns. Actual relation-kind definition, association/assertion and endpoint states differ. Actual Governance19/43/51/53–56/72 and Lifecycle19/20/48 require scope/authority/conditions/effect evidence, retain genuine exact-rule gaps and execute no transition. Approval is necessary, not a fifth definition state, fulfilled condition or automatic adoption/activation/publication/Baseline; missing evidence grants no invented outcome or permission.

---

# 69. Summary

Classification Relationships defines the semantic connections between Classification Elements.

The received primary-hierarchy view is retained as historical evidence:

**Received unnamed visual in §69 (span 63 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Family
            │
            └── contains  ─────►  Type
                                  │
                                  └── contains  ─────►  Class

```

**Current relation scope:** Historical primary role hierarchy plus current domain/evidence/decision responsibility summary;actual complementary roles,property/owner mandates and operational/global limits apply.

| Received label / relation | Current typed interpretation |
|---|---|
| Family | Received Family-hierarchy label or placeholder;current applicable Family is actual canonical component/admitted documentary-area membership,not universal Type owner. An actual scheme hierarchy needs responsible definition;no component or population allocation. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Type | Received primary-Type/hierarchy label or placeholder;current document Type is exactly one uniform Architecture/Structure/Behavior/Reference responsibility with contextual use rules,not Family-owned specialization or a fifth Type. Actual relationship-kind positions are distinguished separately. |
| contains | Actual defined hierarchical-containment meaning in an applicable scheme. Received Family/Type/Class examples are historical/conditional,not current universal documentary-role hierarchy. Do not silently widen to general association or generate records. |
| Class | Received Class/category/definition/use example label;current Class role is optional explicitly defined non-conflicting meaning,not a universal Type child,mandatory field or complete population. Actual state/history/use/identity subject needs its responsible context;no automatic event or migration. |


The relationship model provides:

- semantic associations;
- hierarchical structure;
- inverse relationships;
- cardinality;
- constraints;
- lifecycle;
- supersession;
- replacement;
- historical traceability.

The fundamental responsibility separation is:

**Received unnamed visual in §69 (span 64 in original order).** Exact text below is evidence,not a second governing rule.

```text

            Classification Elements
            │
            └── define what can be classified

            Classification Relationships
            │
            └── define how Classification Elements relate

            Classification Validation
            │
            └── verifies relationship conformance

            Classification Governance
            │
            └── controls relationship evolution

```

**Current relation scope:** Historical primary role hierarchy plus current domain/evidence/decision responsibility summary;actual complementary roles,property/owner mandates and operational/global limits apply.

| Received label / relation | Current typed interpretation |
|---|---|
| Classification Elements | Actual domain role/category/value/definition or other formally defined Classification subject must be identified. Kind/definition,actual association/assertion,assignment,document/exact edition and represented record differ;no universal one-to-one entity/value/field or allocation from a drawing. |
| define what can be classified | Actual Elements/role/category/value/assignment distinction and admitted subject under current owner rules,not complete population,universal Class field or allocation/assignment performed by prose. |
| Classification Relationships | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| define how Classification Elements relate | Actual domain structural relationship meaning/organization contract,not a newly registered component or takeover of common typed connection records,Metadata representation or implementation. Actual semantic owner/source edition and known residuals remain. |
| Classification Validation | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| verifies relationship conformance | Actual scoped nonmutating conformity evidence under ValidationV2R1 matrices16/39/67 and owner rules/authority/observations/coverage. Three rule-dependent outcomes are not approval;missing mandatory evidence withholds broader success without fabricated violation or decision;no operation from this label. |
| Classification Governance | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |
| controls relationship evolution | Actual Classification domain change/decision conditions under GovernanceV2R1 matrices19/43/51 and §§53–56/72. Subject/edition/scope/authority,conditions/fulfillment,rationale and separate effect evidence required;common process/Metadata/executor duties differ. No actual approval/operation from phase command or arrow. |


Classification Relationships therefore provides the semantic connective structure of the Classification component while remaining independent of storage, implementation and discovery mechanisms.

**Current governing scope.** Current roles in§1 replace the received universal hierarchy; actual hierarchical/non-hierarchical semantics, properties, cardinalities, constraints, lifecycle, supersession/replacement and history remain owner-defined. Domain semantics, nonmutating evidence, actual responsible decisions, common record/projection contracts and authorized operation are distinct. No summary arrow executes a change or proves implementation/global acceptance.

---

# 70. Related Documents



**Current governing scope.** Related sources retain actual unique identity/path, current edition and responsible mandatory/advisory scope. Links are navigation, not full conformance, canonical vocabulary admission, allocation or approval. Preserve original order and self-link; current source-specific differences remain independently assessable.

---

## 70.1. Architecture

- [DF-ARC-001 — Architecture Overview](../../../01-Architecture/DF-ARC-001-ArchitectureOverview.md)
- [DF-ARC-002 — Architectural Principles](../../../01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md)
- [DF-ARC-003 — Architectural Concepts](../../../01-Architecture/DF-ARC-003-ArchitecturalConcepts.md)
- [DF-ARC-004 — Architectural Layers](../../../01-Architecture/DF-ARC-004-ArchitecturalLayers.md)
- [DF-ARC-007 — Component Documentation Structure](../../../01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md)

---

## 70.2. Classification

- [DF-CLS-001 — Classification Architecture](../01-Architecture/DF-CLS-001-ClassificationArchitecture.md)
- [DF-CLS-002 — Classification Concepts](../01-Architecture/DF-CLS-002-ClassificationConcepts.md)
- [DF-CLS-003 — Classification Model](../01-Architecture/DF-CLS-003-ClassificationModel.md)
- [DF-CLS-004 — Classification Elements](DF-CLS-004-ClassificationElements.md)
- [DF-CLS-005 — Classification Schema](DF-CLS-005-ClassificationSchema.md)
- [DF-CLS-006 — Classification Lifecycle](../03-Behavior/DF-CLS-006-ClassificationLifecycle.md)
- [DF-CLS-007 — Classification Validation](../03-Behavior/DF-CLS-007-ClassificationValidation.md)
- [DF-CLS-008 — Classification Governance](../03-Behavior/DF-CLS-008-ClassificationGovernance.md)
- [DF-CLS-009 — Classification Relationships](DF-CLS-009-ClassificationRelationships.md)
- [DF-CLS-010 — Classification Constraints](../03-Behavior/DF-CLS-010-ClassificationConstraints.md)
- [DF-CLS-011 — Classification Extensibility](../03-Behavior/DF-CLS-011-ClassificationExtensibility.md)
- [DF-CLS-012 — Classification Best Practices](../04-Reference/DF-CLS-012-ClassificationBestPractices.md)
- [DF-CLS-013 — Classification Dictionary](../04-Reference/DF-CLS-013-ClassificationDictionary.md)
- [DF-CLS-014 — Classification Specification](../04-Reference/DF-CLS-014-ClassificationSpecification.md)
- [DF-CLS-015 — Classification Examples](../04-Reference/DF-CLS-015-ClassificationExamples.md)

---

# 71. Working relationship decisions, affected-source coordination and provenance

This V2.0 R1 source-local working successor records four actual reasoned decisions under adopted Review Policy and current owner contracts. Original meanings remain full before-evidence, exact individually qualified unnamed visuals, original subjects and undated history, not simultaneous conflicting rules. The correct Structure/02-Structure identity/path is retained.

| Actual working decision | Prior meaning / gap | Current bounded contract |
|---|---|---|
| Current roles and actual relation properties | Universal primary/canonical Family→Type→Class hierarchy,Family-owned Type and contextual Class child;property examples inherit those governing roles | Actual membership Family,one uniform primary four-value Type,optional defined non-conflicting Class;actual scheme-specific hierarchy and actual directional/inverse/symmetric/transitive/acyclic semantics remain distinct and responsible-rule dependent |
| Typed relation identity,cardinality and evidenced validity | Untyped endpoint/kind labels,possible Source+Type+Target identity and normal uniqueness,old-role1-to-many illustrations,existence-based validity/orphan shorthand and incomplete coverage context | Relationship kind/definition/assertion/endpoint/assignment/record/document K/local R/exact edition differ;known normalized-role obligations versus genuine general relation-count gaps;actual uniqueness/duplicate exceptions and actual validity/coverage evidence,not a universal physical key or source-existence sufficiency |
| Actual lifecycle,decision,conditions and required historical meaning | Relationship/endpoint/state subjects and selected activation/canonical paths underspecified;correct separate migration and history intent do not fully establish actual authority/conditions/coverage/effects | Actual kind-definition/association/assertion/endpoint state subjects;bounded Lifecycle19/20/48 and Governance19/43/51/53–56/72;approval necessary not proof of fulfillment/adoption/activation/publication/Baseline;required history,original validity,current use and retrieval separate |
| Owner interfaces,necessary assessed evolution and bounded conformance | Element-only Metadata shorthand,domain relationship versus general records/projections underspecified,§57 unqualified semantics freeze and full-model/implementation-independence wording | Classification domain semantics versus common typed connection records,Metadata representation,Identity and Registry/Graph source-edition/freshness,common Automation capabilities and authorized executor;ordinary preservation versus necessary assessed mandate revision;independent mandatory breadth and real providers/cycles/placement residual retained |

**Actual authority, need and alternatives.**

**Current roles and actual relation properties.** Adopted ReviewPolicy3,current Classification Architecture/Concepts/reconstructed Model/Elements/Schema/Governance and actual Constraints/Specification relationship-property mandates. Header-only edits leave binding hierarchy/invariants/examples contradictory. Rejecting all hierarchy/properties would discard real scheme-specific rules. Selected correction replaces universal role ownership while preserving all exact historical views and useful semantic properties with actual typed scope.

**Typed relation identity,cardinality and evidenced validity.** Actual Model14,Schema14/34,Constraints19–30,Specification R011–014/§8/§12/Core16.1,Validation16/39/67,DID0147/12 and common Relationships ownership. A mandatory universal tuple/key,count or complete catalog lacks authority;blanket unknown cardinality waives known duties. Treating every missing lookup as Invalid fabricates observations;ignoring real undefined references waives integrity. Selected matrices20/23/46 retain actual mandates and explicit claim/authority/evidence limits.

**Actual lifecycle,decision,conditions and required historical meaning.** Actual LifecycleV2R1/GovernanceV2R1,Constraints31–36/66–68,Specification R019/R021/R022/R026/R027,Extensibility34/37 and authorized working ReviewPolicy. Approval sufficiency or source presence invents actual actors,guards,execution or permission. A universal extra outcome/state also lacks authority. Selected matrix34 preserves known decisions/use/history obligations,genuine exact-rule/actor/record gaps and separately authorized operations;working Draft correction is not canonical architectural adoption.

**Owner interfaces,necessary assessed evolution and bounded conformance.** Actual ARC0055–8/AP015–018,Specification R018/R028–030/§28/Core16.1,Governance30/65.5/72 and responsible actual source/representation/provider contracts. Calling all cross-owner models external cannot erase common mechanisms or actual indispensable interfaces. Absolute freeze prevents justified reconciliation;arbitrary relabelling hides real cycles. Selected concrete36-path batch preserves actual prior/new authority,need,rationale/alternatives,owners/consumers/interfaces,compatibility/mappings/history/pinned snapshots,authorized transition and later checks.

**Real owner interfaces and independent mandates.** Classification owns actual domain role/category/value/relationship meaning and applicability. General Relationships owns typed connection mechanisms/records under ARC0057.2 and Specification28, not document-only endpoints; domain meaning, actual assertion and represented connection/projection differ. Metadata Dictionary/Schema/Profile/Instance and effective Profile own actual descriptor representation; actual Metadata Validation7.2/14 and Specification R005/§7 mandatory representation requirements remain. Metadata Relationships3/13/16 has broader subjects, no ownership transfer, actual Profile/Instance provider and no architectural dependency-cycle mandates. Local semantic tuples and labels allocate no complete field schema or Metadata Elements. DID0147/12 locally distinguishes qualified K, complete supporting R/assertions/reference and exact edition; residual field/interface/prior-restriction propagation remains, not a globally accepted merger.

Common Workflow/Policies/Reviews/Baselines own documentary process/decision/evidence/snapshot contracts. Domain Governance actualV2R1 conditions/evidence and actual authorized DMS/CMS/tool/manual operation are separate. Approval is necessary in scope, not proof of fulfillment/effective adoption/activation/publication/Baseline inclusion. Missing decision/authority/evidence grants no outcome or permission. Local authorized Draft correction is permitted working activity, not actual canonical architectural approval. Source-local construction is neither domain engine/runtime/replay testing nor deployed enforcement.

Registry/Graph projection authority requires actual source/definition/endpoint/record edition/context and current/historical/snapshot/freshness scope. Real indispensable Classification→Metadata/Identity, conditional Templates structural contracts, and MTD001 depends-only/support versus DID009/README reciprocal Metadata↔Identity requirements remain pending responsible core/descriptor/source-edition/interface/cycle assessment. Projection, inverse, local-scope or document-order labels remove no real required edge/cycle and prove no complete DAG/runtime. Actual physical/descriptor/Profile/reference/index/interface/access/retrieval/usage/history effects and placement mandates remain independent of technology choice.

**Necessary assessed revision.** Ordinary extension preserves meaning/roles/properties. Any necessary normative/foundational/role/interface/domain change requires actual prior/new mandates, need, responsible authority, rationale/alternatives, concrete owners/consumers/indispensable interfaces, honest compatibility, old/new term/kind/definition/association/assignment/record/reference mappings, applicable nonreuse/reservation/history, pinned source/definition/endpoint/decision/result/target edition/bytes/context, authorized coordinated transition and later checks before propagation. Same name/path/tuple or extension label proves no compatible meaning. Preserve required historical interpretation and prior valid observations without arbitrary mutation or owner takeover. Unchanged Metadata and other actual owner restrictions remain source-specific pending differences, not already waived or integrated.

**Concrete batch before mutation.** Thirty-six actual source/owner/consumer/reference paths were identified with exact input coordinates/hashes/clauses, actual path-specific prior/new actions, reason, authority, interfaces and compatibility/history before source mutation. All remain byte-unchanged. This batch identifies concrete coordination for this correction, not every external consumer or completed integration. Any later propagation needs actual authority, assessed successor/contributor/event history and later checks; an external decision alone increments no consumer edition.

| Actual source / functional subject | Exact input edition | Actual path | Pending action |
|---|---|---|---|
| DF-ARC-002 | V2.0 R2; Draft; Baseline Not assigned | 01-Architecture/DF-ARC-002-ArchitecturalPrinciples.md | Keep ordinary preservation versus necessary assessed relationship-role/property/identity/interface mandate revision;actual need/authority/alternatives/history and no universal quality/acceptance claim. |
| DF-ARC-005 | V2.0 R2; Draft; Baseline Not assigned | 01-Architecture/DF-ARC-005-ArchitecturalComponents.md | Map Classification relation semantics versus general Relationships typed records,Registry/Graph source-edition projections,Automation capability and authorized executor;retain real indispensable interfaces/cycles. |
| DF-ARC-007 | V2.0 R2; Draft; Baseline Not assigned | 01-Architecture/DF-ARC-007-ComponentDocumentationStructure.md | Keep legitimate Relationships Structure/02-Structure;known Elements Architecture/02-Structure mismatch remains unmet M13 work,not waived by conceptual independence. |
| DF-CLS-001 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/01-Architecture/DF-CLS-001-ClassificationArchitecture.md | Qualify actual current relation-property/endpoint context and prior Relationships snapshots;no universal documentary-role hierarchy or reopening completed Architecture cycle. |
| DF-CLS-002 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/01-Architecture/DF-CLS-002-ClassificationConcepts.md | Keep current roles and actual conditional scheme-specific hierarchy;qualify broader current Relationships-source readings without rewriting received notes. |
| DF-CLS-003 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/01-Architecture/DF-CLS-003-ClassificationModel.md | Use actual14 role-versus-general-relation cardinality boundaries,definition/assertion/assignment subjects and actual domain/provider context;no restored authentic history or global merger. |
| DF-CLS-004 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/02-Structure/DF-CLS-004-ClassificationElements.md | Retain known obligations and actual source-qualified relationship statements;physical Elements placement remains unmet,not moved or silently revalidated. |
| DF-CLS-005 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/02-Structure/DF-CLS-005-ClassificationSchema.md | Replace current-looking historical Family1→manyType and Type1→manyClass implications in target;do not invent general endpoint counts or waive known role duties;actual schema/Profile owner requirements remain. |
| DF-CLS-006 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/03-Behavior/DF-CLS-006-ClassificationLifecycle.md | Separate relationship-kind definition,actual association assertion and endpoint states;retain real decisions/history/use rules and missing exact routes/guards/actors without universal aliases. |
| DF-CLS-007 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/03-Behavior/DF-CLS-007-ClassificationValidation.md | Use actual16/39/67 known-rule/claim/edition/observations/coverage scope;no existence-only full validity,missing-lookup fabricated Invalid,automatic correction or approval. |
| DF-CLS-010 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/03-Behavior/DF-CLS-010-ClassificationConstraints.md | Retain source/target/type validity,actual duplicate exceptions,required directions and genuinely hierarchical cycle prohibitions;reconcile old role premises later rather than inventing counts or precedence. |
| DF-CLS-011 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/03-Behavior/DF-CLS-011-ClassificationExtensibility.md | Preserve actual34 Request modification and37 conditions fulfilled before canonical extension;necessary assessed relationship mandate revision is not arbitrary additive semantics or an automatic sixth universal outcome. |
| DF-CLS-012 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/04-Reference/DF-CLS-012-ClassificationBestPractices.md | Preserve recommendation authority and actual contextual relationship meaning;do not promote advice into mandatory cardinality,identity or approval. |
| DF-CLS-013 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/04-Reference/DF-CLS-013-ClassificationDictionary.md | Keep exact owner differences and incomplete specific relationship-kind/alias population;do not fabricate approved contains/belongsTo/supersedes/replaces register or merge term/definition/assertion states. |
| DF-CLS-014 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/04-Reference/DF-CLS-014-ClassificationSpecification.md | Retain explicit semantics/source-target/direction/cardinality/constraint duties and owner-scoped hierarchy;source-local correction is not complete Core or architectural approval. |
| DF-CLS-015 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Classification/04-Reference/DF-CLS-015-ClassificationExamples.md | Keep example and historical status;actual labels/arrows allocate no kind/identity,prove no transition or full mandatory conformance. |
| 02-Documentation/Classification/README.md | Functional non-normalized file | 02-Documentation/Classification/README.md | Keep intended document identity/path and source-edition status clear;current old-source notes remain event-time evidence,not silent successor acceptance. |
| DF-DID-009 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/DocumentIdentity/02-Structure/DF-DID-009 - Document Identity Relationships.md | Retain qualified identity and actual general connection-record boundaries;semantic associations are not reverse required edges,while real Metadata↔Identity core/descriptor/cycle claims remain. |
| DF-DID-014 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/DocumentIdentity/04-Reference/DF-DID-014 - Document Identity Specification.md | Keep relationship/kind/entity/assertion/record identity distinct from document K/local R/exact edition and live target;no generic DF allocation,classification-derived rekey or pinned-history retargeting. |
| DF-MTD-001 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/01-Architecture/DF-MTD-001-MetadataArchitecture.md | Keep real indispensable provider/owner/representation interfaces and responsible cycle assessment;Classification relationship projections do not silently reconcile reciprocal requirements. |
| DF-MTD-002 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/01-Architecture/DF-MTD-002-MetadataConcepts.md | Do not transfer domain relation-kind/endpoint/definition authority through descriptor grouping or alias relationship type with document Type. |
| DF-MTD-003 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/01-Architecture/DF-MTD-003-MetadataModel.md | Distinguish relation semantic definition/assertion from actual descriptor/connection representation;no universal endpoint/context tuple or physical field catalog from visual labels. |
| DF-MTD-004 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/01-Architecture/DF-MTD-004-MetadataElements.md | No automatic Metadata Element/document allocation from relationship Source/Type/Target or identity tuple;keep actual entity/record/field duties distinct. |
| DF-MTD-005 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/02-Structure/DF-MTD-005-MetadataSchema.md | Relationship conceptual tuple/inverse/navigation does not allocate physical fields,waive actual Profile/Instance rules or supply a complete merged schema. |
| DF-MTD-009 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/02-Structure/DF-MTD-009-MetadataRelationships.md | Preserve broader actual Metadata subjects and real Profile/Instance provider requirements;Class domain semantics/common connection records/projections differ,and no renamed-away required cycle. |
| DF-MTD-010 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/02-Structure/DF-MTD-010-MetadataConstraints.md | Keep owner requirements explicit while relation checking/decision/implementation remain separate;no arbitrary precedence or permission from partial rollout. |
| DF-MTD-013 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/02-Structure/DF-MTD-013-MetadataDictionary.md | Relationship kind/name/label/inverse/identity/source-target are not automatically cataloged Metadata fields;actual Dictionary authority and incomplete integration remain. |
| DF-MTD-006 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/03-Behavior/DF-MTD-006-MetadataLifecycle.md | Keep actual owner state/authority semantics;no automatic aliases with Classification Active/Deprecated/Retired,document Status or local R assertion. |
| DF-MTD-007 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/03-Behavior/DF-MTD-007-MetadataValidation.md | Retain independent mandatory representation checks;source presence or successful semantic relation checks prove no full descriptor/effective-Profile conformity. |
| DF-MTD-008 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/03-Behavior/DF-MTD-008-MetadataGovernance.md | Use actual owner precedent without granting global operational authority;unchanged Metadata stability/extension clauses retain source-specific pending reconciliation. |
| DF-MTD-011 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/03-Behavior/DF-MTD-011-MetadataExtensibility.md | Necessary assessed Classification relationship revision neither edits nor waives Metadata owner constraints;further propagation requires actual prior/new authority/compatibility/history. |
| DF-MTD-012 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/04-Reference/DF-MTD-012-MetadataBestPractices.md | Do not invent normative relationship identity/cardinality/decision rules from recommendations or interpret independent guidance as actual approval. |
| DF-MTD-014 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/04-Reference/DF-MTD-014-MetadataSpecification.md | Local relationship model does not complete Metadata field/identity/representation integration or waive actual mandatory Profile/Instance interface criteria. |
| DF-MTD-015 | V1.0 R0; Draft; Baseline 1.0 | 02-Documentation/Metadata/04-Reference/DF-MTD-015-MetadataExamples.md | Illustrative node/edge/type/descriptor wording does not authorize canonical relation population,physical schema,transition or publication. |
| DF-RVW-001 | V1.0 R2; Draft; Baseline Not assigned | 03-Governance/Reviews/03-Behavior/DF-RVW-001-ReviewPolicy.md | Keep REVIEW source unchanged and UPDATE pending;honestly assess actual semantic replacement before V2R1,retain historical input/events and earlier Model factual-premise qualifications. |
| DF-CLS-008 | V2.0 R1; Draft; Baseline Not assigned | 02-Documentation/Classification/03-Behavior/DF-CLS-008-ClassificationGovernance.md | Use actual19/43/51/53–56/72,not staleV1R0 snapshot;approval necessary not sufficient evidence of canonical adoption/activation/publication/Baseline;prior valid domain obligations remain event-time/current-scope facts. |

**Current peers and prior-event qualification.** Actual CLS001–008 V2.0 R1 working successors completed their local documentary cycles, not global integrated acceptance. Model remains explicit reconstruction rather than recovered authentic history. Schema34/41 preserves known roles and genuine general multiplicity/population/record gaps; Lifecycle19/20/48 preserves bounded state/use duties and genuine exact routes/guards/actors/record gaps; Validation16/39/67 preserves real rule-dependent results/coverage/nonmutation/replay limits; Governance19/43/51/53–56/72 preserves actual authority/conditions/decision/effect boundaries. Actual Specification/Constraints/Profile/Identity and all independent mandatory owner requirements remain applicable to actual claimed breadth.

Earlier Architecture/Concepts/Model/Elements/Schema/Lifecycle/Validation/Governance RelationshipsV1R0 snapshots and real hierarchy/cardinality/acyclicity/domain observations retain actual event-time and semantic scope. General property/count gaps can remain real after this bounded correction. Any broader current normative/status claim needs separately traced actual-edition qualification, not rewritten prior notes or silently reopened/revalidated completed cycles. Prior Policy4.3/Model factual-premise qualifications remain.

Elements Type Architecture still physically lies under02-Structure contrary to actual ARC007 responsibility-placement requirements: M13 remains Not Started with that known unmet requirement. This correct Relationships Structure/path neither fixes nor waives it. The19 global findings, M14 integrated criteria, actual implementation/permission/architectural-acceptance work remain independent.

**Actual edition and contributor.** Governing universal Family/Type/Class role hierarchy, relation endpoint/property/cardinality/identity/validity/authority/history/evolution/conformance meanings are replaced incompatibly. This is not correct labels or formatting alone. Policy5.2 therefore gives Version1.0→2.0 with minor0, monotonic Revision0→1. Correct ID/title/Family/Component/Type Structure/Language/path remain. Changed exact edition is Draft/Baseline Not assigned, not inherited1.0 membership or prior approval. Preserve original Author Arnaldo Figueira and add actual contributor Codex — AI assistant cumulatively; event attribution remains specific to the real later contribution. Original initial-history table remains verbatim and undated. No original date or completed intermediate edition is invented; unchanged-source VALIDATE later increments neither source coordinate.

All70 original major chapters/72 numbered titles and bodies/75 raw headings, three original table contexts including seven impact rows,28 original list groups,eight validity/twelve integrity/thirteen invariant/ten conformance subjects,20 related subjects and64 exact unnamed spans/260 actual label-relation occurrences retain full before/current maps. Twenty intended local links retain original order/self-link and actual target declarations. Every visual occurrence retains exact text/fence/order with individual typed meaning,relation scope and final complete section text/hash; no diagram ID is invented. Prior paths/exports, failed/pending history and89 progress positions remain. No temporary Author indicator is created.

Twenty-one local corrections are Corrected—pending validation. This UPDATE constructs a Draft successor and traceability evidence only: no source VALIDATE,finding closure,allocation,actual relationship creation/assignment,transition,migration,retirement,permission,canonical adoption,publication,Baseline or engine/complete implementation/global architectural acceptance occurs. Known obligations remain real; missing mandatory authority/check/operation evidence withholds broader success without invented violations,universal new fields/outcomes or waived mandates. Separate unchanged-source VALIDATE must assess exact resulting bytes and all21 original criteria with actual owner/context evidence and residuals.

---

# Change History

| Version | Description |
|---------|-------------|
| 1.0 | Initial definition of Classification Relationships. |

## Actual later contributions

| Date | Version | Revision | Contributor | Event and limits |
|---|---|---|---|---|
| 2026-10-16 | 2.0 | 1 | Codex — AI assistant | Step4.37 UPDATE: current roles and actual scheme-specific relation properties,typed identity/cardinality/validity,authority/conditions/lifecycle/history and necessary-evolution/real-interface correction; original author/history retained. Twenty-one local corrections pending separate VALIDATE. Draft; Baseline Not assigned; no canonical architectural approval or actual operation. |

---

**End of Document**