# Forever After Memories: Recognition Experience Board

Status: public worked example, published with the method on 2026-11-16 by the founder's direction. This board illustrates one product. It does not supply exclusions, sentences, or implementation rules for any other product.

This worked example shows how an emotional responsibility becomes interface behavior and acceptance criteria. It preserves the Recognition example from the original storyboard notes. It is a design illustration, not evidence of participant validation or a complete product specification.

Forever After Memories explores the relationship between people and loved ones who have died. The moment below asks the product to support recognition before asking for interaction.

## Experience Intent

| Field | Example |
| --- | --- |
| Emotional beat | Recognition |
| Human purpose | Help someone feel close again before asking them to act |
| Visitor thought | "That's her." |
| Intended emotion | Warmth, gratitude, calm |
| Experience principle | Presence before information |
| Possible success signal | A visitor pauses, smiles, or describes a sense of recognition |

The principle is used here as a design reference. This example does not establish it as a validated canonical Human Truth. A smile or pause is a possible signal to explore with a person, not proof of an emotional outcome.

## Interface Translation

| Field | Example |
| --- | --- |
| Visual focus | A family-provided portrait and approved presence statement |
| Components | Portrait, name, presence statement; voice only where governed and available |
| Motion | A gentle reveal that allows recognition without rushing participation |
| Visitor action | No immediate action required |
| Navigation | Continue according to the project's governed transition rules |
| States | Loading, unavailable content, offline, and empty states require explicit design |
| Accessibility | Meaningful image alternatives and captions or transcripts where applicable |

These choices translate the intent into a buildable object. They do not substitute for a State Map, Transition Spec, or project-specific accessibility review.

## Boundaries and Positive Form

The ordinary product move being refused is an immediate demand for engagement. The positive designed object is a recognition moment centered on the portrait and approved statement, with room to pause.

AI must remain within the family-provided source. It must not invent personality, speak as the person, or infer a visitor's grief. See [Entrusted Source](../../METHODOLOGY/ENTRUSTED_SOURCE.md).

## Acceptance and Review

Functional checks can establish that the portrait loads, unavailable states behave as specified, approved content is used, and any governed voice control works. Accessibility checks can establish whether the information and controls are perceivable and usable.

Human review asks different questions:

- Does the visitor recognize the person before being asked to interact?
- Does the moment feel welcoming rather than demanding?
- Does the interface support the person's presence without competing with it?
- Can the visitor pause without being pushed onward?

Record what participants say and do, including contrary evidence. Automated checks cannot establish these emotional outcomes. No participant results are claimed in this example.

## Reusing the Pattern

Use the [Experience Board template](../../STARTER_KIT/EXPERIENCE_BOARDS/TEMPLATE.md) to name the emotional beat, human purpose, intended thought and emotion, governing principle, visual direction, components, motion, interaction, system response, accessibility, and success criteria for your own moment.

Keep this chain visible:

```text
Human understanding -> Product intent -> Interface behavior -> Implementation -> Human review
```

The general practice lives in [Experience Boards](../../METHODOLOGY/EXPERIENCE_BOARDS.md) and [Prototype Practice](../../METHODOLOGY/PROTOTYPE_PRACTICE.md). Detailed F.A.M. implementation records belong in that product's repository.
