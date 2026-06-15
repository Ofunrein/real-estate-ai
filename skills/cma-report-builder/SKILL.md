---
name: cma-report-builder
description: Build a client-ready comparative market analysis narrative from property facts, comparable sales, active listings, pending listings, adjustments, and market context. Use for seller pricing, buyer offer strategy, listing prep, valuation narratives, CMA emails, and agent talking points.
---

# CMA Report Builder

Use this skill to turn comp data into a clear pricing narrative without pretending to be an appraiser.

## Inputs

Ask for:
- Subject property: address/area, property type, beds, baths, sqft, lot, condition, upgrades, year built.
- Comp set: sold, pending, active, withdrawn/expired when relevant.
- For each comp: price, date, distance, beds/baths/sqft, condition, concessions, DOM, notes.
- Market context: inventory, median days on market, price changes, rate environment, seasonality.
- Pricing goal: list price, offer range, refinance estimate, investor buy box, seller education.
- Confidence level and data gaps.

## Analysis Workflow

1. Filter comps:
   - Prefer same property type, nearby, recent, similar size, similar condition.
   - Explain why any weaker comp is included.
2. Separate sold, pending, active, and stale listings.
3. Calculate rough indicators:
   - Sold price range.
   - Price per sqft range.
   - Median/central tendency.
   - Subject-positioning range.
4. Qualitatively adjust for:
   - Size, lot, condition, upgrades, parking, floorplan, location, concessions, views, HOA, pool, ADU, age.
5. Recommend a range, not a fake exact value.
6. Produce client narrative and agent notes.

## Output Format

```markdown
# Comparative Market Analysis

## Executive Summary

## Subject Property

## Comp Table
| Comp | Status | Price | Date | Size | Similarity | Key Adjustment |

## Market Signals

## Pricing Logic
- Low anchor:
- Most likely range:
- Stretch price:
- Risks:

## Recommended Price Range

## Client-Ready Narrative

## Agent Talking Points

## Data Gaps / Verify
```

## Guardrails

- Say "CMA" or "pricing opinion," not "appraisal."
- Do not guarantee sale price, appreciation, days on market, or buyer behavior.
- Do not invent comp details.
- If comp data is thin, say confidence is low and list what is needed.
- Do not provide legal, tax, lending, or appraisal advice.

## Quality Bar

- Strong CMAs explain why the best comps matter and why weak comps are weak.
- Active listings show competition, not value by themselves.
- Pending listings are directional unless final sale terms are known.
- Expired listings can show overpricing or market resistance.
- Always make the pricing recommendation easy for a client to understand.
