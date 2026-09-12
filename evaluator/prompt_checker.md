# Prompt Checker

Score the completed prompt before delivery. Award zero to a missing section; do not compensate with decorative adjectives.

| Category | Points | Check |
|---|---:|---|
| Character Acting | 25 | face 5; eyes/breath 5; posture/hands 5; micro-expression 5; transition 5 |
| Camera | 25 | position/distance 5; lens 5; path/direction 5; speed/inertia 5; focus behavior 5 |
| Cinema | 25 | dramatic beat 5; spatial anchors 5; main/fill/back light 5; lighting continuity 5; rhythm/style coherence 5 |
| Reality | 25 | background behavior 5; environmental motion 5; contact/material physics 5; lens/motion/DOF behavior 5; clear negative constraints 5 |

## Decision

`Total Score / 100`

- **80–100:** deliver after checking that stated parameters are supported by the target model.
- **60–79:** automatically add the missing observable direction, prioritizing acting, blocking, camera mechanics, and motivated light.
- **Below 60:** rebuild from the scene analysis; a keyword list is not a repairable director prompt.

If input facts are intentionally absent (for example no secondary character), mark the item `N/A` and redistribute its five points within the same category only when the prompt explicitly provides an equivalent constraint.
