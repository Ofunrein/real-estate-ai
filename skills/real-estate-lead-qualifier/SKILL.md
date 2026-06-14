---
name: real-estate-lead-qualifier
description: Qualify buyer, seller, investor, renter, property-management, and home-service leads. Use for inbound forms, emails, SMS, calls, DMs, open-house notes, or CRM records that need intent scoring, missing fields, next action, and human handoff.
---

# Real Estate Lead Qualifier

Use this skill to turn raw lead text into a structured qualification summary.

## Extract

Capture:
- Name and contact channel when provided.
- Segment: buyer, seller, renter, investor, landlord, property manager, agent, vendor.
- Property/location.
- Timeline.
- Budget, price point, financing, or target deal size when available.
- Motivation or pain.
- Source.
- Consent/relationship context.
- Urgency.
- Missing fields.

## Score

Use this simple scale:
- 5: Explicit appointment or transaction intent now.
- 4: Clear need and timeline under 30 days.
- 3: Interested but missing timeline or budget.
- 2: Researching, vague, or low intent.
- 1: Not a fit, spam, wrong market, or no clear need.

## Next Action

Recommend exactly one next action:
- Book consult/showing/listing call.
- Ask one missing qualification question.
- Send resource.
- Add to nurture.
- Route to licensed agent.
- Mark not a fit.

## Output Format

```markdown
# Lead Qualification

## Summary

## Score
Score:
Reason:

## Missing Fields

## Next Action

## Suggested Reply

## CRM Fields
- segment:
- source:
- urgency:
- stage:
- owner:
- next_action:
```

## Guardrails

- Do not invent financing, price, property condition, or motivation.
- Do not answer legal, mortgage, or contract questions.
- If protected-class or Fair Housing-sensitive content appears, ignore it for scoring and route to a licensed human.
