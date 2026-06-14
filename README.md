# Real Estate AI Skills Pack

Free Claude/Codex-compatible AI skills for real estate operators who want better lead handling, follow-up, listing launches, and CRM hygiene.

Built for agents, small brokerages, property managers, and real-estate teams that need practical AI workflows without rebuilding their whole stack first.

## Skills

- `lead-leak-audit` - find where leads are being lost across forms, calls, texts, CRM stages, and follow-up.
- `speed-to-lead-recovery` - build a first-15-minutes response system for cold or delayed leads.
- `real-estate-lead-qualifier` - score buyer, seller, renter, and investor leads without Fair Housing violations.
- `listing-launch-assistant` - turn listing facts into a launch plan, channel copy, and showing prep.
- `open-house-follow-up` - convert visitor notes into segmented follow-up plans.
- `crm-cleanup-segmenter` - normalize messy CRM exports and create useful segments.
- `ai-receptionist-script` - write safe scripts for inbound calls, SMS, and website chat.

## Install

Claude Code:

```bash
mkdir -p ~/.claude/skills
cp -R skills/* ~/.claude/skills/
```

Codex:

```bash
mkdir -p ~/.codex/skills
cp -R skills/* ~/.codex/skills/
```

If your setup symlinks Codex skills to Claude skills, install once into `~/.claude/skills`.

## Use

Call a skill by name in your AI agent:

```text
Use lead-leak-audit on this CRM export and tell me where we are losing leads.
```

```text
Use ai-receptionist-script for our buyer lead intake calls. Keep it compliant and short.
```

## Lead Magnet Positioning

Offer this as a free pack:

> "7 AI Skills Real Estate Teams Can Use Today to Stop Losing Leads"

CTA:

> Want the full lead-handling system installed for your team? Book a Lumenosis AI audit.

## Compliance Note

These skills produce workflows, scripts, and operational guidance. They do not replace licensed brokerage, legal, lending, tax, or Fair Housing advice.

