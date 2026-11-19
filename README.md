# THE PHILOSOPHY OF VIABILITY LIBRARY PROJECT

## Structural, Editorial, and Referencing Protocol

**Project:** The Philosophy of Viability Library Project
**Repository Root:** `THE_PHILOSOPY_OF_VIABILITY_LIBRARY_PROJECT`
**First Book:** `VS.B01_ONTOLOGY_OF_VIABILITY`
**Architectural Principle:** A shared non-compilable library supporting independently compilable books.

**Document type:** System-wide production protocol
**Applies to:** All books and all structural and supporting content in the Viability Philosophy System
**Audience:** Authors, editors, research assistants, AI agents, translators, and future collaborators

---

# PART ONE: THE LIBRARY

## 1. Project Overview

The Philosophy of Viability Library Project is the central organizational and intellectual infrastructure for the development, documentation, coordination, and publication of the Philosophy of Viability as a coherent philosophical system.

The library provides shared resources, master registries, bibliographic references, conceptual records, and structural and editorial protocols used throughout the development of individual books belonging to the philosophical project.

The library is not itself a book, manuscript, or compilation unit. Its purpose is to support the systematic authorship and maintenance of multiple independent books. Each book constitutes a distinct publication and an independent compilation unit.

### 1.1 Current Project Scope

The current library includes the foundational infrastructure and the first book of the planned philosophical series.

The first book, `VS.B01_ONTOLOGY_OF_VIABILITY`, establishes the ontological foundations upon which subsequent philosophical investigations and publications can be developed.

The library is designed to support the progressive development of additional books. Future books may address further dimensions of the Philosophy of Viability while sharing the project's master resources and structural protocols. The precise scope, organization, and publication sequence of future books remain subject to subsequent architectural and intellectual development.

### 1.2 Language and Documentation Policy

All repository files, including source code, LaTeX documents, registries, metadata, filenames, directory names, comments, and technical documentation, use English. This policy ensures consistency across the repository and its associated technical workflows.

---

## 2. Architectural Principle

The project follows a two-level architectural distinction: the **Library Level** and the **Book Level**.

### 2.1 Library Level

The library is the highest organizational level of the project. It is not intended to be compiled or rendered as a unified document and has no book-level compilation entry point.

Its responsibilities include:

- Maintaining shared bibliographic resources.
- Maintaining master registries of philosophical entities.
- Preserving common structural and editorial protocols.
- Coordinating terminology and conceptual consistency across books.
- Supporting cross-book references and logical dependencies.
- Providing shared intellectual and documentary resources for authorship.

### 2.2 Book Level

Each book is an independent publication unit maintained within its own directory at the library root. The highest compilation level in the project is the individual book.

A book has its own:

- Main document.
- LaTeX configuration and preamble.
- Metadata.
- Content architecture.
- Frontmatter.
- Mainmatter.
- Backmatter.
- Book-specific registries.
- Bibliographic selection.
- Assets.
- Compilation and rendering outputs.

Books may use shared library resources, but their compilation processes remain independent.

---

## 3. Repository Structure

The current top-level organization is:

```text
THE_PHILOSOPY_OF_VIABILITY_LIBRARY_PROJECT/
│
├── BIBLIOGRAPHY/
│
├── REGISTRIES/
│
├── VS.B01_ONTOLOGY_OF_VIABILITY/
│
└── Viability_Philosophy_System_Structural_and_Editorial_Protocol.md
```

Additional books may be introduced as independent directories at the library root. The library architecture is designed to accommodate the gradual expansion of the philosophical book series without requiring the restructuring of existing books.

---

## 4. Master Bibliography

The `BIBLIOGRAPHY/` directory maintains shared bibliographic resources for the entire philosophical project:

```text
BIBLIOGRAPHY/
├── comparative_sources.bib
├── primary_sources.bib
├── references.bib
└── secondary_sources.bib
```

These files provide the shared bibliographic foundation for individual books. Each book may maintain its own bibliographic selection and presentation files, containing the references actually used in that publication.

The distinction is between:

- **Library-level bibliographic resources:** shared and project-wide.
- **Book-level bibliographies:** publication-specific and used in the compilation of the respective book.

Book-level bibliographic files should remain consistent with the shared bibliographic resources. The detailed bibliographic and citation protocol is given in Part Two, Section 13.

---

## 5. Master Registries

The `REGISTRIES/` directory maintains the canonical project-wide records of philosophical entities:

```text
REGISTRIES/
├── axioms.csv
├── definitions.csv
├── propositions.csv
├── theses.csv
├── hypotheses.csv
├── arguments.csv
└── philosophical_foundations.csv
```

These registries provide a common reference framework for the identification, documentation, and coordination of philosophical entities across the book series. They distinguish between different logical and philosophical categories rather than treating all philosophical statements as equivalent.

### 5.1 Registry Scope

The master registries are project-wide and not limited to the content of a single book. A philosophical entity may be introduced, developed, revised, or referenced in multiple books while retaining its canonical identity in the corresponding master registry.

### 5.2 Book-Level Registries

