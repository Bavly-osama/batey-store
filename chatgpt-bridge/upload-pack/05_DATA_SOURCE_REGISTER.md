# Data Source Register — ChatGPT Work Handoff

## Approved sources

| ID | Source | Location | Allowed use | Limitations |
|---|---|---|---|---|
| E1 | Official Facebook photo post | https://www.facebook.com/photo/?fbid=122128176057484360&set=a.122113145175484360 | Page evidence, supervised visual research | Not a canonical Page home URL by itself |
| E2 | Page identity name variants | Face-agent `src/content/content.ts` (read-only) | Confirm Beity Store / بيتي ستور / لقطه naming | Do not modify face-agent; not marketing copy evidence |
| E3 | User business brief | Setup instructions | Categories + Delta cities | No prices/demographics supplied |
| E4 | Groups snapshot CSV | `evidence/groups-snapshot/beity_177_groups.csv` | Group scoring research | Snapshot may drift from live groups; notes may be stale |
| E5 | Brand knowledge pack | `brand/*` | Shared context | Contains explicit UNKNOWN fields |
| E6 | Claude in Chrome | User browser session | Supervised read-only observation | Not verified until `/chrome` Enabled; no publish actions |
| E7 | User analytics exports | Provided ad hoc | KPI filling | Must be dated and attributed |

## Data limitations (always disclose)

- Canonical Page vanity/home URL: UNKNOWN
- No verified sales, inventory, pricing, or demographic stats in this workspace
- Groups CSV is a research prior, not live membership proof
- Facebook access is **not claimed** unless Chrome verification succeeds in-session

## Citation requirements

Every ChatGPT Work recommendation that relies on Claude Code outputs must include:

1. Source ID or URL
2. Observation date when live-checked
3. `UNKNOWN` markers for gaps
4. Clear separation of fact vs hypothesis

## Prohibited sources / methods

Private group scrapes · password collection · mass join/DM automation · Meta restriction bypass · face-agent publishing APIs treated as Claude Code skills
