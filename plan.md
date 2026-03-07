# Plan for Building an Awesome Paper List on Action Chunking in RL

## Goal

Create a curated GitHub repository of papers on **action chunking in reinforcement learning**, covering:

- **Preprints** from arXiv and OpenReview.
- **Published papers** from top-tier **AI, ML, and robotics conferences**.
- A repository structure where papers are organized primarily by **year** and then by **venue**.

The repository should be close in spirit to the two reference repositories you shared: concise, easy to scan, and simple to maintain.

## Guiding Principle

The main risk is scope creep. "Action chunking" overlaps with temporal abstraction, options, macro-actions, hierarchical RL, skill learning, latent plans, and robot action-sequence prediction. The repository should therefore optimize for **precision first**, then expand carefully.

Recommended framing:

- **Core list**: papers where action chunking or multi-step action generation/execution is a central technical idea.
- **Foundational / related section**: older or adjacent papers on temporal abstraction, options, macro-actions, and skill-based control that are important context but not always explicit action chunking papers.

This keeps the repository focused while still useful for researchers entering the area.

## Target Output

The first public version of the repository should contain:

- A clear topic definition and inclusion policy in `README.md`.
- A `Preprints / Under Review` section near the top.
- Main paper sections organized as:
  - `2026`
    - `NeurIPS 2026`
    - `ICML 2026`
    - `ICLR 2026`
    - `CoRL 2026`
    - etc.
  - `2025`
    - venue subsections
  - earlier years
- An optional `Foundations and Related Work` section.
- A contribution workflow in `CONTRIBUTING.md`.

## Scope Definition

### Include

Include papers that satisfy at least one of these:

- The policy outputs or reasons over **multi-step action chunks** rather than only single-step actions.
- The method explicitly uses **action chunking**, **chunked control**, **macro-actions**, **temporally extended actions**, **action sequences**, or **latent action blocks**.
- The work is in **RL**, **offline RL**, **hierarchical RL**, **model-based RL**, or **robot learning** and action chunking is central to the method.
- Robotics papers are included if they are strongly connected to RL/control and the chunking mechanism is technically central.

### Exclude

Exclude papers where:

- Temporal abstraction is only background motivation, not part of the actual method.
- The work is generic sequence modeling, planning, or imitation learning with no meaningful action chunking angle.
- The paper is about unrelated action tokenization for language or multimodal systems without RL/control relevance.
- The paper is only a blog post, talk, or unverified project page.

### Borderline Policy

Use two internal labels during collection:

- `core`: directly about action chunking in RL/control.
- `adjacent`: important context, but only indirectly connected.

Only add `adjacent` papers publicly when they clearly improve the repository, ideally inside a dedicated `Foundations and Related Work` section.

## Recommended Coverage Strategy

To keep the list high-quality and realistically maintainable:

- Make the **modern action chunking list exhaustive** for recent years.
- Make the **historical foundations section selective**, not exhaustive.

Recommended split:

- **Main list**: exhaustive from roughly the recent modern wave of chunked-control papers onward.
- **Foundations section**: representative older papers on options, macro-actions, temporal abstraction, and hierarchical control.

This is better than trying to make the repository fully exhaustive over all of classical temporal abstraction, which would quickly become too broad.

## Venue Coverage

### Primary AI / ML venues

- NeurIPS
- ICML
- ICLR
- AAAI
- IJCAI

### Primary robotics venues

- CoRL
- RSS
- ICRA
- IROS

### Preprint and review sources

- arXiv
- OpenReview

### Optional secondary venues for later expansion

- AISTATS
- UAI
- L4DC
- Humanoids

### Optional journals for a later phase

Only add journals if you want to broaden beyond the original conference-focused scope:

- RA-L
- T-RO
- IJRR
- JMLR

## Repository Structure Plan

### `README.md`

Recommended structure:

1. Repository title and badges.
2. One-paragraph definition of action chunking in RL.
3. Short inclusion and exclusion policy.
4. Table of contents.
5. `Preprints / Under Review`.
6. `2026`
   - venue subsections
7. `2025`
   - venue subsections
8. Earlier years.
9. `Foundations and Related Work`.
10. `Surveys / Benchmarks` if enough relevant material exists.
11. `Contributing`.

### `CONTRIBUTING.md`

Current contribution instructions are already usable. Later, update them only if the metadata schema changes.

### Optional data layer

For v1, keeping `README.md` manually curated is acceptable.

If the repository grows large, add a structured source of truth such as:

- `data/papers.csv`, or
- `data/papers.yaml`

and optionally generate `README.md` from it.

## Paper Metadata Schema

Every paper should be tracked with at least:

- Title
- Paper link
- Authors
- Venue or status
- Year
- Month if available
- Method name
- Domain or task
- Code link

Useful internal-only fields:

- `status`: preprint, under-review, accepted
- `area`: AI/ML, robotics
- `setting`: RL, offline RL, hierarchical RL, model-based RL, imitation, robot learning
- `chunk_type`: continuous chunk, discrete macro-action, latent chunk, option-style abstraction
- `notes`: one short justification for why the paper belongs in the list

