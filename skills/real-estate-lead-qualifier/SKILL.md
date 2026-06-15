---
name: real-estate-lead-qualifier
description: Qualify buyer, seller, investor, renter, property-management, home-service, vendor, and agent-referral leads. Use for inbound forms, emails, SMS, calls, DMs, open-house notes, portal leads, CRM records, AI receptionist transcripts, or missed-call summaries that need intent scoring, missing fields, routing, SLA, next action, and human handoff.
---

# Real Estate Lead Qualifier

Use this skill to turn raw lead text into a structured qualification summary, routing decision, and first response.

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
- Current owner or assigned team when provided.
- Prior conversation history.
- Channel constraints: SMS, email, call, WhatsApp, DM.
- Missing fields.

## Score

Use this scale:
- 5: Explicit appointment, showing, listing, valuation, offer, urgent service, or transaction intent now.
- 4: Clear need and timeline under 30 days, reachable, one important field missing.
- 3: Real interest but missing timeline, budget, property, motivation, or financing.
- 2: Researching, vague, stale, low intent, or nurture-only.
- 1: Not a fit, spam, wrong market, no consent, no clear need, or protected-class/steering request.

## Routing

Choose one:
- Agent now.
- ISA / receptionist follow-up.
- Lender intro.
- Seller consult.
- Property manager / vendor route.
- Nurture sequence.
- Ask one missing question.
- Mark not a fit.

Set SLA:
- Immediate: score 5, active appointment/showing/listing intent.
- Same day: score 4.
- 24h: score 3.
- Nurture: score 2.
- Stop / no action: score 1 or opt-out.

## Next Action

Recommend exactly one next action:
- Book consult/showing/listing call.
- Ask one missing qualification question.
- Send resource.
- Add to nurture.
- Route to licensed agent.
- Mark not a fit.

Prefer the action that creates a booked conversation or clears the highest-risk missing field.

## Output Format

```markdown
# Lead Qualification

## Summary

## Score
Score:
Reason:
Route:
SLA:

## Missing Fields

## Next Action

## Suggested Reply
SMS:
Email:
Call note:

## CRM Fields
- segment:
- source:
- urgency:
- stage:
- owner:
- next_action:
- follow_up_due:
- lead_score:
- consent_status:
```

## Guardrails

- Do not invent financing, price, property condition, or motivation.
- Do not answer legal, mortgage, or contract questions.
- If protected-class or Fair Housing-sensitive content appears, ignore it for scoring and route to a licensed human.
- Do not recommend cold SMS without documented consent.
- Stop messaging if the contact opts out, says wrong number, or says not interested.
- Never claim the AI is a human assistant.

## Automation Angle

When useful, add a short note:

```markdown
## Automation Candidate
- Automate:
- Keep human:
- Escalate when:
```
