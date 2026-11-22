# Cinematic Generation Standard (Kate) · v3, set by the user on 22 Nov 2026

> **This is the master standard for every Google Flow video and image prompt.** It overrides older prompt advice.
> Used by: `kate-content-planner` (this repo). Paste-ready block for the account skills
> `kate-uncovers-video` and `kate-uncovers-weekly-plan` is at the bottom.

## Kate's priorities (in this order)
1. **Photographic realism**
2. **Historically accurate details**
3. **Beautiful but believable lighting**
4. **Natural human movement**
5. **Cinematic camera behaviour**
6. **Consistency between scenes**

## The standard (7 parts: every prompt covers all of them)

### 01. Lighting
Physically motivated lighting (name the real source: window, lamp, candle, fire, street light), natural falloff, realistic shadow depth, controlled highlights, no artificial glow.

### 02. Camera
Specify **camera position**, **lens characteristics** (e.g. 35mm, 50mm, 85mm macro), **depth of field** and **one controlled movement** (slow push-in, slow lateral slide, gentle handheld drift, locked-off).

### 03. Human movement
Natural body weight, believable walking rhythm, realistic hands, anatomically correct movement.
(The standard also mentions subtle facial expressions. **Kate is faceless**, so this applies only to background people, who stay blurred, at a distance or seen from behind.)

### 04. Material realism
Detailed fabric fibres, natural skin texture, aged wood, imperfect surfaces, physically realistic reflections.

### 05. Environmental realism
Natural fire/candle movement, subtle dust, atmospheric depth, environmental interaction (steam, rain on glass, breath in cold air, flour settling).

### 06. Image quality
Photorealistic (historical) cinematography, fine details, natural contrast, realistic dynamic range, no plastic-looking textures.

### 07. Negative constraints
No morphing, no flickering, no duplicated people, no distorted hands, no floating objects, no unnatural movement, no sudden exposure changes.

---

## Kate identity block (MANDATORY whenever any part of Kate is visible)
Flow cannot guess who Kate is. If the prompt doesn't describe her, Flow chooses for itself (see lesson 22 Nov: wrong skin tone, deformed hands).

> **Hands / arms:** `Kate, a 26-year-old British woman with fair skin with warm undertones and natural skin texture, slim hands with five correctly formed fingers, short almond nails painted mocha brown, a thin gold ring on her right index finger, a small gold watch with a brown leather strap on her left wrist, the cuff of an oversized oatmeal knit jumper`
>
> **Back view:** `Kate, a slim 26-year-old British woman with fair skin, seen only from behind, long chestnut-brown hair in a low tortoiseshell claw clip, [outfit from brand-kate.md], no face visible`
>
> **Legs/POV:** `Kate's legs in dark straight-leg jeans / dark tights and brown leather ankle boots, seen from her own point of view`

(Skin tone default = fair with warm undertones. The user can change it in `brand-kate.md`, and then it must change here too.)

## Hands: rules (hands are the #1 failure in AI video)
- **One hand** in frame when possible; two hands only if each has a clear job.
- **One simple action** (pouring, stirring, turning a page). Describe the grip: *"fingers wrapped around the wooden spoon handle, thumb on top"*.
- Medium close-up distance (50mm) is safer than extreme macro.
- Keep hands slow; fast hand movement causes morphing.
- Attach the `kate-hands` reference image as an ingredient whenever the model allows it. If the model/feature doesn't accept ingredients, the identity block in text is essential.
- No text on objects: say *"plain unlabelled candle jar"*, *"plain notebook"*.

## Consistency between scenes
- Same **identity block**, same **ingredients**, same **outfit and props** in every clip of a reel.
- Same **time of day and light direction** within a reel (e.g. "lamp on the left, rainy window on the right").
- Write a one-line **continuity note** per reel ("blue dusk, lamp left, oatmeal jumper, cream bowl").
- Generate clip 1 first; if it's good, reuse it (or its last frame) as the reference for the next clips.

## Historical accuracy (hidden stories)
- Research first; describe only verified, period-correct details (architecture, clothing, tools, food, materials).
- Add `cinematic historical recreation, not archival footage` to historical scenes, and say so in the caption.
- No anachronisms (no modern lamps, plastic, zips, phones in old scenes). Name the period: *"Victorian kitchen, 1880s"*.

---