Individual books may maintain their own registries for publication-specific purposes. These may document:

- Entities used in the book.
- Their canonical identifiers.
- Their locations within the book.
- Their local logical dependencies.
- Their relations to other entities.
- Their publication-specific status and references.

Book-level registries do not replace or independently redefine the master registries. Their purpose is to document the application of project-wide philosophical entities within a particular publication.

---

## 6. Structural Organization Principles

The project follows these general organizational principles.

### 6.1 Separation of Library and Publication

Shared project infrastructure belongs at the library level. Publication-specific content and compilation resources belong within the corresponding book directory.

### 6.2 Independent Book Compilation

Each book must remain independently compilable and renderable. The compilation of one book must not require compiling the entire library.

### 6.3 Hierarchical Aggregation

Each aggregation unit manages its direct subordinate components. Higher-level aggregators should not bypass the established hierarchy to invoke deeply nested content directly.

### 6.4 Controlled Directory Depth

Directory structures should remain sufficiently shallow to support efficient authorship, navigation, debugging, and maintenance. Additional directory levels should be introduced only when they provide a meaningful organizational or functional benefit. The number of files in a directory does not, by itself, justify creating additional directory levels.

### 6.5 Content and Artifact Separation

Substantive textual content and supporting artifacts should be organized according to their distinct roles. Chapters use independently maintained section files. Appendices may maintain their complete textual content in a single file, regardless of length. Supporting figures, diagrams, illustrations, and other assets are maintained in the appropriate asset locations.

### 6.6 Preservation of Canonical Records

Project-wide philosophical entities and bibliographic records should retain stable canonical identities. Book-specific references and local records should not create unintended duplicates or conflicting definitions.

---

## 7. Book Architecture

Each book is maintained as an independent directory at the library root. The first book is `VS.B01_ONTOLOGY_OF_VIABILITY/`, whose purpose is to establish the ontological framework of the Philosophy of Viability.

### 7.1 Standard Top-Level Divisions

Unless the author approves another arrangement, every book uses:

1. **FRONTMATTER** — title page, preface, introduction, and contents.
2. **MAIN BODY** — the substantive parts and chapters.
3. **BACKMATTER** — appendices, notes, bibliographies, glossaries, indexes, and technical materials.

These are organizational divisions, not philosophical categories.

### 7.2 Internal Book Structure

The book's internal architecture is organized into four principal components:

1. `1_FRONTMATTER/`
2. `2_MAINMATTER/`
3. `3_BACKMATTER/`
4. `4_ASSETS/`

The book also maintains its own root-level configuration, metadata, glossary, acronym definitions, documentation, and compilation output. The internal structure and organization of each book are governed by the shared project protocol and its publication-specific requirements.

### 7.3 Hierarchical Aggregation and Compilation

Individual books use a hierarchical aggregation architecture. The root-level `main.tex` of each book serves as its compilation entry point and coordinates the four principal book components through their respective aggregators.

Each aggregating layer is responsible for invoking the direct components belonging to its own structural level. The aggregation hierarchy proceeds recursively from the book level through the main components, parts, chapters, and their internal content groups.

The principal objectives of this architecture are:

- Maintaining a clear compilation hierarchy.
- Avoiding direct invocation of deeply nested files from the book root.
- Isolating compilation responsibilities.
- Simplifying debugging and maintenance.
- Supporting the incremental expansion of book content.
- Preserving a clear distinction between aggregators and substantive content files.

Aggregator filenames must be distinguishable from the filenames of substantive content files and from other aggregators.

### 7.4 Canonical Content Hierarchy

The required hierarchy within a book is:

**Book → Part → Chapter → Section → Subsection → Paragraph**

| Level | Function |
| --- | --- |
| Book | A coherent major work within the system. |
| Part | A major stage or subject area in the book's overall architecture. |
| Chapter | A sustained treatment of a defined topic or question. |
| Section | A distinct argumentative or explanatory unit within a chapter. |
| Subsection | A more specific unit within a section. |
| Paragraph | The smallest normally tracked unit of continuous exposition. |

Do not create additional formal hierarchy levels without the author's approval. Tables, figures, equations, notes, and lists do not automatically constitute new hierarchy levels.

Each structural unit must have a clear function. A chapter must do more than repeat its part's title; a section must perform a distinct step; a subsection must refine its parent section; and a paragraph should normally make one principal move: define, distinguish, explain, support, infer, qualify, object, respond, or transition.

---

## 8. Maintenance and Evolution

The library is intended to evolve as the philosophical system and its publications develop.

Changes to shared resources should preserve cross-book consistency and respect the distinction between canonical project-wide records and book-specific implementations.

Structural changes should be evaluated in terms of their effects on:

- Existing books.
- Master registries.
- Bibliographic references.
- Logical entity identifiers.
- Internal and cross-book references.
- Compilation dependencies.
- Editorial and structural protocols.

Existing architectural decisions should not be altered solely for cosmetic reasons or unnecessary structural symmetry. The governing objective is to maintain a coherent, extensible, and intellectually consistent infrastructure for the development of the Philosophy of Viability.

