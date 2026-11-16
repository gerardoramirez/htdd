# Prototype Practice

This page is a guide for building and reviewing a prototype without losing the Human Truth that inspired it.

It is not a claim that a playable shell has validated the experience.

---

## The artifact chain

When a milestone is ready to be built, HTDD translates emotional architecture through a chain:

```text
Experience Boards
        ↓
State Map
        ↓
Transition Spec
        ↓
Guardrail Checklist
        ↓
Tickets
```

The team should rarely have to reinvent intent. Product Gravity and refusal patterns often give clearer implementation guidance than ordinary acceptance criteria.

Those named files are binding when they exist. They do not replace Human Truths, Experience Boards, or Design Boundaries. They operationalize them.

Observed, not doctrine: later governance can be stricter than an Experience Board. Boards may still hope for warmth that the State Map, Transition Spec, Guardrail Checklist, or an AI test later refuse. If rank is not explicit at implementation time, agents and engineers will choose the warmer document.

When documents conflict, follow the ranked implementation chain unless a Human Truth, Design Boundary, or DDR says otherwise. Record the conflict. Do not silently prefer warmth.

## Missing DDRs

When a governance trigger calls for a DDR and the DDR does not exist, proceed only if the ranked implementation chain gives enough authority. Record the missing DDR as an explicit gap. Do not invent the missing decision.

---

## The milestone that may govern

Operating rules. Not a Human Truth. These are implementation stops.

If a product `AGENTS.md` names a milestone folder, or tells an agent to sort `MILESTONES/`, and `MILESTONES/CURRENT.md` is missing or names a different folder, stop. The agent file is stale. Do not guess the newest folder.

A milestone cannot become governing until it has `MILESTONE_SUMMARY.md` and a short still-in-force list. That list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in `AREAS.md`. A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not copy another product's exclusions into the list.

---

## Review questions are useful during build

The Prototype Review Script is not only a final ceremony.

A review question can prevent a false “done.”

> Does this moment feel like peace, or like the product ran out of things to do?
> Does the visitor feel released, or does leaving feel like an unfinished session?

If the answer is still unclear, the beat is not finished.

---

## Two review modes

A prototype can be reviewed as:

```text
A map the steward can inspect
```

or:

```text
A rhythm the steward must undergo
```

Those are not the same instrument.

A scrollable shell can help a steward see the whole path. Sequential transitions better match the emotional rhythm.

Review chrome — state names, maps, labels added for inspection — is a method tool. It must stay labeled as such, or the prototype starts teaching the visitor a procedure.

Observed from practice, not doctrine.

---

## Tests prove absence, not gifts

Widget tests can prove there is no button, no “welcome back,” no contribution prompt, and no retention language.

They cannot prove Permission, release, peace, or emotional temperature.

Green tests must not replace Arc Steward playback.

---

## Edge work needs its own ticket shape

Transitions into, out of, and back into the arc are easy to treat as leftovers of the nearest state ticket.

They are not leftovers. They are their own emotional objects.

If they are split casually, return behavior leaks into transition work, and the team rebuilds the same threshold twice.

---

## What implementation does not close

Implementation translates governed intent into something playable.

It does not, by itself, prove that an Experience Gift held.

Whether a moment feels ready, whether leaving feels respectful, whether stillness feels like peace — those remain prototype review questions. Record them. Do not declare them solved because the shell runs.

A merged ticket, a green suite, a device pass, and milestone acceptance are different events. Observed from practice, not doctrine.

---

## A ticket names one completion class

Every ticket names the kind of finish it is allowed to claim:

- Specification
- Implementation
- Automated verification
- Human validation
- Freeze or handoff

A ticket may depend on another class. It does not absorb that class's work.

Operating rules. Not a Human Truth.

A ticket also names what it will not absorb, including the next product slice. That edge is what lets one issue and one branch finish.

A quality pass restates the milestone's job. Accessibility, device playback, and named review can still be open after the code has merged.

A quality-pass milestone cannot add a surface, collection, access path, invitation channel, or discovery query. If the work needs one, stop. Open a new milestone first. This is an implementation stop. Adding product so the work feels finished starts the backlog again.

Record how far the work has actually gone:

- Implemented
- Automatically verified
- Ready for validation
- Human validated
- Accepted

An implementation ticket closes when its implementation and its automated acceptance criteria pass. A ticket is not implemented while a test that locks its contract is red. Human validation that the milestone has deferred stays on the milestone validation ticket. It stays visible there. It does not keep the implementation ticket open after the code has merged.

A follow-up pull request states which of these it is:

- Completes a ticket
- Repairs a finding
- Adds evidence
- Changes the governing contract

A merged ticket that needs a follow-up branch stays closed when that follow-up is a repair, new evidence, or a contract change. The status record says which. A follow-up commit that fixes a syntax error, a crash, or a dependency pin from the previous pull request is not that kind of repair. That pull request did not close.

---

## One status record

Each milestone keeps one status record, on its summary. Later evidence cites that record. An earlier test count does not travel forward inside a note as if it were still final.

The record holds:

- Current dependency order
- Merged pull requests
- Open findings
- Deferred validation
- Latest authoritative test counts
- Freeze candidate and accepted freeze

Concern, Blocker, Pass, skipped reproducer, and unresolved scope stay visible as findings.

A skipped reproducer names its blocker, the owning ticket, the condition that removes the skip, and its current status. An unnamed skip is not closed.

Whether work is done is read from this record and the merged pull requests. A chat or a session capture is not the lasting record.

Observed from practice, not doctrine.

---

## Validation is one ticket

Simulator, device, assistive-technology, and named-reviewer work belong on one validation ticket for the milestone, unless a single feature is unusually high risk.

Repeating those requirements on every implementation ticket makes one validation round look like many unfinished tickets.

Keep implementation and evidence on separate branches, so unfinished validation is not mistaken for production readiness. Participant evidence stays outside Git. A review records the exact commit and the freeze identifier it used.

---

## One contract before a group of surfaces

Before a group of production surfaces is built, one governing contract specifies purpose, hierarchy, states, language, accessibility, and visual components.

That contract may live with the milestone's implementation artifacts. It is one document. Two writeups that restate it are the same work split across two tickets. Do not open the second ticket.

A change to a sentence, a route purpose, or an access rule that appears in a governing contract is a contract change. The same change updates the milestone status record. Code that disagrees with the contract is not done. Updating a test to match warmer copy, without that record, is a contract change done backwards.

A screen built before that contract exists can be functionally complete and still need a substantial visual redesign. That redesign is a specification that arrived late.

---

## Human judgment stays named

Automated checks can establish behavior and guardrails.

They are not approval by a named human reviewer. Arc Steward playback is one such review. A project may also name design, accessibility, or privacy review.

Those reviews protect concerns a suite cannot settle. Name a reviewer's judgment only when that person has made it.

---

## Participant testing needs the whole journey

A build may be offered to participants only after it can be walked as the intended end-to-end product journey.

A high-quality portion of that journey is not enough. Validating the emotional arc alone does not show that the application journey exists. A freeze of that portion is not a participant-testing candidate.

This gate is not emotional readiness. Emotional readiness is whether the next moment can begin without force. This gate is whether the product journey is present enough to test.

Engineering review may improve a build before participants see it. It stays labeled as non-participant review. It is not participant validation.

Observed from practice, not doctrine.
