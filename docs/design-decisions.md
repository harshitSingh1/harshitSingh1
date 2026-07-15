# Design Decisions Log

Chronological record of choices made during the profile redesign.

---

## DD-001 — System-first hero

**Decision:** Hero introduces "Harshit Singh Engineering System" before the person.

**Rationale:** User requirement — communicate Builder, not Influencer. Spec sheets name the system first, operator second.

**Alternatives rejected:** Name-first greeting, avatar-centered layout, role tagline hero.

---

## DD-002 — Blueprint blue accent

**Decision:** Accent color `#3b6fa8` (blueprint blue) over terracotta.

**Rationale:** Hero concept merges architectural blueprint + engineering spec. Blue carries domain meaning without neon association.

**Alternatives rejected:** Rainbow accents, green hacker tones, purple gradients.

---

## DD-003 — Hybrid hero concept selected

**Decision:** Concept C — Blueprint Spec Plate (see `prompts/hero.md`).

**Rationale:** Combines grid identity of blueprints with field hierarchy of Apple specs. Most original. Most scalable to footer mirror.

**Alternatives rejected:** Pure ASCII spec (too plain), full patent filing layout (too dense).

---

## DD-004 — Compact table cards for hackathons

**Decision:** One HTML table per project, max 4 rows, no paragraphs.

**Rationale:** User requirement for compact, consistent, beautiful cards. Tables render reliably on GitHub.

**Alternatives rejected:** Blockquote cards, `<details>` per project, two-column grid.

---

## DD-005 — Capability grouping over layer stack

**Decision:** Group technologies by engineering capability, not Languages/Frontend/Backend.

**Rationale:** User requirement. Reflects how a senior engineer describes themselves — by what they can build, not syntax they know.

---

## DD-006 — Analytics minimal set

**Decision:** Keep only GitHub Stats, Streak, Contribution Graph.

**Rationale:** User requirement. These three are earned credentials. Everything else is widget noise.

**Removed:** Top languages chart, trophies, quotes, visitor counter, productive time.

---

## DD-007 — Footer mirrors hero

**Decision:** Footer uses same SVG frame structure with closure fields: document status, revision, endpoints.

**Rationale:** Bookend the document. Creates memorable symmetry without generic sign-off.

---

## DD-008 — No animation

**Decision:** Zero motion across entire profile.

**Rationale:** Design system principle. GitHub README animation ages poorly. Static = premium.

---

## DD-009 — All 20 Devpost projects included

**Decision:** Include every project from Devpost portfolio. Winners listed first.

**Rationale:** User said reuse all existing information, do not remove achievements. Devpost is authoritative source for hackathon data.

---

## DD-010 — Username `aitch-cmd`

**Decision:** GitHub links and analytics reference `aitch-cmd`.

**Rationale:** Confirmed via public GitHub API and LinkedIn cross-reference. Profile repo: `harshitneverdebugs`.

---

## Open items

- [ ] User review of hero SVG in dark mode
- [ ] Confirm LinkedIn URL preference (two profiles found publicly)
- [ ] Validate all live/demo links still active
