# Viability Philosophy System

## Structural, Editorial, and Referencing Protocol

**Document type:** System-wide production protocol\
**Applies to:** All books and all structural and supporting content in
the Viability Philosophy System\
**Audience:** Authors, editors, research assistants, AI agents,
translators, and future collaborators

------------------------------------------------------------------------

## 1. Purpose, scope, and authority

This protocol establishes the mandatory procedures for planning,
writing, editing, organizing, identifying, cross-referencing, and
documenting content throughout the Viability Philosophy System (VPS). It
is written for collaborators who have no prior knowledge of the project.

A collaborator using this protocol must be able to determine: - how
books and their contents are structured; - how structural identifiers
are assigned; - how philosophical and logical entities are identified
across books; - how internal references and dependencies are recorded; -
how external sources and bibliographies are documented; - how main
exposition, technical reconstruction, and comparative study relate;
and - how to create or revise content without silently changing the
philosophical system.

This is an editorial and structural protocol. It does not independently
establish philosophical doctrines.

### 1.1 Order of authority

When instructions or sources conflict, apply this order:

1.  Explicit, current instructions from the system's author.
2.  The author's explicit philosophical commitments and clarifications
    in project discussions.
3.  The latest author-approved manuscript and its established
    terminology.
4.  Earlier manuscript versions and working documents.
5.  This protocol's editorial conventions and examples.
6.  A collaborator's inference or general philosophical knowledge.

A lower-level source must not silently override a higher-level source.
If a conflict cannot be resolved, record it and ask the author. Do not
invent a synthesis.

### 1.2 No silent philosophical invention

A collaborator may improve clarity, structure, argument presentation,
terminology consistency, and documentation. A collaborator must not
silently: - introduce an axiom, definition, proposition, theorem, or
hypothesis; - convert a tentative possibility into an established
doctrine; - present an inference as an explicit authorial commitment; -
remove a qualification that limits a claim; - import assumptions from
another philosophical tradition; - resolve an open metaphysical question
without authorization; or - attribute a view to the author that is only
suggested by an incomplete draft.

Label unauthorized additions as **proposals**, **editorial queries**, or
**open issues**.

------------------------------------------------------------------------

## 2. System-wide book architecture

The Viability Philosophy System consists of multiple books that are
distinct works within one cumulative philosophical system. Their
structural and referencing conventions must therefore be compatible.

### 2.1 Standard top-level divisions

Unless the author approves another arrangement, every book uses:

1.  **FRONTMATTER**
2.  **MAIN BODY**
3.  **BACKMATTER**

These are organizational divisions, not philosophical categories.
Frontmatter may include the title page, preface, introduction, and
contents. The main body contains the substantive parts and chapters.
Backmatter may include appendices, notes, bibliographies, glossaries,
indexes, and technical materials.

### 2.2 Canonical content hierarchy

The required hierarchy is:

**Book → Part → Chapter → Section → Subsection → Paragraph**

  -----------------------------------------------------------------------
  Level                               Function
  ----------------------------------- -----------------------------------
  Book                                A coherent major work within the
                                      system.

  Part                                A major stage or subject area in
                                      the book's overall architecture.

  Chapter                             A sustained treatment of a defined
                                      topic or question.

  Section                             A distinct argumentative or
                                      explanatory unit within a chapter.

  Subsection                          A more specific unit within a
                                      section.

  Paragraph                           The smallest normally tracked unit
                                      of continuous exposition.
  -----------------------------------------------------------------------

Do not create additional formal hierarchy levels without the author's
approval. Tables, figures, equations, notes, and lists do not
automatically constitute new hierarchy levels.

Each structural unit must have a clear function. A chapter must do more
than repeat its part's title; a section must perform a distinct step; a
subsection must refine its parent section; and a paragraph should
normally make one principal move: define, distinguish, explain, support,
infer, qualify, object, respond, or transition.

------------------------------------------------------------------------

## 3. Global structural identifier system

### 3.1 Purpose and format

Structural identifiers locate content across the entire system. They do
not identify the philosophical entity discussed in that content.

Use this canonical format:

