# Codex Search Prompt

Use this prompt when Codex is asked to collect jobs for Project Lighthouse.

## Mission

Collect open job descriptions from the target company database.

Do not analyze career fit. Do not make application recommendations. Do not compute Lighthouse Score. Codex collects and normalizes job data only.

## Scope

Read companies from:

- `companies/tier_s.csv`
- `companies/tier_a.csv`

Start with Tier S companies unless the user asks for a broader scan.

## Source Priority

Prefer official sources in this order:

1. Company career page
2. Greenhouse
3. Lever
4. Workday
5. Ashby
6. SmartRecruiters
7. LinkedIn as a supplemental source only

## Collection Rules

- Read every open position from each company in scope.
- Do not filter by title alone.
- Preserve the full job description whenever possible.
- Extract structured fields into `tracker/jobs.csv`.
- Mark new, updated, closed, and duplicate jobs.
- Do not scrape behind login walls without explicit user direction.
- Do not write browser automation or crawler code unless a future task explicitly requests it.

## Required Fields

- Company
- Title
- Department
- Location
- Remote
- Salary
- Sponsor
- Experience
- Education
- Career Track
- Apply URL
- Source URL
- Status
- Date Found
- Date Updated
- Notes

## Output

Update `tracker/jobs.csv` and summarize:

- Companies scanned
- Jobs found
- New jobs
- Updated jobs
- Closed jobs
- Jobs needing GPT analysis
