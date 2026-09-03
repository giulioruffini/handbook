# How to Write a Good Paper — K & Kaiti House Style

Version 1.0 · distilled from the WP0007 revision process and related theorem-driven manuscript
work. This is the **normative house style for all future BCOM/KT papers**. Agents (Claude Code,
Codex, Kaiti) follow it when drafting or revising any manuscript; the human-readable rendering is
`how_to_write_a_good_paper.html` beside this file. Prose-level rules (register, banned words,
self-grading) are separate and live in `~/.claude/skills/landau/references/landau-style.md`; this
document governs argument architecture and revision discipline.

---

## 1. The governing principle

> A paper is not a container for correct results. It is a guided reconstruction of why the results
> matter, how they fit together, and what they do — and do not — establish.

The central editorial mistake in technical writing is to confuse *having the right ingredients*
with *having the right argument*. A manuscript may contain correct theorems, relevant literature,
useful examples, and careful caveats and still read badly if the reader cannot see the dependency
structure.

**House rule:** preserve the intellectual story first. Cut duplication, not meaning. Move
machinery, not interpretation, to the Appendix.

For theorem-driven interdisciplinary work, the target is a paper that a specialist finds rigorous
and a scientifically literate non-specialist can still follow at the level of the argument.

## 2. Architecture before prose

Do not begin a serious revision by polishing sentences. First reconstruct the paper as a sequence
of intellectual moves. For each section, write one sentence answering:

- **What question is this section answering?**
- **Why does that question arise here?**
- **What changes in the reader's understanding after this section?**
- **Why must the next section follow?**

If two sections answer the same question, either merge them or distinguish their roles. If a
section cannot be summarized by a unique function, it is usually where narrative drift or
repetition has entered.

### A useful canonical arc

| Stage | Function | Typical content |
|---|---|---|
| 1. Problem | Establish the conceptual gap | Why the obvious formulation is insufficient; what is actually unknown |
| 2. Formal setup | Define only what is needed | Observer, model class, objective, assumptions, notation |
| 3. Core negative/positive results | Answer the central technical questions | Theorems, propositions, corollaries |
| 4. Interpretation | Translate mathematics into scientific meaning | What the result says, does not say, and why it matters |
| 5. Constructive/favorable cases | Explain how science can nevertheless succeed | Symmetry, constraints, examples, restricted classes, empirical search |
| 6. Discussion | Reopen the broader intellectual landscape | Related frameworks, limitations, ontology, implications |

**Warning:** do not let the Introduction reproduce this entire arc in miniature. Preview the
argument once; let the paper itself deliver it.

## 3. Writing the Introduction

A strong Introduction makes one clean pass through the problem. It should not repeatedly announce
the same results in different language.

### Recommended structure

1. **Start with the conceptual problem.** State the scientific or mathematical tension in ordinary language.
2. **Identify the crucial distinction.** For WP0007 this was generation vs construction: knowing how a system evolves is not the same as knowing how to construct its useful macroscopic description.
3. **Pose the paper's questions.** Prefer a small number of explicit questions over several paragraphs of diffuse motivation.
4. **Give one compact results paragraph.** State what is proved, with the hierarchy of claims correct.
5. **Introduce the positive scientific notion.** Explain what success would look like, not only what is impossible.
6. **Give only the background machinery needed to read the paper.**
7. **Position against prior work compactly.** Detailed comparisons belong later.
8. **End with a short roadmap.**

### What to avoid

- Problem statement → Q1/Q2/Q3 → theorem preview → barrier taxonomy → post-figure recap. That is four passes over the same material.
- Defining the same object informally, formally, and historically before the reader has used it.
- A miniature Discussion in the Introduction.
- Technical caveats that matter only after the theorem has been understood.

**Good test:** every paragraph in the Introduction should have a distinct job. If two adjacent
paragraphs can be summarized by the same sentence, combine or cut.

## 4. Results and theorem exposition

The most effective local pattern:

> Question → theorem → proof or proof sketch → interpretation → limitation.

1. **State the question before the theorem.** A bare theorem dropped into the text forces the reader to reverse-engineer its purpose.
2. **Make the quantifiers readable.** Prefer formulations that expose the operational content: "find a shortening whenever one exists" is clearer than "discover every shortening."
3. **Interpret every central theorem.** After the proof, explain in plain language: what it establishes; why that matters scientifically; what assumptions do the work; what it *does not* establish. Essential in interdisciplinary papers — a reader may understand the formal statement and still misread its scientific scope.
4. **Preserve the hierarchy of claims.** Do not lead with a technically weaker but more fashionable consequence.
5. **Distinguish theorem from interpretation.** Do not smuggle the scientific conclusion into the definition. Prove the clean mathematical result first; state the regulatory, physical, cognitive, or epistemological reading as interpretation or corollary.

## 5. Proof placement: main text vs Appendix