``` text
VS.B01.P01.C01.S01.SS01.P001
```

  Segment   Meaning
  --------- -----------------------------
  `VS`      Viability Philosophy System
  `B01`     Book number
  `P01`     Part number
  `C01`     Chapter number
  `S01`     Section number
  `SS01`    Subsection number
  `P001`    Paragraph number

The first `P` after the book number means Part; the final `P` means
Paragraph. Their positions distinguish them.

### 3.2 Identifiers for higher-level units

Omit lower-level segments that do not apply:

``` text
VS.B01
VS.B01.P02
VS.B01.P02.C03
VS.B01.P02.C03.S01
VS.B01.P02.C03.S01.SS02
VS.B01.P02.C03.S01.SS02.P004
```

Book numbers are global and permanent. Once `B01` is assigned to a book,
it must not be reused for a different book. A book title may change
without changing its book number.

### 3.3 Assignment rules

1.  Assign identifiers according to the approved structural order.
2.  Use two digits for book, part, chapter, section, and subsection
    numbers; use three digits for paragraph numbers.
3.  Number each level within its immediate parent. The full path ensures
    global uniqueness.
4.  Never assign the same full identifier to two different units.
5.  Every paragraph included in the formal paragraph-level reference
    system must have its own identifier.
6.  Maintain all identifiers in the Structural Identifier Registry.
7.  Give tables, figures, equations, and notes local labels where
    necessary, but do not confuse those labels with canonical paragraph
    IDs.

### 3.4 Moving, splitting, merging, and retiring units

Because a structural ID encodes a unit's current location, moving a unit
may require changing its ID. To preserve traceability:

-   record the former ID;
-   record the new ID;
-   state why the change was made;
-   update all internal references and maps;
-   never silently recycle an obsolete ID.

If one paragraph is split into two, assign two new IDs and record their
predecessor. If two paragraphs are merged, record both predecessor IDs.
Do not imply that a substantially changed unit is identical to its
earlier version.

The Structural Identifier Registry must include: current ID, unit type,
title or description, status, previous ID(s), and change note.

### 3.5 Structural IDs are not logical entity IDs

Never use a structural ID as the permanent identifier of an axiom,
definition, proposition, theorem, hypothesis, argument, or proof. A
logical entity may be introduced in one location and used in many
others, including future books. It needs an identity independent of its
location.

------------------------------------------------------------------------

## 4. Global logical entity identifier system

### 4.1 Purpose

Logical entity identifiers identify formal philosophical or logical
entities independently of where they occur. An entity retains the same
identifier across all books.

Use these prefixes:

  Prefix   Entity class   Example
  -------- -------------- ----------
  `AX-`    Axiom          `AX-001`
  `DF-`    Definition     `DF-001`
  `PR-`    Proposition    `PR-001`
  `TH-`    Theorem        `TH-001`
  `HY-`    Hypothesis     `HY-001`
  `AR-`    Argument       `AR-001`
  `PF-`    Proof          `PF-001`

Number sequentially within each class, globally across the system. Do
not restart numbering in a new book.

### 4.2 Classification guidance

-   **Axiom:** a foundational commitment adopted as a starting point.
-   **Definition:** an approved specification of the meaning or
    conceptual boundaries of a term.
-   **Proposition:** a claim advanced for examination or derivation.
-   **Theorem:** a result presented as demonstrable from stated premises
    and inferential rules.
-   **Hypothesis:** a provisional claim that remains open to
    examination.
-   **Argument:** an organized inferential case supporting or
    challenging a claim.
-   **Proof:** a structured demonstration of a result from specified
    premises and rules.

These are editorial descriptions, not permission to reclassify the
author's work. If an entity's status is unclear, do not promote it to a
stronger category by editorial judgment. Ask the author or mark the
classification provisional.

### 4.3 Assignment rules

1.  Assign an ID when an entity is formally introduced or registered.
2.  Use the next available number in its class.
3.  Never assign one ID to two different entities.
4.  Do not change an ID merely because its wording or location changes.
5.  Do not assign formal IDs to every sentence, example, heading, or
    informal remark.
6.  Do not create new entity classes or prefixes without author
    approval.
7.  An informal first mention is not automatically the formal origin of
    an entity.

