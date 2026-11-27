# Google Flow: prompt lessons

This notebook records what I've learnt making Kate's reels with Google Flow (Veo).
**Read it before writing any Flow prompt, and add a Log entry after every reel.**
**Also read `references/realism-check.md` (23 Nov): why our clips look AI, and the realism block to paste into every prompt.**

---

## Rules that work

### Always include
1. **"Vertical 9:16"** at the start of the prompt, and set 9:16 in Flow's settings.
2. **The look (updated 23 Nov):** the realism block from `references/realism-check.md`: `realistic lifestyle video, looks filmed on a good phone camera, photorealistic, sharp focus on the subject, true-to-life colours, gentle warm white balance, soft natural contrast, well exposed with open shadows and visible detail, matte natural textures`. The old `ultra-sharp … digital cinema look` + `cinematic` gave dark, orange-and-teal, glossy clips.
3. **The camera:** lens + aperture + almost no movement. Default `locked-off camera` or `barely perceptible slow push-in`, 35–50mm at f/4 so the background stays recognisable. Let the subject move, not the camera.
4. **One action per clip, at natural speed** (keep only the *camera* slow), and **movement from the very first frame** (steam already rising, door already open, phone already ringing). Viewers decide in under 2 seconds.
   For events, give the **order and timing**: `already ringing at 0s; within the first 2 seconds the hand lifts the receiver; the ringing stops`.
5. **The same "set" description, word for word, in every clip of a reel** (objects, colours, light, sleeve/hands), so the clips look like one place.
6. **A colour palette line** (e.g. `honey gold, crimson, warm amber against muted navy dusk`).
7. **Real places: describe the real details** from reference photos (look at them **before** the first prompt, never describe from memory) (wall colour, objects, lamps, signs). A generic prompt gives a generic place.
   **Every clip of a real place:** write a **Real-photo check** table first (real detail → what the prompt says), put the details in the prompt **and** the wrong look in the Avoid line. No real photos seen yet → ask Kate for 2–3 photos first.
   **Real colours beat the default palette:** if the real place is dark, keep it dark and make it bright with **light** (windows, lamps, fire, sun), never by changing the materials.
