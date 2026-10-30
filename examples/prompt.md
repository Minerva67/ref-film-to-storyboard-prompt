# Complete Video Generation Prompt (copy as a whole)

> Example output for a fictional brand (Tomo). Source of every on-screen word: the Tomo brief. Items marked `[TBC]` must be replaced before generating — do not invent them.

**Brief:** 20-second minimal desk product film, 16:9, 1920×1080, 24 fps. Title: "Tomo — One turn. One focus." Music-driven with a minimal three-line voiceover. Tone: calm, precise, warm, quiet — a real home-office desk in morning daylight, not a tech demo, not a spinning product showcase.

## Narrative Design
The film borrows five mechanisms from a minimal desk product reference: a single top-down desk as the only stage; the product always centred and still; a hand as the only sign of a person; one big type card per selling point, doubling as a rhythm divider; and a logo card to close. Cuts are hard and land on the beat. The only slow moment (3 s, music drops out) is reserved for the difference that matters: turning the dial makes the light ring fill. The film ends on the wordmark and tagline.
Beats (20 s):
1. Hook (0–2 s)
2. The desk (2–5 s)
3. One turn (5–8 s)
4. A hand (8–10 s)
5. The app (10–13 s)
6. The facts (13–15 s)
7. Focus (15–17 s)
8. Close (17–20 s)