### 4.4 Logical Entity Registry

Maintain one authoritative registry for the whole system. Each record
should contain:

  -----------------------------------------------------------------------
  Field                               Content
  ----------------------------------- -----------------------------------
  Entity ID                           Permanent ID, e.g. `AX-001`.

  Type                                One of the approved entity classes.

  Name / short label                  Concise recognizable title.

  Formal statement                    Approved formulation, where
                                      applicable.

  Origin                              Structural ID of first formal
                                      introduction.

  Canonical location                  Location of authoritative
                                      formulation, if different.

  Status                              Proposed, provisional, active,
                                      revised, superseded, or withdrawn.

  Depends on                          Entity IDs on which it logically
                                      depends.

  Referenced in                       All structural IDs where it is used
                                      or discussed.

  Notes / history                     Qualifications and revision
                                      history.
  -----------------------------------------------------------------------

**Origin** and **Canonical location** may differ. An idea may first
appear provisionally and receive its authoritative formulation later.

### 4.5 Relations between entities and locations

Where relevant, classify each occurrence:

-   **Introduction** --- first formal introduction.
-   **Definition** --- authoritative formulation.
-   **Reference** --- mention or recall.
-   **Premise** --- used as a premise in reasoning.
-   **Derivation** --- derived or used in a derivation.
-   **Application** --- applied to another problem or domain.
-   **Proof** --- used in a proof.
-   **Criticism** --- examined or challenged.
-   **Revision** --- formulation or status revised.

Example:

  Entity ID   Relation       Structural location
  ----------- -------------- --------------------------------
  `AX-001`    Introduction   `VS.B01.P01.C02.S01.SS01.P003`
  `AX-001`    Premise        `VS.B01.P03.C04.S02.SS01.P006`
  `AX-001`    Application    `VS.B02.P01.C03.S01.SS02.P002`

This distinction prevents a passing mention from being confused with a
substantive logical use.

### 4.6 Dependencies

Record a dependency only when the actual reasoning supports it or the
author explicitly approves it. Do not infer a dependency merely because
two entities occur in the same paragraph.

For each dependency, record the dependent entity, the entity on which it
depends, the type of dependency if known, and the structural location
where the dependency is established or used.

------------------------------------------------------------------------

## 5. Entity-to-location maps

At the end of each book, include a **Book-Level Logical Entity Reference
Map**. Maintain a **System-Level Master Logical Entity Map** covering
every book.

Recommended columns:

  -------------------------------------------------------------------------
  Entity ID   Type        Short label Origin /    Other       Relation(s)
                                      canonical   locations   
                                      location    in this     
                                                  book        
  ----------- ----------- ----------- ----------- ----------- -------------

  -------------------------------------------------------------------------

The book-level map includes every formal entity introduced, used, or
substantively discussed in that book. If an entity originates elsewhere,
retain its original ID and origin.

The system-level map is authoritative. A book-level map is a
book-specific view of the master registry, not a competing registry.
Reconcile discrepancies against the approved manuscript and master
registry.

Before a book is complete, verify that: 1. every formally identified
entity has a registry record; 2. every entity used in the book appears
in its book-level map; 3. every listed location actually contains the
stated relation; 4. every structural reference resolves; 5. dependencies
are supported; and 6. superseded formulations are distinguished from
current formulations.

------------------------------------------------------------------------

## 6. Bibliographic and external source protocol

### 6.1 Do not assign source IDs

External books, articles, editions, manuscripts, and other sources must
**not** receive identifiers such as `ARIST-001`, `SRC-001`, or any
equivalent source ID.

Identify a source through ordinary bibliographic information: author,
title, editor or translator, edition, publication details, and other
standard data.

### 6.2 Internal citation locations

Every bibliographic entry must be associated with the structural
location or locations in the Viability Philosophy books where it is
cited.

Example:

``` text
Aristotle.
Metaphysics.
Translated by W. D. Ross.
Oxford: Clarendon Press.

Cited at:
- VS.B01.P01.C01.S02.SS01.P004
- VS.B01.P01.C05.S01.SS02.P003
- VS.B02.P02.C03.S01.SS01.P006
```

