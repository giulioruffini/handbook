# Working-paper versioning

One paper can accumulate several version labels at once. On 2026-09-04, WP0216
simultaneously carried v17.2 (the last committed source), v17.3 (a number
minted inside a web-chat session and never landed anywhere), v17.4 (a bundle
built the same day), v0.4.1 (Calliope's cut counter), and a Zenodo version
DOI. The labels were all locally reasonable; the mess came from three
counters that are never bound together, operated by agents with different
capabilities. This page binds them.

## The three counters

**Manuscript version** (`vX.Y`) is the human-meaningful revision label: the
title-page footnote and the `vX.Y/` folder in `bcom-working-drafts`. It
carries content semantics: bump `X` for a restructuring or a change in what
the paper claims, `Y` for a revision pass, and add `.Z` for fixes that touch
no claim (bibliography, supplement, typography).

**Calliope cut** (semver `v0.X.Y`) is a machine counter of repository
snapshots. It is monotonic per record and carries no content semantics; a
cut number therefore never appears in prose or citations.

**Zenodo DOIs** come in two kinds. The concept DOI names the paper and
resolves to its latest deposit; a version DOI pins one deposit forever.

## Rules

1. **Git mints manuscript versions.** A manuscript version exists exactly
   when its `vX.Y/` folder is committed to `bcom-working-drafts`. A chat
   thread, a Library upload, an Overleaf project, or a zip in Downloads
   cannot create a version, whatever its title page says.

2. **Off-pipeline drafts carry date-and-author labels, never numbers.**
   An agent without commit access returns work as
   `draft-YYYYMMDD-<author>`; whoever imports it assigns the next number.
   A draft that titles itself `vX.Y` is renamed on arrival, and the orphan
   number is skipped, not adopted.

3. **Every Calliope cut note opens with the manuscript label it
   snapshots** ("manuscript v17.2: ..."). The cut, the manuscript label,
   and the resulting Zenodo version DOI are recorded together in the cut
   note and in the version folder's `RELEASE_MANIFEST.md`. This triple is
   the only place the counters meet, so it is mandatory.

4. **Citations use DOIs, not labels.** Cite the concept DOI when the
   reference should follow the paper across revisions; cite a version DOI
   when the content must be pinned. A bare `vX.Y` in a bibliography is a
   defect once the paper is public.

5. **Numbers are never reused or reinterpreted.** A superseded or orphaned
   label stays retired.

6. **Each paper names its current candidate in one place**: the first open
   item of its `todo.md` states which manuscript version is the live
   candidate. Any question of the form "which is the latest?" is answered
   there, or it is a bug in the todo.

7. **Division of labor.** Humans and repo-capable agents commit, number,
   cut, and deposit. Chat-side agents produce `draft-YYYYMMDD-<author>`
   bundles and review against a named committed version. Calliope counts
   cuts and mints DOIs; it never defines what the manuscript version is.

At submission the journal copy and the public snapshot must have matching
content; their labels need not match, because the version DOI, not the
label, identifies the record.
