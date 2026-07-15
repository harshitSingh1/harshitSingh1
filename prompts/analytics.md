# GitHub Analytics — Redesign

Minimal analytics. Earned credentials only.

---

## Design Goal

Present GitHub activity data as **instrument readings** within the engineering document — not as a widget dashboard.

---

## Allowed (only these three)

1. **GitHub Stats** — commits, PRs, issues, contributions
2. **GitHub Streak** — current streak, longest streak, contributions
3. **Contribution Graph** — annual contribution snake/grid

## Removed

- Top languages chart
- Random quotes
- Trophy collections
- Visitor counters
- Productive time / WakaTime
- GitHub profile views

---

## Layout

```
<sub>SECTION 03</sub>
#### GitHub Analytics

<table>
  <tr>
    <td>GitHub Stats card</td>
    <td>GitHub Streak card</td>
  </tr>
</table>

Contribution graph (full width, centered)
```

### Framing rules

- Wrap stats + streak in a single HTML table, 2 columns
- No extra borders around images — let the cards speak
- Contribution graph below, centered
- Username: `aitch-cmd`
- Theme: `default` (respects user GitHub theme)

---

## Image URLs

### Stats
```
https://github-readme-stats.vercel.app/api?username=aitch-cmd&show_icons=false&hide_border=true&title_color=1a1a1a&text_color=525252&icon_color=3b6fa8&bg_color=ffffff&count_private=false
```

### Streak
```
https://github-readme-streak-stats.herokuapp.com/?user=aitch-cmd&hide_border=true&background=ffffff&stroke=e5e5e5&ring=3b6fa8&fire=3b6fa8&currStreakLabel=1a1a1a&sideLabels=525252&currStreakNum=1a1a1a&sideNums=525252&dates=525252
```

### Contribution Graph
```
https://raw.githubusercontent.com/aitch-cmd/harshitneverdebugs/output/github-contribution-grid-snake.svg
```

> Note: Contribution snake requires `.github/workflows/snake.yml` generating to `output/` branch or `dist/` path. Workflow configured in this repo.

---

## Design Director Evaluation

| Criterion | Pass? |
|-----------|-------|
| Only 3 analytics elements | ✓ |
| No banned widgets | ✓ |
| Colors match design system | ✓ Palette tokens in URL params |
| Framed, not floating | ✓ Table wrapper |
| Builder credential, not vanity | ✓ Stats + streak + graph = work proof |

**Verdict:** Approved for README Section 03.