These structural IDs identify the paragraphs in the Viability Philosophy
books that cite the source. They do not replace the precise locator
within the external work.

### 6.3 Exact external locators

Citations must identify the relevant location within the external source
as precisely as possible. Depending on the source, this may be a page
range, book and chapter, section, proposition, theorem, scholium, Bekker
or Stephanus number, volume and page, line numbers, or another stable
scholarly locator.

Example:

``` text
Aristotle, Metaphysics, Γ.3, 1005a19–21.
```

Do not invent page numbers, editions, translators, or passage
references. If a locator cannot be verified, mark it for checking.

### 6.4 Part-level and system-level bibliographies

A book may organize bibliographies by part or chapter. Nevertheless:

1.  each entry must contain complete ordinary bibliographic information;
2.  its system-wide `Cited at` list must preserve all relevant internal
    citation locations across all books;
3.  repeated appearances of one work in part-level bibliographies must
    not be treated as different sources;
4.  the system-level master bibliography should consolidate each work
    into one ordinary entry with all known internal citation locations;
    and
5.  no source-specific ID may be introduced.

A part-level bibliography may display only the locations relevant to
that part for readability, provided the master bibliography preserves
the complete list.

### 6.5 Bibliographic register fields

Track: full bibliographic entry, edition or translation used, exact
external locator(s), internal structural IDs under `Cited at`,
verification status, and notes.

The bibliography is a register of ordinary bibliographic entries and
citation locations. It is not an identifier system for sources.

------------------------------------------------------------------------

## 7. Expository architecture: main text, technical reconstruction, comparison

### 7.1 Main exposition

The main text must remain intelligible and genuinely argumentative. It
is not merely an informal introduction to reasoning hidden in a
technical appendix.

It must provide enough reasoning for readers to understand: - what is
claimed; - what the central terms mean; - why the claim is advanced; -
which distinctions and assumptions it requires; - how the conclusion
follows at the level appropriate to the chapter; and - what limitations
or unresolved issues remain.

Do not remove all justification from the main text in the name of
technical cleanliness.

### 7.2 Technical reconstruction chapters

Where appropriate, a part may end with a dedicated chapter titled or
functioning as **Principles, Arguments, and Formal Reconstruction**.

It gathers technical material that would otherwise interrupt the main
exposition, while leaving sufficient reasoning in the main text.

It may include: - formal statements of axioms and definitions; -
numbered propositions and theorems; - explicit premises and inferential
steps; - detailed argument reconstructions; - symbolic or mathematical
formulations; - proof structures; - dependency relations; - technical
qualifications; and - formal objections and responses.

It must not introduce a different doctrine from the main text. It
reconstructs or formalizes material already established or explicitly
proposed. If formalization exposes ambiguity, inconsistency, or a
missing premise, report it rather than concealing it.

Distinguish clearly between: 1. what the main text explicitly asserts;
2. what follows from those assertions; 3. what the reconstruction
assumes for analysis; and 4. what remains unproved or unresolved.

### 7.3 Comparative studies

Where appropriate, a part may end with a chapter titled or functioning
as **Comparative Ontological Studies**.

Comparison must be substantive, not decorative. Do not include a
philosopher merely because similar vocabulary appears.

A sound comparison identifies: 1. the specific problem being compared;
2. the historical model's relevant assumptions; 3. its account of the
relevant concept or relation; 4. the corresponding account in Viability
Philosophy; 5. genuine similarities; 6. decisive differences; 7.
explanatory advantages and limitations; and 8. what the comparison does
and does not establish.

Do not attribute a position to a historical thinker without reliable
textual support. Distinguish the thinker's own claims from later
interpretations. Similarity does not establish historical influence.

### 7.4 Relationship between the modes

  -----------------------------------------------------------------------
  Mode                    Purpose                 Typical location
  ----------------------- ----------------------- -----------------------
  Main exposition         Develop concepts and    Main chapters of each
                          arguments in a          part.
                          readable, continuous    
                          form.                   

  Technical               Make logical and formal Dedicated chapter near
  reconstruction          structure inspectable   the end of a part,
                          in detail.              where appropriate.

  Comparative study       Compare the account     Dedicated chapter near
                          with relevant           the end of a part,
                          historical models.      where appropriate.
  -----------------------------------------------------------------------

