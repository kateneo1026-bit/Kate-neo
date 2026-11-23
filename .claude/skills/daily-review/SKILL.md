---
name: daily-review
description: Daily check-in for the "Kate" Instagram account. Reads yesterday's numbers in tracking/results.csv, explains what worked and why, improves today's planned post (hook, topic, format, Google Flow prompts), saves an improved copy and ends with a French checklist for today. Use when Kate types "/daily-review" or asks "what should I post today".
---

# Daily review for "Kate"

Kate reads this on her phone. Keep the chat answer **short**: short lines, few tables, no long paragraphs.

## Step 0: Instagram screenshots (if Kate sends them)
Read every screenshot before anything else:
- **Reel insights:** views, viewers, avg watch time, skip rate, likes, reposts, shares, saves, follows, retention curve (how many have left by 3s), "this reel vs your typical reel" curve, sources (Reels tab / Explore), audience (followers %, age, country, gender). Write the numbers into that post's row in `tracking/results.csv`, with the extras in `notes`. **If a reel was posted that isn't in the CSV, add a row for it.**
- **Dashboard → Content (30 days):** refresh `views` and the viewers/likes in `notes` for every older post shown (write "(DD Mon)" for the date you checked).
- **Dashboard → Home / Performance (7 days):** add one row to `tracking/account.csv` (views, viewers, follower and non-follower views, followers, profile visits, bio link taps, reel and story views and interactions).
- **Stories** show a dashed circle in the Content list. Don't add them to `results.csv`.

## Step 1: Check the numbers first
1. Read `tracking/results.csv` (columns: `date,type,topic,hook,views,saves,shares,comments,new_followers,notes`).
2. Find **yesterday's** rows (yesterday = today − 1 day).
3. **If a row for yesterday has an empty `views`, `saves`, `shares` or `new_followers`: stop.** Ask Kate for the missing numbers in one short message, for example:
   > What are yesterday's numbers for "[topic]"? Views / saves / shares / comments / new followers
   Wait for her answer, write the numbers into the CSV, and only then continue.
4. If there was no post yesterday (a Stories-only or rest day), say so in one line and use the last 7 days instead.
5. A post on a day planned as Stories-only still counts: review it as yesterday's post.

## Step 2: Analyse (yesterday + the last 7 days for context)
For each post with numbers:
- **Save rate** = saves ÷ views · **Share rate** = shares ÷ views · **Follow rate** = new_followers ÷ views
- **Score** = (saves + 2 × shares + comments + 3 × new_followers) ÷ views × 100

Compare yesterday's post with the 7-day average and the best post of the week. Then explain in simple words:
- ✅ **What worked:** which number was strong, and why (the hook, its formula number from `hooks/hooks-library.md`, the topic, the format, the posting time)
- ❌ **What didn't:** which number was weak, and the most likely reason
- 👉 **Lesson for today:** one sentence

Also use **skip rate** and **avg watch time as a % of the video length** when they're in `notes`. With so few saves and shares, these are the best signs of a good hook.
**The ~120 wall:** most reels stop at about 120–135 views (Instagram's first test batch). Above ~150 means Instagram pushed it further, so find out why. If the "this reel" curve goes flat after the first hour, the reel didn't pass the test.

The account is small, so compare posts with each other, never with big accounts. With fewer than 3 posts, say the data is still thin.

## Step 3: Improve today's content
1. Find today's plan in `content-plan/week-YYYY-MM-DD.md` (the file whose Monday is in the current week). Also look for today's Flow prompts in `content-plan/prompts/` if they exist.
2. Improve it based on the lesson:
   - **Hook:** if the hook formula or style performed badly, rewrite it with a better formula from `hooks/hooks-library.md`. Aim for **8 words or fewer on screen** (12 maximum), and add the formula number. Follow "What Kate's data says" in `hooks/hooks-library.md` (big, bold text, correct capitals, a time word, a named place).
   - **Topic or format:** move towards what performed best (e.g. more hidden story, a time stamp in the hook, more natural sound), but keep the post type that's planned for today.
   - **Caption:** keep the search keywords, and strengthen the first line.
   - **A reason to save or share:** an address end card, a "save this for your next walk" line, or a "send it to someone who…" line. Most reels so far have 0 saves and 0 shares.
   - **Google Flow prompts** (if today is a reel made with Flow): **first read `references/flow-prompt-lessons.md` and apply every point in "Rules that work".** Then update the prompts only where needed.
   - When Kate shares how her Flow clips turned out (what went wrong, what fixed it), add an entry to the "Log" in `references/flow-prompt-lessons.md`. If the fix is a new lesson, add it to "Rules that work" too.
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
