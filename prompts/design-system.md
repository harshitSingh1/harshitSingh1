# Design System — Harshit Singh GitHub Profile

> Engineering specification document. Not a portfolio site. Not a dashboard.

---

## Visual Identity

**Personality:** Calm · Minimal · Premium · Engineering-first · Builder-focused · Editorial · Modern · Confident · Spacious

**Essence:** A single cohesive engineering document — the kind you'd find attached to a patent filing or an RFC — typeset with care, not decorated with widgets.

### Principles

| Principle | Application |
|-----------|-------------|
| **Typography is the UI** | Hierarchy, weight, and spacing carry the design. Borders are secondary. |
| **Information density** | Compact cards. One line per fact. No paragraphs in showcase sections. |
| **Blueprint honesty** | Grid lines, registration marks, and spec labels communicate structure — not decoration. |
| **Builder over influencer** | Lead with systems built, domains mastered, outcomes verified. |
| **Monochrome discipline** | One accent color. No rainbow stacks. No emoji headers. |

### Anti-patterns (never use)

Capsule Render · Typing SVG · GIFs · Terminal/Mac window chrome · Command palette · Badge walls · Trophy widgets · Visitor counters · Glassmorphism · Neon · Cyberpunk · Matrix effects · Emoji spam

---

## Typography System

GitHub renders system fonts. Design within that constraint.

### Scale

| Role | Markdown | Usage |
|------|----------|-------|
| **System title** | SVG text / `###` | Hero system name only |
| **Display** | `**bold**` inline in hero | Operator name |
| **Section** | `####` | Five main sections |
| **Card title** | `#####` or bold table cell | Project / capability name |
| **Body** | Default | One-line descriptions only |
| **Label** | `` `mono` `` | Field keys: `POSITION`, `STACK`, `STATUS` |
| **Caption** | `<sub>` | Revision notes, footnotes |
| **Metric** | `` `mono` `` bold | `9`, `20+`, streak counts |

### Hierarchy rules

1. Hero introduces the **engineering system**, not the person.
2. Name appears as **operator / author** field in spec layout — second in hierarchy.
3. Sections use numbered prefixes: `01 —`, `02 —`, etc.
4. Mono is functional: metadata, labels, tech stacks, revision IDs.
5. Left-align everything except hero title block (centered within SVG frame).

### Whitespace

- Blank line before and after every section
- Blank line between every card row
- Section gaps feel like page breaks in a spec document

---

## Color Palette

Four colors. No gradients.

| Token | Hex | Role |
|-------|-----|------|
| **Primary** | `#1a1a1a` | Headings, primary strokes (SVG) |
| **Secondary** | `#525252` | Body, descriptions |
| **Accent** | `#3b6fa8` | Blueprint blue — links in SVG, active markers, registration ticks |
| **Muted** | `#a3a3a3` | Grid lines, dividers, captions |
| **Border** | `#e5e5e5` | Card edges, table rules |
| **Surface** | `#fafafa` | SVG card backgrounds (light-mode safe) |

Markdown text uses GitHub default colors for dark/light mode compatibility. Custom color lives in SVG assets only.

---

## Component Library

### Hero — Engineering Specification Plate

Blueprint grid frame + Apple-style spec fields. Introduces the **system**, not the person.

Fields: System ID · Operator · Domains · Verified metrics · Links

### Section Header

```
<sub>SECTION 01</sub>
#### Award Winning Products
```

Followed by `assets/divider.svg` or `---`

### Hackathon Card (compact)

Single HTML table row or 2-row mini-table per project:

| Field | Format |
|-------|--------|
| Position | `Winner` · `Finalist` · mono |
| Name | Linked project title |
| Participants | `solo` · `N members` |
| Description | Max 1 line, 120 chars |
| Technology | Inline mono, ` · ` separated |
| Links | `repo` · `live` · `demo` as text links |

### Shipped Product Card

Same density as hackathon card. Fields: Problem · Interest · Tech · Links

### Capability Block

Grouped by engineering domain — not Languages/Frontend/Backend.

```
##### AI Engineering
`Python` · `LangGraph` · `RAG` · `FastAPI` · `Ollama`
```

### Analytics Frame

Neutral bordered container. Stats left, streak center, graph full-width below. No extra widgets.

### Footer — Spec Closure Plate

Mirrors hero SVG structure. Revision block, document status, contact endpoints. No "thanks for visiting."

### Divider

`assets/divider.svg` — 1px line + center registration mark. Used between all major sections.

---

## Spacing Rules

Base unit: 4px

| Token | px | Usage |
|-------|-----|-------|
| xs | 4 | Label gaps |
| sm | 8 | Inline separators |
| md | 16 | Card padding |
| lg | 24 | Title → content |
| xl | 32 | Card → card |
| 2xl | 48 | Section → section |

Cards stack vertically. Max 2 columns in tables. No horizontal scroll at 320px.

---

## Icon Style

| Allowed | Usage |
|---------|-------|
| Custom SVG | Hero frame, divider, registration marks |
| Unicode | `→` `·` `—` `│` for inline separators |
| Text links | `repo` `live` `demo` — never icon-only |

| Forbidden | Reason |
|-----------|--------|
| Emoji headers | Breaks premium tone |
| Skill icon grids | Widget wall aesthetic |
| Social logo rows | Influencer pattern |
| Shields (except none planned) | Visual noise |

---

## Animation

**None.** Static document. Stillness signals confidence.

---

## GitHub Constraints

| Allowed | Forbidden |
|---------|-----------|
| Markdown, HTML, SVG, tables | JavaScript |
| Inline HTML attributes | External CSS files |
| Shields (minimal) | iframes |
| Images (avatar, graphs) | foreignObject in SVG |
| `<details>` for overflow | SMIL animation |

### Layout strategy

1. SVG for hero + footer frames (visual identity)
2. Markdown + HTML tables for cards (content)
3. Images for GitHub analytics only
4. All assets referenced via relative paths: `assets/...`

---

## Section Map (README structure)

```
┌─ HERO ─────────────────────────────────────┐
│  ENGINEERING SYSTEM SPECIFICATION           │
│  Operator · Domains · Metrics · Links       │
└─────────────────────────────────────────────┘
         │
    ─── divider ───
         │
┌─ 01 AWARD WINNING PRODUCTS ────────────────┐
│  Hackathon cards (all winners + projects)   │
│  Shipped systems (featured repos)           │
└─────────────────────────────────────────────┘
         │
┌─ 02 ENGINEERING CAPABILITIES ──────────────┐
│  AI Engineering · Full Stack · Cloud · etc  │
└─────────────────────────────────────────────┘
         │
┌─ 03 GITHUB ANALYTICS ──────────────────────┐
│  Stats · Streak · Contribution graph        │
└─────────────────────────────────────────────┘
         │
┌─ FOOTER (mirrors hero) ────────────────────┐
│  Document closure · revision · endpoints    │
└─────────────────────────────────────────────┘
```

---

## Design Director Evaluation

**Strengths:** Typography-led, scalable to full docs site, avoids every overused README trope.

**Risks to monitor:**
- Table-heavy layouts can feel dense — mitigate with consistent row height and generous `md` padding
- Blueprint SVG must stay under 5KB and render in dark mode
- Analytics widgets are external images — frame them so they don't break visual unity

**Verdict:** Approved as foundation. Proceed to hero concepts.
