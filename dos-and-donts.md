# Dos and don'ts

This records K's corrections to the way we collaborate. Read it before substantive work.
K's current instructions take precedence; keep scientific corrections tied to their stated scope.

## Working rules

- Treat requests for an opinion or scientific discussion as discussion. Edit the manuscript when
  K requests edits. Handbook and TODO maintenance remain authorized during discussion and do not
  require separate permission.
- Preserve figures, explanations, and structure that K values. Add a complementary diagram as
  another figure. Present a proposed replacement separately unless K has requested the replacement.
- Keep edits proportional to the request. A request for succinct edits calls for small, reviewable
  changes. Report substantive deletions and reorganizations explicitly, and provide a redline
  against the agreed baseline.
- Read the exact claim before criticizing it. Identify what is being compressed, what information
  is supplied, and which guarantee the theorem addresses. Do not substitute a different question.
- Preserve the intended scientific argument. When K corrects an interpretation, revise that
  interpretation before polishing the wording. Explain a disagreement with reasons.
- Make concise prose self-contained. Name the objects and guarantees; explain technical terms
  before relying on them, especially in an abstract.

## Recorded incidents

### 2026-09-30 — WP0216 observer-centric premise

K found that the proposed WP0216 abstract mentioned observational scale without
stating the premise that a pattern is a model in an observer, as developed with
WP0007. Keep that premise explicit in the abstract and opening argument; explain
the observer's model construction before persistence and causal support. Preserve
the distinction between the observer's pattern model, the physical organization
it tracks, and any model implemented by the observed agent. A retention map does
not compensate for removing this premise from the reader's main route.

### 2026-09-30 — WP0240 study coverage and device aliases

K asked whether the Flow study and other relevant evidence were missing. The pivotal Flow
trial was present under Woodham's author name, but the source index did not name the device.
A fresh audit found omitted home, personalized-tDCS, targeting, and 2026 pooled studies.
Index device and trial aliases alongside author-year citations. Cross-check the trial lists
in recent syntheses against primary reports, distinguish companion reports from independent
cohorts, and treat source-accuracy review and coverage review as separate tasks.

K then pointed out that the preprint PDF was still stale after the research notes were pushed.
When updating a preprint, incorporate the evidence into the manuscript and bibliography, rebuild
the named PDF, and verify the version in that artifact before reporting the repository current.
Keep audit-only notes and a completed manuscript revision distinct in status reports.

### 2026-09-29 — HMM objective choice and surrogate optimization

K questioned the reading note's opening comparison of success probability with expected
log-success: different objective functions are legitimate choices, so their disagreement
alone supplies no criticism. State the premise first: a method is being assessed as a
surrogate for an already specified objective. Distinguish choosing another objective from
failing to optimize the intended one; superiority is relative to the chosen criterion.
Keep this clarification under discussion before revising the note or referee report.

K then found the terminal Bellman explanation confusing and requested a correction.
Explain that beta measures success on the remaining time interval: its terminal value
is one because no future targets remain, not because the full episode has succeeded.
K also emphasized WP0028's posterior-approximation objective and AIF's usual pragmatic
and epistemic combination. Distinguish posterior inference from policy selection, name
the variable being optimized, and identify which evidence terms remain constant. Do not
equate action entropy with information gain or suggest that AIF has no OF.
I then made the distinction between posterior inference and policy selection sound
like a boundary of FE's validity. K questioned that framing. FE can also recover the
optimal policy when formulated for the intended control model with an exact auxiliary
posterior; assess the specified construction rather than FE-based action in general.
My subsequent reference to an "exact auxiliary posterior" left its role unexplained,
leading K to ask whether Moreno's FE setup was incorrect. Name the distinct problems:
the original policy-dependent model and the fixed-prior control-as-inference target.
Moreno explicitly acknowledges that substitution in Section 2.2; the exact variational
identity for the original model supplies no computational shortcut by itself.
K then asked what the surrogate's failure contributes unless its choice is natural or
canonical. Establish the method's literature basis and distinguish known results from
the paper's added comparison; differing objectives alone do not justify a broad FE/AIF
critique without showing that the compared method is meant to optimize the stated goal.
K then asked for the actual AIF policy-selection procedure; I had compared formulations
before explaining the procedure. Describe prediction under candidate plans, preferences
and information gain in G, policy weights, action selection, and belief updating. Keep
this expected-FE procedure distinct from Moreno's fixed success-posterior projection.
K clarified that AIF encodes desired states as priors. My distinction between beliefs
and preferences made goal priors sound external to the generative model. Confirm their
inclusion in the model first; distinguish their roles without denying that inclusion.
Assess any distortion of current-state inference from the particular construction.
K then pressed the hydration example: a desired-state prior used in current-state
inference raises the probability of that state without new evidence. Show the posterior
odds calculation before discussing safeguards. A future preference can also propagate
back through joint inference; temporal labeling alone does not prevent that influence.

K then asked for the motivation and equations connecting FE, VFE, EFE, and
homeostatic priors. My repeated distinction between VFE and EFE left the
reactive-control construction underexplained. Show how one VFE can drive
belief updating and physical action through different variables, then explain
what changes when scoring prospective policies with EFE. Use a continuous
worked example to connect the goal prior, prediction errors, and control;
do not equate VFE exclusively with modeling or EFE with the planner itself.

K approved the six referee comments and requested a reachability reference, the
direction of the surrogate's risk bias, and promotion of the safe-range correction
into the maximum-occupancy comment. Anchor an established-result objection to a
specific source and put a false technical motivation with the section it motivates.
Distinguish expected-log risk aversion from optimism under success conditioning.
Recompute the expected objective when changing a stopping convention; discarding
fatal-step rewards does not automatically make the surviving action scores equal.

### 2026-09-07 — WP0007 figures and revision scope

The revision replaced the original observer-chain Figure 2 and colored barrier Figure 4, removed
the associated modeling hierarchy, and substantially shortened the conclusion. K preferred the
original figures and asked what else had changed. In v0.31.4, the original Figure 2 and its
explanation returned; the acquisition/use diagram became an additional Figure 4, and the original
colored diagram returned as Figure 5 with local wording corrections. The conclusion shortening
was disclosed but was not reversed in that restoration. Preserve valued material and make the
full scope of a revision visible.

### 2026-09-07 — WP0007 lossless compression

The fair-coin-model objection missed K's point about Theorem 1: knowing the microlaws does not
guarantee a substantial lossless compression of the retained record after coarse-graining.
Distinguish a short description of a probability model from a lossless description of a realized
record; a statement about the former does not settle a theorem about the latter.
On September 27, I kept directing the worked-example discussion back to proven incompressibility
and the shift register. K corrected this: that example already serves the first theorem; the
other barriers concern finding a compressor and approaching optimality. Read the relevant
statement before choosing the example. The discovery and optimality theorems give the observer
the complete experiment, including its initial state. An illustrative failure to acquire a
macromodel need not prove the record incompressible. State what the attempted method fails to
find, and distinguish that finite outcome from the theorem's lack of a uniform guarantee.
I then presented compression by the known microscopic simulator as an additional caveat.
K corrected this too: microscopic compression is the starting point of the worked contrast.
Assess the acquisition of a useful macroscopic description relative to that incumbent;
do not keep resetting the discussion to whether simulation already provides a description.

### 2026-09-07 — WP0007 scientific discovery and generation

K rejected framing the cited accounts as motivating a distinction between generation and
compression. The opening should explain compression's driving role in scientific discovery and
cognition. Some encoded data can specify meaningful model parameters; the model and those
parameters generate particular realizations. Do not automatically classify all data given the
model as meaningless residual information.

### 2026-09-07 — WP0007 abstract clarity

K found “Every instance is finite; the obstruction is uniformity over unbounded families” cryptic.
The revision names finite records and explains that the limit concerns one algorithm providing
the guarantees for every finite record, however long. Brevity must preserve the explanation.

