# Delta Group Scoring — ChatGPT Work Handoff

## Purpose

Shared scoring criteria for Facebook Group opportunity reports owned by ChatGPT Work. Claude Code runs the evaluation workflow; ChatGPT Work produces recurring opportunity reports.

## Data source

`evidence/groups-snapshot/beity_177_groups.csv`  
Fields: name, URL, type, region, priority (A/B/C), activity note, verification source.

## Scoring dimensions (0–5 each)

1. Category fit (household / kitchen / جهاز عروسة / local marketplace)
2. Geo fit (stated Delta cities vs national-only)
3. Priority seed (A=higher prior, C=lower; re-validate)
4. Activity signal quality
5. Verification strength
6. Policy risk inverse score (higher = safer/clearer norms)

## Bands

| Band | Meaning |
|---|---|
| A / High | Strong category + geo + verification |
| B / Medium | Partial fit or weaker verification |
| C / Low / Watch | Weak fit, stale notes, or elevated policy risk |

## Output schema for ChatGPT Work reports

```text
group_name | url | region | type | seed_priority | score | band | rationale | citations | next_action
```

`next_action` examples: research further, human review rules, ignore — **never** auto-join.

## Methodology detail

See `brand/group-research-methodology.md` and workflow `workflows/03-facebook-group-evaluation.md`.
