# THE PHILOSOPHY OF VIABILITY LIBRARY PROJECT

## 1. Project Overview

The Philosophy of Viability Library Project is the central organizational and intellectual infrastructure for the development, documentation, coordination, and publication of the Philosophy of Viability as a coherent philosophical system.

The library provides shared resources, master registries, bibliographic references, conceptual records, and structural and editorial protocols used throughout the development of individual books belonging to the philosophical project.

The library is not itself a book, manuscript, or compilation unit. Its purpose is to support the systematic authorship and maintenance of multiple independent books.

Each book constitutes a distinct publication and an independent compilation unit.

## 2. Architectural Principle

The project follows a two-level architectural distinction:

### 2.1. Library Level

The library is the highest organizational level of the project.

Its responsibilities include:

- Maintaining shared bibliographic resources.
- Maintaining master registries of philosophical entities.
- Preserving common structural and editorial protocols.
- Coordinating terminology and conceptual consistency across books.
- Supporting cross-book references and logical dependencies.
- Providing shared intellectual and documentary resources for authorship.

The library is not intended to be compiled or rendered as a unified document.

It does not have a book-level compilation entry point.

### 2.2. Book Level

Each book is an independent publication unit maintained within its own directory at the library root.

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

The highest compilation level in the project is the individual book.

Books may use shared library resources, but their compilation processes remain independent.

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

Additional books may be introduced as independent directories at the library root.

The library architecture is designed to accommodate the gradual expansion of the philosophical book series without requiring the restructuring of existing books.

## 4. Master Bibliography

The `BIBLIOGRAPHY/` directory maintains shared bibliographic resources for the entire philosophical project.

Its current organization is:

```text
BIBLIOGRAPHY/
├── comparative_sources.bib
├── primary_sources.bib
├── references.bib
└── secondary_sources.bib
```

These files provide the shared bibliographic foundation for individual books.

Each book may maintain its own bibliographic selection and presentation files, containing the references actually used in that publication.

The distinction is between:

- Library-level bibliographic resources: shared and project-wide.
- Book-level bibliographies: publication-specific and used in the compilation of the respective book.

Book-level bibliographic files should remain consistent with the shared bibliographic resources.

## 5. Master Registries

The `REGISTRIES/` directory maintains the canonical project-wide records of philosophical entities.

Its current organization is:

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

These registries provide a common reference framework for the identification, documentation, and coordination of philosophical entities across the book series.

The registries distinguish between different logical and philosophical categories rather than treating all philosophical statements as equivalent.

### 5.1. Registry Scope

The master registries are project-wide.

They are not limited to the content of a single book.

A philosophical entity may be introduced, developed, revised, or referenced in multiple books while retaining its canonical identity in the corresponding master registry.

### 5.2. Book-Level Registries

Individual books may maintain their own registries for publication-specific purposes.

These may document:

- Entities used in the book.
- Their canonical identifiers.
- Their locations within the book.
- Their local logical dependencies.
- Their relations to other entities.
- Their publication-specific status and references.

Book-level registries do not replace or independently redefine the master registries.

Their purpose is to document the application of project-wide philosophical entities within a particular publication.

## 6. Structural and Editorial Protocol

The file:

`Viability_Philosophy_System_Structural_and_Editorial_Protocol.md`

defines the shared structural and editorial framework governing the organization and development of the philosophical book series.

It serves as a common reference for:

- Book architecture.
- Structural identifiers.
- Logical entity identifiers.
- Internal references.
- Cross-book references.
- Logical dependencies.
- Bibliographic organization.
- Editorial consistency.
- Terminological consistency.

Individual books should follow the shared protocol while retaining the ability to implement publication-specific structural requirements.

## 7. Book Architecture

Each book is maintained as an independent directory at the library root.

The first book is:

`VS.B01_ONTOLOGY_OF_VIABILITY/`

