# Implementation artifacts

This folder holds milestone-specific translation artifacts.

When `PROJECT.yaml` sets `experience_arc` to `true`, they turn the approved emotional architecture of this milestone into prototype build guidance. When it is `false`, this folder does not need an arc. When `PROJECT.yaml` is missing, this copy predates init, and the arc files bind when they exist.

They are not:

- canonical HTDD method essays
- raw discoveries
- individual Experience Boards

The folder may stay empty until this milestone produces build guidance. Do not add files here just to fill the pattern.

A later milestone may add some or all of these files.

Every milestone that produces build guidance:

| File | Role |
| --- | --- |
| `IMPLEMENTATION_GOVERNANCE_NOTE.md` | Entrypoint |
| `PROTOTYPE_BUILD_BRIEF.md` | Build-facing summary |
| `PROTOTYPE_IMPLEMENTATION_TICKETS.md` | Ticket source |

Only when `PROJECT.yaml` sets `experience_arc` to `true`. When it is `false`, the files in this second group are not required. Do not invent them. When `PROJECT.yaml` is missing, they bind when they exist.

| File | Role |
| --- | --- |
| `PROTOTYPE_STATE_MAP.md` | Binding prototype governance |
| `TRANSITION_SPEC.md` | Binding prototype governance |
| `GUARDRAIL_CHECKLIST.md` | Binding prototype governance |
| `PROTOTYPE_REVIEW_SCRIPT.md` | Binding prototype governance |

Notes below that name an arc, a beat, a gift, Product Gravity, or an Arc Steward apply when `experience_arc` is `true`. When it is `false`, skip those notes. Exclusions, the status record, and the ticket completion classes still apply.

Copy this README into each new milestone's `implementation_artifacts/` folder.

When these files exist, they should make ordinary product moves visibly wrong before implementation begins.

A named Product Gravity failure mode is an implementation tool, not only a review label. It is often more useful than the feature list.

A refusal pattern must name both the ordinary product move being refused and the positive designed object that replaces it. A refusal is not an empty screen. Residue can be atmosphere; it cannot be chrome.

Warmer copy is a Product Gravity check. A refusal or a replacement names the ordinary product move and the positive designed object. Reassurance (“that’s okay”) and a pointer at future contribution are ordinary product moves inside an empty moment the experience was meant to hold.

Copy that explains restraint can keep the product central. Treat self-explaining restraint as a Product Gravity risk.

As the relationship becomes more central, product language and chrome should recede.

Review questions in `PROTOTYPE_REVIEW_SCRIPT.md` may be used during build as decision checks, not only at final QA.

Implementation stops:

- A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first.
- A change to a sentence, a route purpose, or an access rule that appears in a governing contract is a contract change. The same change updates the milestone status record. Code that disagrees with the contract is not done. Updating a test to match warmer copy, without that record, is a contract change done backwards.
- A ticket is not implemented while a test that locks its contract is red. A follow-up commit that fixes a syntax error, a crash, or a dependency pin from the previous pull request means that pull request did not close.

Observed, not doctrine:

- An Experience Gift that occurs outside the product still needs a governed threshold, or the last screen will become a completion page.
- Refusal patterns implement faster than positive gifts. They can prevent the wrong product. They do not prove the right emotional experience.
- Progressive recession of UI is a valid implementation of decreasing product centrality. Each beat should justify every remaining word.
- Time can stand in for readiness in a prototype, but it is not readiness. If a `TRANSITION_SPEC.md` fallback cannot be lingered in, it will feel like a funnel.
- Review chrome is a method tool. Label it as such, or the prototype starts teaching the visitor a procedure.
- Edge transitions into, out of, and back into the arc need their own ticket shape, or they will be rebuilt twice.
- Green tests prove absence. They do not replace Arc Steward playback.
- Every ticket names one completion class: Specification, Implementation, Automated verification, Human validation, or Freeze or handoff. An implementation ticket closes when implementation and automated acceptance criteria pass. Deferred human validation stays on the milestone validation ticket.
- A follow-up pull request states whether it completes a ticket, repairs a finding, adds evidence, or changes the governing contract.
- Simulator, device, assistive-technology, and named-reviewer work belong on one validation ticket unless a feature is unusually high risk.
- Before a group of production surfaces is built, one governing contract specifies purpose, hierarchy, states, language, accessibility, and visual components. Do not open a second ticket that restates it.
- A skipped reproducer names its blocker, owning ticket, removal condition, and status.
- Automated checks are not approval by a named human reviewer, including the Arc Steward. A project names its own reviewers.
- A participant-testing candidate demonstrates the end-to-end product journey. Participant evidence stays outside Git.
- A ticket names what it will not absorb, including the next product slice. That edge is what lets one issue and one branch finish.
- Whether work is done is read from the milestone status record and the merged pull requests. A chat or a session capture is not the lasting record.
- A defect stays inside the current shell and the current beat. It does not become a new surface, a new product, or a new beat.
- Adding product so the work feels finished starts the backlog again.
- When a later phase meets an excluded move again, withhold or retire it. Confirming the exclusion does not reopen the design, and the old surface does not become the next brief.

Do not treat a playable shell as proof that an Experience Gift held. That remains a prototype review question.

If a Human Truth forbids invention, representative content must be authored as entrusted source, not inferred personality. Narration may carry that source. It must not invent warmth.

When documents conflict, the ranked implementation chain may be stricter than an Experience Board. If a DDR is required and missing, proceed only from that chain and record the gap.

---

## For agents

When working from an HTDD milestone, read the milestone's `implementation_artifacts/` folder before creating tickets, specs, UI, or code.

Those named files are binding when they exist. The folder can be empty.

Treat `IMPLEMENTATION_GOVERNANCE_NOTE.md` as the entrypoint.
Treat `PROTOTYPE_BUILD_BRIEF.md` as the build-facing summary.
Treat `PROTOTYPE_IMPLEMENTATION_TICKETS.md` as the ticket source, but do not implement tickets that conflict with the governance files.

`PROTOTYPE_STATE_MAP.md`, `TRANSITION_SPEC.md`, `GUARDRAIL_CHECKLIST.md`, and `PROTOTYPE_REVIEW_SCRIPT.md` bind only when `PROJECT.yaml` sets `experience_arc` to `true`. When it is `false`, those files are not required. When `PROJECT.yaml` is missing, they bind when they exist.
