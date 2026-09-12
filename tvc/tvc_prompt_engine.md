# TVC Prompt Engine

Every TVC prompt contains:

```text
Project Type: Commercial TVC
Duration: 15s / 30s / 60s
Aspect Ratio: 16:9
Camera: position, lens, movement, focus, depth
Visual: lighting, color, texture
Character: identity, emotion, action
Product: hero product, material, detail, logo boundary
Sound: music, voice-over, diegetic sound
Continuity: character, product, venue, brand rules
Negative Prompt: AI artifacts and production risks
End State: brand-readable final frame
```

Compile one shot timeline into one copy-ready Seedance 2.5 prompt. Output the final block in Chinese by default, keep it separate from analysis, and do not leave planning placeholders in the final block. Use one consistent vocabulary for the same character, product, venue, and brand across all shots.