These modes complement one another. None should contradict or replace
the others.

------------------------------------------------------------------------

## 8. Specific architecture of *Ontology of Viability*

This section records the currently approved high-level architecture of
*Ontology of Viability*. It must not automatically be imposed on other
books. The exact chapter count, chapter titles, and placement of
supplementary material remain subject to the author's approved detailed
outline.

The main body has four core parts, in this order:

1.  **IDENTITY AND MANIFESTATION**
2.  **THE REALMS OF BEING**
3.  **LIGHT**
4.  **THE DYNAMICS OF BEING**

### 8.1 Part I --- Identity and Manifestation

This part is definitional and conceptual. It establishes what identity
is, what manifestation is, and how they are understood ontologically.

It may clarify, where supported by approved material: - the ontological
status and nature of identity; - the ontological status and nature of
manifestation; - their foundational conceptual relation; - invariance
and what remains identical; - unity and plurality; and - conditions and
domains relevant to manifestation.

**Boundary:** Do not develop relational dynamics, interaction among
components, rules of manifestation, or detailed mechanisms of expression
here. Those belong to the part on the dynamics of being unless the
author revises the architecture.

### 8.2 Part II --- The Realms of Being

This part explains the realms individually and then their integrated
architecture.

The framework distinguishes four fundamental realms:

1.  **First Determination**
2.  **Structural Determination**
3.  **Relational Manifestation**
4.  **Material Manifestation**

It also distinguishes three mediating or *barzakhic* realms:

1.  **Hub of Decree**
2.  **Hub of Signification**
3.  **Hub of Realization**

**Boundary:** Do not present all seven as equivalent items in one
undifferentiated ladder. The four fundamental realms and three barzakhic
realms have different ontological statuses. Explain each realm
individually before presenting the integrated architecture.

The exact status and placement of the **Transcendent Ground** and the
**Throne-Domain** remain open unless explicitly settled in
author-approved material. Do not automatically classify either as one of
the seven realms or as an additional realm.

### 8.3 Part III --- Light

Light is an independent and central part. Begin by establishing its
ontological status and nature. Do not reduce it in advance to an
instrument, mechanism, metaphor, or secondary feature of manifestation.

Maintain a distinction between: - **ontological light**, insofar as the
approved theory gives it an ontological role; and - **epistemic light or
legibility**, concerning knowability, intelligibility, or access.

Do not collapse these senses. Draw precise claims about light from the
author's approved philosophical material.

### 8.4 Part IV --- The Dynamics of Being

This part addresses relations, processes, rules, and dynamics that
should not be introduced prematurely into the definitional part.

Depending on the approved outline, relevant subjects may include: - the
dynamic structure of being; - necessity and rules of expression; - rules
and dynamics of manifestation; - relations and ontological networks; -
causation, law, and possibility; - energy; - time, eternity, and
becoming; - birth and death; - awareness, self-awareness, and mind
considered ontologically; - action and agency; - the cost of expression
or manifestation; - residue and sedimentation; and - reversibility.

This is a scope guide, not a claim that every topic is already
established or must become a separate chapter. Confirm status and
placement against approved material.

### 8.5 Optional integrative part

A further part, provisionally titled **INTEGRATION OF ONTOLOGICAL
PRINCIPLES**, has been considered as a possible place for system-wide
coherence, unity, recursive or holographic structures, limits, open
problems, and conclusions.

This is **not a finalized or mandatory part**. Do not add it without
explicit author approval.

------------------------------------------------------------------------

## 9. Philosophical status and uncertainty

Preserve the status of every substantive claim. Distinguish, as
appropriate:

-   **Established commitment:** explicitly adopted by the author.
-   **Definition:** an approved specification of a term.
-   **Derived result:** a conclusion supported by identified premises
    and reasoning.
-   **Proposition:** a claim advanced for examination or demonstration.
-   **Theorem:** a result accompanied by an appropriate proof.
-   **Hypothesis:** a provisional claim that remains open.
-   **Interpretation:** an explanation of a passage or argument.
-   **Proposal:** a possible development not yet approved as doctrine.
-   **Open problem:** a question not yet resolved.
-   **Editorial suggestion:** a proposed presentation or organizational
    improvement, not a philosophical claim.