---

# PART TWO: SYSTEM-WIDE PRODUCTION PROTOCOL

## 9. Purpose, Scope, and Authority

This protocol establishes the mandatory procedures for planning, writing, editing, organizing, identifying, cross-referencing, and documenting content throughout the Viability Philosophy System (VPS). It is written for collaborators who have no prior knowledge of the project.

A collaborator using this protocol must be able to determine:

- How books and their contents are structured.
- How structural identifiers are assigned.
- How philosophical and logical entities are identified across books.
- How internal references and dependencies are recorded.
- How external sources and bibliographies are documented.
- How main exposition, technical reconstruction, and comparative study relate.
- How to create or revise content without silently changing the philosophical system.

This is an editorial and structural protocol. It does not independently establish philosophical doctrines.

### 9.1 Order of Authority

When instructions or sources conflict, apply this order:

1. Explicit, current instructions from the system's author.
2. The author's explicit philosophical commitments and clarifications in project discussions.
3. The latest author-approved manuscript and its established terminology.
4. Earlier manuscript versions and working documents.
5. This protocol's editorial conventions and examples.
6. A collaborator's inference or general philosophical knowledge.

A lower-level source must not silently override a higher-level source. If a conflict cannot be resolved, record it and ask the author. Do not invent a synthesis.

### 9.2 No Silent Philosophical Invention

A collaborator may improve clarity, structure, argument presentation, terminology consistency, and documentation. A collaborator must not silently:

- Introduce an axiom, definition, proposition, theorem, or hypothesis.
- Convert a tentative possibility into an established doctrine.
- Present an inference as an explicit authorial commitment.
- Remove a qualification that limits a claim.
- Import assumptions from another philosophical tradition.
- Resolve an open metaphysical question without authorization.
- Attribute a view to the author that is only suggested by an incomplete draft.

Label unauthorized additions as **proposals**, **editorial queries**, or **open issues**.

---

## 10. Global Structural Identifier System

### 10.1 Purpose and Format

Structural identifiers locate content across the entire system. They do not identify the philosophical entity discussed in that content.

Use this canonical format:

```text
VS.B01.P01.C01.S01.SS01.P001
```

| Segment | Meaning |
| --- | --- |
| `VS` | Viability Philosophy System |
| `B01` | Book number |
| `P01` | Part number |
| `C01` | Chapter number |
| `S01` | Section number |
| `SS01` | Subsection number |
| `P001` | Paragraph number |

The first `P` after the book number means Part; the final `P` means Paragraph. Their positions distinguish them.

### 10.2 Identifiers for Higher-Level Units

Omit lower-level segments that do not apply:

```text
VS.B01
VS.B01.P02
VS.B01.P02.C03
VS.B01.P02.C03.S01
VS.B01.P02.C03.S01.SS02
VS.B01.P02.C03.S01.SS02.P004
```

Book numbers are global and permanent. Once `B01` is assigned to a book, it must not be reused for a different book. A book title may change without changing its book number.

### 10.3 Assignment Rules

1. Assign identifiers according to the approved structural order.
2. Use two digits for book, part, chapter, section, and subsection numbers; use three digits for paragraph numbers.
3. Number each level within its immediate parent. The full path ensures global uniqueness.
4. Never assign the same full identifier to two different units.
5. Every paragraph included in the formal paragraph-level reference system must have its own identifier.
6. Maintain all identifiers in the Structural Identifier Registry.
7. Give tables, figures, equations, and notes local labels where necessary, but do not confuse those labels with canonical paragraph IDs.

### 10.4 Moving, Splitting, Merging, and Retiring Units

Because a structural ID encodes a unit's current location, moving a unit may require changing its ID. To preserve traceability:

- Record the former ID.
- Record the new ID.
- State why the change was made.
- Update all internal references and maps.
- Never silently recycle an obsolete ID.

If one paragraph is split into two, assign two new IDs and record their predecessor. If two paragraphs are merged, record both predecessor IDs. Do not imply that a substantially changed unit is identical to its earlier version.

The Structural Identifier Registry must include: current ID, unit type, title or description, status, previous ID(s), and change note.

### 10.5 Structural IDs Are Not Logical Entity IDs

Never use a structural ID as the permanent identifier of an axiom, definition, proposition, theorem, hypothesis, argument, or proof. A logical entity may be introduced in one location and used in many others, including future books. It needs an identity independent of its location.

---

## 11. Global Logical Entity Identifier System

### 11.1 Purpose

Logical entity identifiers identify formal philosophical or logical entities independently of where they occur. An entity retains the same identifier across all books.

Use these prefixes:

| Prefix | Entity class | Example |
| --- | --- | --- |
| `AX-` | Axiom | `AX-001` |
| `DF-` | Definition | `DF-001` |
| `PR-` | Proposition | `PR-001` |
| `TH-` | Theorem | `TH-001` |
| `HY-` | Hypothesis | `HY-001` |
| `AR-` | Argument | `AR-001` |
| `PF-` | Proof | `PF-001` |

Number sequentially within each class, globally across the system. Do not restart numbering in a new book.