8. **Kate's account is faceless: no people as the subject.** No woman or "Kate" figure in a scene, **not even seen from behind** (21 Nov: the woman on the bench with a cup was rejected; 25 Nov: the same mistake, caught by Kate). Let places and objects tell the story: an empty bench, an open door, steam from a cup left on a bench. Historical figures **seen only from behind** are OK only in a "past" scene the story needs (19 Nov, the couple on the stairs), with the camera behind them (`heads stay turned away… no face and no profile`). Add `people, a person sitting, faces, silhouettes, hands` to the Avoid line. Small falling objects: `lands flat on its side`.
9. **Audio line:** describe 2–3 natural sounds, then end with `No music, no speech.`
10. **Avoid line:** `film grain, dust, specks, flickering, text, numbers, timestamps, watermarks, logos, faces, extra fingers, distorted hands, fast camera movement, dark underexposed image, crushed blacks, orange-and-teal colour grade, oversaturated colours, cyan or bright blue sky, blown-out lamp, glossy wet-looking surfaces, heavy bokeh, HDR look`.
11. **The same object in every clip: text alone is not enough.** Pause on the best clip, save that frame as an image (Flow's image ➕ button) and use it as an **ingredient or start frame** for every other clip, with the words `exactly the same pillar as in the reference image`.
12. **Name the exact period object** (e.g. `1920s black candlestick telephone: tall upright stem, mouthpiece on top, separate earpiece hanging on a hook at the side`). Otherwise the AI picks a generic one.
13. **Vary the light, and make the hook bright.** Not every reel at night: dark openings lose viewers. Golden hour (low warm winter sun) is bright *and* cosy.
14. **Pick Flow-friendly topics.** The story must work without an exact copy of a strange real object (police box, specific statue, odd building). At most one clip has to look like the real place. Stories carried by people from behind, animals, candlelight or objects work best. (20 Nov police box: 4 rounds, never usable.)
15. **Two-round rule.** A clip that fails twice → use the spare or drop it. The key visual fails twice → change the topic that day.
16. **Famous buildings: one angle, bottom to top.** Pick the single view in a real photo (e.g. the west front, straight on), describe it from the doors up, and list what is *not* there in the Avoid line (`spire in front of the towers, dome`). Never mix parts seen from different sides. No small animals in landmark shots.
17. **Bright first (23 Nov).** Daylight is the default light, with a `pale overcast grey-white sky` (or golden hour). Evenings and pubs: `well lit by two or three warm lamps and the fire, shadows keep detail`. Lamps `glow softly, not blown out`. Never `dark`, `dim`, `moody`, `deep shadows`, `2700K`.
18. **A full still life, not an empty room.** Hero object + 3–5 everyday props at different heights + one natural detail (dried flowers, leaves, berries) + one fabric (creased linen, chunky knit). Matte, dry textures.
19. **One real-speed movement** is the hook: pouring coffee, steam, a candle flame, rain trickling, leaves moving, a bird turning its head.
20. **Frame 1 must prove the hook (26 Nov).** If the hook says "trees *inside* a church", frame 1 must show *inside*: looking up from the nave, open sky where the roof was, branches crossing the empty window arches. A tree in front of a ruin looks like any churchyard (St Dunstan: skip rate 68%, half gone by 2s). Ask: *"With the sound off and no text, does frame 1 already look impossible?"*
21. **Hook text never on sky or a window (26 Nov).** Bright sky is as bad as bright lamps. Put the words on a calm, darker area (stone wall, ground, dark wood) **or** use Instagram/CapCut text with a soft dark background band. Check frame 1 on the phone at arm's length before posting.
20. **A place cue** in the background (slate roofs and chimney pots, a lake, a lane, a church tower), softly out of focus but recognisable.
21. **Fine rain:** `fine small raindrops and a few thin trickles on the glass, the view outside in focus, no reflections in the glass`.

### Never
- **"35mm film" or "grain"** in the prompt. It adds dust, black specks and fake date stamps (e.g. "9/13").
- **Lettering or signs you didn't spell out.** AI writes nonsense ("AULMS", "R:RZLPER"). Either ask for `no lettering` and add the text in CapCut, or spell out the word: `the single word "Rules"… Exact spelling: R-u-l-e-s` + `Avoid: misspelled words, extra letters, any other text`. Re-run once, then fall back to CapCut.
- **"Blue hour", "dusk", "navy sky".** They give a bright cyan sky. Use a pale overcast grey-white sky or golden hour instead.
- **"Cinematic", "moody", "dramatic", "dark", "2700K", "polished/varnished wood".** They give the dark, orange, glossy AI look (23 Nov comparison).
- **Odd props** ("wrapped in paper with string", parcels). Use ordinary objects people own.
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
- **Hook text goes on a calm, darker area** (ask for `the top third of the frame is calm` in clip 1). On the parrot reel the words sat on two bright lamps and were hard to read.
- Real events (fires, wars, disasters): show **glow, smoke and objects**, never a realistic copy of the real building burning, and keep the AI label on.
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

### 2026-11-23 · Reel "In 1926, 200 newspapers reported the death of this pub's parrot" (hidden story, Ye Olde Cheshire Cheese)
- **Prompts:** `content-plan/prompts/2026-11-23-parrot.md` (rules 1–15 applied: bright first frame, parrot moving at 0s, people from behind, master frame as ingredient).
- **Result (24 Nov):** best hold so far: **skip rate 42.3%** (57% king's door, 84.9% collage), **8s average watch**, ~25% stayed to the end. The animal + firelight approach works in Flow.
- **What went wrong:** the hook text sat on top of the two bright pendant lamps and was hard to read. 0 sends, 0 saves: the visuals are no longer the problem, the topic needs a stronger reason to send.
- **Lesson:** keep hook text on a calm, darker area. Clip quality is now good enough: spend the effort on the topic's "send" twist.
- Kate: tell me how each clip did, and I'll add the details.

### 2026-11-24 · Reel "In 2019, Notre-Dame burned. 180,000 bees on its roof survived." (hidden story, Paris)
**Clip 4: Notre-Dame today**
- **First prompt:** a side view from the Seine quay: "the long nave with its flying buttresses, the slender restored spire in the centre, and the two square towers behind", plus a bee crossing the foreground.
- **What went wrong (Kate's screenshot):** Flow mixed the views: a tall spire stood *in front of* the towers, a dome appeared in the middle, the towers were thin and pointed, and the bee came out huge and blurry.
- **Correction (v2):** one simple, straight-on view (the west front from the square), described from Kate's real photo, top to bottom: three portals → row of king statues → rose window → open arched gallery → two identical flat-topped square towers, no spires. Avoid line: `spire in front of the towers, dome, cupola, pointed tower tops`. No bee in that clip. Spare: a closer tilt from the kings to the rose window.
- **Lesson (new rule 16):** for a famous building, choose **one camera angle** that matches a real photo, describe it **from bottom to top**, and say what is **not** there (no spire, no dome). Don't mix parts that are only visible from different sides. Keep small animals out of landmark shots (they come out giant).

### 2026-11-25 · Bees reel results + realism rules merged
- **Result (25 Nov, ~15h):** 476 views, **11s average watch** (best ever, 24s reel), skip rate 43% ("lower" than typical). Broke the ~120 wall: Reels tab 74%, **Explore 26%** (first time). 0 sends, 0 saves, 0 follows.
- **What worked:** golden-light bees moving at 0s, a famous place in the hook, a fire shown only as glow and smoke.
- **Housekeeping:** the 23 Nov realism rules (`references/realism-check.md`, rules 2, 3, 7, 8, 10, 17–21) were on an unmerged branch. Now merged here. Use them from today.

### 2026-11-25 · Reel "A London church with trees inside" (hidden story, St Dunstan-in-the-East)
**Clip 4: today, a quiet bench**
- What went wrong: I wrote "a woman in a camel coat, seen from behind, on the bench". The account is faceless (rule 8): the 21 Nov rule was on an unmerged branch and missing here.
- Correction: an empty bench with a steaming paper cup and a folded scarf left on it, the fountain trickling. `people, silhouettes, hands` in Avoid. Rule 8 restored.

**Clip 2: 1941 glow and smoke**
- First prompt: v1 in `content-plan/daily/2026-11-25-improved.md` ("orange glow from beyond the walls… no visible flames on the building").
- What went wrong (Kate's screenshot): the tracery, embers and glow on the stone were good, but Flow put a bright, blown-out flame on the stone sill at the bottom left. It looks like a campfire on stone, not a city on fire.
- Correction: quick fix = zoom in CapCut on the upper window (tracery + embers + smoke). Re-run (v2) = `the fire itself is out of frame, below and behind the wall; only its orange light on the stone` + Avoid `visible flames, fire on the ground, bonfire, campfire`.
- Result v2 ✅ (12:19): fire out of frame, glow on the stone, smoke and embers through the window, a gable with a cross against a dark sky. Only a tiny flame on the right sill and one at the bottom edge: zoom ~115% and move the frame up in CapCut. Used.
- Lesson: "no visible flames on the building" is not enough: Flow still draws a fire somewhere. Say where the fire is (out of frame) and ban flames in the Avoid line.

**Results (26 Nov, ~18h)**
- 46 views, 13s average watch (**best ever**), save 1, comment 1, 0 sends, 0 follows. **Skip rate 68.2%** (bees 43%, parrot 42%): ~50% gone by 2s, ~70% by 4s, then ~20% stayed flat to the end.
- What went wrong: the story held whoever got past second 2, but the first frame didn't: the hook text sat on the bright window and sky, and the frame looked like a tree in front of a ruin, not a tree *inside* a church. Also the test group had moved after the bees reel (see `reviews/diagnosis-2026-11-26.md`).
- Lesson: new rules 20 (frame 1 proves the hook) and 21 (no hook text on sky).

### 2026-11-27 · Reel "London's real Diagon Alley hides a Roman ruin in a barber's basement" (prep, Leadenhall Market)
- **First prompt (clip 1):** written from text sources only: "arched roof… ironwork painted maroon and cream with dark green details", no dome, no lanterns.
- **What went wrong (before any credits were spent):** Kate's 2 real photos showed it was wrong: the lanes are **barrel vaults** with thin cream ribs, the ironwork isn't green (the green is on shopfronts), and the best view is from **under the octagonal glass dome** (maroon ribs, blue-grey panels, 3 amber lanterns) with **deep-red fluted columns**.
- **Correction:** clip 1 and its spare rewritten from the photos (`content-plan/prompts/2026-11-28-leadenhall.md`); wrong looks added to the Avoid line (pointed Gothic arches, green ironwork, lettering on the frieze).
- **Lesson:** text descriptions of a place are not enough (rule 7 confirmed). Ask Kate for 2 photos **before** writing the prompt, and use other creators' photos only to describe the place in words, never as an ingredient.

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