Do not present a claim as more certain, foundational, or fully
demonstrated than its source warrants.

Preserve qualifications such as *possibly*, *in this sense*, *under
these conditions*, *at this level*, *not necessarily*, and
*provisionally* when they carry philosophical weight.

If a later book refines or challenges an earlier claim, do not silently
rewrite the earlier book to create an appearance of seamless
consistency. Record the development, identify the relevant locations,
and obtain the author's decision about whether either text should be
revised.

------------------------------------------------------------------------

## 10. Writing and editing standards

### 10.1 Prose

Write clear, precise, academically credible prose. The writing should be
accessible to an informed intermediate reader while remaining rigorous
enough for advanced readers.

-   Define specialized terms before relying heavily on them.
-   Use one term consistently for one concept unless a distinction is
    explained.
-   Avoid introducing many technical terms in one paragraph without
    need.
-   Prefer explicit reasoning to rhetorical emphasis.
-   Avoid ornamental repetition and inflated claims.
-   Use examples to clarify, not replace, an argument.
-   Make transitions explain logical relations, not merely announce
    topics.
-   Distinguish metaphor from literal ontological claims.
-   Do not present an analogy or diagram as proof.

### 10.2 Paragraph discipline

Each paragraph should normally have one primary function. When editing,
ask: 1. What is the paragraph's principal claim or function? 2. Does it
depend on terms already defined? 3. Does it introduce a new entity that
should be registered? 4. Is its reasoning adequate for the main
exposition? 5. Does it repeat material without adding a function? 6. Are
the author's qualifications preserved? 7. Are citations and
cross-references accurate?

### 10.3 Headings and hierarchy

Headings must describe the actual content. Do not promise a proof where
only an intuition is offered, or a complete theory where the discussion
is exploratory.

Use heading levels consistently with the canonical hierarchy. Do not
skip levels for visual convenience.

### 10.4 Terminology

Maintain a system-wide glossary or terminology register where needed.
For each important technical term, record: - preferred form; - approved
definition or description; - relevant `DF-` identifier, if formally
defined; - variants or translations; - terms that must not be treated as
synonyms; and - relevant structural locations.

Do not replace a deliberate authorial distinction with a more familiar
term from another tradition.

### 10.5 Figures, tables, and notation

Every figure, table, and formal expression must have a clear purpose and
be explained in the surrounding text.

-   Define symbols before or at first substantive use.
-   Keep notation consistent across books.
-   Do not let a diagram imply a hierarchy, equivalence, direction, or
    causal relation that the text has not established.
-   State the limits of a diagram when it simplifies a more complex
    structure.

------------------------------------------------------------------------

## 11. Procedure for revising an existing file

Follow this workflow whenever a file is revised.

### Step 1 --- Identify the exact source

Confirm the exact file and version. Similarly titled files may differ.
Do not assume that the newest-looking file is authoritative.

### Step 2 --- Inspect the relevant context

Read enough of the file to understand its structure, terminology,
claims, references, and dependencies. If the correction affects other
chapters or registries, inspect those materials too. Do not revise from
an isolated excerpt when the issue depends on the larger argument.

### Step 3 --- Diagnose the defect

Classify the problem, for example: - structural inconsistency; -
conceptual ambiguity; - contradiction; - missing definition; -
unsupported inference; - misplaced content; - repetition; - terminology
inconsistency; - incorrect logical status; - faulty cross-reference; -
bibliographic error; - inadequate explanation; or - formalization
problem.

State what is wrong and why it matters, unless the author has requested
direct editing without a preliminary report.

### Step 4 --- Determine scope

Identify affected paragraphs, sections, chapters, maps, registries, and
files. Avoid unrelated stylistic changes. Explain any necessary broader
change.

### Step 5 --- Preserve valid content

Retain established claims, distinctions, examples, terminology, and
qualifications unless they are part of the defect or the author
instructs otherwise. Do not remove substantive material merely to make
the file shorter.

### Step 6 --- Rewrite completely when requested

