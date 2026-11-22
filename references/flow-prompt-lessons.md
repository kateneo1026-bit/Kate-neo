# Google Flow: prompt lessons

This notebook records what I've learnt making Kate's reels with Google Flow (Veo).
**Read it before writing any Flow prompt, and add a Log entry after every reel.**

---

## Rules that work

### Always include
1. **"Vertical 9:16"** at the start of the prompt, and set 9:16 in Flow's settings.
2. **The look:** `ultra-sharp, clean modern digital cinema look, photorealistic, high detail`.
3. **The camera:** lens + aperture + one slow movement (`slow smooth push-in`, `slow gimbal walk forward`, `static on a tripod`).
4. **One action per clip, at natural speed** (keep only the *camera* slow), and **movement from the very first frame** (steam already rising, door already open, phone already ringing). Viewers decide in under 2 seconds.
   For events, give the **order and timing**: `already ringing at 0s; within the first 2 seconds the hand lifts the receiver; the ringing stops`.
5. **The same "set" description, word for word, in every clip of a reel** (objects, colours, light, sleeve/hands), so the clips look like one place.
6. **A colour palette line** (e.g. `honey gold, crimson, warm amber against muted navy dusk`).
7. **Real places: describe the real details** from reference photos (look at them **before** the first prompt, never describe from memory) (wall colour, objects, lamps, signs). A generic prompt gives a generic place.
8. **People:** `framed from the shoulders down` or `seen only from behind`. Faces are where AI fails most, and they break the "hidden" mood.
9. **Audio line:** describe 2–3 natural sounds, then end with `No music, no speech.`
10. **Avoid line:** `film grain, dust, specks, flickering, text, numbers, timestamps, watermarks, logos, faces, extra fingers, distorted hands, fast camera movement`.
11. **The same object in every clip: text alone is not enough.** Pause on the best clip, save that frame as an image (Flow's image ➕ button) and use it as an **ingredient or start frame** for every other clip, with the words `exactly the same pillar as in the reference image`.
12. **Name the exact period object** (e.g. `1920s black candlestick telephone: tall upright stem, mouthpiece on top, separate earpiece hanging on a hook at the side`). Otherwise the AI picks a generic one.
13. **Vary the light, and make the hook bright.** Not every reel at night: dark openings lose viewers. Golden hour (low warm winter sun) is bright *and* cosy.
14. **Pick Flow-friendly topics.** The story must work without an exact copy of a strange real object (police box, specific statue, odd building). At most one clip has to look like the real place. Stories carried by people from behind, animals, candlelight or objects work best. (20 Nov police box: 4 rounds, never usable.)
15. **Two-round rule.** A clip that fails twice → use the spare or drop it. The key visual fails twice → change the topic that day.

### Never
- **"35mm film" or "grain"** in the prompt. It adds dust, black specks and fake date stamps (e.g. "9/13").
- **Lettering or signs you didn't spell out.** AI writes nonsense ("AULMS", "R:RZLPER"). Either ask for `no lettering` and add the text in CapCut, or spell out the word: `the single word "Rules"… Exact spelling: R-u-l-e-s` + `Avoid: misspelled words, extra letters, any other text`. Re-run once, then fall back to CapCut.
- **"Blue hour" on its own.** It gives a bright cyan sky. Write `muted deep navy-blue sky, just after sunset`.
- **Vague wall art** ("framed cartoons", "pictures"). It gives childish cartoons. Write `black-and-white vintage sketches and gilt-framed oil portraits`.
- **Brand names or logos on products.** Write `no logos or brand names`.
- **Screenshots or clips from other creators** as Flow ingredients or in the reel. That's copyright, even with the watermark removed.
- **A static photo collage as a reel.** It got a 2s average watch time and an 84.9% skip rate.

### Stories (permanent rule, 22 Nov)
Every story in every plan states: **format** (image or video), a **ready-to-use prompt** (Google Flow for video, Gemini for image), the **text on screen**, and a **spare prompt** for every video. Rules 14 and 15 apply to Stories too: Flow-friendly subjects only, and a clip that fails twice → use the spare (if the spare fails, post it as an image). Full rule and Gemini image rules: `content-plan/stories-rule.md`.

### Workflow
- Flow makes ~8s clips. **Trim to ~5s** and cut any still frames at the start. (19 Nov: with 6–7s clips, ~70% of viewers had left by 3s. Faster cuts keep people watching.)
- **The first 3 seconds must be bright enough and show the "strange thing" itself** (the door, the object). A dark, slow opening loses people.
- **5 clips a day:** plan 4 clips + 1 spare for whichever fails.
- **Text on screen, names and addresses:** always add them in CapCut, never rely on Flow for them.
- If the end of a clip is blown out to white, lower Highlights in CapCut or cut before it.
- Realistic AI scenes of real places: turn on Instagram's **AI label** and add "Scenes reimagined with AI" to the caption.

---

## Log

### 2026-11-18 · Reel "A slow morning in brown tones" (lifestyle)
- **First prompt (clip 1):**
  ```
  Vertical 9:16 cinematic macro close-up, shot on a 100mm macro lens at f/2.8, very shallow depth of field. A handmade matte dark-brown stoneware coffee cup with a small handle, filled with black coffee, sits on a small old dark walnut wooden table with visible wood grain. Thin, soft wisps of white steam rise slowly and curl upwards from the coffee, lit from the side by low, soft winter morning sunlight coming through a tall window on the left... No people visible.
  ```
- **What went wrong:** the set was too generic and polished compared with cosy-morning reels that perform well (dark rainy window plus a warm lamp, handheld phone feel). The reel was then posted as a **6s static collage** of stills, which got a 2s average watch, an 84.9% skip rate and 0 saves.
- **Correction:** I rebuilt all 5 clips from reference ideas: a dark rainy pre-dawn window against a warm 2700K lamp, a rust-and-cream striped lampshade, a speckled oatmeal stoneware mug, a chocolate-brown knit sleeve and a "6:40 a.m." time-stamp hook in CapCut.
- **Final prompt (clip 1):**
  ```
  Vertical 9:16 handheld smartphone video, natural gentle hand sway, realistic... Very early morning in a small cosy attic bedroom with a sloped white ceiling, still dark. On the left, a window with raindrops on the glass and a deep blue pre-dawn sky outside... A [SKIN] woman's hand and forearm, in an oversized chocolate-brown chunky cable-knit jumper sleeve covering half the hand, short natural nails, reaches in slowly from the right and switches on the lamp. Warm 2700K amber light softly fills the room... Only the hand and arm are visible, never a face.
  Audio: steady soft rain on the window, a small click of the lamp switch, quiet room tone. No music, no speech.
  ```
- **Lesson:** post the **moving clips**, never a collage. The v2 prompts still said "slight grain", so replace that with the clean look (see Rules).

### 2026-11-19 · Reel "A future king had a secret door built here" (hidden story, Rules, Covent Garden)

**Clip 1: the secret door.** It worked first time ✅
```
Vertical 9:16 cinematic shot, 35mm lens, shallow depth of field. A narrow, hidden door set flush into dark mahogany wood panelling in a Victorian London restaurant at night, almost invisible except for a small brass handle. A man's hand in a black leather glove and a dark wool coat sleeve pushes the door open slowly from the first second; warm golden candlelight spills out through the gap onto the dark wood. Slow push-in towards the opening. Colour palette: deep browns, mahogany, burgundy, warm gold candlelight, soft shadows. Mysterious, quiet, historical mood, realistic, like 35mm film with fine grain. Only the gloved hand is visible, never a face.
Audio: a soft wooden creak of the door, a faint murmur and clink of a distant dining room. No music, no speech.
Avoid: text, subtitles, logos, faces, extra fingers, distorted hands, fast movement.
```
- **What went wrong:** the first ~1s was a still, closed door, and the end was blown out to white.
- **Correction (in CapCut):** trimmed the start, and lowered Highlights at the end.

**Clip 2: the couple on the stairs.** It worked first time ✅
```
Vertical 9:16 cinematic shot, 50mm lens, shallow depth of field, camera following slowly from behind. Late Victorian era, about 1890: a stout bearded gentleman in a black frock coat and top hat and an elegant woman in a long dark burgundy velvet gown with her hair pinned up, both seen only from behind, walk slowly up a narrow, dimly lit wooden staircase lined with gilded picture frames, towards a private candlelit dining room. Warm candlelight from above, deep shadows. Colour palette: deep browns, mahogany, burgundy, warm gold. Secretive, romantic, quiet mood, realistic, like 35mm film with fine grain. Their faces are never visible.
Audio: slow footsteps on wooden stairs, the rustle of a velvet gown. No music, no speech.
Avoid: text, subtitles, logos, visible faces, modern clothing, fast movement.
```
- **Lesson:** "seen only from behind" worked perfectly. (History note: the story is from the late 1870s, when Edward was still Prince of Wales.)

**Clip 3: the Rules front in the rain.** This took 4 versions.
- **First prompt:**
  ```
  Vertical 9:16 cinematic shot, 35mm lens, slow handheld walk forward. A narrow London street in Covent Garden on a rainy winter evening at blue hour: wet cobbled pavement reflecting warm light, old brick buildings, and the glowing windows of an old traditional restaurant with dark red paintwork, brass lanterns and warm golden light inside. A few people with umbrellas pass softly out of focus. The camera slows down and holds still on the warm windows for the last 2 seconds. Colour palette: deep browns, burgundy, warm gold windows against cool blue dusk. Cosy, quiet, mysterious mood, realistic, like 35mm film with fine grain. No faces visible.
  Audio: soft rain on cobblestones, distant city sounds, footsteps. No music, no speech.
  Avoid: text, readable signs, logos, faces, fast movement.
  ```
- **What went wrong:**
  - v1 had a nonsense sign ("AULMS") and a bright cyan sky.
  - v2/v3 (no lettering, real Rules details) looked right, but the awning still had nonsense text ("R:RZLPER") and the name wasn't shown.
- **Corrections:**
  - Muted navy dusk, with rain visible from the first second.
  - The real Rules façade from Kate's reference photos: a honey-gold shopfront, gilded pillars, crimson awning, flower boxes with ivy, gooseneck lamps, and leaded windows upstairs.
  - The exact word "Rules" spelled out on the awning.
  - The clean digital look instead of grain.
- **Final prompt ✅:**
  ```
  Vertical 9:16 ultra-sharp cinematic shot, clean modern digital cinema look, photorealistic, high detail, 35mm lens, slow smooth gimbal move forward along Maiden Lane, a narrow old street in Covent Garden, London, on a rainy winter evening just after sunset, under a muted deep navy-blue sky. Fine rain falls gently and is visible in the lamp light from the first second. On the left is the front of a historic London restaurant: a honey-gold painted wooden shopfront with a panelled lower base, gilded ornate pillar tops between the windows, and a long deep crimson canvas awning. On the awning, the single word "Rules" is written in large, elegant cream-gold cursive script, with the small capital letters "EST 1798" underneath. Exact spelling: R-u-l-e-s. Above the awning, along the top of the shopfront, are window boxes overflowing with white and purple flowers and long trailing green ivy, and a row of small black gooseneck lamps glowing warm. Behind the large windows, a warm golden dining room with white tablecloths and red velvet seats, softly blurred. Upper floors: on the left a cream-painted building with tall black sash windows, on the right old yellow London brick with arched leaded diamond-pane windows and a crimson flag hanging from a pole. The wet cobbled pavement reflects the golden light and the crimson awning. Two people with dark umbrellas walk away in the distance, seen only from behind. The camera slows and holds still on the awning and glowing windows for the last 2 seconds. Colour palette: honey gold, crimson, warm amber against muted navy dusk. Cosy, quiet, mysterious mood.
  Audio: soft steady rain on the pavement and on the canvas awning, distant footsteps, faint muffled chatter from inside. No music, no speech.
  Avoid: misspelled words, extra letters, any other text, numbers, signs, logos, watermarks, film grain, dust, specks, bright blue sky, daylight, faces, fast movement.
  ```

**Clip 4: inside Rules, the waiter and the pie.** This also took 4 versions.
- **First prompt:**
  ```
  Vertical 9:16 cinematic shot, 35mm lens, slow smooth dolly forward. Interior of an old traditional London restaurant: rich red velvet banquettes, dark mahogany wood panelling, walls covered in old framed paintings and cartoons in gilded frames, small brass table lamps with warm amber shades, white linen tablecloths, polished silver cutlery and crystal glasses. A waiter's hands in a white shirt cuff and black waistcoat place a golden-crusted pie on a white plate on a table in the foreground. Warm, cosy, dim evening light. Colour palette: deep browns, burgundy red, mahogany, warm gold, cream. Timeless, elegant, quiet mood, realistic, like 35mm film with fine grain. No faces visible.
  Audio: the soft murmur of a dining room, the gentle clink of cutlery and glasses. No music, no speech.
  Avoid: text, readable words, signs, logos, faces, distorted hands, fast movement.
  ```
- **What went wrong:**
  - v1: "cartoons" gave childish cartoon frames.
  - v2: "35mm film with fine grain" gave black floating specks and a "9/13" date stamp.
  - v3: the clean version had no waiter, and the walls didn't look like the real Rules.
- **Corrections:**
  - Replaced grain with the clean digital look, and added specks, numbers and timestamps to the Avoid line.
  - Put the waiter back, framed from the shoulders down.
  - Described the real Rules walls from Kate's photos: mustard-yellow walls, a black-and-gold frieze, a row of sketches, a black shell-topped niche with a marble bust, antelope heads and antlers, dried hops, a bronze statue lamp with a crimson fringed shade, a gilt landscape painting, and a crimson velvet banquette with gold rope trim.
- **Final prompt ✅:**
  ```
  Vertical 9:16 ultra-sharp cinematic shot, clean modern digital cinema look, photorealistic, high detail, crisp focus, 50mm lens at f/2, very slow smooth push-in. Inside a historic London restaurant in the evening. In the foreground, a table with a crisp white linen tablecloth, crystal wine glasses and polished silver cutlery. A waiter, framed from the shoulders down so his face is never visible, wearing a crisp white shirt, a black waistcoat and a long white apron, steps in from the right and gently places a golden, flaky-crusted steak pie in a white fluted ceramic dish on a white plate in the centre of the table. Soft steam rises from the crust, then he steps back out of frame. The background is in soft focus but clearly recognisable: warm mustard-yellow walls with a black-and-gold painted frieze, and a row of small black-framed vintage sketches along the top. In the centre, a tall black arched niche with a carved scallop-shell top holds a white marble bust of an elegant Victorian lady with curled hair and a pearl necklace. Above the niche, mounted antelope heads with long spiral horns and dark stag antlers on black wooden shields. On the left, a hanging garland of dried golden hops and a bronze statue lamp of a woman holding up a crimson pleated lampshade with a fringe. On the right, a gilt-framed landscape oil painting with a small brass picture light. Below, a long deep crimson velvet banquette with gold rope trim, and dark wooden chairs with crimson seats. Warm amber evening light, soft and even. Colour palette: mustard gold, crimson red, black, dark wood, warm amber, white. Elegant, calm, timeless mood.
  Audio: the soft murmur of a dining room, the gentle clink of glasses, a plate set down softly on linen. No music, no speech.
  Avoid: visible faces, other guests in focus, text, numbers, timestamps, watermarks, logos, film grain, dust, specks, flickering, extra fingers, distorted hands, fast movement.
  ```

---

### 2026-11-20 · Reel "Britain's smallest police station is hiding in this lamp post" (hidden story, Trafalgar Square)
- **First prompts:** see `content-plan/daily/2026-11-20-improved.md`, clips 1–4. The set was written out in each prompt but no reference image was used. Everything was at night.
- **What went wrong:**
  1. The police box looked different in every clip (a stone pillar, a blue wooden box, a thin lamp post).
  2. The hook was dark and slow: the door was closed at 0s and only open by 0:05.
  3. The phone was a generic rotary desk phone. It was lifted very slowly, and the ringing came *after* it was lifted.
  4. Every reel had been at night, so the hook was too dark.
- **Corrections:** used a master frame as an ingredient for every clip; started on an open, glowing door; named the exact phone and gave the action order and timing; used golden-hour light for the next reels.
- **Final prompts:** in the 20 Nov daily file (section "Fixed prompts"). Kate to confirm the result.

- **v3 (golden hour, 20 Nov) still failed:** the box didn't look like the real one (a curly lantern, a wooden door, a tall column with fountains), the door opened before the policeman touched it, and the phone scene was confusing.
- **v4 correction:** the box was rewritten from real reference photos (a plain grey granite pillar, a black door with a grid of glass panes in the top half, a geometric octagonal glass lantern, a plane tree behind, cream Victorian buildings). The door timing was made explicit (`at 0s fully closed… at 2s his hand grips the handle… only then does the door move` + `Avoid: door opening by itself`). The phone stayed in the voiceover only, and the reel was cut to 2 clips.
- **Lesson:** look at real photos of the place **before** writing the first prompt, never describe it from memory. Write a clear story (one idea per clip) and say what is in the voiceover rather than forcing it into a scene.
- **Outcome (Kate, 22 Nov):** v4 failed too. No version gave a usable result, with many mistakes in every round, so **the reel was never posted**. A day of credits was lost.
- **Why it failed:** the whole story depended on Flow copying **one unusual real object exactly** (a hollow granite pillar with a door). Flow can't do that reliably, even with reference photos and a master frame. The king's door reel worked because it relied on atmosphere and people from behind, and only one clip had to look like the real place.
- **Lesson:** choose hidden stories that Flow can tell with **atmosphere, animals, objects and people seen from behind**. Keep the real place to one clip at most, or film it yourself. **Two-round rule:** if a clip fails twice, use the spare or drop the clip, and if the key visual fails twice, change the topic.

### New entry template
```
### YYYY-MM-DD · Reel "[hook]" ([lifestyle / hidden story])
**Clip N: [name]**
- First prompt: ...
- What went wrong: ...
- Correction: ...
- Final prompt ✅: ...
- Lesson: ... (if it's a new rule, add it to "Rules that work")
```