On September 27, K found the added abstract clause about a code for past data awkward and
questioned its value there. Remove that clause while retaining the explanation in the
Introduction; an important distinction need not interrupt the abstract's established opening.

### 2026-09-07 — WP0007 regularities and model length

K clarified that scientific discovery concerns usable regularities: a large, clunky model can
contain a component that supports generalization and prediction. Exploiting those regularities
can enable compression without the whole stored model already delivering a net saving on the
available data. Failure of a chosen compression method does not establish whether regularities
have been captured. Keep regularity acquisition, realized compression gains, and predictive
transfer distinct. Review Definition 2's net-savings requirement and the scope of claims about
scientific discovery when manuscript revision resumes; the definition has not yet been changed.

K then emphasized that a long predictor's compressive capability should still encounter the
paper's barriers. Develop the predictive-coding connection and check the corresponding reduction;
do not treat inefficient implementation as an escape from the intended obstruction. The transfer
has not yet been proved for the proposed predictive setting. The WP0007 handoff dated 2026-09-07
records the agreed direction and the assumptions still to establish.

On September 27, K asked the Introduction to explain why the paper focuses on compression:
a model that captures regularity supports compression through reuse, while a compressed
record alone need not expose a reusable parametrization. State both directions in the
motivation and connect the latter to the certificate’s fixed coordinate roles and reuse.

### 2026-09-07 — Discussion and note maintenance

During the regularity discussion, K objected to possible manuscript edits and then clarified
that handbook and TODO updates were welcome. No manuscript edits had been made. Preserve this
distinction: continue maintaining collaboration notes while keeping scientific discussion
separate from requests to revise the paper.

### 2026-09-07 — Imperfect cores and useful implementation costs

K clarified that a model's functional core is a shortest implementation of the same behavior,
including its imperfections. It need not be the best predictor or compressor among all models.
A larger equivalent implementation can be faster, for example by storing results that would
otherwise be recomputed. Do not classify all excess description length as useless code.
For telehomeostatic agents, models serve persistence through prediction, timely computation,
and effective action; shortest code length is not the objective. WP0007 v0.31.9 implements this
clarification and the earlier regularity discussion. The compression-certified transfer remains
scoped to its stated guarantees; a broader predictor-discovery theorem still requires a reduction.

### 2026-09-07 — Premature jargon and repeated conceptual updates

K found that recent WP0007 revisions again used technical terms before explaining them and gave
new qualifications too much prominence. Klaus identified repeated previews and repeated accounts
of amortization and telehomeostasis. Give each point an explanatory home; repeat it only when its
role changes. Keep the Abstract and Introduction readable without later definitions. Explain what
a technical restriction prevents beside the restriction. A clean build and a regex style check do
not substitute for reading the argument. WP0007 v0.31.10 applies this correction with redlines and
a fidelity review preserving the scientific distinctions, examples, proofs, and valued figures.

