# Codex Job Universe Collection Prompt

Use this prompt when Codex is asked to collect jobs for Project Lighthouse.

## Mission

Collect open job descriptions from the US Bio + AI + Data job universe.

Do not analyze career fit. Do not make application recommendations. Do not compute Lighthouse Score. Codex collects, verifies, deduplicates, and normalizes job data only.

## Scope

The search space is not limited to predefined companies.

Search broadly across:

- Company career sites
- Greenhouse
- Lever
- Workday
- Ashby
- SmartRecruiters
- LinkedIn
- Indeed
- BuiltIn
- Wellfound
- YC Jobs
- Startup career pages
- University spin-outs
- AI biotech startups
- Medical AI companies
- Genomics companies
- Digital manufacturing companies

The company database is dynamic. Every newly discovered high-quality company should be added to `companies/company_intelligence.csv`.

## Source Priority

LinkedIn is a radar, not the source of truth.

Use source trust in this order:

1. Company career page
2. Greenhouse
3. Lever
4. Workday
5. Ashby
6. SmartRecruiters
7. LinkedIn
8. Indeed, BuiltIn, Wellfound, YC Jobs, and other aggregators

If LinkedIn discovers a job, verify it against the company career page or official ATS whenever possible. If official and aggregator information conflict, use the official JD.

## Collection Rules

- Do not filter by title alone.
- Discover jobs by job function, not title.
- Preserve the full job description whenever possible.
- Extract structured fields into `tracker/jobs.csv`.
- Save raw and normalized JD files under `jobs/raw/` and `jobs/normalized/` when a future task enables file-based JD storage.
- Mark new, updated, closed, and duplicate jobs.
- Use a stable external job ID when available.
- Deduplicate across LinkedIn, official career pages, and ATS platforms.
- Do not scrape behind login walls without explicit user direction.
- Do not write browser automation or crawler code unless a future task explicitly requests it.

## First-Pass Filters

Remove or downgrade jobs that clearly contain:

- US citizen only
- Green card only
- No current or future sponsorship
- Wet lab only
- LC-MS
- Protein purification
- Animal work
- Pure publication-driven research
- Principal, Director, Staff, or other senior-only requirements
- PhD mandatory when the JD treats PhD as a hard requirement

Keep jobs with unknown sponsorship if they otherwise match.

## Job Functions To Discover

- Technical Applications
- Scientific Support
- Scientific Solutions
- Implementation
- Customer Success
- Applied AI
- Machine Learning
- Foundation Models
- LLM
- Scientific AI
- Scientific Software
- Platform Engineering
- Workflow Engineering
- Pipeline Engineering
- Clinical Genomics
- Variant Interpretation
- Scientific Product
- Technical Product
- Product Operations
- Digital Manufacturing
- Automation
- MES
- Scientific Computing
- Bio Data Science
- Computational Biology
- Medical AI
- Drug Discovery AI
- Protein AI

## Required Fields

- Company
- External Job ID
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
- Official URL
- LinkedIn URL
- Source Type
- Source Trust
- JD File
- Status
- Date Found
- Date Updated
- Notes

## Output

Update `tracker/jobs.csv` and summarize:

- Sources scanned
- Jobs found
- New jobs
- Updated jobs
- Closed jobs
- Duplicates removed
- Official JDs verified
- New companies discovered
- Jobs needing GPT analysis
