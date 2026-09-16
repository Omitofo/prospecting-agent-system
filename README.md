# Prospecting Agent System

**Agentic prospecting infrastructure** built on [Interpretable Context Methodology (ICM)](https://arxiv.org/abs/2603.16021).

Folder structure *is* the agent. Numbered stages, plain markdown contracts, human review gates, and a clean knowledge base.

Designed for software development agencies (landing pages, web apps, etc.) but fully agnostic — retarget any niche by editing config + campaign context.

## Core Principles

- **One agent + filesystem** instead of multi-agent frameworks
- Stages are sequential and reviewable
- Source of truth = the files themselves
- Multi-campaign isolation so different ICPs never mix
- Value-first outreach (no hard selling)

## Quick Start

1. Talk to your agent (Grok / Claude / etc.) inside this repo.
2. "Start a new campaign for [niche]" → creates `campaigns/YYYY-MM-description/`
3. "Run stage 02" or "Source prospects for the current campaign"
4. Review & edit anything in `output/` before the next stage.
5. All data lives under the campaign folder → clean, navigable, permanent.

## Architecture

```
prospecting-agent-system/
├── AGENT.md                 # Layer 0 – agent identity & global rules
├── CONTEXT.md               # Layer 1 – workspace routing
├── _config/                 # Layer 3 – durable factory settings
├── shared/                  # Reusable templates & reference
├── stages/                  # Stage contracts (the "how")
├── campaigns/               # All real work & knowledge (the "what")
│   ├── _index.md
│   └── <campaign-id>/
│       ├── CONTEXT.md
│       ├── status.md
│       ├── knowledge/
│       └── stages/*/output/
└── setup/
```

## Typical Flow

1. **Define / refine ICP** (stage 01)
2. **Source candidates** (stage 02) – Google Maps, reviews, directories…
3. **Qualify & score** (stage 03)
4. **Enrich** (stage 04) – website audit, pain points, contacts
5. **Outreach prep** (stage 05) – personalized value-first emails + demo notes
6. **Pipeline** (stage 06) – tracking, follow-ups, status

You can jump to any stage, run partial work, or ask the agent to "look at the current campaign and suggest next actions".

## License

MIT (same spirit as the ICM protocol).
