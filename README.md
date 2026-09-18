# Prospecting Agent System

**Agentic prospecting infrastructure** built on Interpretable Context Methodology (ICM).

Folder structure *is* the agent. Numbered stages, plain markdown contracts, human review gates, and a clean knowledge base.

## Core Thesis (evolved)

> Don’t prospect businesses because they lack a website.  
> Prospect businesses because they have something worth protecting/growing — demand, reputation, customers, high-value services — and their digital presence appears to be underperforming relative to that opportunity.

We look for **Digital Opportunities**: strong evidence of demand + trust + high customer value, combined with a meaningful digital-presence / conversion gap.

“No website” is one form of digital weakness. Outdated, slow, confusing, or conversion-poor websites are equally interesting.

## Architecture

```
prospecting-agent-system/
├── AGENT.md / CONTEXT.md     # Global agent rules + routing
├── _config/                  # Durable factory settings (ICP templates, scoring, voice…)
├── shared/                   # Reusable templates
├── stages/                   # Stage contracts (reusable how-to)
├── campaigns/                # Isolated campaign instances (the actual work)
└── setup/
```

Campaign isolation is preserved. Each campaign has its own CONTEXT, ICP, knowledge, outputs, and status.

## Typical flow

1. (Optional) Market / Niche Discovery  
2. Define / refine ICP for the campaign  
3. Source candidates (demand + reputation signals first)  
4. Qualify with multi-dimensional, evidence-based scoring  
5. Enrich (website audit, social, reviews, contacts)  
6. Outreach prep (value-first, evidence-backed)  
7. Pipeline tracking

## Active experimental campaign

See `campaigns/2026-09-local-service-digital-opportunity/` for the first controlled experiment under the new thesis.

## License

MIT
