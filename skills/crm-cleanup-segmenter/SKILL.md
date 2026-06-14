---
name: crm-cleanup-segmenter
description: Clean and segment real estate CRM exports or pasted contact lists into actionable groups. Use for stale leads, messy CSVs, duplicate contacts, missing stages, old Zillow/Realtor/Facebook leads, sphere lists, and follow-up prioritization.
---

# CRM Cleanup Segmenter

Use this skill to convert a messy contact list into prioritized follow-up segments.

## Inputs

Accept:
- CSV columns.
- Pasted CRM rows.
- Lead notes.
- Export summaries.
- Current pipeline stages.

## Workflow

1. Identify available fields and missing fields.
2. Normalize stages into:
   - New.
   - Hot.
   - Warm.
   - Nurture.
   - Past client.
   - Vendor/partner.
   - Not a fit.
   - Unknown.
3. Detect duplicates by name, email, phone, and property.
4. Score follow-up priority.
5. Create tags by source, segment, age, and next action.
6. Produce a cleanup plan and sample follow-up copy.

## Output Format

```markdown
# CRM Cleanup Plan

## Field Audit

## Segments
| Segment | Criteria | Action |

## Priority Leads

## Duplicates / Bad Data

## Tags to Add

## Follow-Up Queue
Day 1:
Day 2:
Day 3:
```

## Guardrails

- Do not expose or repeat unnecessary personal data.
- Do not recommend mass cold SMS.
- If data includes sensitive protected-class details, exclude them from tags and scoring.
