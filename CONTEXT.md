# CONTEXT.md – Layer 1 (Workspace Routing)

## Purpose of this workspace

A complete, expandable prospecting system that can serve any type of business. Primary use case: software development agency looking for prospects who need landing pages or web applications. The system itself is niche-agnostic.

## How to orient yourself

1. Read `AGENT.md` (global rules).
2. Read `campaigns/_index.md` to see all campaigns and which one (if any) is active.
3. For the active campaign, read its `CONTEXT.md` and `status.md`.
4. Stage contracts live in `stages/0X_.../CONTEXT.md`. They describe exactly what to load and where to write.
5. Global durable knowledge lives in `_config/` and `shared/`.

## Multi-campaign model

Every distinct ICP / niche / time-bound prospecting effort gets its own folder under `campaigns/`.

- Campaign folders contain **all Layer 4 artifacts** (outputs, prospect files, lists, logs).
- Stage definitions remain shared templates.
- When the human says "run stage N", write results into the *active campaign’s* `stages/0N_.../output/`.

If the human asks to work on a different campaign, update `_index.md` and proceed.

## Creating a new campaign

1. Create `campaigns/YYYY-MM-short-description/`.
2. Copy a starter `CONTEXT.md` and `status.md` (or generate them).
3. Seed an initial ICP from `_config/icp.md` + human input.
4. Add the campaign to `campaigns/_index.md` and mark it active.
5. Begin with stage 01 or jump to the appropriate stage.

## Key files the agent must know

| Path | Role |
|------|------|
| `AGENT.md` | Global identity & rules |
| `campaigns/_index.md` | Catalog of all campaigns |
| `campaigns/<id>/CONTEXT.md` | This campaign’s ICP, goals, sources |
| `campaigns/<id>/status.md` | Current stage & notes |
| `stages/*/CONTEXT.md` | Stage contracts |
| `_config/*` | Durable factory settings |
| `shared/*` | Templates & reference |

## Default behavior when ambiguous

- Prefer the most recently active campaign.
- If no campaign exists, offer to create one.
- Always confirm before overwriting existing output files that look reviewed.
