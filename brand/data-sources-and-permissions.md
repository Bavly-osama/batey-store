# Data Sources and Permissions

## Allowed sources

| Source | Path / URL | Use |
|---|---|---|
| Official Page photo evidence | https://www.facebook.com/photo/?fbid=122128176057484360&set=a.122113145175484360 | Supervised Page research |
| Brand identity strings | Read-only reference from face-agent content script (do not edit) | Name variants |
| Groups snapshot | `evidence/groups-snapshot/beity_177_groups.csv` | Group scoring research |
| Brand knowledge | `brand/*` | Context for all workflows |
| Installed skills | `.claude/skills/*/SKILL.md` | Methodologies |
| User-supplied exports | Analytics CSVs / screenshots provided by user | KPI filling |

## Claude in Chrome — supervised read-only Facebook research

Prerequisites (from Claude Code docs):
- Chromium browser (Chrome/Edge/etc.)
- Claude in Chrome extension ≥ 1.0.36
- Claude Code authenticated via `/login` (API-key-only auth disables Chrome)
- Start with `claude --chrome` or enable via `/chrome`

### Allowed browser actions
- Open E1 photo/album and publicly visible Page content while user supervises
- Observe public About / posts / group About pages already listed in the snapshot
- Extract observations into local markdown with citations

### Forbidden browser / research actions
- Ask for Facebook passwords in chat
- Scrape private group data
- Automate mass membership requests
- Send bulk unsolicited messages
- Bypass Meta restrictions
- Auto publish, comment, like, or join groups
- Modify `X:\bytiey-face-agent`, Telegram session, Native Host, or Lakta extension

## Ownership reminder

ChatGPT Work manages recurring reports and business decisions. Claude Code produces frameworks, drafts, and evidence packs only.
