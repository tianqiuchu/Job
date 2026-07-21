# Project Lighthouse V2 PRD

## Purpose

Project Lighthouse is a long-term career intelligence platform for Chenshuo Cui.

It should continuously monitor the US Bio + AI + Data job market, preserve official job descriptions, analyze fit, manage application materials, and track the user's movement toward technical leadership.

This project is not a job scraper. This project is not an ATS optimizer. Job collection is only one small part of the system.

## Product Philosophy

The system optimizes for:

- Long-term career growth
- Leadership potential
- Problem solving
- Cross-functional work
- Customer exposure
- Business exposure
- Technical growth

The system does not optimize purely for:

- Number of applications
- ATS score alone
- Job title keyword matches

## V2 Architecture Change

The V1 idea of scanning a short target-company list is not sufficient.

The V2 search space is:

> All available US Bio + AI + Data jobs.

The company database is dynamic company intelligence, not a static search boundary. Every new high-quality company discovered during scans should be added to company intelligence.

## Search Sources

Use all relevant job sources:

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
- Manufacturing and digital manufacturing companies

## Source Trust

LinkedIn is a radar, not the source of truth.

Source trust order:

1. Company career page
2. Official ATS pages such as Greenhouse, Lever, Workday, Ashby, SmartRecruiters
3. LinkedIn
4. Other aggregators

If LinkedIn and the official JD conflict, trust the official JD.

## Daily Pipeline

1. Scan the job universe.
2. Apply first-pass filters.
3. Deduplicate jobs across sources.
4. Verify promising jobs against official sources.
5. Preserve raw and normalized JDs.
6. Produce a list of jobs needing GPT analysis.
7. GPT deeply reads JDs and assigns Lighthouse Score.
8. Generate Top 20 and application list.

## First-Pass Filters

Remove or downgrade:

- US citizen only
- Green card only
- No current or future sponsorship
- Wet lab only
- LC-MS
- Protein purification
- Animal work
- Pure publication-driven research
- Principal, Director, Staff, or senior-only roles
- PhD mandatory roles where PhD is a hard requirement

## Current Repository Scope

The repository stores the operating system for this workflow.

Included:

- Directory structure
- CSV templates
- Prompt templates
- Documentation

Excluded:

- Crawlers
- LinkedIn scraping
- Browser automation
- Scheduled jobs
- Database migrations
- Dashboard UI

## Future Tasks

Task 002: Upgrade repository templates to V2 job-universe architecture.

Task 003: Build source registry and dynamic company intelligence schema.

Task 004: Build job collection workflow.

Task 005: Build JD parser.

Task 006: Generate daily reports.

Task 007: Add application tracker workflow.

Task 008: Generate weekly market analysis.

Task 009: Add resume and cover letter generation workflow.