### 11.2 Classification Guidance

- **Axiom:** a foundational commitment adopted as a starting point.
- **Definition:** an approved specification of the meaning or conceptual boundaries of a term.
- **Proposition:** a claim advanced for examination or derivation.
- **Theorem:** a result presented as demonstrable from stated premises and inferential rules.
- **Hypothesis:** a provisional claim that remains open to examination.
- **Argument:** an organized inferential case supporting or challenging a claim.
- **Proof:** a structured demonstration of a result from specified premises and rules.

These are editorial descriptions, not permission to reclassify the author's work. If an entity's status is unclear, do not promote it to a stronger category by editorial judgment. Ask the author or mark the classification provisional.

### 11.3 Assignment Rules

1. Assign an ID when an entity is formally introduced or registered.
2. Use the next available number in its class.
3. Never assign one ID to two different entities.
4. Do not change an ID merely because its wording or location changes.
5. Do not assign formal IDs to every sentence, example, heading, or informal remark.
6. Do not create new entity classes or prefixes without author approval.
7. An informal first mention is not automatically the formal origin of an entity.

### 11.4 Logical Entity Registry

Maintain one authoritative registry for the whole system. Each record should contain:

| Field | Content |
| --- | --- |
| Entity ID | Permanent ID, e.g. `AX-001`. |
| Type | One of the approved entity classes. |
| Name / short label | Concise recognizable title. |
| Formal statement | Approved formulation, where applicable. |
| Origin | Structural ID of first formal introduction. |
| Canonical location | Location of authoritative formulation, if different. |
| Status | Proposed, provisional, active, revised, superseded, or withdrawn. |
| Depends on | Entity IDs on which it logically depends. |
| Referenced in | All structural IDs where it is used or discussed. |
| Notes / history | Qualifications and revision history. |

**Origin** and **Canonical location** may differ. An idea may first appear provisionally and receive its authoritative formulation later.

### 11.5 Relations Between Entities and Locations

Where relevant, classify each occurrence:

- **Introduction** — first formal introduction.
- **Definition** — authoritative formulation.
- **Reference** — mention or recall.
- **Premise** — used as a premise in reasoning.
- **Derivation** — derived or used in a derivation.
- **Application** — applied to another problem or domain.
- **Proof** — used in a proof.
- **Criticism** — examined or challenged.
- **Revision** — formulation or status revised.

Example:

| Entity ID | Relation | Structural location |
| --- | --- | --- |
| `AX-001` | Introduction | `VS.B01.P01.C02.S01.SS01.P003` |
| `AX-001` | Premise | `VS.B01.P03.C04.S02.SS01.P006` |
| `AX-001` | Application | `VS.B02.P01.C03.S01.SS02.P002` |

This distinction prevents a passing mention from being confused with a substantive logical use.

### 11.6 Dependencies

Record a dependency only when the actual reasoning supports it or the author explicitly approves it. Do not infer a dependency merely because two entities occur in the same paragraph.

For each dependency, record the dependent entity, the entity on which it depends, the type of dependency if known, and the structural location where the dependency is established or used.

---

## 12. Entity-to-Location Maps

At the end of each book, include a **Book-Level Logical Entity Reference Map**. Maintain a **System-Level Master Logical Entity Map** covering every book.

Recommended columns:

| Entity ID | Type | Short label | Origin / canonical location | Other locations in this book | Relation(s) |
|---|---|---|---|---|---|

The book-level map includes every formal entity introduced, used, or substantively discussed in that book. If an entity originates elsewhere, retain its original ID and origin.

The system-level map is authoritative. A book-level map is a book-specific view of the master registry, not a competing registry. Reconcile discrepancies against the approved manuscript and master registry.

Before a book is complete, verify that:

1. Every formally identified entity has a registry record.
2. Every entity used in the book appears in its book-level map.
3. Every listed location actually contains the stated relation.
4. Every structural reference resolves.
5. Dependencies are supported.
6. Superseded formulations are distinguished from current formulations.

---

## 13. Bibliographic and External Source Protocol

### 13.1 Do Not Assign Source IDs

External books, articles, editions, manuscripts, and other sources must **not** receive identifiers such as `ARIST-001`, `SRC-001`, or any equivalent source ID.

Identify a source through ordinary bibliographic information: author, title, editor or translator, edition, publication details, and other standard data.

### 13.2 Internal Citation Locations

Every bibliographic entry must be associated with the structural location or locations in the Viability Philosophy books where it is cited.

Example:

```text
Aristotle.
Metaphysics.
Translated by W. D. Ross.
Oxford: Clarendon Press.

Cited at:
- VS.B01.P01.C01.S02.SS01.P004
- VS.B01.P01.C05.S01.SS02.P003
- VS.B02.P02.C03.S01.SS01.P006
```

These structural IDs identify the paragraphs in the Viability Philosophy books that cite the source. They do not replace the precise locator within the external work.

### 13.3 Exact External Locators

Citations must identify the relevant location within the external source as precisely as possible. Depending on the source, this may be a page range, book and chapter, section, proposition, theorem, scholium, Bekker or Stephanus number, volume and page, line numbers, or another stable scholarly locator.

