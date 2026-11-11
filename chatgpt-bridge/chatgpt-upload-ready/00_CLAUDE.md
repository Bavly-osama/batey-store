# Beity Store — Claude Code Marketing Workspace

Independent Claude Code marketing environment for **Beity Store / بيتي ستور / لقطه**.

## Ownership split

### This workspace (Claude Code) owns
- Local marketing skills (`.claude/skills/`)
- Brand knowledge (`brand/`)
- Reusable specialist workflows (`workflows/`)
- ChatGPT Work handoff frameworks (`handoff/`)
- User-supervised, read-only Facebook research guidance (Claude in Chrome)

### ChatGPT Work owns (do NOT rebuild here)
- Daily and evening reports
- Ongoing marketing conversations
- Group opportunity reports
- Marketing dashboards and documents
- Recurring research and business recommendations

Handoff docs explain frameworks and evidence rules. They are **not** daily reports.

## Hard exclusions

- Do **not** modify `X:\bytiey-face-agent` (Lakta extension, Telegram session, Native Host, Facebook publishing engine).
- Do **not** create a new Facebook publishing system.
- Do **not** request Facebook passwords in chat.
- Do **not** scrape private group data, automate mass membership requests, send bulk unsolicited DMs, or bypass Meta restrictions.
- Do **not** automatically publish, comment, like, or join groups.

## Brand evidence rules

1. Cite sources listed in `evidence/official-sources.md`.
2. Never invent product prices, inventory, offers, sales numbers, demographics, or brand claims.
3. Mark gaps as `UNKNOWN/UNVERIFIED`.
4. Prefer Egyptian Arabic (عامية مصرية) for Facebook copy drafts unless the user asks otherwise.

## How to work

1. Read relevant files under `brand/` first.
2. Invoke the matching installed skill(s) under `.claude/skills/` — do not duplicate their instructions.
3. Prefer a workflow from `workflows/` for multi-skill tasks.
4. Produce outputs suitable for ChatGPT Work handoff (structured markdown, citations, unknowns listed).
5. For live Facebook observation, use Claude in Chrome only under user supervision and read-only constraints documented in `brand/data-sources-and-permissions.md`.

## Primary brand files

- `brand/brand-profile.md`
- `brand/brand-voice.md`
- `brand/audience-profile.md`
- `brand/delta-market.md`
- `brand/facebook-strategy.md`
- `brand/group-research-methodology.md`
- `brand/marketing-kpis.md`
- `brand/data-sources-and-permissions.md`
- `.agents/product-marketing.md` (pointer for `product-marketing` skill)
