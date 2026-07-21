# Source Strategy

## Core Rule

LinkedIn is a radar, not the source of truth.

Project Lighthouse should use LinkedIn and other aggregators to discover jobs, companies, and market trends. Final job analysis should use official company or ATS job descriptions whenever possible.

## Source Trust Ranking

1. Company career page
2. Greenhouse
3. Lever
4. Workday
5. Ashby
6. SmartRecruiters
7. LinkedIn
8. Indeed, BuiltIn, Wellfound, YC Jobs, and other aggregators

## Verification Workflow

1. Discover a job from any source.
2. Identify company, title, location, and possible external job ID.
3. Search for the official company or ATS version.
4. Preserve the official JD as the primary record.
5. Keep aggregator URLs as discovery metadata.
6. Deduplicate across sources.
7. Mark unresolved cases as `Needs Source Verification`.

## Why This Matters

LinkedIn postings can be duplicated, stale, truncated, or missing sponsorship and salary details. Official JDs are more reliable for career scoring, resume tailoring, and application decisions.
