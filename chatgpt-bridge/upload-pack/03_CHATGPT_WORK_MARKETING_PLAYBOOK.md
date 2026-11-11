# ChatGPT Work — Marketing Playbook (Handoff)

This is a **handoff framework**, not a daily report system.

## Ownership

| Owner | Owns |
|---|---|
| **Claude Code** (`X:\Beity-Store-Marketing-Agent`) | Skills, brand knowledge, specialist workflows, evidence packs, draft copy, group scoring research |
| **ChatGPT Work** | Daily/evening reports, ongoing marketing conversations, group opportunity reports, dashboards/docs, recurring research & business recommendations |

Do not rebuild ChatGPT Work reporting inside Claude Code.

## Recommended Claude Code workflows before ChatGPT decisions

| Decision type | Run workflow |
|---|---|
| Channel / Page strategy | `workflows/01-facebook-marketing-strategy.md` |
| Audience / city focus | `workflows/02-delta-audience-research.md` |
| Which groups matter | `workflows/03-facebook-group-evaluation.md` |
| Competitor moves | `workflows/04-competitor-analysis.md` |
| What to post | `workflows/05-content-strategy.md` + `06-egyptian-arabic-copywriting.md` |
| Community replies | `workflows/07-community-management.md` |
| What worked | `workflows/08-engagement-analysis.md` / `10-marketing-performance-analysis.md` |
| Campaign planning | `workflows/09-marketing-campaign-planning.md` |

## Marketing frameworks available

- Brand + voice scaffolds (`brand/`)
- Delta group scoring (`handoff/DELTA_GROUP_SCORING.md`)
- KPI definitions without invented baselines (`brand/marketing-kpis.md`)
- 37 installed skills (see `APPROVED_SKILLS_REGISTER.md`)

## Evidence & citation requirements

1. Cite `evidence/official-sources.md` IDs or direct URLs.
2. Mark unknowns as `UNKNOWN/UNVERIFIED`.
3. Never invent prices, inventory, offers, sales, or demographics.
4. Facebook live observation requires user-supervised Claude in Chrome; do not claim access without verification.

## Publishing boundary

Publishing / Lakta / Telegram / Native Host remain in `X:\bytiey-face-agent` only. ChatGPT Work may recommend posts; humans or that stack execute publishing.
