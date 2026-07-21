# GPT and Codex Workflow

## Division of Labor

Codex collects, normalizes, structures, and maintains data.

GPT interprets JDs, scores opportunities, writes application materials, and makes career recommendations.

## Daily Workflow

1. Codex scans the US Bio + AI + Data job universe.
2. Codex uses LinkedIn and aggregators as radar for discovery.
3. Codex verifies promising jobs against official company or ATS pages.
4. Codex deduplicates jobs across sources.
5. Codex updates `tracker/jobs.csv` and stores JD paths when available.
6. Codex updates dynamic company intelligence for newly discovered companies.
7. GPT reads full official JDs for relevant jobs.
8. GPT assigns Lighthouse Score and recommendation tier.
9. User selects jobs to apply.
10. GPT prepares tailored resume, CV, cover letter, LinkedIn message, and interview prep.
11. Codex updates tracker status if asked.

## Weekly Workflow

1. Summarize new jobs.
2. Summarize applications and responses.
3. Track skill demand trends.
4. Update company database.
5. Update blacklist.
6. Update source quality and duplicate patterns.
7. Recommend next week's application strategy.

## Source Rules

- LinkedIn is a radar, not the source of truth.
- Official company and ATS pages are the source of truth.
- If source information conflicts, trust the official JD.
- Do not use title-only filtering.
- Preserve the full JD whenever possible.

## Status Values

Suggested job statuses:

- New
- Needs GPT Analysis
- Review
- Ready
- Applied
- Interview
- Follow Up
- Rejected
- Closed
- Pass
