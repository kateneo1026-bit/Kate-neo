---
name: daily-review
description: Daily check-in for the "Kate" Instagram account. Reads yesterday's numbers in tracking/results.csv, explains what worked and why, improves today's planned post (hook, topic, format, Google Flow prompts), saves an improved copy and ends with a French checklist for today. Use when Kate types "/daily-review" or asks "what should I post today".
---

# Daily review for "Kate"

Kate reads this on her phone. Keep the chat answer **short**: short lines, few tables, no long paragraphs.

## Step 1: Check the numbers first
1. Read `tracking/results.csv` (columns: `date,type,topic,hook,views,saves,shares,comments,new_followers,notes`).
2. Find **yesterday's** rows (yesterday = today − 1 day).
3. **If a row for yesterday has an empty `views`, `saves`, `shares` or `new_followers`: stop.** Ask Kate for the missing numbers in one short message, for example:
   > What are yesterday's numbers for "[topic]"? Views / saves / shares / comments / new followers
   Wait for her answer, write the numbers into the CSV, and only then continue.
4. If there was no post yesterday (a Stories-only or rest day), say so in one line and use the last 7 days instead.

## Step 2: Analyse (yesterday + the last 7 days for context)
For each post with numbers:
- **Save rate** = saves ÷ views · **Share rate** = shares ÷ views · **Follow rate** = new_followers ÷ views
- **Score** = (saves + 2 × shares + comments + 3 × new_followers) ÷ views × 100

Compare yesterday's post with the 7-day average and the best post of the week. Then explain in simple words:
- ✅ **What worked:** which number was strong, and why (the hook, its formula number from `hooks/hooks-library.md`, the topic, the format, the posting time)
- ❌ **What didn't:** which number was weak, and the most likely reason
- 👉 **Lesson for today:** one sentence

The account is small, so compare posts with each other, never with big accounts. With fewer than 3 posts, say the data is still thin.

## Step 3: Improve today's content
1. Find today's plan in `content-plan/week-YYYY-MM-DD.md` (the file whose Monday is in the current week). Also look for today's Flow prompts in `content-plan/prompts/` if they exist.
2. Improve it based on the lesson:
   - **Hook:** if the hook formula or style performed badly, rewrite it with a better formula from `hooks/hooks-library.md`. Keep it to 12 words or fewer, and add the formula number.
   - **Topic or format:** move towards what performed best (e.g. more hidden story, a time stamp in the hook, more natural sound), but keep the post type that's planned for today.
   - **Caption:** keep the search keywords, and strengthen the first line.
   - **Google Flow prompts** (if today is a reel made with Flow): **first read `references/flow-prompt-lessons.md` and apply every point in "Rules that work".** Then update the prompts only where needed.
   - **Real-photo check (every clip and image of a real place):** look at real photos first and write the check table (rule 7 in `references/flow-prompt-lessons.md`). If no photos are available, ask Kate for 2–3 before writing that prompt.
   - **Realism check:** also read `references/realism-check.md`. Every Flow/Gemini prompt starts with its realism block, uses one of its light recipes (window daylight by default) and its extra Avoid words, and passes its 30-second check. Never `cinematic`, `moody`, `dark`, `blue dusk`, `2700K`.
   - When Kate shares how her Flow clips turned out (what went wrong, what fixed it), add an entry to the "Log" in `references/flow-prompt-lessons.md`. If the fix is a new lesson, add it to "Rules that work" too. When Kate sends screenshots of our clips next to reels she likes, compare them with the table in `references/realism-check.md` and add any new difference there.
3. If today is a Stories-only day, improve the 3 Stories instead.
4. **Stories always follow `content-plan/stories-rule.md`:** format (image or video), a ready-to-use prompt (Flow for video, Gemini for image), the text on screen, and a spare prompt for every video.

## Step 4: Save (never overwrite the original)
- Save the improved version to `content-plan/daily/YYYY-MM-DD-improved.md` (today's date).
- At the top, put a small table with columns **Before → After** (hook, topic, format) and a one-line reason.
- Then the full improved post: hook, script, caption, hashtags, CTA, Flow prompts (if any), and today's 3 Stories.
- Leave the week plan file unchanged so Kate can compare the two.
- If the hook or topic changed, update today's row in `tracking/results.csv` (the `hook` and `topic` columns only).

## Step 5: Reply in chat (short, for a phone)
1. Yesterday in 3 lines: ✅ worked · ❌ didn't · 👉 lesson
2. Today's change in 1–2 lines (new hook) + the file path
3. Finish with this checklist **in French**:

```
✅ Aujourd'hui
- Publier : [type + sujet] à [heure, heure UK]
- 3 stories : matin [..] · midi [..] · soir [..]
- Après la publication :
  - Répondre à tous les commentaires dans la 1re heure
  - Commenter 5 comptes de ta niche (cosy / slow living / hidden places UK et Europe), avec de vrais commentaires de plus de 5 mots
  - Ce soir : noter les chiffres d'aujourd'hui dans tracking/results.csv
```

Post times (UK): weekdays at 12:30 or 19:30, weekends at 10:00, unless the data shows a better time.
