# Hero — Design Exploration

Three concepts for the profile hero. Each must introduce the **engineering system**, not the person.

---

## Concept A — Pure Specification Sheet

**Visual:** White field, no grid. Apple product-spec layout. Label-value pairs only.

```
┌─────────────────────────────────────────┐
│  PRODUCT SPECIFICATION                  │
│                                         │
│  System        Harshit Singh Eng. Sys   │
│  Operator      Harshit Singh            │
│  Class         AI · Full Stack · OSS    │
│  Focus         AI products, real-world  │
│  Domains       Healthcare · Education…  │
│                                         │
│  ┌──────┐ ┌──────┐ ┌──────┐            │
│  │  9   │ │ 20+  │ │ AI   │            │
│  │ wins │ │ proj │ │ OSS  │            │
│  └──────┘ └──────┘ └──────┘            │
│                                         │
│  github · linkedin · devpost            │
└─────────────────────────────────────────┘
```

**Strengths:** Maximum clarity. Extremely readable. Fast to implement.

**Weaknesses:** Generic. Could be any premium README. Lacks distinctive visual identity. Doesn't leverage blueprint inspiration.

**Score:** 7/10

---

## Concept B — Architectural Blueprint Plate

**Visual:** Full blueprint grid, dimension lines, sheet number, heavy registration marks. Monospace throughout.

```
┌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┐
╎ ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ ╎
╎ ░  BLUEPRINT: HS-ENG-SYS-001          ░ ╎
╎ ░  SCALE: 1:1  SHEET: 01              ░ ╎
╎ ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ ╎
╎                                         ╎
╎  OPERATOR ─── Harshit Singh             ╎
╎  DOMAINS ─── Healthcare · AI · …        ╎
╎                                         ╎
└╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┘
```

**Strengths:** Highly distinctive. Strong "builder" signal. Memorable.

**Weaknesses:** Risk of feeling gimmicky if over-drawn. Hard to fit metrics + links without crowding. Dark mode grid visibility concerns.

**Score:** 8/10

---

## Concept C — Blueprint Spec Plate (Hybrid) ✓ SELECTED

**Visual:** Blueprint grid as background texture + Apple-style spec field hierarchy + patent-style title block + compact metric cells.

Combines:
- Grid + registration marks from Concept B
- Label-value hierarchy from Concept A
- Title block / document ID from patent filings

**Hierarchy (as implemented):**
1. System title — `ENGINEERING SYSTEM SPECIFICATION`
2. Name — `Harshit Singh` (display scale)
3. Domains — `Healthcare · Education · Accessibility · …`
4. Verified achievements — `9` wins · `20+` projects · disciplines
5. Links — endpoints as mono links

**Strengths:**
- Original — not a trope
- Scales to footer mirror (`assets/footer-spec.svg`)
- Blueprint identity without overwhelming content
- Metric cells feel like engineering instrumentation
- Title block creates document authenticity

**Weaknesses:**
- SVG complexity (~4KB) — within budget
- Requires testing in GitHub dark mode

**Score:** 9.5/10

---

## Design Director Decision

**Selected: Concept C — Blueprint Spec Plate**

**Reasoning:** Concept A is clean but forgettable. Concept B is memorable but risks decoration-over-information. Concept C earns its visual elements — every mark communicates document structure. It directly satisfies the brief: blueprint + spec sheet + Apple product spec.

**Implementation:** `assets/hero-spec.svg`

---

## Critical Evaluation

| Criterion | Pass? | Notes |
|-----------|-------|-------|
| Introduces system, not person | ✓ | System title leads |
| Builder, not influencer | ✓ | Metrics are output-based |
| No banned tropes | ✓ | No terminal, capsule, typing |
| GitHub compatible | ✓ | Static SVG, no scripts |
| Footer mirrorable | ✓ | Same frame language |
| Dark mode safe | ⚠ | Light surface — monitor; grid uses muted strokes |
| Mobile width | ✓ | 800px scales down; text remains readable |

**Verdict:** Approved for README integration.
