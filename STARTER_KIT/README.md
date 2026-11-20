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

4. A person starts at `INIT.md` and answers there before either bootstrap. Agents start at `AGENTS.md`, which sends them to `INIT.md` while `PROJECT.yaml` is still unset.

Do not copy this kit over a folder that already has project work.

---

## The first week

`INIT.md` is the first sitting. It asks three questions and records the answers in `PROJECT.yaml`. A person answers. An agent may write the answer down and may not choose it.

When all three values are set:

1. Open only the bootstrap `INIT.md` names. `founder` uses `PROJECT_BOOTSTRAP.md`. `internal_b2b` uses `PROJECT_BOOTSTRAP_INTERNAL.md`. Leave the other file blank.
2. Continue in `HUMAN_TRUTH_DISCOVERY.md`. Separate what someone lived from what the team infers.
3. Copy `MILESTONES/001_EXAMPLE_MILESTONE` to a draft folder. Renaming that folder is fine until `MILESTONES/CURRENT.md` points at it.
4. A human writes the exclusions this product binds. `CURRENT.md` stays at "None yet." until that list exists. A decision to do something later is written under Deferred on the milestone summary. It is not an exclusion.

---

## After the copy

| File | Purpose |
| --- | --- |
| [SOURCE.md](SOURCE.md) | Origin of this copy and a pointer to the methodology |
| [INIT.md](INIT.md) | First sitting. A person sets the project type |
| [PROJECT.yaml](PROJECT.yaml) | Record of those answers. Agents do not infer them |
| [AGENTS.md](AGENTS.md) | How agents find governing artifacts and avoid collisions |
| [PROJECT_BOOTSTRAP.md](PROJECT_BOOTSTRAP.md) | Founder experience and meaning research. Used when `bootstrap` is `founder` |
| [PROJECT_BOOTSTRAP_INTERNAL.md](PROJECT_BOOTSTRAP_INTERNAL.md) | Team, internal, and indirect-chain meaning research. Used when `bootstrap` is `internal_b2b` |
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

### Day one

Start at [INIT.md](INIT.md) while any value in [PROJECT.yaml](PROJECT.yaml) is `unset` or unknown. Read only that page. A person answers. You may record the answer. You may not choose it, rank `skilled_builder` above `learning_the_ropes`, or nudge toward either label.

`builder` is kept for later guidance. It does not choose the bootstrap, and it does not choose the artifact chain. Do not write a second set of rules from it.

When the values are set, read only the bootstrap `INIT.md` names. Leave the other bootstrap as the blank template. Do not invent meaning to fill either page. Do not implement from `001_EXAMPLE_MILESTONE`.