If the author requests a complete rewritten file, return the entire
revised file, not only replacement paragraphs or a list of suggestions.
The result must be internally coherent and ready to replace the previous
version.

### Step 7 --- Update identifiers and references

If structural locations or logical entities change, update: - the
Structural Identifier Registry; - the Logical Entity Registry; -
book-level and system-level maps; - affected internal
cross-references; - bibliographic citation-location lists; and -
identifier history.

Do not knowingly leave broken references.

### Step 8 --- Report unresolved matters

List philosophical issues, missing sources, uncertain attributions, or
unresolved dependencies that cannot be settled from approved material.
Do not conceal uncertainty by writing around it.

### Step 9 --- Final consistency check

Check architecture, terminology, philosophical status, structural IDs,
logical IDs, internal references, external citations, consistency
between exposition and technical reconstruction, and cross-book
implications.

------------------------------------------------------------------------

## 12. Procedure for creating new content

Before drafting a new unit:

1.  Identify its book and intended structural location.
2.  Confirm that the subject belongs at that level of the architecture.
3.  Review relevant existing material to avoid duplication or
    contradiction.
4.  Identify terms that require definition.
5.  Check whether claims already exist in the logical entity registry.
6.  Reuse existing logical entity IDs when referring to existing
    entities.
7.  Register genuinely new entities only when formally introduced and
    their status is clear.
8.  Assign structural IDs according to the global hierarchy.
9.  Add justified cross-references and dependencies.
10. Add external citations with precise source locators.
11. Update relevant book-level and system-level maps.
12. Mark unresolved decisions instead of silently deciding them.

A new file must not establish a parallel terminology, numbering scheme,
bibliography, or logical registry that conflicts with the system-wide
apparatus.

------------------------------------------------------------------------

## 13. Required registers and supporting documents

Maintain one clearly designated canonical version of each register.
Registers may be separate files or parts of a structured database.

### 13.1 Structural Identifier Registry

Tracks all books and structural units, their current IDs, headings,
status, and identifier history.

### 13.2 Logical Entity Registry

Tracks all axioms, definitions, propositions, theorems, hypotheses,
arguments, and proofs across all books.

### 13.3 Entity-to-Location and Dependency Map

Tracks where each entity is introduced, defined, referenced, used,
derived, proved, applied, criticized, or revised, and records supported
dependencies. This may be implemented within the Logical Entity
Registry, but the information must remain explicitly available.

### 13.4 Bibliographic Reference Register

Tracks ordinary bibliographic entries, exact external locators, internal
structural citation locations, and verification status. It must not
assign source-specific IDs.

### 13.5 Terminology Register

Tracks preferred technical terms, definitions, variants, translations,
and distinctions that must be preserved.

### 13.6 Change Log

Records significant changes to architecture, structural identifiers,
logical entities, terminology, and cross-book relations. Each entry
should include date, affected item, nature of change, reason, and author
approval status.

------------------------------------------------------------------------

## 14. Quality-control checklist

Use this checklist before approving a new or revised file.

### Structural integrity

-   [ ] The file belongs to the correct book and location.
-   [ ] Its function is clear at the assigned hierarchy level.
-   [ ] It follows the approved architecture.
-   [ ] Structural IDs are valid and unique.
-   [ ] No obsolete ID has been silently reused.

### Philosophical integrity

-   [ ] Authorial claims and distinctions are preserved.
-   [ ] Established commitments are distinguished from hypotheses and
    proposals.
-   [ ] No unsupported doctrine has been introduced.
-   [ ] Definitions are stable and consistently used.
-   [ ] Inferences are not presented as explicit premises.
-   [ ] Open problems remain open.

### Logical integrity

-   [ ] Formal entities have the correct type and ID.
-   [ ] Existing entities reuse their global IDs.
-   [ ] New entities are registered.
-   [ ] Premises and dependencies are accurately represented.
-   [ ] Proofs support the results they claim to establish.
-   [ ] Main exposition and technical reconstruction are consistent.

### Reference integrity

