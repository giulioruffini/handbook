# Lean Formalization Practice — KTAIT

How machine-checking is woven into the papers. The style rules for *claiming* formalization are in
`../writing/HOW_TO_WRITE_A_GOOD_PAPER.md` §9; this document is the operational practice behind
them, built around the **KTAIT** development (github.com/giulioruffini/KTAIT) and its status paper
**WP0195**, which carries the declaration-by-declaration inventory and the axiom audit.

## The standing rule

New propositions with AIT or computability content go into the KTAIT Lean 4 repo, **sorry-free**,
with a WP0195 inventory entry — without waiting to be asked. A result that cannot be stated in
Lean without inventing hypotheses does not go in the paper. Writing the *statement* is the test
even when the proof is deferred: Lean forces types (a symbol cannot denote a bounded program at
its definition and an unbounded runtime state at its use), explicit hypotheses (having to invent
one to make the statement well-formed *is* the finding), and direction (a prose biconditional
becomes two lemmas, and the converse is usually where the error hides).

## Style of formalization

- **Named hypotheses over re-proved classics.** Classical AIT facts (uncomputability of K,
  fixed-margin non-approximability) enter as named hypotheses — `KUncomputable`,
  `KNotApproximableOnSlackCompressible` — rather than being re-proved. The paper says so
  explicitly; the honesty is the point.
- **Analytic inputs as named hypotheses in the module's house style** (e.g. `LengthUnbounded`,
  `CompetitorBound`, `BoundOutrun`, `WitnessCompresses` for the relational optimality barrier), so
  a reader of the Lean statement sees exactly which counting or coding argument each part carries.
- **Abstract over the witness.** State reductions over any computable faithful embedding, not the
  particular expository witness, so the machine-checked result does not depend on the example
  chosen for the paper.
- **Relational forms when foundations are at stake.** Where a paper claims survival under a
  reading in which K is not available as a number, the Lean statement quantifies only over
  exhibited descriptions (no `min`, no global K-function).

## Wiring papers to Lean

Two LaTeX macros, one meaning each:

- `\lean{...}` — incidental Lean text: an identifier, a filename, a core axiom.
- `\ktait{decl}` — a machine-checked-claim citation: the prose asserts a result and names the
  KTAIT declaration that proves it. Declarations only; the guard rejects filenames and core
  axioms inside it.

Every theorem-like environment in a registered paper carries a **claim-coverage annotation**
directly above it:

```latex
% ktait: relational_optimality_barrier
\begin{Corollary}[Relational optimality barrier]\label{cor:relational-optimality}

% ktait: none -- classical Kolmogorov-Solomonoff-Chaitin, proved at paper level; enters the
%   development as the named hypothesis KUncomputable and is not re-proved
\begin{Theorem}[Kolmogorov, Solomonoff, Chaitin]\label{thm:uncomp}
```

`none` requires a reason; a bare `none` is rejected as an oversight. A `\ktait{}` in the body
counts by itself. Papers are registered in `docs/citing-papers.txt`.

## The guard: `scripts/check_sync.sh`

Seven checks, each born from a failure that actually happened:

1. **Sorry-free** — no proof gap behind a "machine-checked" claim.
2. **WP0195 coverage** — the status paper lists every module and non-helper theorem.
3. **Citing papers** — every `\lean{}`/`\ktait{}` name a registered paper cites resolves to a
   real declaration.
4. **Statement drift** — a declaration's statement must not change while the prose describing it
   stands still (fingerprint manifest).
5. **Named, not numbered** — prose in the repo names results; numbers belong where `\ref`
   maintains them.
6. **`--released`** — before a paper goes public: tree clean AND HEAD pushed. "Machine-checked"
   is a promise about GitHub, not a laptop.
7. **Claim coverage** — the only check that runs from the prose *back* to Lean: every stated
   result must carry a recorded formal status (`% ktait:` annotation validated against the
   development). Checks 1–6 walk from citations outward and are structurally blind to a new prose
   result with no Lean counterpart; this one exists because exactly that shipped once.

What no guard can do: judge whether a Lean statement *faithfully renders* the prose. That
judgment is human (or an adversarial review lens); the guard only forces the question to be
answered somewhere other than in someone's head.

## Discipline

- **Commit the Lean and the papers together.** Never ship a machine-checked claim that is not
  pushed.
- Run `check_sync.sh` after any Lean-adjacent change; run `check_sync.sh --released` before any
  paper goes public.
- When a paper's statement of a formalized result changes, re-read the Lean beside it — the guard
  checks names and fingerprints, not meaning. `#print axioms` on cited declarations catches an
  assumed conclusion hiding behind a hypothesis.
- Scope every prose claim exactly: "the core reductions are machine-checked" (with the concrete
  coding construction at paper level, if it is) — never "all proofs are Lean checked" unless that
  is literally true.
