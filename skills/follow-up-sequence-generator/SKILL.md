---
name: follow-up-sequence-generator
description: Generate multi-touch real estate follow-up sequences across email, SMS, call notes, voicemail, and CRM tasks. Use for open-house leads, buyer inquiries, seller valuation leads, expired listings, past clients, cold/warm database leads, recruiting, referrals, and stale paid leads.
---

# Follow-Up Sequence Generator

Use this skill to build a practical sequence that turns interest into a booked conversation without spammy pressure.

## Inputs

Collect:
- Lead type: buyer, seller, renter, investor, past client, referral, agent recruit, vendor.
- Source and consent context.
- Time since last interaction.
- Known motivation, timeline, property, area, and objections.
- Approved channels: SMS, email, call, voicemail, DM, WhatsApp.
- Brand voice and CTA.
- Stop conditions and escalation owner.

## Sequence Design

1. Classify lead temperature:
   - Hot: requested appointment, showing, valuation, offer, call, or immediate details.
   - Warm: asked a question, downloaded a guide, attended open house, engaged recently.
   - Nurture: early research, future timeline, past client, sphere.
   - Cold/stale: no response or old CRM record.
2. Match cadence:
   - Hot: 0, 5 min, 30 min, same day, next day.
   - Warm: day 0, 1, 3, 7, 14.
   - Nurture: weekly/monthly value touches.
   - Stale: permission-based reactivation.
3. Write short messages that ask one question.
4. Add CRM updates and stop conditions.
5. Add human escalation for replies, objections, urgency, complaints, and legal/financing questions.

## Output Format

```markdown
# Follow-Up Sequence

## Lead Context
- Segment:
- Source:
- Consent:
- Temperature:
- Goal:
- CTA:

## Cadence
| Touch | Timing | Channel | Purpose | Copy |

## Call / Voicemail Script

## CRM Tasks

## Stop Conditions

## Escalation Rules

## Personalization Tokens
```

## Copy Rules

- SMS should usually be under 320 characters.
- Start with context: why you are reaching out.
- Do not ask multiple questions in one message.
- Do not guilt, pressure, or fake scarcity.
- Include opt-out language where appropriate.
- Do not cold-text without documented consent.

## Sequence Templates

Use these defaults when no cadence is provided:
- Open house: same day value recap, next-day criteria question, day 3 similar homes, day 7 check-in.
- Buyer inquiry: immediate property response, tour CTA, lender/pre-approval question, search setup.
- Seller valuation: valuation context, equity/goal question, call CTA, market update.
- Past client: value-first check-in, home equity/market update, referral ask only after value.
- Expired listing: empathy, non-blaming diagnosis, concise next-step offer.
