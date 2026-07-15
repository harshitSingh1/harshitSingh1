# Featured Projects — Shipped Systems

Non-hackathon repositories presented as **shipped products**, not repo cards.

Source: [github.com/aitch-cmd](https://github.com/aitch-cmd) public repositories.

---

## Design Goal

Each entry answers three questions in compact form:
1. **What problem did it solve?**
2. **Why is it interesting?**
3. **Links + Tech**

Same card schema as hackathons. One table per project.

---

## Card Schema

| Row | Fields |
|-----|--------|
| **Header** | `STATUS` · `PRODUCT NAME` |
| **Problem** | Single line — the pain point |
| **Interest** | Single line — the technical or product insight |
| **Technology** | Inline mono stack |
| **Links** | `repo` · `live` · `docs` |

---

## Shipped Systems

### AegisOps
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Production incidents require manual diagnosis across K8s, logs, and runbooks under time pressure |
| Interest | LangGraph ReAct agent with episodic/semantic/procedural memory and Slack-gated remediation |
| Technology | `Python` · `LangGraph` · `FastAPI` · `Ollama` · `Kubernetes` · `pgvector` · `Redis` |
| Links | [repo](https://github.com/aitch-cmd/AegisOps-DRI-Autonomous-SRE-Agent) |

### Open SWE
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Engineering orgs need internal coding agents connected to their systems with safety boundaries |
| Interest | Open-source async coding agent on LangGraph — sandboxes, Slack/Linear triggers, automatic PRs |
| Technology | `TypeScript` · `LangGraph` · `Deep Agents` · `GitHub OAuth` |
| Links | [repo](https://github.com/aitch-cmd/open-swe) |

### AgenticDB
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Non-technical users cannot query databases without SQL expertise |
| Interest | Human-verified natural language database interface with guardrails |
| Technology | `Python` · `NLP` · `Database` · `Agentic AI` |
| Links | [repo](https://github.com/aitch-cmd/AgenticDB-Human-Verified-Natural-Language-Database-Interface) |

### RealEstate Agent
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Property search lacks intelligent conversational filtering and recommendation |
| Interest | AI agent for real estate discovery with natural language property queries |
| Technology | `Python` · `AI Agent` · `Real Estate` |
| Links | [repo](https://github.com/aitch-cmd/RealEstate_Agent) |

### TravelGraphRAG
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Travel planning requires synthesizing scattered information across sources |
| Interest | GraphRAG pipeline for intelligent travel recommendations and itinerary building |
| Technology | `Python` · `RAG` · `Graph` · `LangChain` |
| Links | [repo](https://github.com/aitch-cmd/TravelGraphRAG) |

### ZoneWatch
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Video surveillance needs real-time object detection with custom zone triggers |
| Interest | Multi-model pipeline — YOLOv5, YOLOv8, Detectron2 with polygon zone monitoring |
| Technology | `Python` · `YOLOv8` · `Detectron2` · `Computer Vision` · `CUDA` |
| Links | [repo](https://github.com/aitch-cmd/ZoneWatch) |

### ResuMatchAI
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Job seekers struggle to tailor resumes to specific role requirements |
| Interest | AI-powered resume matching and optimization against job descriptions |
| Technology | `Python` · `NLP` · `AI` |
| Links | [repo](https://github.com/aitch-cmd/ResuMatchAI) |

### HabitatAgent
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Smart home systems lack intelligent autonomous decision-making |
| Interest | AI agent for habitat automation with contextual awareness |
| Technology | `Python` · `AI Agent` · `IoT` |
| Links | [repo](https://github.com/aitch-cmd/HabitatAgent) |

### Lead Auto-Qualification Agent
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Sales teams waste time on unqualified leads |
| Interest | Django + agentic AI pipeline for autonomous lead scoring and qualification |
| Technology | `Django` · `Python` · `Agentic AI` |
| Links | [repo](https://github.com/aitch-cmd/Lead-Auto-Qualification-Agent) |

### ReAct RAG
| Field | Value |
|-------|-------|
| Status | Active |
| Problem | Standard RAG lacks reasoning loops for complex multi-step retrieval |
| Interest | ReAct-pattern retrieval augmented generation with tool-use reasoning |
| Technology | `Python` · `RAG` · `ReAct` · `LangChain` |
| Links | [repo](https://github.com/aitch-cmd/ReAct_RAG) |

---

## Design Director Evaluation

| Criterion | Pass? |
|-----------|-------|
| Shipped product framing | ✓ Problem + Interest rows |
| Compact | ✓ No paragraphs |
| Real repos only | ✓ All from aitch-cmd |
| Consistent with hackathon cards | ✓ Same table schema |
| Interesting, not generic | ✓ Technical insight per row |

**Verdict:** Approved as subsection within Section 01 (Award Winning Products → Shipped Systems).
