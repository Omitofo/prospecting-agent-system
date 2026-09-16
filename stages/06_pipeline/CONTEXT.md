# Stage 06 – Pipeline & Follow-up

## Inputs

- Layer 4: all previous stage outputs for the campaign
- Campaign `knowledge/outreach_log.md` (if exists)
- Human status updates

## Process

Maintain a living view of every prospect that has entered the pipeline:

- Current status (Not contacted / Email sent / Replied / Meeting / Closed / Nurture / Dead)
- Last action + date
- Next recommended action
- Notes

Update the campaign’s `knowledge/outreach_log.md` and produce a clean dashboard the human can scan.

Also suggest follow-up timing and light follow-up copy when appropriate (using `shared/email_templates/follow_up.md`).

## Outputs

- `pipeline_status.md` → `output/`
- Updated `../../knowledge/outreach_log.md`