If the repository already contains a product, read [When the product already exists](#when-the-product-already-exists). Do not fill the bootstrap from the code. Do not treat an existing spec as governing, or as the answer to an `[open]`.

If `PROJECT.yaml` is missing, this copy was made before init. Absence is not `experience_arc: false`. Follow the governing rules below. Do not invent a `PROJECT.yaml` that turns the arc off. A person may add `INIT.md` and `PROJECT.yaml` later without overwriting filled work.

### Once a milestone is governing

Start at [AGENTS.md](AGENTS.md). Do not hardcode a milestone folder name.

Root folders contain living canonical project truth.
Milestone folders contain reviewed context, decisions, snapshots, and implementation artifacts for a specific phase.
A milestone must not silently fork or replace a canonical root artifact.

Before starting new work, read [MILESTONES/CURRENT.md](MILESTONES/CURRENT.md). It names one governing milestone. Read only that folder. Incoming implementation artifacts belong in that milestone's `implementation_artifacts/` folder, not in a guessed later folder.

If `AGENTS.md` names a milestone folder, or tells an agent to sort `MILESTONES/`, and `MILESTONES/CURRENT.md` is missing or names a different folder, stop. The agent file is stale. Do not guess the newest folder.

If `MILESTONES/CURRENT.md` does not name a real milestone folder, stop. `001_EXAMPLE_MILESTONE` is a template. It is not governing.

A milestone cannot become governing until it has `MILESTONE_SUMMARY.md` and a short still-in-force list. That list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in [MILESTONES/AREAS.md](MILESTONES/AREAS.md). A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not point `CURRENT.md` at the folder until that list is written. Do not copy another product's exclusions into the list.

A Deferred section is a decision to do something later. Do not build it inside the governing milestone, and do not move it into the still-in-force list. It is not an `[open]` line, and it is not deferred validation in the status record.

A quality pass restates the milestone's job. A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first. This is an implementation stop.

Read the milestone's `MILESTONE_SUMMARY.md`, including its release entries, for governing root truth sources, and `BOARD_SNAPSHOT.md` for the reviewed state of [EXPERIENCE_BOARDS/](EXPERIENCE_BOARDS/). Do not treat milestone files as replacements for those root artifacts.

Do not read any other milestone folder, `MILESTONES/archive/`, or the archived release log. `MILESTONES/RELEASE_LOG.md` holds high-level entries for the governing milestone only. `MILESTONES/AREAS.md` names the last file for each area when troubleshooting.

When working from an HTDD milestone, read the milestone's `implementation_artifacts/` folder before creating tickets, specs, UI, or code.

Those named files are binding when they exist. The folder can be empty.

Treat `IMPLEMENTATION_GOVERNANCE_NOTE.md` as the entrypoint.
Treat `PROTOTYPE_BUILD_BRIEF.md` as the build-facing summary.
Treat `PROTOTYPE_IMPLEMENTATION_TICKETS.md` as the ticket source, but do not implement tickets that conflict with the governance files.

`PROTOTYPE_STATE_MAP.md`, `TRANSITION_SPEC.md`, `GUARDRAIL_CHECKLIST.md`, and `PROTOTYPE_REVIEW_SCRIPT.md` bind only when `PROJECT.yaml` sets `experience_arc` to `true`. When it is `false`, those files are not required. Do not invent an arc, a beat, a gift, or an Arc Steward to fill them. When `PROJECT.yaml` is missing, they bind when they exist.

Notes below that name an arc, a beat, a gift, Product Gravity, or an Arc Steward apply when `experience_arc` is `true`. When it is `false`, skip those notes. Exclusions, the status record, and the ticket completion classes still apply.

If the named bootstrap is incomplete and the governing milestone's implementation artifact chain is complete, proceed from that chain. Do not invent founder or team meaning to fill the bootstrap.

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

**Kit templates.** If the starter kit later adds a root folder or new fields on a blank template, compare `STARTER_KIT/` at a newer commit with this folder. Copy only new blank files or empty sections. Never overwrite filled `PROJECT_BOOTSTRAP.md`, `PROJECT_BOOTSTRAP_INTERNAL.md`, `PROJECT.yaml`, project truths, boards, discoveries, milestones, or lessons. Then update the date and commit in `SOURCE.md`.

**Do not** copy the whole kit over this folder again. That would erase project work.

## When the product already exists

The copy steps above still apply. Do not copy this kit over a folder that already has project work. The bootstrap does not have to narrate the app that is already running.

A person may label what is already in the repository. An agent does not choose the label.

- **Baseline.** The product that already runs, and the documents that describe it. Baseline is not a Human Truth, and it is not a milestone decision.
- **Evidence.** Something a person lived, or the team observed. It can be cited from `HUMAN_TRUTH_DISCOVERY.md`. Age does not make it governing.
- **Governing.** Only what a milestone names: the truth sources, the principles, and the exclusions. An existing spec, ticket, or design document does not govern because it is present.

Why and guardrails live in this folder. What the product does, and how it is built, stay in the product's own specs. Those specs remain the source for mechanism. They do not choose the milestone.

If a spec disagrees with an exclusion or a principle, stop and ask a person. Do not fill the bootstrap from the code. Do not treat the code as the answer to an `[open]`.

Classifying old documents is not a gate. A milestone still governs only after a human writes the still-in-force list.

## Existing product repositories

This note is for a copy that already has the kit. A product that predates the kit follows [When the product already exists](#when-the-product-already-exists).

Projects that already copied the kit do not receive later operating rules by refreshing `METHOD/`.

Add `MILESTONES/CURRENT.md`, `MILESTONES/AREAS.md`, and `MILESTONES/RELEASE_LOG.md` if they are missing. Point `CURRENT.md` only after the new milestone names the exclusions this product binds. Replace any `AGENTS.md` that hardcodes a milestone folder with the current `AGENTS.md`. If an older copy tells every project to bind another product's exclusions, replace that sentence with this product's own list. Do not overwrite filled milestone work.

A later kit may add a blank Deferred heading, or room on the internal bootstrap for more than one audience. Copy those empty lines by hand. Do not overwrite a filled bootstrap, a filled exclusion list, or a decision a person already wrote. Do not invent an audience, a boundary, or a deferral to fill them.

A copy that already governs does not need `PROJECT.yaml` to keep going. Missing `PROJECT.yaml` is not `experience_arc: false`. A person may add `INIT.md` and `PROJECT.yaml` beside the filled bootstrap and set `bootstrap` to match the page already in use. Do not overwrite that page, and do not invent `experience_arc: false` for a milestone that already uses the arc files.

Methodology: https://github.com/gerardoramirez/htdd
