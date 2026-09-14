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

## Maintenance

When K says an action or interpretation was unwanted, update this file during that session.
Record the date, project, action, correction, and resulting practice in a short entry. Extend an
existing entry when feedback concerns the same incident. Distinguish K's explicit preferences
from unresolved suggestions; do not invent prohibitions or turn a local correction into a
universal scientific claim. Apply the lesson in subsequent work.
