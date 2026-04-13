# Leveling Up Your GitHub Profile

## 1. Create the profile README (the big unlock)

GitHub shows a `README.md` from a repo named **exactly your username** on your profile. Most people don't know this exists.

```bash
# Create repo named "eldarski" (matching your handle)
# Add README.md — it renders above the contribution graph
```

## 2. Better-than-default stat widgets

### **github-readme-stats** (most popular)

```markdown
![Stats](https://github-readme-stats.vercel.app/api?username=eldarski&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=eldarski&layout=compact&theme=tokyonight)
```

Key flags: `include_all_commits=true` and `count_private=true` — without these your stats only count this year's public commits (which is why your graph looks "lame" despite 564 commits).

### **github-readme-streak-stats**

```markdown
![Streak](https://streak-stats.demolab.com?user=eldarski&theme=tokyonight)
```

Shows current streak + longest streak — way more motivating than the default squares.

### **github-profile-trophy**

```markdown
![Trophies](https://github-profile-trophy.vercel.app/?username=eldarski&theme=tokyonight&no-frame=true&row=1)
```

### **wakatime** (coding time, not just commits)

If you install the WakaTime extension in your editor:

```markdown
![Wakatime](https://github-readme-stats.vercel.app/api/wakatime?username=eldarski&theme=tokyonight)
```

This shows **hours coded per language per week** — far more honest than commit counts.

## 3. Fix the contribution graph itself

The default graph only shows:

- Commits to `master`/`main` of public repos
- Commits where your commit email matches a verified GitHub email

Your graph is likely undercounting because:

1. **Zingyy is private** → Settings → Profile → check **"Include private contributions on my profile"**
2. **Commits on feature branches don't count unless merged** — you squash-merge PRs, so check that the squash commits are attributed to you (they should be).
3. **Email mismatch** — verify `117188568+eldarski@users.noreply.github.com` is in your GitHub verified emails (Settings → Emails).

## 4. Activity graph alternatives

### **github-readme-activity-graph** (line chart instead of squares)

```markdown
![Activity](https://github-readme-activity-graph.vercel.app/graph?username=eldarski&theme=tokyo-night&hide_border=true)
```

### **Snake eating contributions** (GitHub Action that animates your graph)

Add `.github/workflows/snake.yml` using `Platane/snk` — generates an SVG where a snake eats your contribution squares. Sounds gimmicky, it's actually great.

## 5. Pinned repos with images

Pin up to 6 repos. For private work you can't show, create **pinned gists** with summaries, or use:

```markdown
![Pin](https://github-readme-stats.vercel.app/api/pin/?username=eldarski&repo=zingyy&theme=tokyonight)
```

## 6. Dynamic content (GitHub Actions)

Auto-update your README with a workflow:

- **Latest blog posts** — `gautamkrishnar/blog-post-workflow`
- **Recent activity** — `jamesgeorge007/github-activity-readme` (last 5 PRs/issues/commits)
- **Now playing on Spotify** — `novatorem/novatorem`

## 7. Honest advice

The "lame graph" problem is usually about **what it counts, not how it looks**:

- Your 564 commits in zingyy **probably aren't showing** if the repo is private and the setting is off.
- Fix that one toggle → your graph goes from sparse to fully green overnight.
- After that, `github-readme-stats` with `include_all_commits=true` will reflect your real output.

## Minimal starter template

```markdown
### Hi, I'm Eldar 👋

Building [zingyy](https://zingyy.com) — AI interview platform.

![Stats](https://github-readme-stats.vercel.app/api?username=eldarski&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true)
![Streak](https://streak-stats.demolab.com?user=eldarski&theme=tokyonight)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=eldarski&layout=compact&theme=tokyonight)
```

Start with that + flip the private-contributions toggle. That alone will make your profile look ~3× more active.
