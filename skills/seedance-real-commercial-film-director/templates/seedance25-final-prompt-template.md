# Seedance 2.5 Final Prompt Template

```markdown
【规格】<duration>秒，<aspect ratio>，<fps>，字幕：<有/无>，BGM：<有/无>，旁白：<有/无>。
【导演意图】<one sentence>
【参考素材职责】<each asset role, inherit, do not inherit>
【人物锁】<identity block, CHARACTERS_ID>
【产品锁】<shape, color, material, logo, quantity, prohibited changes; delete if no product>
【场景锁】<venue landmarks, time, light, screen direction>
【时间轴】<each segment has TIME / SHOT / ACTION / CAMERA / AUDIO>
【摄影】<position, distance, lens, one movement, speed, focus, inertia>
【光线】<source, direction, color temperature, shadow, continuity>
【声音】AMBIENCE / SFX / VOICE / DIALOGUE / BGM
【连续性】<identity, venue, props, product, direction>
【负面约束】<high-risk project-specific failures>
【结尾状态】<last 1–2 seconds>
```

Use Chinese by default, retain necessary English camera terms, and do not add unsupported model controls. Output `PROMPT_READINESS: PASS` or `INCOMPLETE`.