Example:

```text
Aristotle, Metaphysics, Γ.3, 1005a19–21.
```

Do not invent page numbers, editions, translators, or passage references. If a locator cannot be verified, mark it for checking.

### 13.4 Part-Level and System-Level Bibliographies

A book may organize bibliographies by part or chapter. Nevertheless:

1. Each entry must contain complete ordinary bibliographic information.
2. Its system-wide `Cited at` list must preserve all relevant internal citation locations across all books.
3. Repeated appearances of one work in part-level bibliographies must not be treated as different sources.
4. The system-level master bibliography should consolidate each work into one ordinary entry with all known internal citation locations.
5. No source-specific ID may be introduced.

A part-level bibliography may display only the locations relevant to that part for readability, provided the master bibliography preserves the complete list.

### 13.5 Bibliographic Register Fields

Track: full bibliographic entry, edition or translation used, exact external locator(s), internal structural IDs under `Cited at`, verification status, and notes.

The bibliography is a register of ordinary bibliographic entries and citation locations. It is not an identifier system for sources.

---

## 14. Expository Architecture: Main Text, Technical Reconstruction, Comparison

### 14.1 Main Exposition

The main text must remain intelligible and genuinely argumentative. It is not merely an informal introduction to reasoning hidden in a technical appendix.

It must provide enough reasoning for readers to understand:

- What is claimed.
- What the central terms mean.
- Why the claim is advanced.
- Which distinctions and assumptions it requires.
- How the conclusion follows at the level appropriate to the chapter.
- What limitations or unresolved issues remain.

Do not remove all justification from the main text in the name of technical cleanliness.

### 14.2 Technical Reconstruction Chapters

Where appropriate, a part may end with a dedicated chapter titled or functioning as **Principles, Arguments, and Formal Reconstruction**.

It gathers technical material that would otherwise interrupt the main exposition, while leaving sufficient reasoning in the main text. It may include:

- Formal statements of axioms and definitions.
- Numbered propositions and theorems.
- Explicit premises and inferential steps.
- Detailed argument reconstructions.
- Symbolic or mathematical formulations.
- Proof structures.
- Dependency relations.
- Technical qualifications.
- Formal objections and responses.

It must not introduce a different doctrine from the main text. It reconstructs or formalizes material already established or explicitly proposed. If formalization exposes ambiguity, inconsistency, or a missing premise, report it rather than concealing it.

Distinguish clearly between:

1. What the main text explicitly asserts.
2. What follows from those assertions.
3. What the reconstruction assumes for analysis.
4. What remains unproved or unresolved.

### 14.3 Comparative Studies

Where appropriate, a part may end with a chapter titled or functioning as **Comparative Ontological Studies**.

Comparison must be substantive, not decorative. Do not include a philosopher merely because similar vocabulary appears.

A sound comparison identifies:

1. The specific problem being compared.
2. The historical model's relevant assumptions.
3. Its account of the relevant concept or relation.
4. The corresponding account in Viability Philosophy.
5. Genuine similarities.
6. Decisive differences.
7. Explanatory advantages and limitations.
8. What the comparison does and does not establish.

Do not attribute a position to a historical thinker without reliable textual support. Distinguish the thinker's own claims from later interpretations. Similarity does not establish historical influence.

### 14.4 Relationship Between the Modes

| Mode | Purpose | Typical location |
| --- | --- | --- |
| Main exposition | Develop concepts and arguments in a readable, continuous form. | Main chapters of each part. |
| Technical reconstruction | Make logical and formal structure inspectable in detail. | Dedicated chapter near the end of a part, where appropriate. |
| Comparative study | Compare the account with relevant historical models. | Dedicated chapter near the end of a part, where appropriate. |

These modes complement one another. None should contradict or replace the others.

---

## 15. Specific Architecture of *Ontology of Viability*

This section records the currently approved high-level architecture of *Ontology of Viability*. It must not automatically be imposed on other books. The exact chapter count, chapter titles, and placement of supplementary material remain subject to the author's approved detailed outline.

The main body has four core parts, in this order:

1. **IDENTITY AND MANIFESTATION**
2. **THE REALMS OF BEING**
3. **LIGHT**
4. **THE DYNAMICS OF BEING**

### 15.1 Part I — Identity and Manifestation

This part is definitional and conceptual. It establishes what identity is, what manifestation is, and how they are understood ontologically.

It may clarify, where supported by approved material:

- The ontological status and nature of identity.
- The ontological status and nature of manifestation.
- Their foundational conceptual relation.
- Invariance and what remains identical.
- Unity and plurality.
- Conditions and domains relevant to manifestation.

**Boundary:** Do not develop relational dynamics, interaction among components, rules of manifestation, or detailed mechanisms of expression here. Those belong to the part on the dynamics of being unless the author revises the architecture.

### 15.2 Part II — The Realms of Being

This part explains the realms individually and then their integrated architecture.

The framework distinguishes four fundamental realms:

