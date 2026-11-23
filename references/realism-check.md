# Realism check: why some AI reels look real and ours look AI

Comparison made on 23 Nov 2026 from Kate's screenshots.
- **Looks real (Instagram, @markizon_ai, also AI-made):** autumn tablescape with books and candles · lake bench with book and coffee · Paris breakfast table by a rainy window · coffee poured into a floral china cup · rainy Paris window with zinc roofs. Described here in words only: **never use other creators' frames as Flow/Gemini ingredients** (copyright).
- **Looks AI (ours):** `references/realism/kate/` 1 pub room · 2 panel and fire · 3 Flow rain window with muffin · 4 parrot through leaded window · 5 lamp, hydrangea and mug.

Read this together with `references/flow-prompt-lessons.md` before every Flow or Gemini prompt.

---

## What the real-looking ones do (and ours don't)

| # | Real-looking reels | Ours | Fix in the prompt |
|---|---|---|---|
| 1 | **Bright, well exposed.** Soft daylight from a window; you can see every object, even in the "cosy" ones. | Dark, low-key, crushed black shadows (1, 2, 4). | `well exposed, open shadows with visible detail, nothing too dark` |
| 2 | **Natural, muted colours:** cream, oatmeal, caramel, soft grey. White balance only slightly warm. | Strong orange vs. saturated cyan-blue (3, 5): the classic AI "orange-and-teal" look. | `true-to-life colours, gentle warm white balance, muted natural saturation` + Avoid `orange-and-teal grade, oversaturated colours` |
| 3 | **The sky outside is pale overcast grey-white.** | Bright cyan/blue window (3, 5). | `pale overcast grey-white sky outside` (never "blue", "dusk blue", "navy") |
| 4 | **Lamps and candles glow softly**; daylight does most of the work. | Lamp blown out to hot orange, "2700K" light everywhere (3, 5). | `the lamp glows softly, not blown out; daylight is the main light` |
| 5 | **Matte, dry textures:** creased linen, chunky knit, paper pages, dry leaves, crumbs. | Wood looks wet and varnished, glossy highlights everywhere (1, 2, 3). | `matte surfaces, dry natural wood grain` + Avoid `glossy wet-looking surfaces` |
| 6 | **A full, readable scene:** a styled still life of 4–6 everyday objects at different heights (books, cup, candle, vase of dried flowers, croissant, napkin), with one natural detail (leaves, berries). | Empty rooms or one abstract surface with no subject (1, 2). | Describe the still life: hero object + 3–5 supporting props + one natural detail + one fabric |
| 7 | **Moderate depth of field:** background soft but recognisable (Paris roofs, lake). | Heavy bokeh hides everything (2) or a dark blur (4). | `35–50mm at f/4, background softly out of focus but recognisable` |
| 8 | **A clear "where":** zinc mansard roofs, a lake and lamp post. The place is part of the hook. | No place cue (1, 2). | One recognisable background detail of the place (rooftops, chimney pots, a street, water) |
| 9 | **One small real-speed movement** (coffee pouring, steam, candle flame, rain trickling, ripples); the camera is still or almost still. | Camera moves and "cinematic" push-ins; the subject barely moves. | `locked-off camera` or `barely perceptible slow push-in`; the subject moves at natural speed |
| 10 | **Fine rain:** many small droplets and a few thin trickles; the view outside is sharp. | Big uniform drops and a ghostly lamp reflection (3). | `fine small raindrops and a few thin trickles on the glass, the view outside in focus, no reflections in the glass` |
| 11 | **Everyday-lovely objects:** vintage floral china with a gold rim, speckled vase, croissant. | Odd objects (a muffin wrapped in a paper parcel with string, 3). | Name ordinary, real objects; avoid "wrapped", "parcel", "string" |
| 12 | **Looks like lifestyle photography,** not a film still. | "Cinematic", "ultra-sharp", "moody" → dark, over-graded film look. | Drop `cinematic`, `moody`, `dramatic`; use the realism block below |

**What already worked in ours:** 5 (lamp, hydrangea, knit, speckled mug) has the right props and textures; it only needs daylight, a grey sky and a softer lamp. 4 (parrot through a leaded window) is a strong idea; it only needs to be brighter.

---

## The realism block (paste into every prompt)

**Start (replaces the old "ultra-sharp cinematic … digital cinema look" line):**
```
Vertical 9:16 realistic lifestyle video, looks filmed on a good phone camera, photorealistic, sharp focus on the subject, true-to-life colours, gentle warm white balance, soft natural contrast, well exposed with open shadows and visible detail, matte natural textures.
```
For a Gemini image, use the same words with `photo` instead of `video`.

**Light (pick one):**
- **Daylight (default):** `Soft overcast daylight from a large window on the left, bright and airy, a pale grey-white sky outside.`
- **Golden hour:** `Low soft winter sun from the side, warm but not orange, long gentle shadows, everything clearly visible.`
- **Evening / pub / fire:** `Evening, but the room is well lit by two or three warm table lamps and the fire; lamps glow softly, not blown out; shadows keep detail; the whole scene is easy to see.`

**Avoid line (add to the existing one):**
```
dark underexposed image, crushed blacks, orange-and-teal colour grade, oversaturated colours, cyan or bright blue sky, blown-out lamp, glossy wet-looking surfaces, heavy bokeh, HDR look, plastic textures
```

---

## 30-second check before sending a prompt
1. Is the light **daylight or well-lit**? No "dark", "moody", "deep shadows", "dim".
2. Is any sky **pale grey-white** (or golden hour), never blue/navy/cyan?
3. Is there a **still life of 4–6 real objects** + one natural detail + one fabric?
4. Is there **one real-speed movement**, with a still or barely moving camera?
5. Is there a **place cue** in the background?
6. Are the realism block and the extra Avoid words in?

## Check after the clip (before you post)
Pause on frame 1. If it's darker than an Instagram feed post, too orange, or the sky is blue → fix with one re-run (or in CapCut: Exposure +, Shadows +, Saturation −10, Temperature − a little). Two-round rule still applies.
