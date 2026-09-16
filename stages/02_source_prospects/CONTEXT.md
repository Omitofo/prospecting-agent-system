# Stage 02 – Source Prospects

## Inputs

- Layer 3: `../../_config/sources.md`
- Layer 3: `../../_config/icp.md` (or campaign override)
- Layer 4: campaign `CONTEXT.md` + `stages/01_define_icp/output/icp.md` (if exists)
- Any existing lists in the campaign’s `knowledge/lists/`

## Process

Find candidate businesses that match the campaign ICP.

Capture for each candidate (minimum):
- Business name
- Location / area
- Google rating + approximate review count
- Website URL or "none"
- Google Maps / search link
- One-sentence note on why it looks promising (digital gap observation)

Prefer structured output (markdown table or individual prospect stubs) that stage 03 can score easily.

Quality > quantity. Aim for a focused batch the human can actually review.

## Outputs

- `candidates.md` or `candidates_table.md` → `output/`
- Optionally individual stub files in the campaign’s `knowledge/prospects/` if the batch is small