1. **First Determination**
2. **Structural Determination**
3. **Relational Manifestation**
4. **Material Manifestation**

It also distinguishes three mediating or *barzakhic* realms:

1. **Hub of Decree**
2. **Hub of Signification**
3. **Hub of Realization**

**Boundary:** Do not present all seven as equivalent items in one undifferentiated ladder. The four fundamental realms and three barzakhic realms have different ontological statuses. Explain each realm individually before presenting the integrated architecture.

The exact status and placement of the **Transcendent Ground** and the **Throne-Domain** remain open unless explicitly settled in author-approved material. Do not automatically classify either as one of the seven realms or as an additional realm.

### 15.3 Part III — Light

Light is an independent and central part. Begin by establishing its ontological status and nature. Do not reduce it in advance to an instrument, mechanism, metaphor, or secondary feature of manifestation.

Maintain a distinction between:

- **Ontological light**, insofar as the approved theory gives it an ontological role.
- **Epistemic light or legibility**, concerning knowability, intelligibility, or access.

Do not collapse these senses. Draw precise claims about light from the author's approved philosophical material.

### 15.4 Part IV — The Dynamics of Being

This part addresses relations, processes, rules, and dynamics that should not be introduced prematurely into the definitional part.

Depending on the approved outline, relevant subjects may include:

- The dynamic structure of being.
- Necessity and rules of expression.
- Rules and dynamics of manifestation.
- Relations and ontological networks.
- Causation, law, and possibility.
- Energy.
- Time, eternity, and becoming.
- Birth and death.
- Awareness, self-awareness, and mind considered ontologically.
- Action and agency.
- The cost of expression or manifestation.
- Residue and sedimentation.
- Reversibility.

This is a scope guide, not a claim that every topic is already established or must become a separate chapter. Confirm status and placement against approved material.

### 15.5 Optional Integrative Part

A further part, provisionally titled **INTEGRATION OF ONTOLOGICAL PRINCIPLES**, has been considered as a possible place for system-wide coherence, unity, recursive or holographic structures, limits, open problems, and conclusions.

This is **not a finalized or mandatory part**. Do not add it without explicit author approval.

---

## 16. Philosophical Status and Uncertainty

Preserve the status of every substantive claim. Distinguish, as appropriate:

- **Established commitment:** explicitly adopted by the author.
- **Definition:** an approved specification of a term.
- **Derived result:** a conclusion supported by identified premises and reasoning.
- **Proposition:** a claim advanced for examination or demonstration.
- **Theorem:** a result accompanied by an appropriate proof.
- **Hypothesis:** a provisional claim that remains open.
- **Interpretation:** an explanation of a passage or argument.
- **Proposal:** a possible development not yet approved as doctrine.
- **Open problem:** a question not yet resolved.
- **Editorial suggestion:** a proposed presentation or organizational improvement, not a philosophical claim.

Do not present a claim as more certain, foundational, or fully demonstrated than its source warrants.

Preserve qualifications such as *possibly*, *in this sense*, *under these conditions*, *at this level*, *not necessarily*, and *provisionally* when they carry philosophical weight.

If a later book refines or challenges an earlier claim, do not silently rewrite the earlier book to create an appearance of seamless consistency. Record the development, identify the relevant locations, and obtain the author's decision about whether either text should be revised.

---

## 17. Writing and Editing Standards

### 17.1 Prose

Write clear, precise, academically credible prose. The writing should be accessible to an informed intermediate reader while remaining rigorous enough for advanced readers.

- Define specialized terms before relying heavily on them.
- Use one term consistently for one concept unless a distinction is explained.
- Avoid introducing many technical terms in one paragraph without need.
- Prefer explicit reasoning to rhetorical emphasis.
- Avoid ornamental repetition and inflated claims.
- Use examples to clarify, not replace, an argument.
- Make transitions explain logical relations, not merely announce topics.
- Distinguish metaphor from literal ontological claims.
- Do not present an analogy or diagram as proof.

### 17.2 Paragraph Discipline

Each paragraph should normally have one primary function. When editing, ask:

1. What is the paragraph's principal claim or function?
2. Does it depend on terms already defined?
3. Does it introduce a new entity that should be registered?
4. Is its reasoning adequate for the main exposition?
5. Does it repeat material without adding a function?
6. Are the author's qualifications preserved?
7. Are citations and cross-references accurate?

### 17.3 Headings and Hierarchy

Headings must describe the actual content. Do not promise a proof where only an intuition is offered, or a complete theory where the discussion is exploratory.

Use heading levels consistently with the canonical hierarchy. Do not skip levels for visual convenience.

### 17.4 Terminology

Maintain a system-wide glossary or terminology register where needed. For each important technical term, record:

- Preferred form.
- Approved definition or description.
- Relevant `DF-` identifier, if formally defined.
- Variants or translations.
- Terms that must not be treated as synonyms.
- Relevant structural locations.

Do not replace a deliberate authorial distinction with a more familiar term from another tradition.

### 17.5 Figures, Tables, and Notation

Every figure, table, and formal expression must have a clear purpose and be explained in the surrounding text.

