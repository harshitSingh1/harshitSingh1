# Hackathon Section — Redesign

Source: [Devpost portfolio](https://devpost.com/sharshitsingh007) — all projects preserved, presentation redesigned.

---

## Design Goal

Transform hackathon entries from widget cards into **compact engineering specification rows** — each project is a line item in a build catalog.

---

## Card Schema

Each project = one HTML `<table>` block. No paragraphs. Max 4 rows.

| Row | Fields |
|-----|--------|
| **Header** | `POSITION` · `PROJECT NAME` · `PARTICIPANTS` |
| **Description** | Single line, ≤ 120 characters |
| **Technology** | Inline mono stack, ` · ` separated |
| **Links** | `repo` · `live` · `demo` · `devpost` — text only, omit if unavailable |

### Visual treatment

- `width="100%"` table, `cellpadding="8"`
- Label column: `` `mono` `` at 90px width
- Border: `1px solid` via table attribute where supported, or markdown `---` separator between cards
- Winners listed first, then remaining projects
- Blank line between each card

---

## Winner Projects (9 International Hackathon Wins)

### 01 — First30.ai
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Voice-guided emergency assistance for the critical first 30 minutes before professional help arrives |
| Technology | `React` · `TypeScript` · `Supabase` · `ElevenLabs` · `Edge Functions` |
| Links | [repo](https://github.com/harshitSingh1/First-30) · [live](https://preview--first-30-aid.lovable.app/) · [devpost](https://devpost.com/software/first30-ai) |

### 02 — CodeMentor
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Progressive AI hints for competitive programming — guides without spoiling across 4 platforms |
| Technology | `Chrome MV3` · `JavaScript` · `OpenAI` · `Gemini` · `Claude` |
| Links | [repo](https://github.com/harshitSingh1/CodeMentor) · [devpost](https://devpost.com/software/codementor-0ix5lu) |

### 03 — Lumen
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Chrome extension transforming any webpage into dyslexia-friendly, low-vision, and ADHD-friendly content |
| Technology | `Chrome AI` · `Gemini Nano` · `JavaScript` · `MV3` |
| Links | [devpost](https://devpost.com/software/lumen) |

### 04 — Sestara
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | AI curricula with mastery tracking and 20+ languages — democratizing private tutoring infrastructure |
| Technology | `AI` · `NLP` · `Education Platform` |
| Links | [devpost](https://devpost.com/software/sestara) |

### 05 — CivicLens
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Report civic issues via photo and map pin; authorities broadcast hazard alerts to residents |
| Technology | `Full Stack` · `Maps` · `Civic Tech` |
| Links | [devpost](https://devpost.com/software/civiclens) |

### 06 — BreakBuddy
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | 3 members |
| Description | Chrome extension turning homepage into a hub for productive breaks — blogs, games, AI chat, to-do |
| Technology | `JavaScript` · `HTML` · `CSS` · `Chrome Extension` · `NLP` |
| Links | [repo](https://github.com/harshitSingh1/BreakBuddy) · [devpost](https://devpost.com/software/breakbuddy-tvk1xd) |

### 07 — CareerArk
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Free AI career platform — recommendations, assessments, roadmaps, and resume reviews for all stages |
| Technology | `AI` · `Full Stack` · `Career Tech` |
| Links | [devpost](https://devpost.com/software/career-ark) |

### 08 — Healthcare AI
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | ML models predicting likelihood of Diabetes, Heart Disease, and Parkinson's Disease |
| Technology | `Python` · `Machine Learning` · `Scikit-learn` |
| Links | [devpost](https://devpost.com/software/healthcare) |

### 09 — HealthMentor AI
| Field | Value |
|-------|-------|
| Position | Winner |
| Participants | Team |
| Description | Vector-search medical record advisor delivering expert-level clinical insights for underserved regions |
| Technology | `Next.js` · `FastAPI` · `MongoDB Atlas` · `Vertex AI` · `Docker` |
| Links | [devpost](https://devpost.com/software/healthmentor-ai) |

---

## Additional Hackathon Projects

### 10 — SpendSense
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Real-time visibility into AI and cloud spend — per tenant, per feature, per minute |
| Technology | `Cloud` · `FinOps` · `AI Cost Tracking` |
| Links | [devpost](https://devpost.com/software/spendsense) |

### 11 — Green Cloud Auto-Resolver
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | GitLab agent using Vertex AI to autonomously fix UI bugs and enforce green software standards |
| Technology | `Vertex AI` · `GitLab` · `Green Software` |
| Links | [devpost](https://devpost.com/software/green-cloud-auto-resolver) |

### 12 — CareForAll
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | AI health and mental wellness support with daily check-ins, pattern alerts, and expert-verified guidance |
| Technology | `AI` · `Healthcare` · `Mental Wellness` |
| Links | [devpost](https://devpost.com/software/careforall) |

### 13 — NagrikAI
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | 2 members |
| Description | Agentic AI copilot helping Indian citizens access government schemes in their own language |
| Technology | `Agentic AI` · `NLP` · `Civic Tech` · `Multilingual` |
| Links | [devpost](https://devpost.com/software/nagrikai) |

### 14 — GenConnect
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | 2 members |
| Description | Connects teenagers with senior citizens for mentorship, skill-sharing, and companionship |
| Technology | `Full Stack` · `Social Platform` |
| Links | [devpost](https://devpost.com/software/genconnect) |

### 15 — FarmingNow
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | 2 members |
| Description | NASA-data-driven agriculture — crop recommendations, soil analysis, irrigation, weather, pest control |
| Technology | `NASA APIs` · `AI` · `Agriculture` |
| Links | [devpost](https://devpost.com/software/farmingnow) |

### 16 — Daily Detective
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Interactive riddles on Reddit via full-stack Devvit app with web views, Redis, and auto-scheduling |
| Technology | `Devvit` · `Redis` · `Reddit API` · `Full Stack` |
| Links | [devpost](https://devpost.com/software/daily-detective) |

### 17 — Kiroscope
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Real-time codebase architecture visualization with AI-powered structural insights |
| Technology | `AI` · `Developer Tools` · `Visualization` |
| Links | [devpost](https://devpost.com/software/kiroscope) |

### 18 — Baseline Upgrade CLI
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Scans codebases for Baseline-approved modernization alternatives with global progress tracking |
| Technology | `CLI` · `JavaScript` · `Developer Tools` |
| Links | [devpost](https://devpost.com/software/baseline-upgrade-cli) |

### 19 — GetRichify
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | AI startup idea generator transforming ordinary concepts into exaggerated business opportunities |
| Technology | `AI` · `GenAI` |
| Links | [devpost](https://devpost.com/software/getrichify) |

### 20 — Auto-Assist Mobility Chair
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Smart semi-automated wheelchair with shock-absorbing suspension, ergonomics, and CAD-optimized stability |
| Technology | `CAD` · `Hardware` · `Accessibility` |
| Links | [devpost](https://devpost.com/software/auto-assist-mobility-chair) |

### 21 — DeepSea Portfolio
| Field | Value |
|-------|-------|
| Position | Built |
| Participants | Team |
| Description | Immersive marine-themed developer portfolio with interactive sea creatures and functional terminal |
| Technology | `Frontend` · `Animation` · `Interactive` |
| Links | [devpost](https://devpost.com/software/deepsea-portfolio) |

---

## Design Director Evaluation

| Criterion | Pass? |
|-----------|-------|
| All projects preserved | ✓ 21 entries from Devpost |
| Compact — no paragraphs | ✓ |
| Consistent schema | ✓ |
| Position + participants visible | ✓ |
| Tech + links on every card | ✓ |
| Winners prioritized | ✓ |
| No banned elements | ✓ |

**Verdict:** Approved for README Section 01.
