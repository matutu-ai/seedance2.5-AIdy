# Seedance Cinematic Director Skill v1.0

`seedance-cinematic-director` converts a premise into a production-ready cinematic direction package. It is an AI video director workflow: it analyzes dramatic intent, stages performance, camera, light, space, background behavior, and physical continuity before compiling a prompt.

## Workflow

`story → scene analysis → acting + emotion arc → blocking → camera + light → world + realism → prompt compiler → score`

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

## Extending the skill

Add a focused reference when it changes a directing decision, then link it from `SKILL.md`. Add a target-model template only when its prompt grammar or controls differ materially. Keep core engines platform-neutral; avoid adding generic word lists or duplicate workflows.