## Prompt structure v3 (fill every line, in this order)
```
Vertical 9:16, 8-second shot.
SCENE: [what happens, where, the 1–2 hero objects, the season/time].
KATE: [identity block for what shows: hands / back / legs] + [the one action, with the grip].
CAMERA: [position], [lens], [depth of field], one movement: [move].
LIGHT: [motivated source(s) and direction], natural falloff, realistic shadow depth, controlled highlights, no artificial glow.
MATERIALS: [fabric fibres, skin texture, aged wood, imperfect surface, reflections relevant to the scene].
ENVIRONMENT: [steam / rain on glass / candle flicker / dust / atmospheric depth].
MOOD & COLOUR: quiet and cosy, chocolate brown, caramel, cognac and cream tones, natural contrast, realistic dynamic range.
QUALITY: photographic realism, cinematic camera behaviour, fine detail, no plastic-looking textures.
SOUND: ambient sound only: [sounds].
AVOID: no morphing, no flickering, no duplicated people, no distorted hands, no extra fingers, no floating objects, no unnatural movement, no sudden exposure changes, no face visible, no text, no labels, no logos, no watermarks, no music, no speech.
```
Write each prompt as one standalone paragraph (Flow doesn't remember the previous prompt).

## Example: Stir-up Sunday, clip A (rewritten after the failed generation)
```
Vertical 9:16, 8-second shot. SCENE: a cosy London kitchen table on a rainy November evening, a cream ceramic mixing bowl full of dark sticky Christmas pudding mixture with raisins and candied peel. KATE: one hand of Kate, a 26-year-old British woman with fair skin with warm undertones and natural skin texture, slim hand with five correctly formed fingers, short almond nails painted mocha brown, a thin gold ring on her right index finger, the cuff of an oversized oatmeal knit jumper; her fingers are wrapped around a wooden spoon handle, thumb on top, stirring slowly in one direction; her other hand is out of frame. CAMERA: high angle at 45 degrees above the table, 50mm lens, shallow depth of field focused on the spoon and the hand, one movement: a very slow push-in. LIGHT: warm table lamp from the left and cool blue rainy window light from the right, natural falloff, realistic shadow depth, controlled highlights, no artificial glow. MATERIALS: aged walnut table with fine scratches, visible knit fibres, natural skin texture, glossy sticky mixture, a few grains of flour on the wood. ENVIRONMENT: a plain unlabelled candle jar flickering softly at the edge of frame, faint rain on the window. MOOD & COLOUR: quiet and cosy, chocolate brown, caramel, cognac and cream tones, natural contrast, realistic dynamic range. QUALITY: photographic realism, cinematic camera behaviour, fine detail, no plastic-looking textures. SOUND: ambient sound only: spoon against ceramic, soft rain. AVOID: no morphing, no flickering, no duplicated hands, no distorted hands, no extra fingers, no floating objects, no unnatural movement, no sudden exposure changes, no face visible, no text, no labels, no logos, no watermarks, no music, no speech.
```

---

## Paste-ready block for the account skills (kate-uncovers-video, kate-uncovers-weekly-plan)
These two skills are synced from the user's Claude account. Edit them in Claude's skill settings.
**Both skills:** add this section under "Flow prompt rules":

```
### Cinematic Generation Standard (mandatory, v3)
Priorities: photographic realism; historically accurate details; beautiful but believable lighting; natural human movement; cinematic camera behaviour; consistency between scenes.
Every prompt covers: 01 Lighting: physically motivated, natural falloff, realistic shadow depth, controlled highlights, no artificial glow. 02 Camera: position, lens, depth of field, one controlled movement. 03 Movement: natural body weight, believable walking rhythm, realistic hands, anatomically correct movement. 04 Materials: fabric fibres, natural skin texture, aged wood, imperfect surfaces, realistic reflections. 05 Environment: natural fire movement, subtle dust, atmospheric depth, environmental interaction. 06 Quality: photorealistic historical cinematography, fine detail, natural contrast, realistic dynamic range, no plastic textures. 07 Avoid: no morphing, no flickering, no duplicated people, no distorted hands, no floating objects, no unnatural movement, no sudden exposure changes.
Kate identity (always when hands, legs or back show): a 26-year-old British woman with fair skin with warm undertones, slim hands with five correctly formed fingers, short almond mocha-brown nails, a thin gold ring on the right index finger, a small gold watch with a brown leather strap, an oversized oatmeal knit cuff; from behind: long chestnut-brown hair in a low tortoiseshell claw clip. Never show her face.
Hands: one hand, one slow action, describe the grip, 50mm medium close-up, no labels or text on objects.
Consistency: same identity, outfit, props, time of day and light direction in every clip of a reel.
```

### Story rule for `kate-uncovers-weekly-plan` (matches kate-content-planner)
In section 5 ("Weekly mix"), **replace** the line that starts with "1 Story a day:" with:
```
- 3 Stories every day (21 a week), at fixed times (UK):
  07:30 Mood: a calm clip or still (coffee, window, rain) + a poll or "Quiet Question".
  12:30 Value + link: behind the post / an extra tip + a link sticker (affiliate, with "Ad" on the frame).
  20:30 Tribe: question box, "this or that", poll results, a reply to a DM (anonymous), or a teaser of tomorrow.
  Stories reuse Reel clips and stills, so they cost few or no extra Flow credits.
```
In section 10 ("Workflow"), step 3, **replace** "and 7 Stories" with "and 21 Stories (3 a day)".
In section 11 ("Output format"), **replace** the Stories line with:
```
- Stories: a table with one row per day and three columns (07:30 Mood · 12:30 Value + link · 20:30 Tribe), each with what's on screen, sticker and text, and visual source.
```

