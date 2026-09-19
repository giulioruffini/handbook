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

On September 15, in the WP0216 program discussion, K objected to using APB before expanding
and explaining it, and to an abstract closing question about compact rules versus episode
records. Spell out Algorithmic Persistence Balance before using the acronym and explain its
reconstruction premise. State the intended scientific distinction with a concrete example;
do not introduce an unexplained research question as the program's central question.

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

K then corrected the proposed framing: WP0203 stems from algorithmic-information conservation,
not from the failed corollary. He requested a readable revision centered on the ART setup and
why the chosen output is made simple, an early diagram, a motivated explanation of grounding,
and definitions before every technical term, symbol, and acronym. Introduce each theorem's
question and interpret its result; move the symbol table to an appendix. Valid probability
statements can appear in the main text with proofs in the appendix. Keep the ART correction
plan separate and ready for the editor's response, without making its history the paper's story.

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

### 2026-09-17 — AI training and morality require the KT framework

In discussing whether RL could produce psychopathic AI behavior, I framed the question mainly
through behavioral analogies and left KT's experience–valence account peripheral. K directed me
to the morality papers and clarified the concern: training and prompts may deform the Objective
Function or Modeling Engine, including self-modeling. Practice: consult WP0009 and WP0053 and
reason explicitly through ME/OF/PE and inter-agent objective couplings. Treat AI consciousness
as a possibility within KT, distinguish that theoretical premise from empirical findings, and
separate changes to self-models, valuation, and permitted reports. Do not treat prompt effects
as necessarily superficial or assume that every behavioral change identifies an OF change.

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
productive FTEs exclude administration, finance, and IT; external rate uses those employees'
paid T1/T2 project hours over available hours. T1 is public project work, T2 private consultancy,
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

### 2026-09-18 — Brain-plot is explicit-only

K asked to stop loading brain-plot by default. Set its Codex skill policy
`allow_implicit_invocation: false`; keep it available through an explicit
`$brain-plot` request. Preserve this setting in later skill updates.