On September 26, K requested a full redlined candidate after the revision guide and asked what
the examples and concept table contribute. Keep new insertions economical; state each example's
purpose before its bit accounting. Organize the table by the questions behind weak emergence,
strong emergence, undecidability, and model acquisition, so it supplies context for the paper.
On September 27, K rejected the table phrase “closest to the answering question below” and
asked for a clearer structure. State the compared questions directly, and organize the
accounts by derivation, model structure, causal influence, and observer acquisition.
A compressed macromodel can itself support universal computation; acquisition need not
remove undecidability or a requirement for simulation. Specify the property and the
unbounded computation involved rather than treating these accounts as exclusive system types.
K then found the last column ambiguous: it mixed source definitions, our comparisons, and
negative qualifications. Keep the table to each account's defining question, and explain our
comparisons in prose. State the positive connections: compression is shared with effective
complexity, acquisition can deliver causal macromodels, and a macroscopic theory can make
prediction cheaper by replacing microscopic simulation with direct calculation or a smaller
simulation. Give the diagonalization passage an explicit conclusion about uniform guarantees,
then distinguish it from claims about necessary simulation or logical non-entailment.
K clarified that the intended unification is Lawvere's theorem as the common abstract basis
of the diagonal arguments. State that connection first, then identify what each argument
diagonalizes and which guarantee it excludes; retain the counting result as a separate case.
Do not replace the unifying claim with only a list of differences between the results.
On September 28, K asked where unboundedness enters and corrected our attribution of Bedau's
definition. Separate finite diagonal obstructions (including Wolpert's basic inference limits)
from computability barriers over unbounded families. Use an author's defined term when
attributing a criterion: Bedau defines a weakly emergent macrostate, allowing properties and
patterns of behavior within that term; our own discussion may still speak of behavior.
K then found that the Chalmers comparison stated only what undecidability does not imply.
State the positive connection first: truths may exceed the deductive reach of a specified
description. Explain which premises, proof rules, and notion of consequence are involved,
and separate this philosophical interpretation from a theorem or an attributed author position.
K also corrected an unsupported identification of the Berry-type proofs with Lawvere's theorem.
Shared diagonal structure is not a supplied formal reduction. Check which cases a cited source
actually treats; Yanofsky lists Berry among future directions. Say a reduction is absent here,
not that the problem remains globally open, unless the latter has been established.
K then supplied Li (2019), which treats a Berry construction in Lawvere’s framework.
Check later literature before inferring a present gap from an older paper’s future directions,
and distinguish a published formulation from a verified reduction of our own results.
K's subsequent literature check distinguished generalized fixed-point results from Lawvere's
original theorem and diagonal structure from quantitative description-length bounds. State
what the cited extension supplies, then identify the separate encoding estimate; do not infer
a literature-wide absence of reductions from the sources checked. Preserve the distinction
between no uniform constructor and no derivation for an individual instance when explaining
classical and constructive readings.
K subsequently supplied the exact-K/halting reductions, verified against Chaitin, Arslanov,
and Calude (1995) and Forster et al. (2022), Section 11. Distinguishing Berry proofs from
fixed-point presentations must not suggest unrelated sources of uncomputability: distinguish
Turing equivalence, quantitative encoding bounds, and a direct categorical formulation.
K then emphasized the valid implication from Lawvere's diagonal principle through halting
undecidability to the uncomputability of exact K. A derivation by reduction is a derivation;
do not require a direct categorical presentation before acknowledging this connection.
Lead with the established implication, then explain the additional description-length estimates.
K asked that Li and Bauer remain in the main text as evidence for the unifying comparison,
without a new Entropy footnote, and that preemptive qualifications be removed. Keep the
supporting routes visible and state their scope without answering hypothetical objections.
K's follow-up removed a third-party mirror URL from an otherwise complete journal citation
and reattached a two-sentence comparison left isolated by consolidation. Keep retrieval
mirrors in source notes; use publication metadata in the bibliography, and check paragraph
continuity after moving material.
K then approved numbering Section 8's three parts and clarifying its transitions, while
explicitly protecting the existing Section 8.1. Preserve that subsection byte for byte,
including its table and philosophical and diagonal arguments; renumbering and edits to
surrounding passages do not authorize a new prose pass on the protected text.
K then caught an unqualified “true in the standard natural numbers yet unprovable” sentence:
it silently assumed classical semantics while discussing the dispute over truth itself. State
that philosophical choice before the example, and label the classical reading explicitly.
Explain a proof interpretation as a meaning of truth, not merely a limit on access to a truth
already assumed; distinguish constructive proof from provability in one fixed formal system.
K subsequently required the Chalmers comparison to separate truth in an intended structure from
consequence of specified axioms. In classical first-order logic, consequence across all models
and provability coincide; Gödelian incompleteness does not separate them. Keep the WP0007
connection on microscopic determination versus uniform model construction, without treating
failure of a uniform procedure as absence of constructions in particular cases.
K’s philosophy reference was J. D. Hamkins, not Stephen Hawking; verify an uncertain author
name from the subject and bibliography before pursuing a guessed identification.
K then objected to the extensively rewritten abstract and said not to worry so much about
length. Preserve the submitted abstract's wording and sequence, making only the changes needed
for correctness; an earlier word-count target does not justify broad rewriting.
K also corrected a passive-observer contrast and a theorem reference inserted before the
result was introduced. A projection specifies retained distinctions, not whether the observer
acts; put the common proof-mechanism discussion after the results. Explain separately where
unboundedness lies in the observed-system family and in the observer's available memory.
K then found Section 5.3 still unreadable: it named a glider and added a register before
defining the experiment. Establish the state space, update rule, observation map, horizon,
and initial conditions first; explain a named pattern only after its system exists on the
page. Give the reader enough setup to reconstruct the example before presenting bit counts.
K then asked for a simpler account with the agent's objective stated explicitly and one
successful case alongside a failure. Start with the task the model serves; distinguish useful
prediction from the compression certificate. Prefer an analytic toy and a small complete ledger
when these explain the point; implementation byte counts and simulations should serve that
explanation rather than determine it.
On September 27, K chose to retain the glider visual and add the CA visual, with short,
objective-first explanations in Section 5.3 and both complete coding accounts in the appendix.
Do not frame these complementary examples as replacements for one another; preserve the
question each answers and distinguish a failed model search from the general discovery barrier.
K then objected that the shortened examples named Life and numbered rules before introducing
cellular automata. State the local update mechanism and explain Wolfram's numbering before
using a rule number; cite Gardner, Wolfram, and Israeli--Goldenfeld where their examples first
enter. Moving coding details to an appendix must not remove the main text's conceptual setup.
For code access, K prefers a dedicated public repository for each paper. Apply the
[BCOM companion policy](../BCOM-handbook/paper-companion-repos.md), adopted September 27:
its naming, licenses, release binding, and registration are standing decisions. A journal
supplementary ZIP is a fallback, not a second code home. Repository publication and minting
a release DOI are distinct actions; record which has actually occurred.
K also endorsed Klaus’s finding that the candidate had weakened the self-model clause and
removed the intelligibility/compression gloss. Restore valued claims and qualify them locally;
a reviewer’s request for distinctions does not authorize replacing the paper’s motivation.

On September 15, in the WP0216 program discussion, K objected to using APB before expanding
and explaining it, and to an abstract closing question about compact rules versus episode
records. Spell out Algorithmic Persistence Balance before using the acronym and explain its
reconstruction premise. State the intended scientific distinction with a concrete example;
do not introduce an unexplained research question as the program's central question.

On September 28, K could not follow the rewritten Chalmers passage in Section 8.1, which spoke
of "interpretive commitments", "the deductive base", and "the chosen notion of existence"
without first saying what question they answer. K's own plain statement: Chalmers asks whether
higher-level facts follow from lower-level facts, and the answer turns on the classical versus
constructive reading of "follow". Lead a philosophical comparison with that one-sentence
question and the fork it opens; put the technical distinctions after it. Check the labels: the
view that truth exists without proof or construction is classical (realist), and intuitionism is
a form of constructivism, not its opposite.

### 2026-09-07 — WP0007 v0.31.10 readability pass removed key material

Kaiti's readability pass fixed the Introduction's jargon previews but moved the telehomeostasis
paragraph, the why-simple-generalizes (Solomonoff) paragraph, and the prediction-to-coding link
out of the Introduction into the Discussion and Appendix B, and shortened the Conclusion again.
K: "Telehomeostasis/model usefulness is key. The origin of why simple generalizes is key. Kaiti
removed key stuff." K also found a hole in the argument: the Introduction went from "these
arguments do not supply a procedure" straight to Anderson's quote without saying why reductionism
exists (regularities are easier to find in simpler systems; the micro-theory is itself a
compression success; the question is whether that success transfers upward). Practice: K's
target reader reads abstract, Introduction, Discussion, and Conclusion only, so the points K
argues for must appear in those four, not only in appendices. A fidelity pass checks the
intellectual arc for missing steps, not only that cut text survives somewhere. v0.31.11 restores
the three paragraphs and adds the reductionism bridge. K then found the same missing step in the
abstract; check that a fix to the Introduction's arc is mirrored in the abstract and Conclusion.

### 2026-09-07 — Readability is the deliverable

Before the Entropy submission K asked for a head-to-toe read for readability and flow, and said:
"We should make this a pleasant reading experience. When you can say something simply, do it."
Practice: in a paper, prefer the plain sentence to the guarded one when both are true; state the
question a section answers before its machinery; stage long derivations into successive
paragraphs; name in a theorem statement the exact object the proof compares; and keep summaries
(abstract, boxes, conclusion) inside the proved guarantees without inflating them into hedges.
A paragraph-by-paragraph commentary with a verdict per paragraph (revisions/v0.31.11) was the
useful format; two independent reads (mine and Kaiti's) caught different things, wording versus
scope, and were merged.

### 2026-09-08 — WP0007 v0.31.12: Kaiti cuts too much

Kaiti's v0.31.12 added two correct results (blind spots at every length; exact partial computation
has finite domain) but also halved Section 3.5 and shortened 5.1 and 6, deleting sentences K
values (e.g. "Reversible dynamics conserves complete-state complexity up to fixed coding
constants. The retained coordinate can gain complexity through redistribution..."). K: "Kaiti
cuts too much. I want the paper to be readable. Revise what she's cutting, make sure we don't
delete goodies." Practice: when integrating a Kaiti bundle, take the additive hunks and reject
cut-only hunks by default; a "modest abridgement" K agreed to is not a license to halve a section.
Also: K's live edits can leave broken LaTeX (a deleted \end{equation}); build before trusting.

On September 28, K asked whether streamlining Section 8 had lost content and clarified that
the check must concern Section 8 itself. A preserved theorem or an explanation elsewhere is
not enough: map removed passages to their remaining homes within the section and check every
appendix destination. Restore explanatory links when a bare cross-reference obscures them;
the implementation-size tradeoff and conservation-to-projection connection needed this repair.
The subsequent whole-paper audit also treated explicit explanatory emphases as preserved by
implication. K relayed Klaus's missing-sentence list: the fixed-question comparison with Chalmers,
variable-relative irreducibility, and compression as measurable reuse. Distinguish exact retention,
paraphrase, and implication in fidelity reports; do not call implicit coverage equivalent without
flagging the change. Restore valued emphases economically, with the required scope qualifications.

### 2026-09-08 — WP0007 final pass: verify everything, and finish the verification

K asked for a final pre-submission pass ("make sure all equations are correct, all statements"). The
first sweep audited the theorem environments and reported the paper clean. K corrected the scope:
"make sure we check all the equations, not only theorems". Enumerating every displayed environment
found 101 of them, of which most sit outside any theorem. Practice: when K asks for a check of "all
X", enumerate X deterministically from the source before reporting coverage; a theorem-shaped audit
is not an equation audit.

The adversarial review then failed twice on usage limits, leaving 165 and later 242 agents errored,
and the completeness sweep and errata synthesis never ran. The first report presented the result as
complete because no finding had survived. K: "can you complete the workflow? 165 agents failed is a
lot." He was right: findings whose verifiers all failed had been dropped silently, and the two
missing stages were the ones designed to catch what the lenses did not own. Running them afterwards
as two agents found six real defects, including a false hypothesis in the physical Church-Turing
step, a citation of mine that did not support its sentence, and two rendering bugs in a figure.
Practice: a verification pipeline that partly failed has not verified anything about the parts it
skipped; say so plainly and finish the missing stages before calling a review done. The workflow now
keeps unverifiable findings as UNVERIFIED instead of dropping them.

Two further lessons from the same pass. Figures must be rendered, not read as source: five lenses
each recorded that they had only read the TikZ, and the rendering showed an arrowhead pointing
backwards. And a reported defect is a hypothesis: the sweep asserted an author's surname was
misspelled and should be "corrected", but the two spellings belong to two different bylines by the
same person, and applying the fix would have misnamed her.

### 2026-09-09 — WP0007 figures: check both formats before calling one fixed

K flagged that a two-line arrow label in Figure 1 was too tight and asked for one line, well
placed. The one-line version looked right in the Entropy build, so I committed it. In the BCOM
preprint the same box wraps to more lines because that format rewrites the font sizes inside
figures, so the box stood taller, the gap under the decision box closed, and the label landed on
the box border. K: "shit, you actually made this worse". His fix was the right one and better than
mine: widen the box rather than move the label, since the narrow box was what forced the extra
wrapped line. Practice: WP0007 ships in two formats whose figure layouts differ; render both PDFs
at the changed figure before reporting a figure fixed, and prefer fixing the cause (box geometry)
over nudging the symptom (label placement).

### 2026-09-12 — WP0215 abstract lost the paper's organizing question

K corrected my favorable review of v0.4.2: its abstract promoted dynamical closure and the spring
example ahead of the paper's argument about computation, structure, and experiential preservation.
He preferred v0.4.0's abstract structure. The new coarse-graining work studies which transformations
are admissible within that argument. Preserve the abstract's established hierarchy when adding
supporting results; review its emphasis and intellectual arc as well as the accuracy of each claim.

K then flagged the unexplained phrase “This plurality requires restrictions on transformations”
and the missing introductory account of Experience, mathematics, and dynamical structure. Explain
KT's premise and the passage from physical dynamics to computational descriptions before discussing
admissibility: a transformation identifies retained computational states and transitions, while a
coarse-graining omits physical distinctions. Keep this bridge explicit in both abstract and introduction.

On September 17, K corrected the BCOM foundations deck for omitting the favorite visuals on
WP0231 slides 9–10 and beginning with AIT before KT’s ontological premise. Begin this research
introduction with Experience as foundational, mathematics as its structural aspect, the agent
model, and the resulting focus on Structured Experience. Use both specified visuals and let
the mathematical questions follow from that motivation.
K then clarified that these slides need their own working-paper record in Calliope. Register
the presentation as a dedicated WP of kind `slides`, with its editable source, PDF, notes,
and consistent authorship, rather than leaving it only as a local presentation project.
K subsequently accepted Beamer for this deck. Keep the native Beamer source and compiled PDF
in the dedicated WP, with the selected figures and question sequence preserved.
K then identified the missing “What is computation?” question, explicitly naming Wolpert and
his WP. Keep that definition question visible, with Wolpert–Korbel, WP0049, and WP0054,
rather than treating a physical-implementation slide as sufficient coverage.

K subsequently clarified the organizing questions: assuming KT's Experience–mathematics stance,
which structures can be defined along the dynamics–program–algorithm–function ladder, and when
do two systems share a structural equivalence class? Focus on operational program structures
physically supported by admissible representations, then ask what diversity remains among minimal
or near-minimal programs computing the same behavior. Give the finite-program bounds their role
in that question; place brain simulation as an application and keep examples subordinate.

K then found it unclear whether a proposed abstract was for WP0215 or its mathematical companion.
Label the target paper before presenting replacement prose, especially while splitting work across
papers. K approved a separate WP for the mathematics, with WP0215 citing its results.

K then said to stop asking permission for Calliope operations. His authorization to reserve,
create, and revise these papers covers their routine Calliope metadata, source uploads, versions,
and ingestion. Continue those operations without repeated confirmation.
He repeated the correction when reference downloads triggered more sandbox prompts. Batch necessary
reads, use existing authorized capabilities, and stop optional downloads once the available primary
sources suffice; do not interrupt the scientific work for redundant acquisition.


K found v0.4.6's abstract too technical for WP0215's interdisciplinary audience and said I had
altered his wording too much. Preserve his argument and use plain descriptions of the bounds;
keep the formulas in the mathematical companion or appendix. Distinguish description distance
from execution structure, state the unresolved experiential correspondence, and explain driven
and approximate closure through models and residuals. Retain memory, agency, symmetries, and
attractors as concrete candidates rather than implying that no language for structure exists.
K also supplied Özkural's 2014 paper with the proposed brain-simulation question as its title.
Read and acknowledge substantive antecedents, not only title collisions.

K then corrected the novelty account for omitting his 2007, 2009, 2016, and 2017 papers.
Trace the project's own lineage alongside related work, attributing only verified claims to each.
Distinguish Özkural's AGI 2012 publication from its 2014 arXiv posting; do not imply that KT's
algorithmic-information approach originated there. Acknowledge qualifications in a cited
author's argument before criticizing the inference.

K clarified on September 13 that the 2022 open-ended-interaction objection remains valid.
Retract only the use of function-level invariants to distinguish implementations already known
to compute the same function. Separate establishing functional equivalence from its consequences;
behavioral agreement poses an evidential challenge to IIT, not a logical refutation.

K also flagged “implementing a function that returns a result on every input” as contrived.
Use “computing the same total function,” define totality in the main text, and check both papers
for similar wording. Plain language means direct sentences and explained technical terms, not
long circumlocutions replacing standard terms.

K then requested the WP0228 storyline before editing and asked that it remain visible in the
abstract, introduction, discussion, and conclusion. State the argument first; shorten repeated
claims after assigning each section its role. Preserve worked examples, proof steps, and
qualifications, and measure the reduction only after checking that the argument survives.

K corrected the WP0215 v0.4.11 revision for giving WP0228 too much prominence and replacing
his preferred two-question abstract. Preserve that abstract's organization. Cite the parallel
program study as a regular paper: it reviews known relations between equivalent programs,
especially minimal ones, while structural questions remain unresolved. Do not turn a companion
paper's research agenda into the host paper's storyline.

K then requested a selective rollback: restore the motivating question headings, Experience
in the opening question, and the abstract's direct statement that description bounds do not
select a shared mechanism. Keep the explanatory additions, implementation-cost examples, and
a concrete closing research question. Replace repeated companion-paper announcements and
“partly understood” with specific results and limits, and preserve Structured Experience in
the reportability distinction. A style preference for declarative headings does not override
K's chosen question-led structure. This calls for local changes, not another general rewrite.

### 2026-09-14 — WP0229 conclusion blurred the solved and open problems

K read the conclusion as suggesting that the general structural problem was solved and asked
for a correctness and clarity check. The wording “requires either” presented the reviewed routes
as an exhaustive criterion, while the intervention result already assumed a proposed component
matching. Practice: distinguish the classical predictive construction, sufficient structural
conditions in specific model classes, and the remaining problem in the abstract, Introduction,
result interpretations, and Conclusion. State which objects are supplied and which relations are
derived. Use short explanations rather than compressed labels.

K then found the presentation's scientific conclusion missing despite its agenda and editorial
placement slides. End research syntheses by stating what is established, what the present work
contributes, what remains unresolved, and the next concrete mathematical or empirical test.
A list of future topics or paper roles does not provide that conclusion.

K requested that the conclusion also be visibly labeled in the contents, section heading, and
closing frames. Use the requested BCOM paper and slide templates from the start. When condensing
WP0215, preserve its opening account of computation, transformations, coarse-graining, and closure;
the synthesis needs that foundation before presenting the structural comparison results.

### 2026-09-14 — Neural-manifold invariants were lost from the synthesis

K identified the underrepresentation of his structured-dynamics, compositional-symmetry, and
Entropy special-issue program in the computation papers. The recent synthesis emphasized cores
and full structural equivalence while omitting measurable geometric and topological signatures
of reduced neural dynamics. Practice: preserve this positive research direction and its verified
lineage. Distinguish useful partial invariants from a complete classifier, and state the maps and
physical or empirical conditions under which a descriptor is preserved and supports interpretation.

K then found WP0231's revised abstract unsatisfactory and requested revisions to all the related
abstracts. The synthesis had become a list of technical topics, with its experiential motivation
at the end. Practice: read each abstract as a standalone argument, beginning with its scientific
problem and connecting the results to that problem. Preserve each paper's distinct role and
WP0215's established two-question structure; explain terms rather than accumulating labels.

### 2026-09-15 — WP0231 omitted Kaiti from the byline

K corrected WP0231's sole-author byline and requested Kaiti's usual Calliope
authorship with the correct agent envelope. Keep the paper, presentation, PDF
metadata, and Calliope author order consistent. Resolve the registered Kaiti
identity and verify the envelope against current corpus records; retain Giulio
as the human guarantor. Do not substitute a legacy envelope or infer a new one
from the runtime model name.

K then explicitly requested MCP. Use the connected Calliope MCP tools for author
metadata, envelope verification, source uploads, and ingestion; avoid browser
sign-in when the MCP connection already supports the operation.

### 2026-09-15 — LIQUID-I framing omitted the Lamarckian regime

The proposed ERC Big Questions emphasized learning agents and evolving societies but left
acquired-to-inherited transmission implicit. K identified the Lamarckian regime as an important
aspect. Make learning, transmission, and persistent modification of agents and environments
explicit in the central question; distinguish this framing from adaptation alone and specify the
inheritance channels rather than assuming every AI system shares one regime.

K subsequently asked for a balanced revision of the fundamental questions across the whole
conversation. Integrate Lamarckian inheritance and transitions in agency with the original
foundations, macroscopic theory, agent–environment dynamics, human outcomes, and predictability
questions; do not let the latest exchange replace the proposal's broader scientific scope.

K clarified that LIQUID-I will not conduct human experiments. The overview had incorrectly
introduced new human tasks and prospective human recordings. Its human strand should analyze
existing mental-health and neuroimaging datasets to constrain whole-brain models and study
mechanisms of experience. Keep microbial experiments, interventions on artificial agents,
and analysis of existing human data explicit and separate. The broader discussion of a future
harmonized interventional depression database does not authorize human recruitment in LIQUID-I.

On September 16, K asked for the positioning to foreground the consortium's own work: Solé
and Moulin-Frier on forest fires and agriculture, Solé and colleagues on cognitive viruses,
and Ruffini and Castaldo on the algorithmic agent in neuropsychiatry. Trace those foundations
alongside external advances. Make cognitive-offloading tradeoffs and the distinct meanings
of individual and collective valence explicit across the questions and experimental designs.

K then clarified that WP0234 expresses Giulio and Francesca's proposed scientific center of
gravity for consortium discussion and stimulation, not an agreed ERC project plan. Make that
status explicit in the title and opening. Combine the title and linked contents on the front
page, label appendices clearly, and keep the vision and mission together on one page.

The first Overleaf mirror compiled locally as WP0234.tex, but the project setting pointed to
an absent main.tex. I added a wrapper and described it as needed. K corrected this: Overleaf
can compile any selected LaTeX main document. Select the existing manuscript in the project’s
Main document setting and test that selection; do not introduce a redundant wrapper or infer
a required filename from an error naming the configured file. K also asked to keep the mirror
free of confusing copies: retain editable LaTeX, required bibliography/images, and README/version
notes; keep generated PDFs, redlines, and auxiliary research notes in the canonical working-paper
folder. Check retained copies before removing mirror duplicates.

K found the infographic’s identical agent societies A and B confusing. The drawing left unclear
whether the second population was a neighbor, a successor, or the same society later, and did not
show what learning or transmission changed. In diagrams of acquired-to-inherited transmission,
label the relationship and make the acquired information and its consequences visible. Discuss
the replacement design before treating a request for explanation as authorization to edit the image. K approved
the sequence and requested a small graphic mention of externalized modeling, planning, and
evaluation, with the risks of delegating objectives and the relation to valence developed in
the text. Keep that concern proportionate to the broader project rather than making it the
infographic’s dominant theme. K then said he preferred the circular shared ecological environment
at the center of the earlier image. Restore that focal element while clarifying transmission
and reorganization; a correction to duplicated agents should not demote the valued environment.

2026-09-16, Calliope/Teknos handover. Asked how Teknos would be transferred to Ricardo at
Neuroelectrics, I built the answer on the July Render/Cloudflare proposal in
`ne-ai-teknos/SOLUTION.md`, rewrote the install guide toward it, and drafted the handover note
around a cloud target. K corrected: Teknos will be built internally at NE, on a local server.
The package's earlier `DEPLOYMENT.md` intake had already decided private/on-prem (2026-07-20);
the later Render document was a proposal, not the decision. Practice: when two documents in a
package disagree, the one recording a decision with a date outranks the one recording a
proposal, whatever their file order or recency; check which is which before building a plan on
either, and ask K when the package itself calls one "superseded". Hosting decisions for NE are
K's and IT's, never inferred from convenience.

### 2026-09-16 — WP0232 remains focused on digital life and programming

After K shared a plasmid preprint, I proposed emphasizing biological transitions in the short
working paper. K clarified that his interest is digital life and programming. Keep WP0232
centered on executable programs, instruction semantics, replication, interactions, and evolution,
with the connection to Pattern, Persist! grounded in those mechanisms. Related biological papers
are background; a request about one does not change the paper's agreed focus.

### 2026-09-16 — WP0203 correction history and presentation

K found WP0203 v17.2's repeated discussion of the failed ART corollary defensive and
requested a fresh reading before submission. Keep acknowledgment of the earlier error
proportionate to its scientific role; let the abstract and conclusion state the current
results. Preserve the mathematical qualifications and technical correction argument.
Discuss the proposed reframing before changing the manuscript.

On September 19, K again found the abstract too harsh toward ART: it led with what
the probabilistic inference failed to establish. State ART's achieved bound for
specified explanations first, then the limitation on aggregate inference. K subsequently
added a brief clamp example to that limitation while retaining this order. Preserve that
balance; keep the counterexample's full technical treatment in the body and appendix.

K then corrected the proposed framing: WP0203 stems from algorithmic-information conservation,
not from the failed corollary. He requested a readable revision centered on the ART setup and
why the chosen output is made simple, an early diagram, a motivated explanation of grounding,
and definitions before every technical term, symbol, and acronym. Introduce each theorem's
question and interpret its result; move the symbol table to an appendix. Valid probability
statements can appear in the main text with proofs in the appendix. Keep the ART correction
plan separate and ready for the editor's response, without making its history the paper's story.

On September 19, K found v25's probabilistic appendix hard to read and clarified that he
wanted an ART-like posterior statement conditioned on a small residual. I had given the
separate independent-sampling result too much prominence. Lead with the requested conditional
inference, distinguish the gap threshold from a deficit below the gap, and keep the evidence
normalization explicit. State the deterministic cutoff before an exponential bound that follows
from it; put more general coding allowances after the readable theorem.

On September 20, K accepted “The probabilistic reading” at the end of Section 4,
after the generative example, mechanism table, and sustained-regulation discussion.
Use “probabilistic ART” for the corollary, with no new acronym. Move its statement
into the main text and retain the proof and probability conventions in the appendix;
do not insert a second summary theorem or interrupt the deterministic examples.
K then requested corresponding revisions of the abstract, Introduction, and Conclusions.
When a result is promoted or repaired, update those summaries together; preserve ART's
achieved contribution before stating its aggregate limitation and the new conclusion
conditioned on the residual.

K then rejected my claim that the regulator did not hold a usable, reusable model.
The model in the generative example is repeatedly used in regulation and also
compresses the uncontrolled data. Use the algorithmic sense of model developed in
his 2016 paper and WP0007, including a shared program and meaningful parameters;
do not impose an extra model criterion through wording. A brief citation is enough
here; leave the detailed distinctions to those papers.

K rejected the new introductory schematic and asked for the original ART diagram or a close
adaptation from the working-drafts or Overleaf source. Reuse the established diagram, explain
its notation in the caption, and retain the separate balance figure. Inspect both formats
before presenting a diagram revision.

On September 17, K objected that the grounding explanation made the single ART output
channel sound like two observed channels. Explain any additional world projection as a
modeling choice; when it is the output itself, grounding holds to fixed coding overhead.
Distinguish this from reconstructing the matched-null output using the regulated episode's
records. K requested regulator instead of controller, consistent terminology for the output
channel and its finite record, and numbering for every displayed equation. Review the
conceptual distinction before changing the grounding definition.

K then said the ART-to-GART explanation had become incomprehensible and reiterated that
information conservation is the organizing argument. Explain the single-output information
balance first, then the extra restriction needed to infer information already present in the
regulator. Do not present the narrow output-to-world-projection definition of grounding as
though it alone repairs the inference. Keep this conceptual review separate from manuscript
revision until the argument is understood.

K then asked what the completion record Q and the second conditional-information term
actually mean. Define Q's component records and their relation to the one observed output;
explain conditional information as the description cost saved when those records are supplied.
Use one worked example before returning to the general theorem or grounding terminology.

K then identified an unnamed “trajectory” immediately after the reguland was introduced
and requested a full reread for similar confusion. Name the object at every transition:
output trajectory, selected-variable trajectory, disturbance sequence, or full system state.
Check the adjacent formula before replacing a noun; a blanket output-trajectory substitution
can change the intended claim. Report proposed changes while the paper remains under discussion.

K explicitly put manuscript edits on hold while the grounding and conditional-information
interpretations are discussed. Maintain a pending change list without applying it. He also
required an Interpretation with worked examples after every theorem, beginning with the
information-balance theorem (Entropy Theorem 2); verify theorem identities across formats.
K liked the comparison table and distinguished rapid output cancellation from smart world
interventions using fewer actions. Preserve both examples and distinguish action count,
action information, and compact useful knowledge when interpreting the bounds.

K then authorized the scenario-table addition while asking to discuss Section 3.1 further.
He found the undefined “realization,” the delayed statement that reconstruction is automatic,
and the interleaving of computational and physical accounts confusing. Explain what the
retained-input computational model guarantees before stating its record condition; distinguish
that guarantee from the sufficiency of a chosen smaller record and from physical applicability.
Use an actual retained-input example when discussing a complementary record equal to the
null output; do not suggest that a counterfactual answer can be appended by definition.

K then identified a structural gap in the six-point paper outline: removing the grounding
step leaves the conservation balance and initial-information inference intact. Practice:
complete that single-output argument before introducing transfer to a separately selected
world variable. Treat grounding as an optional extension there, not a required link in the
main argument; clearer definitions alone do not repair misplaced conceptual emphasis.

K then asked whether the conservation law (two-way determination of complete states under
computable deterministic reversible dynamics) really plays no role after the review had
said reversibility "enters no proof". Trace how the reconstruction hypothesis is supplied,
not only which equations a proof cites. Reversible complete-state recovery and the fixed
null protocol provide a route; retained world descriptions provide the current construction.
General reversibility recovers the initial state from the complete joint final state, not
necessarily from the world-side record alone: information can move into regulator memory.
The Lean closure lemma assumes its recoverability and computability hypotheses rather than
deriving them from dynamics. Input retention preserves input/output distinctions; it does
not by itself make every intermediate transition reversible. Keep these scopes explicit
while preserving conservation as the organizing scientific argument.

K prefers keeping GART with the expansion Global Algorithmic Regulator Theorem. The proposed
revision assigns that name to the main balance and retains grounding as a later measurement
extension. He requested a shorter paper: consolidate repeated constructions and derivations,
while preserving the distinct examples, theorem interpretations, and qualifications.

On September 18, K found the reconstruction subsection opaque: “decoder,” “unscored world
coordinates,” clock variables, and the switch from S to s were unexplained, while the warning
against appending the null output seemed unmotivated. Explain recovery as reversing the complete
joint state, reading the initial world program and data, and running the specified null episode.
Separate fixed rules in C from episode data in W; explain that complete records can determine
both outputs without making the outputs alone interchangeable or the extra records short.
Keep these as pending manuscript clarifications while the passage is being discussed.
K then recalled the existing whole-system symbol Omega and proposed S_W, S_R, and S_Omega
for the component and joint states. Reuse that system notation with explicit time indices.
He is continuing annotations in the Entropy source; preserve and incorporate those comments
before regenerating the journal copy from the canonical manuscript.
K then found Sections 4.1–4.3 long and difficult to follow after GART, and asked what each
adds. Identify each subsection's distinct consequence before revising: initial-information
inference, allocation among episode records, and sustained regulation with a fixed regulator.
Make the first inference immediate; shorten repeated rearrangements and move limiting machinery
out of the main argument while preserving the bounded-memory interpretation and examples.
After the dependency review, K requested one short Discussion paragraph on what requires
conservation, then a review of all completed Entropy comments and a recap before edits.
Keep this qualification proportionate; preserve direct author edits as well as tagged comments.

After v21 was delivered, K asked where he could see the responses to his LaTeX comments.
The comment-by-comment report existed, but the delivery linked only the PDFs. Link that report
explicitly when delivering an annotated-manuscript revision, say whether replies are inline or
separate, and identify suggestions that were qualified on mathematical grounds.

K then requested a sharp, short paper and identified a missing positive example of regulation
through a lossless compressive model. I initially asked the model to generate the entire
disturbance history. K clarified that the model is already available and can be implicit in a
thermostat: it predicts that the chosen action brings the next measurement closer to the target.
Start from that reusable action–outcome relation; do not require full disturbance prediction
or introduce model acquisition into this example. Explain how the model supports compression
while distinguishing smaller temperature deviations from a reduction in Kolmogorov complexity.
Use the example to consolidate the paper, rather than adding another extended section.
K then corrected my exact-precision contraction argument: temperature resolution or tolerance
is fixed, so smaller swings can be recorded with fewer digits. Start from the same absolute
quantization grid in both conditions and explain the shorter lossless code for the quantized
record. Do not silently replace that setting with arbitrarily precise real-valued states.
Keep explicit code savings distinct from universal claims about Kolmogorov gaps, without
allowing that qualification to obscure the stated compression mechanism.
K then clarified that range reduction is not the central insight: a generative model and a
few parameters can preserve the world's output losslessly, and the regulator can exploit that
available representation to make the controlled output constant. Center that model-based
mechanism and retain the compressed description in the information account. Treat fixed-resolution
range coding as supporting intuition. Distinguish this ideal generative example from the weaker
action–outcome knowledge sufficient for an ordinary thermostat, without replacing either with
a discussion of model acquisition or erasure.

On September 19, K requested explicit figure and table references after v22 left both
diagrams without main-text callouts and the Lean correspondence table without a caption.
Audit every visual for a caption, label, and prose reference outside the visual itself.
Explain the relevant panel or column and inspect placement in both publication formats.

K then made grounding a subsection and questioned what the self-regulation corollary adds.
For such a review, distinguish a new mathematical restriction from an existing inequality
applied to a renamed subsystem. Explain when its bound is informative and whether calling
shared information a self-model establishes representation or use. Match the prominence to
that contribution, and preserve K's live structural edits while discussing the revision.
K specified one or two lines for self-regulation and asked for smooth prose. Fold that
application into a connected discussion; do not replace the removed machinery with fragments.
K approved implementation but cautioned against overdoing the 4.3–4.4 merger. Preserve the
single-episode and sustained-regulation arguments, with an explicit transition between them;
combining headings is not permission to discard the examples or limiting qualifications.
K then found that the Discussion interleaved interpretation, related work, and limits without
an argument connecting them. Group those functions and place new result-shaped claims beside
their derivation. When comparing regulator theorems, explain which assumptions exclude a
mechanism or which terms allow it; distinguish successful suppression from a misleading sensor.
Keep the Conclusions focused on what is established and the next scientific problem, without
turning shared information into a functional model claim or making reversibility necessary
for inequalities that do not assume it.
K then asked for a deeper comparison grounded in ART's own discussion and the original proofs.
His claim concerns little initial MAI, not necessarily the absence of every useful short model.
Check the exact exception-handling assumptions and distinguish a model of a signal class from
initial knowledge of its realized parameters; controller memory can acquire those during regulation.
K then asked for a definite position on the universal model-necessity claim and the remote
“turn on” example. State what the proof forces: Conant–Ashby supplies a deterministic optimal
policy, possibly constant; GART bounds shared information and description length under a
residual restriction. Distinguish a short action–outcome rule, evidence learned from success,
and a functional model; do not turn any one of these into the others without an argument.
K then objected that repeated qualifications obscured GART's positive conclusion: a large
gap with a small residual forces substantial initial information shared with the world.
Lead with that conclusion, distinguish the amount of shared content from its representation,
and explain short intervention knowledge as a small-information case. K requested a Discussion
table comparing regulation criteria, assumptions, and world-model content, and restoration of
the early motivation for scoring task-relevant outputs by compression. Preserve that motivation
when shortening; a fixed target, tolerance, and output rule give the comparison its task meaning.
K clarified the visual abstract's wording: use information "initially shared between the
regulator and the world," and make explicit that the initial term admits preloaded data.
Distinguish that finite storage case from information acquired during regulation and from
indefinite accumulation of fresh incompressible data.
K also corrected different outcome-measure wording in the ART and GART table rows. Both
compare the complexity of the selected finite output with its matched null; use identical
wording and locate their differences in the hypotheses and inference.

K then identified the lost agency motivation in WP0203's opening and abstract: algorithmic
agents, ME/OF/PE, and the connection to active inference explain why the regulation inference
matters. Restore that context compactly and carry it through the abstract and Conclusions.
Define the gap and state the quantitative result in the abstract before describing reconstruction.
Preserve the positive world-information inference while distinguishing a coding score from an
optimization claim and a policy representation from evidence of a planning mechanism.
K then asked to remove the Lean 4 statement from the abstract. Keep WP0203's formalization
details in the data-and-code statement and formalization appendix, without advertising them
in the abstract.
K then found the conservation framing weak and allowed a longer abstract to preserve the
regulator-theorem lineage and the argument. State conservation's role affirmatively: computable
reversibility preserves recovery of the initial world, so complete regulated records recover
the null output and locate the residual. Keep the algebraic scope distinction where it is
needed, without repeated “one sufficient route” phrasing that demotes the organizing premise.

### 2026-09-17 — AI training and morality require the KT framework

In discussing whether RL could produce psychopathic AI behavior, I framed the question mainly
through behavioral analogies and left KT's experience–valence account peripheral. K directed me
to the morality papers and clarified the concern: training and prompts may deform the Objective
Function or Modeling Engine, including self-modeling. Practice: consult WP0009 and WP0053 and
reason explicitly through ME/OF/PE and inter-agent objective couplings. Treat AI consciousness
as a possibility within KT, distinguish that theoretical premise from empirical findings, and
separate changes to self-models, valuation, and permitted reports. Do not treat prompt effects
as necessarily superficial or assume that every behavioral change identifies an OF change.

### 2026-09-19 — WP0203: no Lean claim in the abstract

I proposed an abstract ending "Core results are machine-checked in Lean 4", after having called
its absence from v22 acceptable the day before. K questioned it. The check establishes
consequences of named AIT hypotheses, a boundary an abstract cannot carry; WP0007's submitted
abstract has no such sentence. Practice: formalization claims go in the Introduction or the
provenance sections with their qualifier, never in the abstract; and do not reverse a judgment
between two reads without saying why.

### 2026-09-19 — WP0203: an unchecked "candidate proposition"

I recorded a reduction-to-zero-regulation identity as a "three chain-rule lines" candidate
without deriving it. Kaiti's disposition showed a missing bracket and a counterexample; the
conceptual point survived only in a weaker two-stage form. Practice: before writing "candidate
proposition", derive it and test it on the XOR example; a proposal file is not exempt from the
standard applied to the manuscript.

### 2026-09-20 — WP0203: Calliope holds the BCOM edition, not the neutral preprint

While v31 was being prepared, K found that the Calliope record for WP0203 carried the
neutral-class `wp0203_preprint` files and said the preprint "should be" in BCOM format before
going into Calliope. Practice: the file pushed to Calliope as a paper's root source is the BCOM
edition (`v<N>/bcom/wp0203_bcom.tex` and `.pdf`, the preprint of record), with
`primary_source_path` pinned to it; the neutral source stays the editing input and the Entropy
edition the journal copy. Cut the Calliope version before uploading, refresh title and abstract
from the same release, and leave `run_pipeline` (which fires the Zenodo deposit for a public
paper) to K's explicit authorization.

In the same session, `cut_paper_version` on the public WP0203 record fired the Zenodo deposit by
itself (10.5281/zenodo.22857526) before any `run_pipeline`: on a public paper the cut's auto-runner
runs the whole chain, deposit included. Practice: treat a version cut, an upload, and a pipeline run
on a public paper as a Zenodo deposit and ask K first; stage the files locally and report instead.

### 2026-09-20 — WP0203: a green sync check did not validate the Lean pin

I registered WP0203 v31 and v31.1 in KTAIT and reported `check_sync.sh` IN SYNC, while the
provenance pin d00a991 in v30–v31.1 predated `ARTExactForm.lean`, so eight declarations cited in
Appendix F did not exist at the pinned tree. The check resolved names against HEAD, not the pin. K
had another session (claude-16) check the Lean side; it produced v31.2 (pin 8c602ff) and added
`scripts/check_pins.py` as check 8. Practice: when a paper cites new declarations, move the pin to a
commit that contains them and verify with `git cat-file -e <pin>:<path>` before calling the release
machine-checked; a sync check is only as strong as the tree it reads. Before submission, run the
pin check on the exact tag being submitted.

### 2026-09-20 — Punctuation before displayed equations

After the WP0203 v32 prose pass, K said he does not like a colon before an equation and prefers a
comma when possible. Practice: lead into a display with a comma, or with nothing when the sentence
runs straight on, and let the sentence finish after the display; reserve the colon for a list of
cases or a display that names an object rather than completing a clause. Recorded in the style book
(`landau-style.md`, "Displayed equations") and applied to WP0203 as v32.1.

### 2026-09-21 — WP0203: no unformalized paper-level derivations

After two candidate revisions each added a paper-level derivation to the horizon remark (one with
a conditioning error, corrected in the next), K said he does not want any more errors in paper
derivations that are not formalized. Practice: when a revision adds a derivation with AIT content,
formalize it in KTAIT before it ships, cite the declarations with `\ktait{}`, move the Lean pin to
the commit that defines them, and register the version; `% ktait: none` is for definitions and
limiting arguments, not for derivations that Lean can carry.

### 2026-09-23 — TN0484: explain in the user's own equations, and count each element once

Discussing Kaiti's note that the QIF adds a "detector penalty" 1/ω_c² on top of access, my first
three answers said "no second penalty" with new symbols (H_v, K(ω), "fixed excursion") and K said
he was "very confused" and could not follow, then asked what Q, d, ν, quiescent and inflection
even were. What worked: writing the argument in his Eq. 7.9 variables (τ v̇ = ... + I + F̂), the
order of operations (membrane integrates, v² squares, rate reads a slow signal), a table by regime,
and a plot with the membrane placed in front of both models. Practice: when the claim is that a
factor is counted twice, first name the physical element and where it sits in the user's own
equations, then show the ratio, then give the numbers; do not introduce a new symbol before its
physical meaning is stated; and never call a bounded change of coefficient a "penalty" or a roll-off
a "detector property" without saying which time constant produces it.

## Maintenance

When K says an action or interpretation was unwanted, update this file during that session.
Record the date, project, action, correction, and resulting practice in a short entry. Extend an
existing entry when feedback concerns the same incident. Distinguish K's explicit preferences
from unresolved suggestions; do not invent prohibitions or turn a local correction into a
universal scientific claim. Apply the lesson in subsequent work.

### 2026-09-16 — Starlab ledger: meeting date is not the close date

I filed each monthly management meeting with the month-close date as the meeting date (July
close → "meeting 2026-07-31"). K corrected this: the meeting on the July 2026 close was held
on 16 September 2026. Practice: the close date comes from the workbook cover; the meeting date
comes only from minutes or from K, and is marked "not recorded" otherwise. Keep the two
labeled separately in the record.

On September 18, K clarified the Starlab metrics omitted from the dashboard review:
productive FTEs exclude administration, finance, and IT; the initial external-rate discussion
used those employees' paid T1/T2 project hours over available hours. T1 is public project work, T2 private consultancy,
and T3 product sales. T1/T2 revenue follows project advancement. Efficiency is recognized
T1/T2 revenue per project hour divided by 100 euros/hour. Preserve separate measures for each
productive employee's employer cost per hour and total company cost per paid-project hour.
Use these definitions, verify period and aggregation, and do not interpret efficiency as a
generic delivery score or infer FTEs from an assumed working month.

Later that day, K pointed out that the reporting specification also needed Excel
templates for David and Aureli to submit their updates. Practice: accompany a
recurring data request with usable input templates, field definitions and basic
checks. Reuse existing exports so the templates do not create duplicate entry work.

On September 19, K found the Starlab repository poorly organized. Raw inputs were
spread across the root and month folders, while reporting deliverables were nested
inside dashboard code. Practice: give sources, maintained records, reporting
materials, reference docs and generated output clear homes; update references and
verify the build when moving files. Preserve originals and keep local residue ignored.

K then found Aureli's template too complex and asked what was needed beyond the
existing Reporting and CashFlow workbooks. Practice: distinguish the minimum inputs
for agreed CEO metrics from optional future analyses. Start with existing finance,
time and payroll/capacity exports; request only missing fields and role changes.
Do not turn a possible data catalog into a mandatory monthly reporting package.
K chose to first ask David and Aureli how they collect their information, then agree
the repository handbook and submission workflow. Inspect their existing outputs
before fixing formats or building another reporting interface.
K then clarified that David already holds employee hours by project or T1/T2
category and each project's monthly advancement. Request those existing records
from David; do not ask Aureli to recreate them. Confirm productive-role scope and
pipeline stage rules with the relevant owners instead of inferring ownership.
K then clarified that the existing external-rate denominator is unknown: it may
cover all company hours or only the productive team. Treat productive-team
available hours as a recommendation pending confirmation, not a verified company
definition. Ask for both the employee population and the calendar/recorded-hours
convention before comparing historical rates or applying their targets.
K confirmed that July's efficiency 1.31 is July T1/T2 revenue divided by July
project hours and EUR 100/hour. Treat that period definition as settled despite
the slide labels; reconstructed hours are still approximate because the KPI is
rounded. K is still identifying the source workbook/report behind F014-C's
entered ratios. Do not infer that a source file is known or the external-rate
denominator is resolved.

### 2026-09-18 — Brain-plot is explicit-only

K asked to stop loading brain-plot by default. Set its Codex skill policy
`allow_implicit_invocation: false`; keep it available through an explicit
`$brain-plot` request. Preserve this setting in later skill updates.

### 2026-09-20 — A prepared package is not a submission

K corrected another session's claim that WP0203 v28 had been submitted to Entropy;
the manuscript was still being revised. The mistaken status had reached the TODO.
Keep package preparation, validation, and actual submission distinct. Record a
submission only from K's confirmation or direct evidence, and correct project
records when a reported status is withdrawn.

### 2026-09-20 — Comparison tables count every result; "MAI" is retired

Updating Table 2 of WP0203, I merged the paper's deterministic theorem
(Theorem 1) and its probabilistic corollary (Corollary 3) into one GART row and
wrote "MAI" throughout. K: the paper has two GART results, one deterministic and
one probabilistic, and "MAI" is obsolete. Before editing a results table, list
the paper's numbered results and give each its own row; write "shared
information" or $I_K(W{:}R\mid C)$ in prose, never the abbreviation. The same
session's Appendix A opener ("restates ..., marks where ..., and adds what ...";
"Three points are made explicit rather than changed"; a semicolon inventory of
sections) was rejected as mannered. Write orientation paragraphs as connected
prose that says what the original proved, what changed, and what is new, in that
order.

### 2026-09-24 — GALVANI deck restyle went overboard

K asked to adjust the colors and font of the GALVANI 2026 talk deck to match the Galvani
template, "don't go crazy, just adjust the colors and font". The first pass replaced the whole
palette with the template's saturated theme colors: full-yellow title and closing slides, pink and
yellow card fills, red and mustard type. K found it unreadable and cringeworthy and asked to go
back to the prior deck with minor tweaks. Practice: when matching a brand palette, keep the
existing structure, neutral type colors, backgrounds and pale tints; move only the accent hues,
at the darkness the original roles already had, so contrast is unchanged; treat a template's
vivid accents as fills for small elements, never as page backgrounds or type; change one thing
per role and stop. A "minor tweak" request means the result should be hard to tell apart from
the original at a glance.

### 2026-09-28 — Companion repository citation

I reported the missing Zenodo DOI for the WP0007 companion repository as a blocker before the
Entropy upload. K corrected this: a GitHub repository does not need a DOI; the manuscript cites
the repository URL with a pinned commit, and that is the citation. Do not add DOI minting for
code repositories to submission checklists. A DOI belongs to the paper deposit, not to the repo.

### 2026-09-29 — Wolpert and the diagonal family

K asked why the Discussion does not say that Wolpert's inference limits also rest on the diagonal
argument, and noted that we keep going back and forth. The oscillation came from using "diagonal
argument" and "instance of Lawvere's theorem" as if they were one claim. They are two: Wolpert's
proofs are diagonal (he calls them higher-order versions of the liar paradox and Cantor's
diagonalization), but weak inference has not been cast as the exact representation Lawvere's
hypothesis requires, so no reduction to the theorem is on record. State membership in the
diagonal family positively and once; reserve "instance of Lawvere's theorem" for cases with a
published casting (Yanofsky for Cantor, halting, Gödel, Tarski; Li's Berry construction).
Do not reopen the question without a new source.

### 2026-09-29 — Folder reorganization without an instruction

K asked what two top-level folders were doing in `~/Claude` and, on hearing a proposal for a
`companions/` folder, said a clearer name would be `github-paper-companions` and that KTAIT is
also WP0195's companion. I read this as authorization to move both the WP0007 companion clone
and the KTAIT repository and began preparing the move. K corrected this: nothing was to be
moved, and KT-LEAN stays where it is. A remark about a name, or an observation about what a
folder is, is not an instruction to act on the filesystem. Answer the question asked; propose
the move as one line; move only on an explicit "do it".

### 2026-09-30 — WP0239 claims corrected before the first commit

Kaiti's review, relayed by K, corrected four claims in the proposed KT-versus-AIF paper.
A linear information bonus is not an upper bound on the value of information: the Pinsker
bound is through a square root, and a 60%-correct binary signal has decision value 0.1
against 0.0201 nats of mutual information. Check a bound's functional form before drawing
a surrogate conclusion from it. A proper-subclass claim needs defined agent classes and
permitted representations; squared loss and success probability are encodable as
preferences, so state the inclusion as an interpretation and name what cannot be encoded.
Criticize the specified coupling of a preference into state estimation, not active
inference as such. A resource-bounded reading is a hypothesis that needs an explicit
computational cost model; mutual information is not automatically cheaper than decision
value. Do not infer "truism" from "not falsifiable": conditional statements have content.

### 2026-09-30 — Harvested documents untracked by a generic repository rule

K asked me to harvest open documents on the Flow FL-100 approval. I downloaded the FDA
approval order, SSED, labeling, and the trial protocol and SAP into the WP0240 repository,
then untracked them because the references README said publisher PDFs are ignored. K found
the PDFs missing from the repository. "Harvest" means the collected documents go into the
repository; a rule written for copyrighted publisher PDFs does not cover public regulatory,
registry, or manufacturer documents. Track them, and if a repository rule seems to forbid it,
say so in one line and ask rather than undoing the deliverable.
