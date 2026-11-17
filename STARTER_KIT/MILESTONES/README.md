# Milestones

`MILESTONES/` contains approved phases of product understanding and implementation.

Use it when a project moves from discovery into a reviewed body of work.

Each milestone should preserve:

- source artifacts used
- reviewed conclusions
- implementation implications
- governance notes
- open questions
- next workstream

Root folders contain living canonical project truth.
Milestone folders contain reviewed context, decisions, snapshots, and implementation artifacts for a specific phase.
A milestone must not silently fork or replace a canonical root artifact.

Do not put `source_truths/` or `experience_boards/` inside a milestone. Point at the root files instead.

Milestones should not replace `HUMAN_TRUTHS/`, `PRODUCT_PRINCIPLES.md`, `ETHICAL_AI_PRINCIPLES.md`, `LESSONS_LEARNED.md`, `EXPERIENCE_BOARDS/`, `DISCOVERIES/`, or `METHOD/`.
They package a point-in-time decision state so future work can proceed without reopening every prior conversation.

Number folders `001_NAME/`. A draft folder may be renamed until [CURRENT.md](CURRENT.md) points at it. After it governs, the name stays. Replace the example milestone folder when the first real milestone exists, and point [CURRENT.md](CURRENT.md) at that folder. Copy `MILESTONE_SUMMARY.md`, `BOARD_SNAPSHOT.md`, and `implementation_artifacts/` into each new folder.

```text
MILESTONES/
  CURRENT.md
  RELEASE_LOG.md
  AREAS.md
  001_NAME/
    MILESTONE_SUMMARY.md
    BOARD_SNAPSHOT.md
    implementation_artifacts/
      README.md
  archive/
    README.md
    RELEASE_LOG.md
```

`BOARD_SNAPSHOT.md` references the living boards in `EXPERIENCE_BOARDS/` and records their reviewed status. It does not duplicate board bodies. Use a `board_snapshot/` folder only when the milestone explicitly needs frozen archival copies.

`implementation_artifacts/` holds milestone-specific translation artifacts. When `PROJECT.yaml` sets `experience_arc` to `true`, they turn approved emotional architecture into prototype build guidance. When it is `false`, the milestone can govern with a governance note, a build brief, and tickets, and without an arc. They are not method essays, raw discoveries, or Experience Boards. The folder may stay empty until the milestone produces build guidance. When `PROJECT.yaml` is missing, this copy predates init, and the arc files bind when they exist.

Do not hardcode a milestone folder name in agent instructions. [CURRENT.md](CURRENT.md) names the governing milestone. Incoming implementation artifacts belong in that milestone's `implementation_artifacts/` folder.

[RELEASE_LOG.md](RELEASE_LOG.md) holds high-level release entries for the governing milestone only. When a milestone is archived, its entries move to `archive/RELEASE_LOG.md`.

[AREAS.md](AREAS.md) names the last file that touched each product area. Use it when troubleshooting. Do not read `archive/` unless `CURRENT.md`, `AREAS.md`, or the user names a file.

---

## For agents

Before starting new work, read `CURRENT.md`. It names one governing milestone. Read only that folder. Do not sort this directory to guess. A later folder may be a review and may not own the implementation artifacts.

If `AGENTS.md` names a milestone folder, or tells an agent to sort `MILESTONES/`, and `CURRENT.md` is missing or names a different folder, stop. The agent file is stale. Do not guess the newest folder.

If `CURRENT.md` does not name a real milestone folder, stop. `001_EXAMPLE_MILESTONE` is a template. It is not governing.

A milestone cannot become governing until it has `MILESTONE_SUMMARY.md` and a short still-in-force list. That list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in `AREAS.md`. A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not point `CURRENT.md` at the folder until that list is written. Do not copy another product's exclusions into the list.

A quality pass restates the milestone's job. A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first. This is an implementation stop.

Read the milestone's `MILESTONE_SUMMARY.md`, including its release entries, for governing root truth sources, and `BOARD_SNAPSHOT.md` for the reviewed state of `EXPERIENCE_BOARDS/`. Do not treat milestone files as replacements for those root artifacts.

Do not read any other milestone folder, `archive/`, or `archive/RELEASE_LOG.md`.

When working from an HTDD milestone, read the milestone's `implementation_artifacts/` folder before creating tickets, specs, UI, or code.

Those named files are binding when they exist. The folder can be empty.

Treat `IMPLEMENTATION_GOVERNANCE_NOTE.md` as the entrypoint.
Treat `PROTOTYPE_BUILD_BRIEF.md` as the build-facing summary.
Treat `PROTOTYPE_IMPLEMENTATION_TICKETS.md` as the ticket source, but do not implement tickets that conflict with the governance files.

