# HTDD Starter Kit

This folder is everything a product needs to begin Human Truth Driven Design.

Copy it into the product repository. From that moment the product owns the files at the kit root. The methodology repository stays the source of philosophy and practice. A reserved [METHOD/](METHOD/) folder is where those essays copy in later, without touching project work.

The files in this kit do not assume a path. They work wherever the team keeps product writing.

---

## What to copy

Copy the contents of this folder, including `METHOD/`.

Do not copy `FOUNDATIONS/`, `METHODOLOGY/`, the canonical `HUMAN_TRUTHS/` registry, `CASE_STUDIES/`, or the methodology `DISCOVERIES/` log into the kit root. Those remain in the HTDD repository until they are ready. Then they copy into [METHOD/](METHOD/). [SOURCE.md](SOURCE.md) points at the origin.

---

## How to add this kit to a project

1. Copy this folder into the product repo's `docs/` directory, then rename `STARTER_KIT` to `htdd` so the work lives at `docs/htdd/`.

   ```text
   cp -R STARTER_KIT path/to/docs/
   mv path/to/docs/STARTER_KIT path/to/docs/htdd
   ```

   Also valid: `docs/`, `htdd/`, `design/htdd/`, or any path the team already uses. If you choose one of those, change the name in the commands above.

2. Fill in `SOURCE.md` with the copy date and, optionally, the commit or tag of the methodology repository.

3. Add one sentence to the **product** README so people and agents can find the work:

   > Human Truth work lives in `docs/htdd/`.

   Change the path in that sentence if you chose a different destination.

4. Start at `PROJECT_BOOTSTRAP.md`. Agents start at `AGENTS.md`.

Do not copy this kit over a folder that already has project work.

---

## After the copy

| File | Purpose |
| --- | --- |
| [SOURCE.md](SOURCE.md) | Origin of this copy and a pointer to the methodology |
| [AGENTS.md](AGENTS.md) | How agents find governing artifacts and avoid collisions |
| [PROJECT_BOOTSTRAP.md](PROJECT_BOOTSTRAP.md) | Founder experience and meaning research |
| [HUMAN_TRUTH_DISCOVERY.md](HUMAN_TRUTH_DISCOVERY.md) | Draft workbook for evidence, candidate truths, and product principles |
| [HUMAN_TRUTHS/](HUMAN_TRUTHS/) | This project's truths, not the canonical registry |
| [PRODUCT_PRINCIPLES.md](PRODUCT_PRINCIPLES.md) | What this product must honor because of its truths |
| [ETHICAL_AI_PRINCIPLES.md](ETHICAL_AI_PRINCIPLES.md) | What this product's AI must honor and refuse |
| [EXPERIENCE_BOARDS/](EXPERIENCE_BOARDS/) | Living canonical boards. Milestones reference them. |
| [DISCOVERIES/](DISCOVERIES/) | Realizations from this product |
| [MILESTONES/](MILESTONES/) | Approved phases of product understanding and implementation |
| [CHECKLISTS/](CHECKLISTS/) | Optional working lists |
| [LESSONS_LEARNED.md](LESSONS_LEARNED.md) | What this product taught the team |
| [METHOD/](METHOD/) | Reserved snapshot of HTDD method essays. No product writing. |

---

## For agents

Start at [AGENTS.md](AGENTS.md). Do not hardcode a milestone folder name.

Root folders contain living canonical project truth.
Milestone folders contain reviewed context, decisions, snapshots, and implementation artifacts for a specific phase.
A milestone must not silently fork or replace a canonical root artifact.

Before starting new work, read [MILESTONES/CURRENT.md](MILESTONES/CURRENT.md). It names one governing milestone. Read only that folder. Incoming implementation artifacts belong in that milestone's `implementation_artifacts/` folder, not in a guessed later folder.

If `AGENTS.md` names a milestone folder, or tells an agent to sort `MILESTONES/`, and `MILESTONES/CURRENT.md` is missing or names a different folder, stop. The agent file is stale. Do not guess the newest folder.

If `MILESTONES/CURRENT.md` does not name a real milestone folder, stop. `001_EXAMPLE_MILESTONE` is a template. It is not governing.

A milestone cannot become governing until it has `MILESTONE_SUMMARY.md` and a short still-in-force list. That list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in [MILESTONES/AREAS.md](MILESTONES/AREAS.md). A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not point `CURRENT.md` at the folder until that list is written. Do not copy another product's exclusions into the list.

A quality pass restates the milestone's job. A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first. This is an implementation stop.

Read the milestone's `MILESTONE_SUMMARY.md`, including its release entries, for governing root truth sources, and `BOARD_SNAPSHOT.md` for the reviewed state of [EXPERIENCE_BOARDS/](EXPERIENCE_BOARDS/). Do not treat milestone files as replacements for those root artifacts.

Do not read any other milestone folder, `MILESTONES/archive/`, or the archived release log. `MILESTONES/RELEASE_LOG.md` holds high-level entries for the governing milestone only. `MILESTONES/AREAS.md` names the last file for each area when troubleshooting.

