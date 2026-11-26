---
name: daily-review
description: Daily check-in for the "Kate" Instagram account. Reads yesterday's numbers in tracking/results.csv, explains what worked and why, improves today's planned post (hook, topic, format, Google Flow prompts), saves an improved copy and ends with a French checklist for today. Use when Kate types "/daily-review" or asks "what should I post today".
---

# Daily review for "Kate"

Kate reads this on her phone. Keep the chat answer **short**: short lines, few tables, no long paragraphs.

## Step 1: Check the numbers first
1. Read `tracking/results.csv` (columns: `date,type,topic,hook,views,saves,shares,reposts,comments,new_followers,avg_watch_s,skip_rate,notes`).
   If Kate sends Instagram insight screenshots, read every number from them (views, viewers, likes, saves, shares, reposts, comments, follows, average watch, skip rate, the retention curve, sources, followers vs non-followers, age, gender, country) and write them into the CSV (extra details go in `notes`).
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

**The ~120 wall check (always do this):** Instagram shows each reel to a test group of ~120 non-followers in the first 1–2 hours and only pushes further if people **send, save or follow**. If views stopped at ~120 and sends + saves = 0, say the reel *stalled at the test group*, and look first at the reel's "send reason", not the visuals. Use `avg_watch_s` and `skip_rate` to judge the hook (skip rate falling = hook improving). Ignore the 1 repost almost every reel gets: it's probably the same person each time. Background: `reviews/diagnosis-2026-11-24.md`.

**The country check (always do this, since 26 Nov):** the target is **UK + Ireland + Europe**. Note each reel's top 3 countries in `notes`. If under 70% of viewers are UK/Ireland/Europe, say the topic was *too global* (the bees reel went 54% India; the next reel stalled at 46 views because the test group moved). High views with a like rate under 1% and 0 sends = empty global reach, not success. Every new topic must pass the **go-there test**: *could someone in the UK go there this month?* and carry local signals (UK location tag, Tube station / "free" / Eurostar on screen, UK hashtags, a save-or-send-for-a-plan CTA). Remind Kate: VPN off for Instagram, Meta AI translations off. Background: `reviews/diagnosis-2026-11-26.md`.

If Kate says something feels wrong, also check: the share of views from followers, Story viewers vs follower count, profile taps, the bio and name field, the audience (age, gender, country) vs the plan's target, and anything odd in the screenshots (typos in stickers, VPN, posting gaps).

## Step 3: Improve today's content
1. Find today's plan in `content-plan/week-YYYY-MM-DD.md` (the file whose Monday is in the current week). Also look for today's Flow prompts in `content-plan/prompts/` if they exist.
2. Improve it based on the lesson:
   - **Hook:** if the hook formula or style performed badly, rewrite it with a better formula from `hooks/hooks-library.md`. Keep it to 12 words or fewer, and add the formula number.
   - **Topic or format:** move towards what performed best (e.g. more hidden story, a time stamp in the hook, more natural sound), but keep the post type that's planned for today, unless Kate asks for a change.
   - **Send test:** every hidden story must pass *"Would someone send this to a friend with 'look at this'?"*. Best so far: a famous place + an impossible origin or a surprising survivor (the warships reel, 431 views). End the reel and caption with **one** send CTA ("Send this to someone who loves [city]").
   - **Hook text:** on a calm, darker area (top third), never over a bright light.
   - **Caption:** keep the search keywords, and strengthen the first line.
   - **Google Flow prompts** (if today is a reel made with Flow): **first read `references/flow-prompt-lessons.md` and apply every point in "Rules that work".** Then update the prompts only where needed.
   - When Kate shares how her Flow clips turned out (what went wrong, what fixed it), add an entry to the "Log" in `references/flow-prompt-lessons.md`. If the fix is a new lesson, add it to "Rules that work" too.
3. If today is a Stories-only day, improve the 3 Stories instead.
4. **Stories always follow `content-plan/stories-rule.md`:** format (image or video), a ready-to-use prompt (Flow for video, Gemini for image), the text on screen, and a spare prompt for every video.

## Step 4: Save (never overwrite the original)
- Save the improved version to `content-plan/daily/YYYY-MM-DD-improved.md` (today's date).
- At the top, put a small table with columns **Before → After** (hook, topic, format) and a one-line reason.
- Then the full improved post: hook, script, caption, hashtags, CTA, Flow prompts (if any), and today's 3 Stories.
- Leave the week plan file unchanged so Kate can compare the two.
- If the hook, topic or type changed, update today's row in `tracking/results.csv` (`type`, `topic`, `hook` only). If a planned post moves to another day, move its row too.

## Step 5: Reply in chat (short, for a phone)
1. Yesterday in 3 lines: ✅ worked · ❌ didn't · 👉 lesson
2. Today's change in 1–2 lines (new hook) + the file path
3. Finish with this checklist **in French**:

```
✅ Aujourd'hui
- Publier : [type + sujet] à [heure, heure UK]
- 3 stories : matin [..] · midi [..] · soir [..]
- Après la publication :
  - Envoyer le reel à 3–5 vrais amis et leur demander un commentaire dans la 1re heure
  - Répondre à tous les commentaires dans la 1re heure
  - Commenter 5 comptes de ta niche (cosy / slow living / hidden places UK et Europe), avec de vrais commentaires de plus de 5 mots
  - Demain matin : envoyer les captures des statistiques (vues, partages, enregistrements, abonnés, durée moyenne, taux de skip)
```

Post times (UK): weekdays at 12:30 or 19:30, weekends at 10:00, unless the data shows a better time.

Before the checklist, remind Kate in one line of any open profile fix (bio, name field, pinned reels) and to turn the VPN off when she posts.
