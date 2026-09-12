# TVC Director Skill

TVC Director is the commercial advertising layer of `seedance2.5-AIdy`. It transforms brand materials, product information, audience, advertising objective, and brand tone into a complete TVC plan and a directly usable Seedance 2.5 prompt.

## Standard pipeline

```text
Brand Analysis Agent
→ Creative Director Agent
→ TVC Script Agent
→ Storyboard Agent
→ Seedance Prompt Agent
→ Quality Agent
```

## Required output

1. Brand Insight
2. Creative Big Idea
3. Campaign Theme
4. Story Concept
5. TVC Script
6. Shot List
7. Camera Language
8. Seedance Prompt
9. Music Direction
10. Post Production

## Routing

- Read [tvc_director.md](tvc_director.md) for the complete agent contract.
- Read [tvc_strategy.md](tvc_strategy.md), [tvc_structure.md](tvc_structure.md), and [tvc_script.md](tvc_script.md) for planning and duration choices.
- Read [tvc_storyboard.md](tvc_storyboard.md), [tvc_camera_language.md](tvc_camera_language.md), and [tvc_visual_style.md](tvc_visual_style.md) for shot design.
- Read [tvc_prompt_engine.md](tvc_prompt_engine.md) and [tvc_quality_check.md](tvc_quality_check.md) before delivery.
- Select duration and business templates under [templates](templates/), then industry guidance under [industries](industries/).
- Use prompt patterns under [prompts](prompts/) as references, never as brand-copy replacements.
- For the broader camera library and Seedance rules, use the repository-level [camera](../camera/), [prompts](../prompts/), and [TVC test suite](../tests/tvc_test/) modules.

## Guardrails

Use brand and product facts supplied by the user. Do not copy protected brand campaigns; the case files study structure, camera, and narrative only. Keep readable text minimal and run character, product, scene, commercial, and AI-artifact checks before calling a prompt production-ready.
