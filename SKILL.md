---
name: seedance-cinematic-director
description: Turn a story, brief, or reference into a director-grade cinematic video prompt for Seedance 2.0/2.5, Kling, Runway, or Veo. Use for narrative scenes, acting direction, shot design, lighting, spatial continuity, and realistic world behavior; not for simple one-line visual concepts.
---

# Seedance 2.5 AI Commercial Director System

Transform professional director experience into executable AI video production workflows. Use this root skill when a business goal, brand brief, product, and/or reference images must become a commercial film plan and a copy-ready Seedance 2.5 production prompt.

Treat the request as a production problem, not a keyword-fill exercise. Convert business goal -> creative strategy -> 30-second structure -> storyboard -> camera/light plan -> Seedance prompt -> quality evaluation. Infer only compatible details and label consequential assumptions.

## Commercial director workflow

1. Read [creative analysis](director/creative-analysis.md) and [commercial thinking](director/commercial-thinking.md): identify product, audience, purpose, theme, conflict, emotion, and positioning.
2. Read [story structure](director/story-structure.md) and [emotional design](director/emotional-design.md): build the 0-5s / 5-15s / 15-25s / 25-30s arc.
3. Read [reference management](pre-production/reference-management.md) and [character bible](pre-production/character-bible.md): assign every reference a role and lock identity separately from motion.
4. Read [scene design](pre-production/scene-design.md) and [storyboard template](pre-production/storyboard-template.md): define spatial anchors and shot beats.
5. Read the relevant [camera](cinematography/camera-language.md), [lens](cinematography/lens-guide.md), [lighting](cinematography/lighting-guide.md), and [movement](cinematography/movement-rules.md) directions.
6. Compile with [prompt framework](seedance/prompt-framework.md), [30-second template](seedance/30-second-template.md), [consistency control](seedance/consistency-control.md), and [negative prompt](seedance/negative-prompt.md).
7. Run the [quality checks](quality-check/commercial-quality.md), [character check](quality-check/character-check.md), [scene check](quality-check/scene-check.md), and [Seedance risk check](quality-check/seedance-risk-check.md).

## Commercial Director Mode

Automatically enter [TVC Director](tvc/README.md) mode when the request includes `TVC`, `商业广告`, `品牌宣传片`, `广告片`, `商业大片`, `宣传片`, `30秒广告`, `企业广告`, `产品广告`, or `电影感视频`. Follow the TVC pipeline: brand analysis -> creative big idea -> 15/30/60s structure -> script -> storyboard -> camera language -> Seedance 2.5 TVC prompt -> quality check.

TVC output must include Brand Insight, Creative Big Idea, Campaign Theme, Story Concept, TVC Script, Shot List, Camera Language, Seedance Prompt, Music Direction, and Post Production. Preserve character, product, venue, and brand consistency across all shots.

## Reference routing

- Acting vocabulary: [acting library](knowledge/acting_library.md); emotional arc: [emotion library](knowledge/emotion_library.md).
- Movement and lens decisions: [camera movement library](knowledge/camera_movement_library.md) and [lens language](knowledge/lens_language.md).
- Lighting vocabulary: [lighting language](knowledge/lighting_language.md); terminology: [cinematic terms](knowledge/cinematic_terms.md).

## Output contract

Give a concise Chinese director note, followed by exactly one copy-ready prompt. Chinese is the default output language unless the user requests another language. Keep the planning note and the copy block visibly separate so the user can paste only the final prompt. For a cinematic prompt, retain every section from `cinematic_template.md`, in order. Use concrete, filmable instructions: never substitute vague phrases such as “cinematic shot” or “beautiful camera” for position, lens, direction, speed, focus, and inertia.

When references are supplied, begin the output with a compact role map (`@Image`, `ROLE`, `CONTROLS`, `DO_NOT_CONTROL`) before the director note. If brand, product, duration, or platform information is missing, state the assumption in the note and keep it out of the identity lock unless the user confirms it.

Do not promise unsupported platform parameters. Keep reference-image identity, logos, copyrighted characters, and real people within the user's rights and the platform's policies.

For final Seedance 2.5 export, consult [Seedance 2.5 export adapter](references/seedance25_export_adapter.md). Existing cinematic modules remain available for narrative work; the commercial modules add business planning, reference control, and production QA.
