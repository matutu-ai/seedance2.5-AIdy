---
name: seedance-cinematic-director-agent
description: Turn user images and a commercial brief into a production-ready Seedance 2.5 director prompt with reference roles, character consistency, venue memory, storyboard beats, prompt compilation, and quality checks.
---

# Seedance Cinematic Director Agent

Use this skill when the user provides reference images, a product or venue, and a commercial video request. The output must be a directly usable Seedance 2.5 video-director prompt, not generic advertising copy.

## Agent pipeline

```text
Input images + brief
  -> Reference Intelligence Engine
  -> Character Lock Engine
  -> Venue Memory Engine
  -> Storyboard Generator
  -> Prompt Compiler
  -> Quality Checker
  -> Final Seedance 2.5 Prompt
```

Read the relevant workflow and reference files before generating the final prompt:

1. Assign a single role and inheritance boundary to every asset with [reference intelligence](workflows/reference-intelligence.md).
2. Separate identity facts from shot-specific motion with [character lock](workflows/character-lock.md).
3. Build one landmark map for all venue views with [venue memory](workflows/venue-memory.md).
4. Convert the brief into timed commercial beats with [storyboard generator](workflows/storyboard-generator.md).
5. Compile the production prompt using [prompt compiler](workflows/prompt-compiler.md).
6. Run [quality checker](workflows/quality-checker.md) and report any unresolved assumption.

## Six engines

- **Reference Intelligence Engine**: classifies image, video, audio, product, character, scene, style, and venue responsibilities.
- **Character Lock Engine**: fixes face, age impression, hair, body, wardrobe, and identity boundaries; keeps motion separate.
- **Venue Memory Engine**: stores entrances, stage, screen, seating, aisles, windows, columns, and camera directions as persistent spatial anchors.
- **Storyboard Generator**: creates a commercial arc with shot duration, action, camera, light, sound, and continuity.
- **Prompt Compiler**: emits one copy-ready Seedance 2.5 prompt with specifications, locks, timeline, camera, sound, negative constraints, and end state.
- **Quality Checker**: checks reference roles, identity continuity, venue continuity, human motion, prompt completeness, and contradiction risks.

## Required output

```text
Video Concept
Reference Role Map
Character Lock
Venue Memory / Scene Lock
Commercial Storyboard
Camera, Lighting and Sound
Negative Prompt
Final Seedance 2.5 Prompt
Quality Report
```

## Hard constraints

- Do not blend all references into one visual instruction.
- Identity answers “who”; motion answers “what happens in this shot.”
- All venue shots must use the same spatial map; never silently move entrances, stage, seating, proportions, or screen direction.
- Use one dominant camera movement per shot.
- Describe realism through observable action, weight transfer, contact, inertia, and settling; adjectives such as `8K` do not establish realism.
- Preserve the user's product, dialogue, duration, aspect ratio, and creative intent. Label assumptions instead of inventing decisive facts.

## Resources

- [Reference role template](templates/reference-role-template.md)
- [30-second commercial template](templates/30s-commercial-video-template.md)
- [Final prompt template](templates/seedance25-final-prompt-template.md)
- [GEO training camp case](examples/geo-training-camp-case.md)
- [Consistency tests](tests/consistency-test.md)
