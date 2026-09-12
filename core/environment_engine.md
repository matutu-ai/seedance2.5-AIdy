# Environment and Spatial Relationship Engine

Prevent drifting bodies and empty-background behavior through an anchored set plan.

## Blocking map

```text
Character A: position, facing direction, distance from camera and landmarks
Character B: position, facing direction, distance from A
Camera: start position, end position, height, movement path
Set anchors: doors, furniture, vehicles, windows, horizon, product
Background characters: positions and independent repeatable actions
Environmental motion: wind, rain, traffic, practical lights, particles
Random events: at most one subtle event that supports the beat
```

Keep screen direction continuous unless the camera visibly crosses the line. Background activity must not duplicate the protagonist's action or compete with the story beat.

**Example:** Character A stands two meters in front of camera at a corridor threshold, facing north. Character B remains eight meters beyond the directory, half-hidden by a column. Camera travels from behind A to her left side without crossing the corridor centerline. A loose report page slides along the floor after a draft; distant officers continue cataloging evidence.