- Define symbols before or at first substantive use.
- Keep notation consistent across books.
- Do not let a diagram imply a hierarchy, equivalence, direction, or causal relation that the text has not established.
- State the limits of a diagram when it simplifies a more complex structure.

---

## 18. Procedure for Revising an Existing File

Follow this workflow whenever a file is revised.

**Step 1 — Identify the exact source.** Confirm the exact file and version. Similarly titled files may differ. Do not assume that the newest-looking file is authoritative.

**Step 2 — Inspect the relevant context.** Read enough of the file to understand its structure, terminology, claims, references, and dependencies. If the correction affects other chapters or registries, inspect those materials too. Do not revise from an isolated excerpt when the issue depends on the larger argument.

**Step 3 — Diagnose the defect.** Classify the problem, for example:

- Structural inconsistency.
- Conceptual ambiguity.
- Contradiction.
- Missing definition.
- Unsupported inference.
- Misplaced content.
- Repetition.
- Terminology inconsistency.
- Incorrect logical status.
- Faulty cross-reference.
- Bibliographic error.
- Inadequate explanation.
- Formalization problem.

State what is wrong and why it matters, unless the author has requested direct editing without a preliminary report.

**Step 4 — Determine scope.** Identify affected paragraphs, sections, chapters, maps, registries, and files. Avoid unrelated stylistic changes. Explain any necessary broader change.

**Step 5 — Preserve valid content.** Retain established claims, distinctions, examples, terminology, and qualifications unless they are part of the defect or the author instructs otherwise. Do not remove substantive material merely to make the file shorter.

**Step 6 — Rewrite completely when requested.** If the author requests a complete rewritten file, return the entire revised file, not only replacement paragraphs or a list of suggestions. The result must be internally coherent and ready to replace the previous version.

**Step 7 — Update identifiers and references.** If structural locations or logical entities change, update:

- The Structural Identifier Registry.
- The Logical Entity Registry.
- Book-level and system-level maps.
- Affected internal cross-references.
- Bibliographic citation-location lists.
- Identifier history.

Do not knowingly leave broken references.

**Step 8 — Report unresolved matters.** List philosophical issues, missing sources, uncertain attributions, or unresolved dependencies that cannot be settled from approved material. Do not conceal uncertainty by writing around it.

**Step 9 — Final consistency check.** Check architecture, terminology, philosophical status, structural IDs, logical IDs, internal references, external citations, consistency between exposition and technical reconstruction, and cross-book implications.

---

## 19. Procedure for Creating New Content

Before drafting a new unit:

1. Identify its book and intended structural location.
2. Confirm that the subject belongs at that level of the architecture.
3. Review relevant existing material to avoid duplication or contradiction.
4. Identify terms that require definition.
5. Check whether claims already exist in the logical entity registry.
6. Reuse existing logical entity IDs when referring to existing entities.
7. Register genuinely new entities only when formally introduced and their status is clear.
8. Assign structural IDs according to the global hierarchy.
9. Add justified cross-references and dependencies.
10. Add external citations with precise source locators.
11. Update relevant book-level and system-level maps.
12. Mark unresolved decisions instead of silently deciding them.

A new file must not establish a parallel terminology, numbering scheme, bibliography, or logical registry that conflicts with the system-wide apparatus.

---

## 20. Required Registers and Supporting Documents

Maintain one clearly designated canonical version of each register. Registers may be separate files or parts of a structured database.

### 20.1 Structural Identifier Registry

Tracks all books and structural units, their current IDs, headings, status, and identifier history.

### 20.2 Logical Entity Registry

Tracks all axioms, definitions, propositions, theorems, hypotheses, arguments, and proofs across all books.

### 20.3 Entity-to-Location and Dependency Map

Tracks where each entity is introduced, defined, referenced, used, derived, proved, applied, criticized, or revised, and records supported dependencies. This may be implemented within the Logical Entity Registry, but the information must remain explicitly available.

### 20.4 Bibliographic Reference Register

Tracks ordinary bibliographic entries, exact external locators, internal structural citation locations, and verification status. It must not assign source-specific IDs.

### 20.5 Terminology Register

Tracks preferred technical terms, definitions, variants, translations, and distinctions that must be preserved.

### 20.6 Change Log

Records significant changes to architecture, structural identifiers, logical entities, terminology, and cross-book relations. Each entry should include date, affected item, nature of change, reason, and author approval status.

---

## 21. Quality-Control Checklist

Use this checklist before approving a new or revised file.

### 21.1 Structural Integrity

- [ ] The file belongs to the correct book and location.
- [ ] Its function is clear at the assigned hierarchy level.
- [ ] It follows the approved architecture.
- [ ] Structural IDs are valid and unique.
- [ ] No obsolete ID has been silently reused.

### 21.2 Philosophical Integrity

- [ ] Authorial claims and distinctions are preserved.
- [ ] Established commitments are distinguished from hypotheses and proposals.
- [ ] No unsupported doctrine has been introduced.
- [ ] Definitions are stable and consistently used.
- [ ] Inferences are not presented as explicit premises.
- [ ] Open problems remain open.

