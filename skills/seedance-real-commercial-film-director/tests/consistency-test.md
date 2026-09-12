# Consistency Test

Run this checklist against every generated director package. A test passes only when evidence is present in the prompt, not merely implied by adjectives.

## Character consistency

- [ ] One `CHARACTER_ID` is declared for each principal person.
- [ ] Face, age impression, hair, body, wardrobe, shoes, and accessories are locked separately from motion.
- [ ] Every shot repeats the same identity block or references it without contradiction.
- [ ] Gaze, hands, weight transfer, clothing, and hair are physically executable at the stated shot distance.
- [ ] No face merge, identity swap, clothing swap, extra fingers, hand intersection, or robotic synchronized movement.

## Venue consistency

- [ ] Each asset has `ROLE_VENUE_CONSISTENCY` only when it contributes a landmark or sightline.
- [ ] The spatial map names at least two anchors per shot.
- [ ] Entrance, stage, seating, aisle, windows, proportions, and screen direction stay fixed.
- [ ] Conflicting views are marked with a confidence choice rather than silently averaged.

## Prompt completeness

- [ ] Specs include duration, aspect ratio, subtitles, BGM, and voice assumptions.
- [ ] Reference role map includes inherit and do-not-inherit boundaries.
- [ ] Timeline has `TIME / SHOT / ACTION / CAMERA / AUDIO` for every segment.
- [ ] Camera has one dominant movement, lens, speed, focus, and inertia.
- [ ] Lighting, continuity, negative constraints, and a 1–2 second ending state are present.
- [ ] Dialogue is verbatim and appears once when used.

## Result

```text
CHARACTER_CONSISTENCY: PASS / FAIL
VENUE_CONSISTENCY: PASS / FAIL
PROMPT_COMPLETENESS: PASS / FAIL
PROMPT_READINESS: PASS / INCOMPLETE
SHOT_FEASIBILITY_WARNING: NONE / <specific conflict>
```
