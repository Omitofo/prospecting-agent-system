# Stage 03 – Qualify & Score

## Inputs

- Layer 3: `../../_config/scoring.md`
- Layer 4: `../02_source_prospects/output/` (candidates)
- Layer 4: campaign ICP (`stages/01_define_icp/output/icp.md` or campaign CONTEXT)

## Process

Score each candidate using the dimensions in `scoring.md` (or campaign-adjusted weights).

For every prospect produce:
- Numeric scores + short justification
- Overall weighted score
- Recommendation: Shortlist / Maybe / Skip

Produce a clean ranked shortlist the human can approve or edit.

## Outputs

- `scored_candidates.md` → `output/`
- `shortlist.md` → `output/` (only the ones above threshold, ready for enrichment)