When working from an HTDD milestone, read the milestone's `implementation_artifacts/` folder before creating tickets, specs, UI, or code.

Those named files are binding when they exist. The folder can be empty.

Treat `IMPLEMENTATION_GOVERNANCE_NOTE.md` as the entrypoint.
Treat `PROTOTYPE_STATE_MAP.md`, `TRANSITION_SPEC.md`, `GUARDRAIL_CHECKLIST.md`, and `PROTOTYPE_REVIEW_SCRIPT.md` as binding prototype governance.
Treat `PROTOTYPE_BUILD_BRIEF.md` as the build-facing summary.
Treat `PROTOTYPE_IMPLEMENTATION_TICKETS.md` as the ticket source, but do not implement tickets that conflict with the governance files.

If `PROJECT_BOOTSTRAP.md` is incomplete and the governing milestone's implementation artifact chain is complete, proceed from that chain. Do not invent founder meaning to fill the bootstrap.

When markdown governance and code comments drift, markdown governance wins. Code comments are local implementation notes, not source-of-truth artifacts.

Do not write product work into [METHOD/](METHOD/). Do not treat this project's [HUMAN_TRUTHS/](HUMAN_TRUTHS/) as the canonical HTDD registry.

Named Product Gravity is an implementation tool. A refusal or a replacement names the ordinary product move and the positive designed object. Warmer copy is the same check. Reassurance (“that’s okay”) and a pointer at future contribution are ordinary product moves inside an empty moment the experience was meant to hold. Review questions may be used during build, not only at final QA.

A change to a sentence, a route purpose, or an access rule that appears in a governing contract is a contract change. The same change updates the milestone status record. Code that disagrees with the contract is not done. Updating a test to match warmer copy, without that record, is a contract change done backwards. A ticket is not implemented while a test that locks its contract is red. A follow-up commit that fixes a syntax error, a crash, or a dependency pin from the previous pull request means that pull request did not close.

Observed, not doctrine: refusals prevent the wrong product; they do not prove the right emotional experience. Time can proxy readiness, but it is not readiness. Review chrome must stay labeled. Green tests do not replace Arc Steward playback. A ticket names one completion class and closes inside that class. A ticket names what it will not absorb, including the next product slice. That edge is what lets one issue and one branch finish. Whether work is done is read from the milestone status record and the merged pull requests. A chat or a session capture is not the lasting record. Deferred human validation stays on the milestone validation ticket. Automated checks are not named-reviewer approval. Participant evidence stays outside Git. A participant-testing candidate demonstrates the end-to-end product journey. A defect stays inside the current shell and the current beat. It does not become a new surface, a new product, or a new beat. Adding product so the work feels finished starts the backlog again.

Do not reopen earlier design decisions unless:

- a contradiction is found
- a Human Truth conflicts with implementation reality
- a new milestone explicitly requires review
- the user asks for reconsideration

When a later phase meets an excluded move again, withhold or retire it. Confirming the exclusion does not reopen the design, and the old surface does not become the next brief.

When one of those applies, start from the governing milestone. Name the area. Open only the file `MILESTONES/AREAS.md` names. If that file does not explain the failure, read that milestone's release entry, then the one predecessor it names.

---

## Updating

Three kinds of change. They are handled differently.

**Method snapshot.** When `FOUNDATIONS/`, `METHODOLOGY/`, the canonical `HUMAN_TRUTHS/`, or `DISCOVERIES/` in the HTDD repository are ready, copy those trees into the matching children of `METHOD/`. Same folder names. Do not copy `STARTER_KIT/`, `CASE_STUDIES/`, or the HTDD root README. It is safe to refresh `METHOD/` the same way later. Those paths must not contain product work.

```text
cp -R FOUNDATIONS/.   path/to/docs/htdd/METHOD/FOUNDATIONS/
cp -R METHODOLOGY/.   path/to/docs/htdd/METHOD/METHODOLOGY/
cp -R HUMAN_TRUTHS/.  path/to/docs/htdd/METHOD/HUMAN_TRUTHS/
cp -R DISCOVERIES/.   path/to/docs/htdd/METHOD/DISCOVERIES/
```

**Kit templates.** If the starter kit later adds a root folder or new fields on a blank template, compare `STARTER_KIT/` at a newer commit with this folder. Copy only new blank files or empty sections. Never overwrite filled `PROJECT_BOOTSTRAP.md`, project truths, boards, discoveries, milestones, or lessons. Then update the date and commit in `SOURCE.md`.

**Do not** copy the whole kit over this folder again. That would erase project work.

## Existing product repositories

Projects that already copied the kit do not receive later operating rules by refreshing `METHOD/`.

Add `MILESTONES/CURRENT.md`, `MILESTONES/AREAS.md`, and `MILESTONES/RELEASE_LOG.md` if they are missing. Point `CURRENT.md` only after the new milestone names the exclusions this product binds. Replace any `AGENTS.md` that hardcodes a milestone folder with the current `AGENTS.md`. If an older copy tells every project to bind another product's exclusions, replace that sentence with this product's own list. Do not overwrite filled milestone work.

Methodology: https://github.com/gerardoramirez/htdd
