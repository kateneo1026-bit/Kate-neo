---
name: weekly-review
description: Read tracking/results.csv for the "Kate" Instagram account, say what worked, what to repeat and what to stop, then propose next week's plan. Use when Kate asks for a review, "/weekly-review", or "what worked this week".
---

# Weekly review for "Kate"

## 1. Read the data
- Open `tracking/results.csv`. Columns: `date,type,topic,hook,views,saves,shares,comments,new_followers,notes`.
- Ignore rows where `views` is empty: they're planned posts that haven't been posted yet or have no numbers yet.
- Focus on the last 7 days, and compare them with older rows if there are any.
- Also read `tracking/account.csv` (7-day account totals: followers, profile visits, bio link taps).
- If Kate sends Instagram screenshots, first follow "Step 0" in `.claude/skills/daily-review/SKILL.md` to put the numbers into the CSVs.

## 2. Calculate (for each post)
- **Save rate** = saves ÷ views
- **Share rate** = shares ÷ views
- **Follow rate** = new_followers ÷ views
- **Score** = (saves + 2 × shares + comments + 3 × new_followers) ÷ views × 100

When `notes` has them, also compare **skip rate**, **avg watch time as a % of length** and **views vs the ~120 wall** (most reels stop at 120–135 views; above ~150 means Instagram pushed it). These are the main signals while saves and shares are near zero.

Shares and new followers count most: the goal is to build a community. The account is small, so judge posts **against each other**, not against big-account benchmarks. With fewer than 5 posts, say the data is too thin and give direction rather than firm conclusions.

## 3. Write the review
Save it to `reviews/review-YYYY-MM-DD.md` (today's date) with these sections:

1. **Numbers this week:** a small table of posts sorted by score (date, type, topic, views, score)
2. **What worked:** the top 1–2 posts and *why* (topic, hook formula, format, day). Look at the `notes` column too.
3. **Repeat:** 3 concrete actions (e.g. "Another hidden-story reel about an old London shopfront, using hook formula 7")
4. **Stop:** 1–3 things to drop or change (low score, weak hook, bad day or time)
5. **Test next week:** 1 new idea to try

Also update the "What Kate's data says" list in `hooks/hooks-library.md` if the week taught something new about hooks.

Be honest and short. Use plain English, with no jargon.

## 4. Next week
Then follow `.claude/skills/weekly-plan/SKILL.md` to create next week's plan, using the "Repeat", "Stop" and "Test" lists above.

## 5. In chat
Give Kate a short summary: best post, 3 repeats, the things to stop, and the link to the new plan file.
