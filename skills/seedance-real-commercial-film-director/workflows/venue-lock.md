# Venue Multi-View Lock Workflow

Treat multiple venue images as observations of one set, not separate locations.

## View labels

```text
Image_Wide: overall boundaries, entrances, ceiling, floor, horizon
Image_Left: left-side architecture and sightlines
Image_Right: right-side architecture and sightlines
Image_Stage: stage, screen, podium, or hero zone
Image_Audience: seating, audience orientation, aisle relationships
```

## Spatial map

Record fixed landmarks, relative distances, screen direction, and camera-accessible paths. Every shot must cite at least two anchors (for example, “stage screen behind subject, entrance on camera-left”).

## Lock rules

- Do not change building proportions, entrance direction, seating layout, stage position, ceiling height, or window placement.
- A camera may reveal a hidden area only if the path and prior landmarks support it.
- Keep audience eyelines, presenter orientation, and stage-facing direction consistent.
- If views conflict, mark the conflict and choose the highest-confidence view; do not average incompatible architecture.
