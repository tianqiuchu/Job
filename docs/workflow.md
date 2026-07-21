# GPT and Codex Workflow

## Division of Labor

Codex collects, normalizes, structures, and maintains data.

GPT interprets JDs, scores opportunities, writes application materials, and makes career recommendations.

## Daily Workflow

1. Codex scans target companies.
2. Codex updates `tracker/jobs.csv`.
3. GPT reads full JDs for relevant jobs.
4. GPT assigns Lighthouse Score and recommendation tier.
5. User selects jobs to apply.
6. GPT prepares tailored resume, CV, cover letter, LinkedIn message, and interview prep.
7. Codex updates tracker status if asked.

## Weekly Workflow

1. Summarize new jobs.
2. Summarize applications and responses.
3. Track skill demand trends.
4. Update company database.
5. Update blacklist.
6. Recommend next week's application strategy.

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
