---
name: closing-timeline-checklist
description: Build a real estate transaction timeline and checklist from contract to close. Use for buyer closing timelines, seller closing timelines, inspection/appraisal/financing milestones, agent task lists, client email summaries, and CRM transaction workflows.
---

# Closing Timeline Checklist

Use this skill to create a transaction roadmap that is useful to clients and operators.

## Inputs

Ask for:
- Buyer or seller side.
- Contract date, option/inspection deadline, financing deadline, appraisal deadline, closing date.
- State/market if provided.
- Property type and occupancy.
- Parties: agent, TC, lender, title/escrow, inspector, attorney, HOA, insurance.
- Known contingencies.
- Communication preference.
- Brokerage or local checklist constraints.

## Workflow

1. Build a date-based timeline from contract to close.
2. Separate client tasks from agent/team tasks.
3. Mark hard deadlines vs soft reminders.
4. Include dependency chains:
   - inspection before repair negotiation.
   - lender docs before clear to close.
   - appraisal before final loan approval.
   - title/escrow before signing/funding.
5. Add reminder messages.
6. Add escalation rules for missed deadlines.

## Output Format

```markdown
# Closing Timeline

## Transaction Summary
- Side:
- Contract date:
- Closing date:
- Key deadlines:

## Client Checklist
| Due | Task | Owner | Notes |

## Agent / Team Checklist
| Due | Task | Owner | Notes |

## Critical Path

## Client Email Summary

## Reminder Messages

## Escalation Rules

## Verify With Local Contract
```

## Guardrails

- Do not interpret contract terms as legal advice.
- Do not invent deadlines if not provided; label assumptions.
- Recommend confirming all dates against the signed contract and local brokerage process.
- Route legal disputes, contract interpretation, financing, title, appraisal, or insurance issues to the proper licensed professional.

## Quality Bar

- Make the timeline actionable by owner and due date.
- Highlight the next three urgent tasks.
- Include "what can delay closing" in plain language.
- Keep client-facing copy calm and clear.