The main text preserves the *reasoning* required to understand the result. The Appendix absorbs
technical machinery necessary for rigor but not for conceptual flow.

**Keep the full proof in the main text when:** the proof contains the central conceptual idea; the
construction itself is scientifically informative; the proof is short enough that moving it would
make the theorem feel unmotivated; or later arguments depend on the proof mechanism.

**Move the detailed proof to the Appendix when:** the main-text reader already understands the
reduction; most of the proof tracks coding constants, technical cases, or auxiliary translations;
the same machinery is already developed in an Appendix construction; or a short sketch communicates
the decisive idea accurately.

**The Proposition 1 pattern (WP0007):** the proposition stayed in the main text with a concise
sketch of the two reductions; the full proof moved next to the repeat-x machinery in the Appendix,
where the fixed-overhead program↔compressor translations are actually constructed. This avoids
explaining the same machinery twice.

**Principle:** main text = argument and proof idea; Appendix = coding constants, diagonal
mechanics, auxiliary reductions, and constructions already supported by technical lemmas. Do not
move all proofs reflexively — a paper with "proof in Appendix" after every result often becomes
harder to read.

## 6. Context, examples, and prior work

Context is not decoration. In a theoretical scientific paper it often carries the bridge from
formal result to scientific relevance.

**Keep context when it:** shows how a formal barrier manifests in real scientific practice;
explains favorable cases where additional structure helps; distinguishes the present claim from a
nearby literature; gives a concrete example that prevents an overly strong interpretation; or shows
how microscopic information remains useful through symmetry, conservation, scale separation, or
collective variables.

**Do not cut a section merely because it is "not a theorem section."** The right question is not
"does this prove something new?" but "does this advance the reader's understanding?"

**Use examples economically.** One example can establish intuition; three should establish a
pattern. If five examples make the same point, choose the most complementary set.

## 7. Writing the Discussion

The Discussion should **revisit** the story, not **repeat** the paper. Its job is to change level:
the Results establish what follows under explicit assumptions; the Discussion asks what that means
in the wider conceptual landscape — separating senses a main argument might conflate, comparing to
existing literatures, explaining restricted classes, clarifying epistemological vs ontological
scope, identifying how real science bypasses universal impossibility.

**Warning:** do not compress the Discussion simply because some concepts appeared earlier.
Repetition is bad only when the intellectual function is the same. Revisiting a theorem at a new
explanatory level is not redundant.

**Discussion test:** for every paragraph, ask "what new level of interpretation does this add
beyond the theorem and its immediate reading?" If the answer is "none," shorten or remove it.

## 8. Notation, definitions, and quantifiers

1. **Define before use.** Every technical symbol or term is defined immediately before or at first use; an informal term used early gets a plain-language gloss ("additive error — or regret — relative to the shortest description").
2. **Maintain a notation table** in the Appendix for notation-heavy papers — a recovery aid, not a substitute for local definitions.
3. **Separate assumptions from conclusions.** Make clear whether a restriction is part of the theorem, a modeling convention, an observer choice, a physical assumption, or an interpretation.
4. **Qualify universality carefully.** "Blocked in general," "no universal constructor," "under the stated model class" — never turn a universal impossibility result into the claim that useful construction is impossible in particular systems.

## 9. Lean / formal verification claims

Formal verification language must be narrower than casual prose. Never write "all proofs are Lean
checked" unless literally every relevant proof and auxiliary assumption is mechanized at the same
level.

**Preferred formulations:** "The core reductions are machine-checked in Lean 4." / "The barrier
results and their supporting reductions are formalized in Lean 4." / "Proposition X has a
Lean-checked counterpart under explicit translation/overhead hypotheses."

**State the boundary explicitly.** If the concrete coding construction is paper-level while Lean
proves the abstract reduction, say so. If classical AIT facts are imported as named
assumptions/interfaces rather than reproved, say so. If an auxiliary statement is not formalized,
do not imply otherwise.

**Formalization principle:** distinguish "the mathematical dependency is machine checked" from
"the prose proof is replayed line-by-line in Lean."

*(Operationally at BCOM: every stated result carries a `% ktait:` annotation naming its KTAIT
declaration or `none -- <reason>`; `check_sync.sh` in the KTAIT repo enforces this, plus name
resolution, statement drift, and the released gate. Run `check_sync.sh --released` before any
paper goes public.)*

## 10. Controlling repetition without losing meaning

| Bad repetition | Useful recurrence |
|---|---|
| The same barrier listed in the Introduction, theorem preview, figure caption, post-figure recap, and Discussion with no change in function | A theorem stated formally, interpreted scientifically, and later revisited philosophically |
| Re-defining the same object several times before it is used | Reminding the reader of one key definition after many pages when needed for a new argument |
| Repeating technical machinery in both main text and Appendix | Main-text proof sketch plus full Appendix derivation |

