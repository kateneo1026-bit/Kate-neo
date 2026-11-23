---
name: weekly-plan
description: Generate next week's Instagram plan for the "Kate" account (Quiet days and Hidden stories), with 3 reels, 2 carousels and 3 stories per day, then save it in content-plan/. Use when Kate asks for a weekly plan, "/weekly-plan", or "plan my week".
---

# Weekly plan for "Kate"

## The account
- **Name:** Kate. **Bio:** "Quiet days and Hidden stories"
- **Niche:** brown lifestyle (warm brown aesthetic: coffee, wood, linen, old stone, soft light) + hidden stories about UK and European places (cafés, old buildings, hotels, restaurants, streets, food)
- **Audience:** UK and Europe, English language
- **Goal:** build a small, loyal community first. Earn affiliate income later from hotels, restaurants, travel guides and tours, home decor and useful home items.
- **Filming:** Android phone only, alone, no face needed. Use natural sound and a calm voiceover or text on screen.

## Before writing
1. Read `tracking/results.csv`. Don't repeat a topic from the last 4 weeks. If there's data, lean towards the types and topics with the most saves, shares and new followers.
2. If a review file exists in `reviews/`, follow its "Repeat" and "Stop" lists.
3. Read `hooks/hooks-library.md` and build every hook from one of its formulas. Write the formula number next to the hook.
4. The plan starts on the **next Monday** after today, unless Kate gives a date.

## What to produce (exactly)
- **3 Reels:** 2 lifestyle (vibe) + 1 hidden story
- **2 Carousels:** 1 lifestyle + 1 hidden story
- **3 Stories per day**, Monday to Sunday (21 in total)

Suggested days: Reel Mon, Wed, Fri · Carousel Tue, Sat · Sun = rest day (Stories only). Post times (UK): 12:30 or 19:30 on weekdays, 10:00 at weekends.

### For each Reel
- **Topic:** one line
- **Hook (first 2 seconds):** the words on screen + what the viewer sees. Make it strange, specific and calm, never clickbait shouting. Add the formula number.
- **Script (25–30 s):** a table with columns time · shot (filmable on an Android phone, alone) · voiceover/text. Use 5–7 shots.
- **Caption:** first line = the hook rephrased. Then 2–4 short lines. Work in **search keywords** naturally (e.g. "hidden café in London", "quiet weekend in Bruges"), because Instagram search reads captions.
- **Hashtags:** 5–8, a mix of niche and place tags. No huge generic tags like #love.
- **CTA:** one only. Use save, share, comment a word, or follow for more hidden stories.
- **Affiliate (optional, one line):** a natural link idea (hotel, restaurant, tour, home item). Only if it fits. If used, the caption must start with "#ad" (UK ASA rules).

- **Google Flow prompts (when a reel will be made with Flow, or Kate asks for them):** first read `references/flow-prompt-lessons.md` and apply every point in "Rules that work". Write ~7-second clips (4 clips + 1 spare per reel).
- **Realism check:** also read `references/realism-check.md`. Every Flow/Gemini prompt starts with its realism block, uses one of its light recipes (window daylight by default) and its extra Avoid words, and passes its 30-second check. Never `cinematic`, `moody`, `dark`, `blue dusk`, `2700K`.

### For each Carousel
- Topic, a hook (slide 1 text), a slide plan of 6–8 slides (one line each), caption with search keywords, hashtags and CTA (usually "Save this").

### Stories (3 per day)
**Permanent rule:** read `content-plan/stories-rule.md` and follow it for every story. Each story needs its format (image or video), a ready-to-use prompt (Google Flow for video, Gemini for image), the text on screen and sticker, and a spare Flow prompt for every video. Start with the quick table below, then add one block per story.
A table with columns day · morning (engage: poll, quiz or question) · midday (behind the scenes or a quiet moment) · evening (share today's post, or a link sticker if there's an affiliate link). One line per cell.

## Style rules
- Calm, warm, a little mysterious. Short sentences. British spelling.
- Only use facts you're sure of. Mark anything to check with **[check]** (dates, prices, opening times).
- Places must be real and reachable from the UK or Europe.
- Keep it simple and filmable this week with a phone.
- **Look:** bright, natural and real (soft window daylight, cream and caramel tones, a full still life, one small real movement). Not dark and cinematic. See `references/realism-check.md`.

## Output
Save to `content-plan/week-YYYY-MM-DD.md` (Monday's date) with these sections:
1. Week at a glance (a table with day, post, type, topic)
2. Reels
3. Carousels
4. Stories
5. Shot list for the week, grouped by location so Kate can film everything in 1–2 outings

Then add one line for each planned Reel and Carousel (not Stories) to the end of `tracking/results.csv` (date, type, topic, hook, leave the numbers empty). Finally, give Kate a 5-line summary in chat.