Its purpose is to establish the ontological framework of the Philosophy of Viability.

The book's internal architecture is organized into four principal components:

1. `1_FRONTMATTER/`
2. `2_MAINMATTER/`
3. `3_BACKMATTER/`
4. `4_ASSETS/`

The book also maintains its own root-level configuration, metadata, glossary, acronym definitions, documentation, and compilation output.

The internal structure and organization of each book are governed by the shared project protocol and its publication-specific requirements.

## 8. Hierarchical Aggregation and Compilation

Individual books use a hierarchical aggregation architecture.

The root-level `main.tex` of each book serves as its compilation entry point.

It coordinates the four principal book components through their respective aggregators.

Each aggregating layer is responsible for invoking the direct components belonging to its own structural level.

The aggregation hierarchy proceeds recursively from the book level through the main components, parts, chapters, and their internal content groups.

The principal objectives of this architecture are:

- Maintaining a clear compilation hierarchy.
- Avoiding direct invocation of deeply nested files from the book root.
- Isolating compilation responsibilities.
- Simplifying debugging and maintenance.
- Supporting the incremental expansion of book content.
- Preserving a clear distinction between aggregators and substantive content files.

Aggregator filenames must be distinguishable from the filenames of substantive content files and from other aggregators.

## 9. Structural Organization Principles

The project follows these general organizational principles:

### 9.1. Separation of Library and Publication

Shared project infrastructure belongs at the library level.

Publication-specific content and compilation resources belong within the corresponding book directory.

### 9.2. Independent Book Compilation

Each book must remain independently compilable and renderable.

The compilation of one book must not require compiling the entire library.

### 9.3. Hierarchical Aggregation

Each aggregation unit manages its direct subordinate components.

Higher-level aggregators should not bypass the established hierarchy to invoke deeply nested content directly.

### 9.4. Controlled Directory Depth

Directory structures should remain sufficiently shallow to support efficient authorship, navigation, debugging, and maintenance.

Additional directory levels should be introduced only when they provide a meaningful organizational or functional benefit.

The number of files in a directory does not, by itself, justify creating additional directory levels.

### 9.5. Content and Artifact Separation

Substantive textual content and supporting artifacts should be organized according to their distinct roles.

Chapters use independently maintained section files.

Appendices may maintain their complete textual content in a single file, regardless of length.

Supporting figures, diagrams, illustrations, and other assets are maintained in the appropriate asset locations.

### 9.6. Preservation of Canonical Records

Project-wide philosophical entities and bibliographic records should retain stable canonical identities.

Book-specific references and local records should not create unintended duplicates or conflicting definitions.

## 10. Current Project Scope

The current library includes the foundational infrastructure and the first book of the planned philosophical series.

The first book, `VS.B01_ONTOLOGY_OF_VIABILITY`, establishes the ontological foundations upon which subsequent philosophical investigations and publications can be developed.

The library is designed to support the progressive development of additional books.

Future books may address further dimensions of the Philosophy of Viability while sharing the project's master resources and structural protocols.

The precise scope, organization, and publication sequence of future books remain subject to subsequent architectural and intellectual development.

## 11. Language and Documentation Policy

All repository files, including source code, LaTeX documents, registries, metadata, filenames, directory names, comments, and technical documentation, use English.

This policy ensures consistency across the repository and its associated technical workflows.

## 12. Maintenance and Evolution

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

Existing architectural decisions should not be altered solely for cosmetic reasons or unnecessary structural symmetry.

The governing objective is to maintain a coherent, extensible, and intellectually consistent infrastructure for the development of the Philosophy of Viability.

---

**Project:** The Philosophy of Viability Library Project

**Repository Root:** `THE_PHILOSOPY_OF_VIABILITY_LIBRARY_PROJECT`

**First Book:** `VS.B01_ONTOLOGY_OF_VIABILITY`

**Architectural Principle:** A shared non-compilable library supporting independently compilable books.