**Deletion test.** Before cutting a passage, classify it: new fact → keep; new qualification →
usually keep; new example with a distinct role → keep; new interpretive level → keep; same claim,
same function, different wording → cut or merge. Do not optimize word count directly; optimize
duplication.

## 11. Revision workflow

- **Pass 1 — Architecture.** One-sentence purpose of every section; dependency chain; sections that preview later sections too fully; protect the core storyline before editing.
- **Pass 2 — Paragraph flow.** One job per paragraph; first sentence follows from the previous paragraph; last sentence motivates the next; remove duplicate-job paragraphs.
- **Pass 3 — Theorem exposition.** Question before theorem; quantifiers checked; proof placement checked; interpretation and "does not say" present.
- **Pass 4 — Fidelity pass.** Compare against the pre-revision manuscript. For every deletion, ask whether it removed a useful distinction, qualification, example, or reader aid. Restore conceptual payload even if it costs words.
- **Pass 5 — Length reduction** (only after the architecture is stable): move long technical proofs to the Appendix; collapse repeated literature positioning; reduce examples making identical points; shorten conclusions that restate the abstract; trim setup made obvious by later definitions.
- **Pass 6 — Formal and LaTeX integrity.** All notation defined; all references resolve; bib keys exist; theorem hierarchy correct; formalization claims match what is checked; PDF visually inspected. *(Also: byte-level check for control characters and a `pdftotext` spot-check of load-bearing formulas — a clean compile log is not evidence of a clean PDF.)*
- **Pass 7 — Redline.** Generate a redline against the original substantive draft, not merely the previous revision, to verify clarity was gained without silently losing good content.

**When to stop:** stop global editing when further shortening would begin to remove explanation,
scientific context, or interpretive structure rather than duplication. After that point, reopen the
architecture only in response to a specific reader confusion.

## 12. Submission checklist

- [ ] Can the paper's central problem be stated in two sentences without notation?
- [ ] Does the Introduction make only one pass through the main argument?
- [ ] Does every main section have a unique intellectual job?
- [ ] Are definitions introduced before or at first use?
- [ ] Are theorem quantifiers exactly what is intended?
- [ ] Is the hierarchy theorem → corollary → interpretation logically correct?
- [ ] Does every central theorem have a plain-language interpretation?
- [ ] Does each interpretation say what the theorem does *not* imply?
- [ ] Are long technical proofs in the Appendix when a short main-text sketch suffices?
- [ ] Is machinery explained only once?
- [ ] Are scientific examples complementary rather than repetitive?
- [ ] Does the Discussion change explanatory level rather than retell the Results?
- [ ] Are literature comparisons detailed where they matter and compact elsewhere?
- [ ] Are formal-verification claims scoped precisely?
- [ ] Has a fidelity pass been made against the earlier strong version?
- [ ] Has a redline been visually inspected?
- [ ] Has the PDF been compiled and checked for unresolved references and layout defects?
- [ ] Can one remove anything else without deleting meaning? If not, stop.

## 13. Reusable review prompt

For future papers, give the following to an editor or AI collaborator:

```
Revise this manuscript as a rigorous scientific editor, not merely a copy editor.

First reconstruct the paper's argument architecture section by section and paragraph by
paragraph. Do not edit until the architecture is clear.

Protect the intellectual storyline, scientific context, interpretation, and carefully developed
Discussion. Do not reduce the paper to bare results.

Check:
1. overall argument flow and section dependencies;
2. whether the Introduction makes one clean pass through the problem rather than previewing the
   paper repeatedly;
3. paragraph-to-paragraph transitions;
4. theorem hierarchy and quantifiers;
5. definitions before use;
6. theorem -> proof -> interpretation -> limitation structure;
7. whether long technical proofs should become short main-text sketches with full Appendix proofs;
8. duplication of technical machinery between main text and Appendix;
9. repetition versus legitimate revisiting at a new explanatory level;
10. whether examples are complementary;
11. whether prior-work comparisons are in the right place;
12. whether formal-verification claims match exactly what is machine checked;
13. LaTeX, citations, labels, references, and notation integrity.

After revising, perform a fidelity pass against the original strong version. For every deletion,
ask whether a useful distinction, qualification, example, or reader aid was lost. Restore
conceptual payload where needed.

Prefer shortening by removing duplicated function, not by removing meaning.

Finally provide:
- a clean revised manuscript;
- a redline against the original;
- a concise architecture/editorial memo;
- a list of any remaining referee vulnerabilities.

Stop global editing when further compression would start removing clarity, context, or
interpretation rather than redundancy.
```

## 14. The short version

> Architecture first. One job per paragraph. One pass through the Introduction. Theorem → proof →
> interpretation → limitation. Move machinery, not meaning, to the Appendix. Let the Discussion
> change level. Define before use. Quantify exactly. Verify formalization claims narrowly. Redline
> against the original. Stop before clarity becomes compression damage.
