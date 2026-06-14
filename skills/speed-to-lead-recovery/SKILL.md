---
name: speed-to-lead-recovery
description: Build a consent-aware speed-to-lead and missed-lead recovery workflow for real estate and home-service businesses. Use when leads are stale, paid leads are not converting, calls are missed, inboxes are slow, or a team needs SMS/email/call follow-up scripts and routing rules.
---

# Speed-to-Lead Recovery

Use this skill to recover missed inquiries and prevent new ones from going cold.

## Inputs

Ask for:
- Lead source and original opt-in context.
- Time since inquiry.
- Lead type: buyer, seller, renter, investor, owner, vendor, home-service request.
- Existing conversation history.
- CRM stage and assigned owner.
- Allowed channels: email, SMS, call, WhatsApp, DM.
- Booking link or next action.

## Workflow

1. Classify the lead:
   - Hot: asked to tour, sell, book, price, schedule, call, or get details.
   - Warm: asked a general question or downloaded a resource.
   - Cold: no reply after multiple touches or old CRM contact.
2. Check consent and channel safety.
3. Write one short recovery message per approved channel.
4. Add a human escalation rule.
5. Create a 7-day follow-up cadence.
6. Define stop conditions: opt-out, wrong number, not interested, already handled.

## Output Format

```markdown
# Recovery Plan

## Lead Summary
- Source:
- Age:
- Intent:
- Consent:
- Owner:

## Message 1
Channel:
Copy:

## 7-Day Cadence
Day 0:
Day 1:
Day 3:
Day 7:

## Escalation Rule

## CRM Update
Stage:
Next action:
Follow-up date:
```

## Copy Rules

- Keep SMS under 320 characters.
- Ask one question at a time.
- Use plain language: leads, calls, showings, appointments, CRM, follow-up.
- Do not pressure. Do not fake urgency.
- Include opt-out language when appropriate.
