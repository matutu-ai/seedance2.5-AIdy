# Reference Intelligence Engine

Create a role map before writing shots. Every asset gets exactly one primary role, the shots where it applies, what may be inherited, and what must not be inherited.

```text
ASSET_ID | ROLE | COVERAGE | INHERIT | DO_NOT_INHERIT
图片1    | CHARACTER_IDENTITY | whole film | face, hair, wardrobe | pose, room, lighting
图片2    | VENUE_WIDE         | venue shots | geometry, landmarks | actor identity
图片3    | PRODUCT_DETAIL     | product shot | material, logo, proportions | background
```

If a reference has multiple possible roles, ask for clarification or state the chosen role and why. Never let a style image overwrite identity or venue geometry.
