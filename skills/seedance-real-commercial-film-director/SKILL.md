---
name: seedance-real-commercial-film-director
description: Create Seedance 2.5 commercial live-action video plans from character, venue, multi-view, product, or storyboard references. Use for identity consistency, venue locking, realistic human motion, commercial storyboards, and final production prompts; not for market research or generic copywriting.
---

# Seedance Real Commercial Film Director

This is a commercial-directing layer inside `seedance2.5-AIdy`. It turns reference assets into a stable, filmable Seedance 2.5 production prompt while preserving the parent cinematic-director skill's scene, acting, camera, lighting, environment, realism, and evaluation logic.

## Core formula

```text
Reference Intelligence
+ Character Lock
+ Venue Multi-View Lock
+ Camera Language
+ Human Motion Realism
+ Commercial Timeline
= Seedance 2.5 Production Prompt
```

## Workflow

1. Read [reference analysis](workflows/reference-analysis.md) and assign exactly one primary role to every image/video/audio asset.
2. Read [character lock](workflows/character-lock.md) for visible people. Keep identity separate from motion and load only dynamics the shot can show.
3. Read [venue lock](workflows/venue-lock.md) when a location has multiple views. Build one spatial map before designing coverage.
4. Read [cinematic storyboard](workflows/cinematic-storyboard.md) to shape the commercial beats, then [prompt generation](workflows/prompt-generation.md) to compile a final Seedance prompt.
5. Use the relevant references for character consistency, venue geometry, human motion, and camera language. Validate with [consistency test](tests/consistency-test.md).

## Required output

```text
Video Concept
Character Lock
Reference Role Map
Scene / Venue Lock
Commercial Timeline or Storyboard
Camera Design
Lighting and Sound
Negative Prompt
Final Seedance 2.5 Prompt
QA: character consistency, venue consistency, prompt completeness
```

## Non-negotiable rules

- Never merge all reference images into one undifferentiated visual instruction.
- Identity answers “who is this”; motion answers “how does this person move.” Keep them in separate blocks.
- Every venue shot must belong to the same spatial map; do not silently change entrances, proportions, stage position, seating, or screen direction.
- Use one dominant camera movement per shot. Warn when a requested action cannot fit the duration or frame.
- Human realism is observable action, inertia, contact, and temporal continuity—not `photorealistic`, `8K`, or `masterpiece` adjectives.
- Preserve the user's creative brief, product design, dialogue, and reference responsibilities. State assumptions instead of inventing decisive facts.
