# Prompt Generation Workflow

Compile the director package into one copy-ready Seedance 2.5 prompt. Use the local parent templates for cinematic structure and this order for platform export:

```text
规格 → 导演意图 → 参考素材职责 → 人物/产品锁 → 场景锁 → 时间轴
→ 摄影 → 光线 → 声音 → 连续性 → 负面约束 → 结尾状态
```

## Minimum specification

State duration, aspect ratio, frame rate when known, subtitles, BGM, and voice. Default to 9:16, no subtitles, and no BGM only when the user has not specified otherwise; label assumptions.

## Timeline contract

Each segment must include:

```text
TIME / SHOT / ACTION / CAMERA / AUDIO
```

Dialogue is verbatim, appears once, and is assigned to a speaker and time range. Reference assets state what they inherit and what they must not inherit. Negative prompts list only project-specific risks.

## Final QA

Return `PROMPT_READINESS: PASS` only when role map, character/venue locks, timeline, camera, light, sound, continuity, ending state, and negative constraints are present. If a required module is missing, return `INCOMPLETE` and identify it instead of hiding the gap.
