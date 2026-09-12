# Reference Analysis Workflow

Create a role map before writing a prompt. One asset may have a primary role and limited secondary evidence, but never an undefined “overall reference” role.

## Role map

| Asset | Primary role | May inherit | Must not inherit |
|---|---|---|---|
| `@图片1` | `ROLE_CHARACTER_IDENTITY` | face, age impression, hair, wardrobe | background, pose, lighting, text |
| `@图片2` | `ROLE_SCENE` | location layout, architecture, time cues | character identity, product design |
| `@图片3` | `ROLE_SCREEN_STYLE` | palette, contrast, texture, framing mood | exact actor or venue geometry |
| `@图片4–9` | `ROLE_VENUE_CONSISTENCY` | landmarks and spatial relationships | new architecture or changed proportions |

## Procedure

1. Inventory each asset and note viewpoint, visible boundaries, and confidence.
2. Assign role, inheritance, non-inheritance, and shot coverage.
3. Mark missing evidence rather than fabricating hidden sides.
4. Carry the role map into the final prompt unchanged.

For a reference video, extract structure, pace, and camera language only; do not copy identifiable people, logos, or proprietary content without authorization.
