# Seedance 2.5 AI Commercial Director Skill

This repository packages professional director experience into executable AI video production workflows. It transforms a business requirement, reference images, and brand information into an AI Director Plan, 30-second film structure, storyboard, camera and lighting design, Seedance 2.5 production prompt, and quality evaluation.

## Workflow

`business goal → creative strategy → 30s structure → references → storyboard → camera/light → Seedance prompt → quality check`

Use `$seedance-cinematic-director` and provide the story plus any known model, duration, aspect ratio, visual references, or non-negotiable details. If these are omitted, the skill makes and labels conservative production assumptions.

## Input

```text
Model: Seedance 2.5
Duration: 12 seconds, 16:9
Story: A woman enters an abandoned hospital looking for her missing brother.
Style: restrained psychological thriller, realistic live action
Must keep: a red flashlight and rainy night exterior
```

## Output

The final prompt follows the fixed sections: Story Context, Character Acting, Emotion Timeline, Body Movement, Camera Direction, Lighting, Environment, Background Behavior, Physical Realism, Negative Prompt, and Model Parameters. A checker rates acting, camera, cinema, and reality readiness out of 100.

## Examples

- [Action scene](examples/action_scene.md): armed search in an abandoned building.
- [Emotional scene](examples/emotional_scene.md): reunion with restrained micro-expression.
- [Fashion scene](examples/fashion_scene.md): editorial movement with clothing continuity.
- [Commercial scene](examples/commercial_scene.md): an electric vehicle city film.
- [GEO growth journey](examples/GEO-growth-journey.md): 《当AI成为运营伙伴》.

## Public-class demo

- [15-minute demo: 《当AI成为运营伙伴》](demos/public-class-15min.md): from business requirement to director analysis, 30-second structure, cinematography, Seedance prompt, quality check, and the GEO → Seedance → Content enterprise growth loop.

## Commercial video generation

1. Understand product, brand, audience, and marketing purpose.
2. Generate theme, conflict, emotional curve, visual style, and commercial positioning.
3. Build 0-5s Hook, 5-15s Problem/Transformation, 15-25s Solution/Value, and 25-30s Memory Point/Brand Emotion.
4. Assign reference roles, lock character identity, and build a multi-view venue memory.
5. Generate storyboard, camera language, lens, movement, lighting, sound, and continuity rules.
6. Compile and quality-check a copy-ready Seedance 2.5 prompt.

## Director modules

The root modules are organized as `director/`, `pre-production/`, `cinematography/`, `seedance/`, `templates/`, and `quality-check/`. The existing `seedance-real-commercial-film-director` and `seedance-cinematic-director-agent` remain available as focused sub-skills.

The public demo is designed for a live 15-minute class: it shows the complete production chain instead of presenting the repository as a collection of prompt templates.

## Commercial live-action director layer

The independent [Seedance Real Commercial Film Director](skills/seedance-real-commercial-film-director/SKILL.md) skill adds character locking, multi-view venue locking, realistic human motion, and commercial storyboard generation without changing the original director skill. Use it when reference images, a real person, a venue, or a 30-second commercial structure must remain consistent across shots.

- Commercial flow: reference roles → character/venue locks → storyboard → camera/light/sound → final Seedance 2.5 prompt → consistency QA.
- Image assignment: every asset receives a role, coverage, inheritance, and do-not-inherit boundary; never treat all references as one mixed image.
- Multi-view stability: wide, left, right, stage, and audience views become one landmark map. Entrances, stage, seating, proportions, and screen direction remain fixed.
- Tests: [consistency-test.md](skills/seedance-real-commercial-film-director/tests/consistency-test.md).
- Full case: [GEO operator's AI growth journey](skills/seedance-real-commercial-film-director/examples/geo-training-camp-case.md).

## Cinematic director agent layer

The independent [Seedance Cinematic Director Agent](skills/seedance-cinematic-director-agent/SKILL.md) orchestrates reference intelligence, character locking, venue memory, storyboard generation, prompt compilation, and quality checking. Input images and a commercial brief; output a directly usable Seedance 2.5 director prompt.

- Commercial video flow: reference roles → character lock → venue memory → storyboard → camera/light/sound → prompt compiler → quality checker.
- Multi-view space locking: convert wide, left, right, stage, and audience views into one landmark graph; preserve entrances, stage, seating, proportions, and screen direction.
- Live-action consistency: keep identity separate from shot motion and describe eye direction, weight transfer, contact, inertia, and settling.
- Tests and case: [consistency-test.md](skills/seedance-cinematic-director-agent/tests/consistency-test.md) and [GEO运营人的AI成长之旅](skills/seedance-cinematic-director-agent/examples/geo-training-camp-case.md).

## Acceptance checks

- [Character consistency test](tests/character-consistency-test.md)
- [Venue consistency test](tests/venue-consistency-test.md)
- [Prompt completeness test](tests/prompt-completeness-test.md)

## Extending the skill

Add a focused reference when it changes a directing decision, then link it from `SKILL.md`. Add a target-model template only when its prompt grammar or controls differ materially. Keep core engines platform-neutral; avoid adding generic word lists or duplicate workflows.
