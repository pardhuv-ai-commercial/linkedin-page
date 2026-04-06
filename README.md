# The Deployment Gap

**Practitioner intelligence on agentic AI, enterprise strategy, and the distance between what works in theory and what survives production.**

> *Published by Pardhu V — Senior Director, Business Development · Aicadium · Singapore*
> *Human in the loop. Lead author and final authority on all content.*

🌐 **Live site:** [pardhusg.github.io](https://pardhusg.github.io)
&nbsp;&nbsp;💼 **LinkedIn:** [linkedin.com/in/pardhusg](https://www.linkedin.com/in/pardhusg/)

---

## What this is

Most AI projects look good on a vendor slide. Many fail quietly in production — not because the technology doesn't work, but because the architecture wasn't designed for real conditions: multiple vendors, regulated data, fragmented communication platforms, and humans who have to be accountable for autonomous decisions.

**The Deployment Gap** publishes practitioner-grade research on exactly that space. Not hype. Not tutorials. Architecture decisions, governance frameworks, and the failure modes nobody puts in their case studies — drawn from 17+ years of business development across MNCs and startups in APAC, now amplified by a structured human-AI research practice.

---

## Published research

| # | Title | Series | Status |
|---|-------|--------|--------|
| 01 | [Agentic AI in Financial Institutions — Deep-Stack Reference Architecture](fi-agentic-stack.html) | Reference Architecture | ✅ Published |
| 02 | [Architecting the Agent-Native Data Layer](agent-native-data-layer.html) | Enterprise Intelligence | ✅ Published |
| 03 | [Context-Window as a Scarce Resource — Enterprise LLM Architecture](context-window.html) | LLM Architecture | ✅ Published |
| 04 | [Format Selection for Agentic AI Documentation](format-selection.html) | Documentation Standards | ✅ Published |
| 05 | Agentic AI Governance for APAC Financial Institutions — MAS MGF Practitioner Guide | Governance | 🔬 In research |
| 06 | The Multi-Party Support Deadlock — Field Case Study | Case Study | ✍️ Drafting |

---

## Site structure

```
root/
├── index.html                    # Homepage — publication index
├── about.html                    # About Pardhu V — background, methodology, POV
├── fi-agentic-stack.html         # Publication 01
├── agent-native-data-layer.html  # Publication 02
├── context-window.html           # Publication 03
├── format-selection.html         # Publication 04
└── README.md                     # This file
```

Each HTML file is fully self-contained — no build tools, no frameworks, no dependencies beyond Google Fonts. Drop a new `.html` file into this root folder and it is live within 60 seconds of pushing to `main`.

---

## How new publications are added

1. Write the new piece as a standalone `.html` file following the BCG dark-mode design system used across the site
2. Add the shared nav block at the top of `<body>` (copy from any existing file)
3. Open `index.html` and promote the next `pub-upcoming` placeholder to a full `pub-row` entry, linking to the new file
4. Push both files to `main` — GitHub Pages rebuilds automatically

No CI/CD pipeline. No static site generator. No config files. Just HTML files in a flat folder.

---

## Research methodology

Each publication is produced through a structured **human-in-the-loop collaboration** with a coordinated team of specialised AI agents, each with a defined research mandate and governed output scope:

| Agent | Mandate |
|-------|---------|
| **ArchitectAgent** | Reference architecture diagrams, layered system models, vendor trade-off analysis |
| **ResearchAgent** | Live web research across Substack, Medium, arXiv, academic preprints — production reality gap |
| **IndustryAgent** | Sector analysis — financial services, industrial, logistics, aviation, telecoms |
| **GovernanceAgent** | Governance patterns, failure taxonomies, MAS / EU AI Act / HIPAA regulatory signal analysis |
| **VendorAgent** | Middle-layer platform analysis — Oracle, Snowflake, Databricks, SAP, Neo4j, IBM WatsonX |
| **NarrativeAgent** | MBB-style consulting narrative — executive POV, implications, practitioner voice |
| **DesignAgent** | Full HTML/CSS implementation — typography, layout, diagrams, print optimisation |
| **Pardhu V** | Research agenda · editorial validation · final authority on all positions and claims |

All agent outputs are reviewed, validated, and curated before inclusion. The strategic intelligence, practitioner credibility, and accountability for every position published here rests entirely with the human author.

---

## Topics covered

- **Agentic AI architecture** — multi-agent systems, MCP gateway, LangGraph orchestration, agent spec files
- **Enterprise AI deployment** — production failure modes, multi-party operations, MTTR, operational support
- **AI governance** — MAS TRM, IMDA Model AI Governance Framework, APAC regulatory alignment
- **LLM architecture** — context window management, memory-first design, RAG pipelines, vector stores
- **Financial services AI** — AML/KYC automation, compliance workflows, regulated environment constraints
- **Documentation standards** — C4 model, Mermaid, ADRs, arc42, docs-as-code for agentic systems
- **AI commercialisation** — BD strategy, POC-to-ARR conversion, value-based pricing, TCO frameworks

---

## About the author

**Pardhu V** is a Senior Director leading AI transformation initiatives at Aicadium, bridging enterprise strategy with scalable AI deployment. He drives business-led discussions on data infrastructure, governance, and agentic AI adoption across industrial and technology sectors in APAC.

- 17+ years in business development across MNCs and startups
- Specialisation: Industrial AI, IIoT, Computer Vision, AIoT, Agentic Workflows
- Location: Singapore
- LinkedIn: [linkedin.com/in/pardhusg](https://www.linkedin.com/in/pardhusg/)

---

## Design system

The site uses a BCG-inspired dark-mode palette:

| Token | Value | Usage |
|-------|-------|-------|
| Background | `#0D0D0D` | Page base |
| Surface | `#141414` | Cards, nav, footer |
| BCG Green | `#00A651` | All accents, rules, highlights |
| Body type | DM Sans | Prose, labels |
| Display type | Cormorant Garamond | Headlines, large numbers |
| Monospace | DM Mono | Eyebrows, tags, nav links, code |

Subtle dot-grid background texture. 3px BCG green rule at top of hero sections. Square headshot with offset green border. Flush grid card layouts with 1px rule separators. All files are print-ready.

---

## License

Content © Pardhu V 2026. All rights reserved.

Research produced with AI agent assistance. All positions, claims, and editorial decisions are the author's own. AI agents do not independently publish or represent views on this site.

---

*Published when the argument is ready — not on a schedule.*
