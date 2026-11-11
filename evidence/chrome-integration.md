# Claude in Chrome — Integration Status & Setup

Reference: https://code.claude.com/docs/en/chrome

## Intended use for Beity Store

User-supervised, **read-only** Facebook research:

1. Open the official evidence photo/album.
2. Observe public Page content while the user is present.
3. Capture citations into `evidence/` or brand updates.
4. Never publish, comment, like, join, or mass-message.

## Prerequisites checklist

| Requirement | Notes |
|---|---|
| Chromium browser (Chrome/Edge/Brave/etc.) | Required |
| Claude in Chrome extension ≥ 1.0.36 | Chrome Web Store |
| Claude Code with `/login` (Anthropic plan) | API-key-only / setup-token auth keeps Chrome off |
| Not WSL | Windows native is OK |
| Launch | `claude --chrome` or `/chrome` inside Claude Code |

## Setup steps

1. Install/update Claude in Chrome extension.
2. From this project directory, run Claude Code with Chrome: `claude --chrome`.
3. Run `/chrome` and confirm panel shows Status: Enabled and Extension: Installed.
4. Approve site permissions for facebook.com when prompted (read/observe only).
5. Start with E1: https://www.facebook.com/photo/?fbid=122128176057484360&set=a.122113145175484360

## Runtime verification log

| Date | Check | Result |
|---|---|---|
| 2026-11-10 | Skills workspace created; Chrome status probed from this agent session | See `evidence/chrome-verification.txt` (if present). Do not claim Facebook access unless that file records a successful `/chrome` Enabled status and a supervised page open. |

## Forbidden actions (repeat)

- Passwords in chat
- Private group scraping
- Mass join / bulk DM
- Bypass Meta limits
- Auto publish / like / comment / join
- Touching Lakta / face-agent / Native Host / Telegram session
