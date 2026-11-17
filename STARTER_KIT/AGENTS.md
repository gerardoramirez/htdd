# Agent Instructions

This is the operational instruction file for work in this folder.

## Init

On a new copy, start at `INIT.md`. `PROJECT.yaml` holds `builder`, `bootstrap`, and `experience_arc`. A person sets them. You may record an answer. You may not choose one, rank `skilled_builder` above `learning_the_ropes`, or nudge toward either label.

If any of those three values is `unset`, or is not one of the allowed values, stop. Read only `INIT.md`. Do not fill a bootstrap, do not draft a milestone, and do not invent meaning.

`builder` is a record for later guidance. It does not choose the bootstrap and it does not choose the artifact chain. Do not write a second set of rules from it.

When `bootstrap` is `founder`, the bootstrap is `PROJECT_BOOTSTRAP.md`. When it is `internal_b2b`, the bootstrap is `PROJECT_BOOTSTRAP_INTERNAL.md`. Leave the other file as the blank template. Do not copy answers across.

When `experience_arc` is `true`, the arc files named below bind once a milestone governs. When it is `false`, those files are not required. Do not invent an arc, a beat, a gift, or an Arc Steward to fill them. The milestone summary says this milestone is not an experience arc.

If `PROJECT.yaml` is missing, this copy was made before init. Do not treat the absence as `experience_arc: false`. Follow the rules below. Do not invent a `PROJECT.yaml` that turns the arc off. A person may add the file later without overwriting filled work.

An `[open]` mark is an unanswered line. Do not close it by writing an answer.

## Day one

Before a governing milestone exists, follow `INIT.md`, then only the bootstrap it names, then `HUMAN_TRUTH_DISCOVERY.md`. Do not implement from `001_EXAMPLE_MILESTONE`. A draft milestone folder may be renamed until `MILESTONES/CURRENT.md` points at it.

## Once a milestone is governing

Before doing implementation work, read `MILESTONES/CURRENT.md`. It names one governing milestone. Read only that folder.

Do not hardcode a milestone folder name from memory or from an older copy of this file. Do not sort `MILESTONES/` to guess. Do not read any other milestone folder, `MILESTONES/archive/`, or `MILESTONES/archive/RELEASE_LOG.md`.

## Implementation stops

Operating rules. Not a Human Truth.

If this file names a milestone folder, or tells an agent to sort `MILESTONES/`, and `MILESTONES/CURRENT.md` is missing or names a different folder, stop. The agent file is stale. Do not guess the newest folder.

If `MILESTONES/CURRENT.md` says there is no governing milestone yet, stop. The example folder shipped with the kit is a template. Do not implement from it.

A milestone cannot become governing until it has `MILESTONE_SUMMARY.md` and a short still-in-force list. That list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in `MILESTONES/AREAS.md`. A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not point `CURRENT.md` at the folder until that list is written. Do not copy another product's exclusions into the list.

A quality pass restates the milestone's job. A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first. This is an implementation stop.

Then read:

1. `SOURCE.md`
2. The bootstrap `PROJECT.yaml` names. `founder` is `PROJECT_BOOTSTRAP.md`. `internal_b2b` is `PROJECT_BOOTSTRAP_INTERNAL.md`. If `PROJECT.yaml` is missing, read `PROJECT_BOOTSTRAP.md`.
3. That milestone's `MILESTONE_SUMMARY.md`, including its release entries, and `BOARD_SNAPSHOT.md`
4. That milestone's `implementation_artifacts/` folder, when it exists

Treat `IMPLEMENTATION_GOVERNANCE_NOTE.md` as the entrypoint.
Treat `PROTOTYPE_BUILD_BRIEF.md` as the build-facing summary.
Treat `PROTOTYPE_IMPLEMENTATION_TICKETS.md` as the ticket source, but do not implement tickets that conflict with the governance files.

`PROTOTYPE_STATE_MAP.md`, `TRANSITION_SPEC.md`, `GUARDRAIL_CHECKLIST.md`, and `PROTOTYPE_REVIEW_SCRIPT.md` bind only when `PROJECT.yaml` sets `experience_arc` to `true`. When it is `false`, those files are not required. Do not invent an arc to fill them. When `PROJECT.yaml` is missing, they bind when they exist.

Notes in this file that name an arc, a beat, a gift, Product Gravity, or an Arc Steward apply when `experience_arc` is `true`. When it is `false`, skip those notes. Exclusions, the status record, and the ticket completion classes still apply.

Incoming implementation artifacts belong in the governing milestone's `implementation_artifacts/` folder. Do not put them in `METHOD/`, `HUMAN_TRUTHS/`, `EXPERIENCE_BOARDS/`, or a guessed later milestone folder.

## Incomplete bootstrap

If the named bootstrap is incomplete and the governing milestone's implementation artifact chain is complete, proceed from that chain.

Do not invent founder experience, team experience, human impact, or success language to fill the bootstrap. Incomplete bootstrap is later human work. It is not an implementation blocker when the milestone chain is already complete.

If both the bootstrap and the milestone chain are incomplete, stop. Do not invent governing meaning.

## Authority

`METHOD/` teaches HTDD. Do not write product work there.

`HUMAN_TRUTHS/` contains this project's truths only. It is not the canonical HTDD registry.

When markdown governance and code comments drift, markdown governance wins. Code comments are local implementation notes, not source-of-truth artifacts.

Do not reopen earlier design decisions unless a contradiction is found, a Human Truth conflicts with implementation reality, a new milestone explicitly requires review, or the user asks for reconsideration.

