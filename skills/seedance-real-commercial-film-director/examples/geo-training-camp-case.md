# Case: GEO运营人的AI成长之旅

## Video Concept

A GEO operator works alone late at night, enters an AI training camp, learns to turn scattered questions into a clear strategy, and leaves the venue with a confident team and a visible plan. The film is a 30-second commercial for an AI growth-training program.

## Reference Role Map

```text
@图片1 — ROLE_CHARACTER_IDENTITY — one operator's face, hair, age impression, wardrobe — do not inherit pose, room, or lighting — full film
@图片2 — ROLE_SCENE — night office layout, desk and window — do not inherit actor identity — 0–8s
@图片3 — ROLE_VENUE_CONSISTENCY — training-camp wide hall — do not inherit unrelated people or text — 8–30s
@图片4 — ROLE_VENUE_CONSISTENCY — hall left side, entrance and aisle — do not change architecture — 8–20s
@图片5 — ROLE_VENUE_CONSISTENCY — stage and screen — do not invent a second stage — 12–30s
@图片6 — ROLE_VENUE_CONSISTENCY — audience orientation and right side — preserve seating direction — 12–30s
```

## Locks

**Character:** `CHARACTER_GEO_OPERATOR`, the same person from `@图片1`; fixed face, shoulder-length dark hair, navy shirt, light jacket, and canvas bag. Motion changes from tired concentration to grounded confidence; identity never changes.

**Venue:** one training hall. The stage screen stays at the far end, entrance remains camera-left, aisle runs along the right, and audience faces the stage. The office is a separate opening location and transitions through a motivated light bridge rather than pretending it is the same room.

## 30-second storyboard

```text
0–8s | Problem / hook
SHOT: over-shoulder medium shot in the night office; scattered notes and a dim monitor.
ACTION: operator pauses over contradictory search questions, eyes move from note to note, exhales, and closes one notebook.
CAMERA: slow dolly in from behind the left shoulder; 50mm; focus shifts from notes to eyes.
AUDIO: keyboard tail, room hum, one quiet breath.

8–12s | Transition
SHOT: close-up of the notebook page as a thin reflected light bridge travels across it.
ACTION: handwritten fragments align into one clear route, without readable invented brand text.
CAMERA: controlled push in; match cut through the light into the training hall screen.
AUDIO: soft riser, no abrupt teleportation.

12–20s | Learning / transformation
SHOT: wide hall view anchored by stage screen, entrance camera-left, aisle right.
ACTION: operator now stands near the first row, listens, then raises one hand and points to a single strategic path on the screen; audience turns attention together but not in synchronized robotic motion.
CAMERA: measured arc from front-left toward the aisle, preserving screen direction and venue landmarks.
AUDIO: trainer voice, room response, subtle chair movement.

20–27s | Result
SHOT: medium three-quarter shot of the operator beside the stage, same wardrobe and face.
ACTION: eyes first find a teammate, torso turns, hand passes a printed plan, teammate receives it with real contact; a small confident smile appears.
CAMERA: 65mm focus pull from plan to operator's eyes, then hold.
AUDIO: paper contact, restrained human reaction, music optional only if specified.

27–30s | Brand moment
SHOT: wide-to-medium final composition with the stable stage and team behind.
ACTION: operator faces the group, everyone settles into a purposeful working pose; hold the final frame for two seconds.
CAMERA: gentle push in, no compound movement.
AUDIO: room tone resolves naturally; no subtitles unless supplied as a separate authorized asset.
```

## Final prompt excerpt

Use the [Seedance 2.5 final prompt template](../templates/seedance25-final-prompt-template.md) to compile the complete version. The final prompt must repeat the character and venue locks, preserve the light-bridge transition, and include negative constraints for face drift, venue drift, extra stages, mirrored aisle direction, unreadable text, extra fingers, floating paper, and abrupt teleportation.
