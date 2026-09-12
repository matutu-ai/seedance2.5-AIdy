# Seedance 2.5 Export Adapter

This adapter references the public `matutu-ai/seedance2.5-skill` repository when exporting a final Seedance 2.5 prompt. It is an export layer only; the cinematic-director core modules remain authoritative for scene, acting, emotion, camera, lighting, environment, realism, and score.

Source repository: https://github.com/matutu-ai/seedance2.5-skill

## Merge order

1. Use this skill's director analysis and selected template as the creative source of truth.
2. Apply Seedance 2.5 export constraints from the source repository: explicit specs, reference-material responsibility, identity/product locks, timestamped actions, camera and audio layers, continuity, negative constraints, and ending state.
3. Keep the final prompt in the selected local template's section order. Do not replace its director sections with a generic commercial template.
4. Add only platform details supported by the source repository and the user's stated mode. If a parameter is unknown, label it as an assumption.

## Export contract

```markdown
【规格】时长、画幅、帧率、字幕、BGM、旁白
【导演意图】一句话的 dramatic objective and visual strategy
【参考素材职责】每个 @素材 的用途、继承项、禁止继承项
【人物/产品锁】identity, wardrobe, geometry, logo, quantity, continuity
【场景锁】place, time, spatial anchors, light conditions
【时间轴】每段包含 SHOT / ACTION / CAMERA / AUDIO
【摄影】shot size, camera position, lens, movement, speed, focus, inertia
【光线】source, direction, color temperature, contrast, change or continuity
【声音】AMBIENCE / SFX / VOICE / DIALOGUE / BGM
【连续性】identity, props, screen direction, object state, ending state
【负面约束】only project-specific high-risk failures
【结尾状态】last 1–2 seconds and natural hold
```

## QA before delivery

- Duration is within the target model's supported range.
- The first beat begins with an observable action, not an empty establishing shot.
- Every reference has a role and a boundary.
- Camera uses one dominant movement and motivated focus changes.
- Human realism is written as behavior and physics, not quality adjectives.
- Dialogue, if present, is verbatim and appears once; unspecified BGM and subtitles default to none.
- Report `PRE-GENERATION RISK SCORE` when no video has been generated. Do not call it a measured visual-quality score.

## Conflict rule

If the source repository's platform rules conflict with a creative request, preserve the user's creative intent where possible and state the exact platform limitation. Never silently change identity, product design, dialogue, or reference responsibility.