## Rendering Rules
**Constant product description (repeat in every shot that shows the product):** Tomo is a round desk timer about 9 cm across and 4 cm tall, with a matte warm-white body, a single knurled aluminium dial on top, and a thin light ring around the base that glows tomato red (#E5553B). No screen and no other buttons. One USB-C cable exits at the back and runs off-frame. Tomo never changes shape, colour, proportion or brand mark between shots.

**Layer A — Live-action footage (≈4 of 20 s).** Photorealistic, cinematic live-action look: real skin, real knit fabric, real oak wood grain, natural daylight from the left, shallow depth of field, locked-off camera, film-like colour, mild grain. These shots must NOT be rendered as illustration, flat vector, cel-shaded, 3D-cartoon or motion-graphic style — they must read as footage shot with a camera at a real desk. Cast: one adult in a plain grey knit sweater, short dark hair. Frame them from above, from behind or at the hands only — never a face, never two people. No shot on this layer longer than 2 s. Set: a light oak desk, a closed sage-green notebook, one black pen, a plain white mug, Tomo in the centre. Same set in every live shot.

**Layer B — Precision graphics (≈10 of 20 s).** Vector-sharp, digit-accurate typography and layout; brand palette: paper #F3EFE6 (background), ink #1F2421 (type), tomato red #E5553B (accent, light ring, underlines), sage #9DB5A0 (secondary), grey #8C8A84 (small print). Typeface: a bold geometric sans-serif for headlines, the same family in regular weight for small text. Text is identical to this prompt, letter for letter. Title cards, spec chips and the top-down desk plan live here.

**Layer C — Product hero render (≈3 s).** One physically-based hero shot of Tomo on the oak desk, studio softbox reflections on the aluminium dial, real material response on the matte body; used only in Beat 3.

**App screen.** Flat, clean phone UI in the brand palette showing a weekly bar chart; clearly a screen, not the real world. Bar heights and numbers: [TBC — use the client's real app UI; do not invent values].

**Transitions:** hard cuts only. **Music:** soft piano over a low pulse; the music drops out during Beat 3, leaving only the dial's click. **Text animation:** snap in on the beat, no bounce, no glow.
**Voiceover:** one voice, warm, unhurried; three lines only, landing at the timecodes below and matching the on-screen text word for word; silence elsewhere.

---
## Hook | 0:00–0:02
**VO (0:00–0:02):** "Turn the dial. Your focus session starts."
1. **[GRAPHIC]** 0:00–0:02 — Full-frame paper #F3EFE6. Two lines of bold ink #1F2421 type, left-aligned: "Turn the dial." / "Your focus session starts." A thin tomato-red #E5553B line draws under the second line from left to right. Duration 2 s.

## The desk | 0:02–0:05
2. **[GRAPHIC]** 0:02–0:05 — Flat, vector-sharp top-down plan of the desk: light oak surface, closed sage notebook, black pen, white mug, Tomo exactly in the centre per the constant description. The light ring is off for 1 s, then glows once in tomato red and dims. No text. Duration 3 s.

## One turn | 0:05–0:08
3. **[PRODUCT RENDER]** 0:05–0:08 — 45° close-up of Tomo on the oak desk. The knurled dial turns clockwise at an even speed; with each click one more segment of the light ring lights up; the dial stops and the lit segments hold. No numbers on screen. One continuous 3 s shot, no cuts. Music is silent; only the click is heard. Duration 3 s.

## A hand | 0:08–0:10
4. **[LIVE · top-down]** 0:08–0:10 — Locked-off top-down view of the same desk, Tomo centred. A hand in a grey knit sleeve enters from the right and rests two fingertips on the dial, then holds still. The hand does not turn the dial. No face. Duration 2 s.

## The app | 0:10–0:13
**VO (0:10–0:13):** "The Tomo app counts your focus minutes."
5. **[APP · full-frame]** 0:10–0:13 — Phone screen fills the frame: the Tomo app's weekly focus chart. Bars grow from left to right one after another; the last bar stops on today. On-screen text: "The Tomo app counts your focus minutes." Bar values: [TBC]. Duration 3 s.

## The facts | 0:13–0:15
6. **[GRAPHIC]** 0:13–0:15 — Paper background. Two spec chips stacked, each with a tomato-red dot on the left: "1 click = 1 minute" / "Up to 60". They slide up 12 px into place on consecutive beats, no bounce. Duration 2 s.

## Focus | 0:15–0:17
7. **[LIVE · from behind]** 0:15–0:17 — From behind and slightly above, the person in the grey knit sweater sits at the same desk writing in the open notebook; Tomo glows softly beside the notebook. Back of the head and shoulders only. Very slow 3% push-in. No VO. Duration 2 s.

## Close | 0:17–0:20
**VO (0:17–0:20):** "Tomo. One turn. One focus."
8. **[GRAPHIC]** 0:17–0:20 — Full-frame paper. Ink wordmark "Tomo" centred; below it, in tomato red, "One turn. One focus."; below that, in small grey type, the URL [TBC]. The wordmark cuts in on the beat, the tagline appears 0.3 s later, hold 2 s. Duration 3 s.

## Hard Constraints
1. Total 20 s exactly; 8 numbered shots on whole-second boundaries (2 / 3 / 3 / 2 / 3 / 2 / 2 / 3 s).
2. Live-action shots (4, 7) must read as photorealistic camera footage — no illustration, vector or cartoon look. No live shot longer than 2 s.
3. Faces: never shown. People appear from above, from behind, or as a hand only; never more than one person.
4. Tomo's appearance is identical in every shot per the constant description; the cable always exits at the back.
5. Same desk set in every live shot: light oak desk, closed sage notebook, black pen, white mug.
6. All on-screen text letter-for-letter, and nothing else: "Turn the dial." · "Your focus session starts." · "The Tomo app counts your focus minutes." · "1 click = 1 minute" · "Up to 60" · "Tomo" · "One turn. One focus." · URL [TBC]. No prices.
7. Palette on the graphic layer only: #F3EFE6, #1F2421, #E5553B, #9DB5A0, #8C8A84. The live layer keeps natural daylight colour.
8. Transitions: hard cuts only. Music drops out during shot 3.
9. Countable check: shot 2 shows exactly 3 objects besides Tomo (notebook, pen, mug); shot 6 shows exactly 2 spec chips; shot 4 shows exactly one hand.
10. VO is exactly these 3 lines, in order, at the listed timecodes: "Turn the dial. Your focus session starts." (0:00–0:02) · "The Tomo app counts your focus minutes." (0:10–0:13) · "Tomo. One turn. One focus." (0:17–0:20) — nothing else is spoken; no VO during shots 2, 3, 4, 6 and 7.
