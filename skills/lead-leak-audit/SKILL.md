---
name: lead-leak-audit
description: Audit a real estate lead path to find where inquiries are leaking before they become appointments. Use for agents, teams, brokerages, property managers, investors, or home-service operators who want to map lead sources, response time, CRM handoff, qualification, follow-up, and booking conversion.
---

# Lead Leak Audit

Use this skill to turn a messy lead process into a simple leak report and 30-day fix plan.

## Inputs

Ask for:
- Business type and market.
- Lead sources: Zillow, Realtor.com, Meta, Google, website, open house, referrals, calls, email, portals.
- Current response time by channel.
- CRM/tool stack.
- Monthly lead volume and approximate value of a converted appointment.
- Who responds first, who qualifies, and who books.
- Follow-up cadence after no reply.

## Workflow

1. Map the current path from source to booked appointment.
2. Mark every handoff: source, inbox, phone, CRM, agent, ISA, calendar, follow-up.
3. Identify the first leak that loses money.
4. Score severity:
   - Critical: no response under 5 minutes, no owner, no CRM record, no opt-out handling.
   - High: slow follow-up, weak qualification, no booking CTA, stale paid leads.
   - Medium: inconsistent notes, no daily report, no source attribution.
5. Recommend the smallest workflow that fixes the first leak.
6. Produce a 30-day plan with owner, tools, scripts, and metric.

## Output Format

```markdown
# Lead Leak Audit

## Current Lead Path
Source -> Capture -> First response -> Qualification -> Booking -> CRM -> Follow-up

## Biggest Leak
- Leak:
- Why it matters:
- Revenue at risk:
- Evidence:

## 30-Day Fix
- Week 1:
- Week 2:
- Week 3:
- Week 4:

## Automation Candidate
- Keep human:
- Automate:
- Escalate:

## Metrics
- Speed to lead:
- Appointment set rate:
- Stale leads:
- Follow-up completion:
```

## Guardrails

- Do not recommend cold SMS unless consent is documented.
- Do not give legal, mortgage, commission, or Fair Housing advice.
- Route legal, contract, pricing, or protected-class questions to the licensed professional.
- Focus on operations: routing, response, CRM hygiene, booking, reporting, and escalation.
