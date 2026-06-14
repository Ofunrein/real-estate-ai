---
name: open-house-follow-up
description: Segment open-house visitors and create follow-up messages, CRM updates, and next actions. Use for sign-in sheets, notes, buyer conversations, agent observations, QR form exports, or post-open-house lead routing.
---

# Open House Follow-Up

Use this skill to convert open-house traffic into organized follow-up.

## Inputs

Ask for:
- Visitor list or notes.
- Property shown.
- Visitor comments.
- Timeline and budget if known.
- Agent notes.
- Preferred contact method and consent context.
- CRM fields available.

## Segments

Classify each visitor:
- A: ready buyer, asked specific buying/showing/offer questions.
- B: active buyer, needs nurture or lender/criteria clarity.
- C: neighbor/seller lead.
- D: casual/browser.
- E: agent/vendor/not a lead.

## Workflow

1. Extract each visitor into a row.
2. Segment and score intent.
3. Draft a short follow-up for each segment.
4. Create CRM tags.
5. Assign next action and due date.
6. Flag any seller leads separately.

## Output Format

```markdown
# Open House Follow-Up

## Visitor Table
| Name | Segment | Intent | Notes | Next Action |

## Messages
Segment A:
Segment B:
Segment C:
Segment D:

## CRM Tags

## Same-Day Tasks
```

## Guardrails

- Do not imply representation or agency relationship unless provided.
- Do not use protected-class details in segmentation.
- Keep follow-up helpful, specific to the property, and one-question focused.