### README display format

Your current contribution file already suggests a compact table format:

```markdown
| Paper | Method | Date | Domain/Task | Code | Venue |
```

That is a good default because it stays readable even when the list becomes large.

## Search and Collection Workflow

### Phase 1: Seed the list with obvious papers

Start with papers that explicitly use terms such as:

- action chunking
- chunked control
- macro-action
- temporally extended action
- action sequence policy
- latent action chunk
- action sequence modeling for control

This seed set gives you anchor papers for citation snowballing.

### Phase 2: Use systematic keyword search

Search combinations such as:

- `"action chunking" reinforcement learning`
- `"action chunking" robot learning`
- `"macro-action" reinforcement learning`
- `"temporally extended action" reinforcement learning`
- `"action sequence" policy reinforcement learning`
- `"open-loop action sequence" robot learning`
- `"latent action" reinforcement learning`
- `"chunked control" robotics`

Use these sources:

- arXiv
- OpenReview
- Google Scholar
- Semantic Scholar
- DBLP
- official conference proceedings

### Phase 3: Venue-by-venue sweep

For each target year:

1. Check each primary venue.
2. Search titles and abstracts for chunking-related terms.
3. Review related accepted papers from RL and robotics tracks.
4. Add candidate papers to a working spreadsheet or markdown staging list.

This prevents over-reliance on keyword search alone.

### Phase 4: Backward and forward snowballing

For each strong seed paper:

- inspect references for earlier foundational work
- inspect citations for newer follow-up papers
- inspect author pages or project pages when the area is niche

This is especially important because relevant papers may not all use the exact phrase "action chunking".

## Screening Rules

For each candidate paper:

1. Verify that the paper is actually about RL, control, or robot learning.
2. Verify that action chunking is a technical mechanism, not just a passing remark.
3. Record the paper metadata.
4. Check whether an accepted venue version exists.
5. Check whether code exists.
6. Decide whether the paper belongs in `core` or `adjacent`.

## Deduplication Rules

To avoid noisy entries:

- Prefer the **accepted conference version** as the canonical venue listing.
- Use the **arXiv link as the paper link** when it is the easiest public version to access.
- If a paper first appears as a preprint and is later accepted, move it from `Preprints / Under Review` into the appropriate `Year -> Venue` section.
- Do not keep the same paper duplicated in multiple main sections.

## Public Organization Strategy

The public structure should stay simple:

- organize first by **year**
- organize second by **venue**
- keep extra categorization lightweight using the `Domain/Task` field or short tags

Recommended tags for internal use or compact notes:

- `RL`
- `offline RL`
- `hierarchical RL`
- `model-based RL`
- `robotics`
- `imitation`
- `continuous chunk`
- `macro-action`
- `latent chunk`

This gives you richer filtering later without making the top-level README too complex.

## Quality Control Checklist

Before publishing or merging additions, verify:

- the title is correct
- the link resolves
- the venue and year are correct
- the status is correct: preprint, under review, or accepted
- the paper is not already in the repository
- the code link is official when possible
- the paper actually belongs in the scope

## Proposed Execution Plan

### Step 1: Lock the scope

- Finalize the distinction between `core` and `foundations / related work`.
- Finalize the conference list.
- Decide the starting year for the main exhaustive list.

### Step 2: Build the repository skeleton

- Draft the `README.md` headings and anchors.
- Add `Preprints / Under Review`.
- Add year headings and venue subheadings.
- Add an optional `Foundations and Related Work` section.

### Step 3: Create the initial seed bibliography

- Collect a first batch of highly confident papers.
- Include recent preprints.
- Include representative accepted conference papers.
- Include a small number of foundational papers.

### Step 4: Run a systematic venue sweep

- Sweep each primary venue year by year.
- Fill missing accepted papers.
- Normalize venue names and dates.

### Step 5: Validate and deduplicate

- Remove duplicates.
- Merge preprint and accepted versions cleanly.
- Check links and metadata.
- Reclassify borderline papers if needed.

### Step 6: Publish v1

- Ensure the README is readable.
- Ensure coverage is strong for the targeted year range.
- Invite PRs for missing papers.

### Step 7: Maintain the repository

- review recent arXiv/OpenReview papers monthly
- update accepted papers after conference decisions
- triage community pull requests

## Definition of Done for Version 1

Version 1 is complete when:

- the repository has a clear topic definition
- papers are organized as `Preprints / Under Review` plus `Year -> Venue`
- the main target venues have been swept for the chosen year range
- every entry has consistent metadata
- obvious duplicates are removed
- the repository is clear enough that outside contributors can extend it correctly

## Immediate Next Actions After This Plan

- Decide the year range for the first complete release.
- Draft the `README.md` skeleton.
- Build the initial seed paper list.
- Sweep preprints.
- Sweep top-tier conference proceedings.
- Normalize and deduplicate entries.
- Publish the first curated version.