### 21.3 Logical Integrity

- [ ] Formal entities have the correct type and ID.
- [ ] Existing entities reuse their global IDs.
- [ ] New entities are registered.
- [ ] Premises and dependencies are accurately represented.
- [ ] Proofs support the results they claim to establish.
- [ ] Main exposition and technical reconstruction are consistent.

### 21.4 Reference Integrity

- [ ] Internal references resolve to existing structural IDs.
- [ ] Entity-to-location maps are updated.
- [ ] Bibliographic details are accurate.
- [ ] External citations include precise locators where available.
- [ ] Internal citation locations are recorded.
- [ ] No source-specific identifier has been created.

### 21.5 Editorial Integrity

- [ ] Prose is clear and precise.
- [ ] Paragraphs have identifiable functions.
- [ ] Headings accurately describe content.
- [ ] Repetition has been removed only when genuinely redundant.
- [ ] Examples and diagrams do not overstate the argument.
- [ ] The complete revised file is supplied when requested.

---

## 22. Ambiguity and Escalation

Ask the author when a decision materially affects philosophical content or system architecture and cannot be resolved from approved sources.

Examples:

- Uncertainty whether a claim is an axiom, proposition, or hypothesis.
- Uncertainty about the ontological status of a realm or domain.
- Conflict between author-approved formulations.
- Uncertainty whether two concepts are identical, included, or distinct.
- A proposed change to the four-part architecture of *Ontology of Viability*.
- A proposed new logical entity class or prefix.
- Uncertainty about the accuracy of a historical attribution.
- A structural change affecting many references.
- A proof that appears to require an unstated premise.

A clarification request must state:

1. The exact issue.
2. Relevant structural or entity IDs.
3. Competing interpretations.
4. Why the choice matters.
5. The decision required.

Ask a precise question rather than a broad one.

---

## 23. Core Operating Principles

1. **One system, multiple books:** books are distinct but connected.
2. **One global structural hierarchy:** structural IDs locate content across the system.
3. **One global logical entity system:** formal entities retain their IDs across books.
4. **Location and identity are different:** structural IDs identify where; logical IDs identify what.
5. **No source IDs:** external works use ordinary bibliographic data and internal citation locations.
6. **Traceability:** formal entities, structural changes, dependencies, and citations must be traceable.
7. **No silent invention:** inference, interpretation, and suggestion must not become doctrine without approval.
8. **Preserve distinctions:** authorial conceptual and ontological distinctions must remain explicit and stable.
9. **Readable rigor:** the main exposition must be understandable and reasoned; technical detail may be concentrated without emptying the main text of argument.
10. **Substantive comparison:** historical comparisons must be accurate, relevant, and analytically meaningful.
11. **Cross-book consistency:** changes in one book must be checked against their implications elsewhere.
12. **Authorial authority:** unresolved philosophical and architectural decisions belong to the author.

---

# APPENDICES

## Appendix A. Identifier Examples

### A.1 Structural Locations

```text
VS.B01
VS.B01.P01
VS.B01.P01.C01
VS.B01.P01.C01.S01
VS.B01.P01.C01.S01.SS01
VS.B01.P01.C01.S01.SS01.P001
```

### A.2 Logical Entities

```text
AX-001
DF-001
PR-001
TH-001
HY-001
AR-001
PF-001
```

### A.3 Cross-Book Use

An axiom first introduced in Book 01 retains its ID when used in Book 02:

```text
Entity: AX-001

Origin:
VS.B01.P01.C02.S01.SS01.P003

Referenced in:
VS.B01.P03.C04.S02.SS01.P006
VS.B02.P01.C03.S01.SS02.P002
VS.B02.P04.C02.S03.SS01.P008
```

### A.4 Bibliographic Entry

```text
Aristotle.
Metaphysics.
Translated by W. D. Ross.
Oxford: Clarendon Press.

External locations cited:
- Γ.3, 1005a19–21
- Ζ.1, 1028a10–20

Cited at:
- VS.B01.P01.C01.S02.SS01.P004
- VS.B01.P01.C05.S01.SS02.P003
- VS.B02.P02.C03.S01.SS01.P006
```

The bibliographic entry has no source ID. Internal structural IDs identify where the source is cited; external locators identify the passages in the external work.

---

## Appendix B. Minimum Record Templates

### B.1 Structural Unit Record

```text
Current ID:
Unit type:
Book:
Parent unit:
Title / description:
Status:
Previous ID(s):
Change note:
```

### B.2 Logical Entity Record

```text
Entity ID:
Type:
Name / short label:
Formal statement:
Origin:
Canonical location:
Status:
Depends on:
Referenced in:
Relation types:
Revision history:
Notes:
```

### B.3 Bibliographic Record

```text
Full bibliographic entry:
Edition / translation used:
External source locations cited:
Internal structural locations (Cited at):
Verification status:
Notes:
```

### B.4 Change-Log Record

```text
Date:
Affected item(s):
Previous state:
New state:
Reason:
Affected references / registers:
Author approval:
```

---

**End of Document**