When a later phase meets an excluded move again, withhold or retire it. Confirming the exclusion does not reopen the design, and the old surface does not become the next brief.

When one of those exceptions applies, start from the governing milestone. Name the area. Read `MILESTONES/AREAS.md` and open only the file it names. If that file does not explain the failure, read that milestone's release entry, then the one predecessor it names. Stop there unless the user names another folder.

## Release and archive

When a milestone is completed or materially updated, write a short release entry in its `MILESTONE_SUMMARY.md` and append the same entry to `MILESTONES/RELEASE_LOG.md`. That log holds only the governing milestone's entries. Build work reads the milestone, not the log.

Archive a milestone only when a new milestone is governing, and every decision that still binds is restated on the new release entry or named as absorbed into a living root file. If the only copy of a binding decision lives in the closed milestone, `MILESTONES/AREAS.md` must point at that file.

Then move the closed folder to `MILESTONES/archive/`, move its release entries to `MILESTONES/archive/RELEASE_LOG.md`, point `CURRENT.md` at the new folder only after its still-in-force list is written, and update `AREAS.md` for areas the closed milestone last touched.

## Build-time rules

Named Product Gravity is an implementation tool. The named failure mode is often more useful than the feature list. Use it to make ordinary product moves visibly wrong before they are built.

A refusal pattern must name the ordinary product move being refused and the positive designed object that replaces it. A refusal is not an empty screen. Residue can be atmosphere; it cannot be chrome.

Warmer copy is a Product Gravity check. A refusal or a replacement names the ordinary product move and the positive designed object. Reassurance (“that’s okay”) and a pointer at future contribution are ordinary product moves inside an empty moment the experience was meant to hold.

Copy that explains restraint can keep the product central. Treat self-explaining restraint as a Product Gravity risk.

As the relationship becomes more central, product language and chrome should recede.

Review questions in `PROTOTYPE_REVIEW_SCRIPT.md` may be used during build as decision checks, not only at final QA. A review question can prevent a false "done."

## Ticket lifecycle

Observed from practice. Operating rules for how work closes. Not a Human Truth.

Every ticket names one completion class: Specification, Implementation, Automated verification, Human validation, or Freeze or handoff.

A ticket names what it will not absorb, including the next product slice. That edge is what lets one issue and one branch finish.

Record state as Implemented, Automatically verified, Ready for validation, Human validated, or Accepted. A later state is not a name for an earlier event.

Close an implementation ticket when its implementation and automated acceptance criteria pass. A ticket is not implemented while a test that locks its contract is red. Deferred human validation stays on the milestone validation ticket. It stays visible there. It does not keep the implementation ticket open.

A change to a sentence, a route purpose, or an access rule that appears in a governing contract is a contract change. The same change updates the milestone status record. Code that disagrees with the contract is not done. Updating a test to match warmer copy, without that record, is a contract change done backwards.

A follow-up pull request states whether it completes a ticket, repairs a finding, adds evidence, or changes the governing contract. A follow-up commit that fixes a syntax error, a crash, or a dependency pin from the previous pull request means that pull request did not close.

Keep one status record on the governing milestone's `MILESTONE_SUMMARY.md`: dependency order, merged pull requests, open findings, deferred validation, the latest authoritative test counts, the freeze candidate, and the accepted freeze. Evidence notes cite that record.

Whether work is done is read from that record and the merged pull requests. A chat or a session capture is not the lasting record.

Simulator, device, assistive-technology, and named-reviewer checks belong on that validation ticket unless one feature is unusually high risk.

Before a group of production surfaces is built, one governing contract specifies purpose, hierarchy, states, language, accessibility, and visual components. Do not open a second documentation ticket that restates it.

A participant-testing candidate demonstrates the intended end-to-end product journey. A freeze of one portion, including the emotional arc alone, is not that candidate.

A skipped reproducer is a finding. Name its blocker, owning ticket, removal condition, and status.

Automated checks can establish behavior and guardrails. They are not approval by a named human reviewer, including the Arc Steward. A project names its own reviewers. Record that judgment only when that person has made it.

Participant evidence stays outside Git. Keep implementation and evidence on separate branches. Record the exact commit and freeze identifier a review used.

## Observed build warnings

These are practice notes, not finalized doctrine.

An Experience Gift that occurs outside the product still needs a governed threshold, or the last screen will become a completion page.

Refusal patterns can prevent the wrong product, but they do not by themselves prove the right emotional experience. Green tests prove absence. They do not replace Arc Steward playback.

Progressive recession of UI is a valid implementation of decreasing product centrality. Each beat should justify every remaining word.

Time can stand in for readiness in a prototype, but it is not readiness. If a time-based fallback cannot be lingered in, it will feel like a funnel.

Review chrome is a method tool. Keep it labeled as such, or the prototype starts teaching the visitor a procedure.

Edge transitions into, out of, and back into the arc need their own ticket shape, or they will be rebuilt twice.

If a Human Truth forbids invention, representative content is a closed source kit. Narration may restore, read, organize, or compose from that kit. It must not become a plausible story about the person.

When documents conflict, later ranked implementation governance may be stricter than an Experience Board. Do not silently prefer the warmer document.

When a governance trigger calls for a DDR and the DDR does not exist, proceed only if the ranked implementation chain gives enough authority. Record the missing DDR as an explicit gap.

A defect stays inside the current shell and the current beat. It does not become a new surface, a new product, or a new beat. Adding product so the work feels finished starts the backlog again.
