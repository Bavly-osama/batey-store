# Facebook Group Research Methodology

## Purpose

Evaluate Facebook Groups for Beity Store relevance in Egypt / Delta household markets. This is research scoring — not join/publish automation.

## Primary dataset

`evidence/groups-snapshot/beity_177_groups.csv`  
Columns (Arabic headers):

| Column | Meaning |
|---|---|
| # | Row index |
| اسم الجروب | Group name |
| الرابط | Public Facebook group URL |
| النوع | Category / type |
| المنطقة | Region |
| الأولوية | Priority A / B / C |
| إشارة النشاط/ملاحظة | Activity signal / note |
| مصدر التحقق | Verification source |

## Scoring rubric (for ChatGPT Work + Claude Code)

Score each group 0–5 on:

1. **Category fit** — household, kitchen, bridal/جهاز عروسة, local marketplace relevance
2. **Geo fit** — Delta city / region match vs national-only
3. **Priority seed** — existing A/B/C as a starting prior, not final truth
4. **Activity signal quality** — note usefulness / freshness (UNKNOWN if stale)
5. **Verification strength** — presence and credibility of `مصدر التحقق`
6. **Policy risk** — spamminess, commercial hostility, unclear rules (flag only; no bypass)

**Composite bands**
- A / High: strong category + geo + verification
- B / Medium: partial fit or weaker verification
- C / Low / Watch: weak fit, outdated notes, or high policy risk

## Process

1. Filter CSV by region / type.
2. Apply rubric; keep citations (URL + note).
3. Output a scored table for ChatGPT Work — do not auto-join.
4. Mark anything not directly evidenced as UNKNOWN.

## Forbidden

- Scraping private member lists or private posts
- Automating join requests
- Publishing into groups from this workspace

## Related skills

`facebook-groups`, `community-marketing`, `competitor-analysis`, `content-research-and-sourcing`.