`PROTOTYPE_STATE_MAP.md`, `TRANSITION_SPEC.md`, `GUARDRAIL_CHECKLIST.md`, and `PROTOTYPE_REVIEW_SCRIPT.md` bind only when `PROJECT.yaml` sets `experience_arc` to `true`. When it is `false`, those files are not required. Do not invent an arc, a beat, a gift, or an Arc Steward to fill them. When `PROJECT.yaml` is missing, they bind when they exist.

Notes below that name an arc, a beat, a gift, Product Gravity, or an Arc Steward apply when `experience_arc` is `true`. When it is `false`, skip those notes. Exclusions, the status record, and the ticket completion classes still apply.

If the bootstrap named in `PROJECT.yaml` is incomplete and this milestone's implementation artifact chain is complete, proceed from the chain. If `PROJECT.yaml` is missing, that bootstrap is `PROJECT_BOOTSTRAP.md`. Do not invent founder or team meaning to fill it.

When markdown governance and code comments drift, markdown governance wins. Code comments are local implementation notes, not source-of-truth artifacts.

Named Product Gravity is an implementation tool. A refusal must name the ordinary product move being refused and the positive designed object that replaces it. A refusal is not an empty screen. Warmer copy is the same check. Reassurance (“that’s okay”) and a pointer at future contribution are ordinary product moves inside an empty moment the experience was meant to hold.

Review questions in `PROTOTYPE_REVIEW_SCRIPT.md` may be used during build as decision checks, not only at final QA.

Observed, not doctrine: time-based fallbacks in a Transition Spec are not readiness. If the fallback cannot be lingered in, it will feel like a funnel. Review chrome must stay labeled as a method tool. Edge transitions into, out of, and back into the arc need their own ticket shape. Green tests prove absence; they do not replace Arc Steward playback. A defect stays inside the current shell and the current beat. It does not become a new surface, a new product, or a new beat. Adding product so the work feels finished starts the backlog again.

Follow the ticket lifecycle in `AGENTS.md`. Every ticket names one completion class and closes inside that class. A ticket names what it will not absorb, including the next product slice. That edge is what lets one issue and one branch finish. Deferred human validation stays on the milestone validation ticket. Maintain the status record on this milestone's `MILESTONE_SUMMARY.md`, and cite it for test counts. Whether work is done is read from that record and the merged pull requests. A chat or a session capture is not the lasting record. A change to a sentence, a route purpose, or an access rule that appears in a governing contract is a contract change. The same change updates the milestone status record. Code that disagrees with the contract is not done. Updating a test to match warmer copy, without that record, is a contract change done backwards. A ticket is not implemented while a test that locks its contract is red. A follow-up commit that fixes a syntax error, a crash, or a dependency pin from the previous pull request means that pull request did not close. A skipped reproducer is an open finding: blocker, owning ticket, removal condition, and status. Automated checks are not approval by a named human reviewer, including the Arc Steward. A participant-testing candidate demonstrates the end-to-end product journey. Participant evidence stays outside Git.

## Release entries

When a milestone is completed, or materially updated, write a short entry under `Release` in its `MILESTONE_SUMMARY.md` and append the same entry to `RELEASE_LOG.md`. Newest first.

Each entry names the date, the folder, and the kind: completed or updated. The work is a few sentences. It names areas touched. It does not copy tickets, specs, or board bodies.

On completion, say what is still in force, or which living root file absorbed it: a principle, a board, or a lesson. Name the predecessor folder when this milestone replaced one. A sentence that only names the predecessor is not that list. The list names the exclusions this product binds. A first milestone names the exclusions it binds. Do not copy another product's exclusions into the list.

`RELEASE_LOG.md` holds only the governing milestone. Build work reads the milestone, not the log.

## Archive

Archive a milestone only when a new milestone is governing, and every decision that still binds is restated on the new release entry or named as absorbed into a living root file. If the only copy of a binding decision lives in the closed milestone, `AREAS.md` must point at that file.

Then:

1. Move the closed folder to `archive/`.
2. Move its entries from `RELEASE_LOG.md` to `archive/RELEASE_LOG.md`.
3. Point `CURRENT.md` at the new governing folder only after its still-in-force list is written.
4. Update `AREAS.md` for areas the closed milestone last touched.

Do not reopen earlier design decisions unless:

- a contradiction is found
- a Human Truth conflicts with implementation reality
- a new milestone explicitly requires review
- the user asks for reconsideration

When a later phase meets an excluded move again, withhold or retire it. Confirming the exclusion does not reopen the design, and the old surface does not become the next brief.

When one of those applies, start from the governing milestone. Name the area. Open only the file `AREAS.md` names. If that file does not explain the failure, read that milestone's release entry, then the one predecessor it names. Stop there unless the user names another folder.