-   [ ] Internal references resolve to existing structural IDs.
-   [ ] Entity-to-location maps are updated.
-   [ ] Bibliographic details are accurate.
-   [ ] External citations include precise locators where available.
-   [ ] Internal citation locations are recorded.
-   [ ] No source-specific identifier has been created.

### Editorial integrity

-   [ ] Prose is clear and precise.
-   [ ] Paragraphs have identifiable functions.
-   [ ] Headings accurately describe content.
-   [ ] Repetition has been removed only when genuinely redundant.
-   [ ] Examples and diagrams do not overstate the argument.
-   [ ] The complete revised file is supplied when requested.

------------------------------------------------------------------------

## 15. Ambiguity and escalation

Ask the author when a decision materially affects philosophical content
or system architecture and cannot be resolved from approved sources.

Examples: - uncertainty whether a claim is an axiom, proposition, or
hypothesis; - uncertainty about the ontological status of a realm or
domain; - conflict between author-approved formulations; - uncertainty
whether two concepts are identical, included, or distinct; - a proposed
change to the four-part architecture of *Ontology of Viability*; - a
proposed new logical entity class or prefix; - uncertainty about the
accuracy of a historical attribution; - a structural change affecting
many references; or - a proof that appears to require an unstated
premise.

A clarification request must state: 1. the exact issue; 2. relevant
structural or entity IDs; 3. competing interpretations; 4. why the
choice matters; and 5. the decision required.

Ask a precise question rather than a broad one.

------------------------------------------------------------------------

## 16. Core operating principles

1.  **One system, multiple books:** books are distinct but connected.
2.  **One global structural hierarchy:** structural IDs locate content
    across the system.
3.  **One global logical entity system:** formal entities retain their
    IDs across books.
4.  **Location and identity are different:** structural IDs identify
    where; logical IDs identify what.
5.  **No source IDs:** external works use ordinary bibliographic data
    and internal citation locations.
6.  **Traceability:** formal entities, structural changes, dependencies,
    and citations must be traceable.
7.  **No silent invention:** inference, interpretation, and suggestion
    must not become doctrine without approval.
8.  **Preserve distinctions:** authorial conceptual and ontological
    distinctions must remain explicit and stable.
9.  **Readable rigor:** the main exposition must be understandable and
    reasoned; technical detail may be concentrated without emptying the
    main text of argument.
10. **Substantive comparison:** historical comparisons must be accurate,
    relevant, and analytically meaningful.
11. **Cross-book consistency:** changes in one book must be checked
    against their implications elsewhere.
12. **Authorial authority:** unresolved philosophical and architectural
    decisions belong to the author.

------------------------------------------------------------------------

## Appendix A. Identifier examples

### A.1 Structural locations

``` text
VS.B01
VS.B01.P01
VS.B01.P01.C01
VS.B01.P01.C01.S01
VS.B01.P01.C01.S01.SS01
VS.B01.P01.C01.S01.SS01.P001
```

### A.2 Logical entities

``` text
AX-001
DF-001
PR-001
TH-001
HY-001
AR-001
PF-001
```

### A.3 Cross-book use

An axiom first introduced in Book 01 retains its ID when used in Book
02:

``` text
Entity: AX-001

Origin:
VS.B01.P01.C02.S01.SS01.P003

Referenced in:
VS.B01.P03.C04.S02.SS01.P006
VS.B02.P01.C03.S01.SS02.P002
VS.B02.P04.C02.S03.SS01.P008
```

### A.4 Bibliographic entry

``` text
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

The bibliographic entry has no source ID. Internal structural IDs
identify where the source is cited; external locators identify the
passages in the external work.

------------------------------------------------------------------------

## Appendix B. Minimum record templates

### B.1 Structural unit record

``` text
Current ID:
Unit type:
Book:
Parent unit:
Title / description:
Status:
Previous ID(s):
Change note:
```

### B.2 Logical entity record

``` text
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

### B.3 Bibliographic record

``` text
Full bibliographic entry:
Edition / translation used:
External source locations cited:
Internal structural locations (Cited at):
Verification status:
Notes:
```

### B.4 Change-log record

``` text
Date:
Affected item(s):
Previous state:
New state:
Reason:
Affected references / registers:
Author approval:
```

------------------------------------------------------------------------

**End of Protocol**
