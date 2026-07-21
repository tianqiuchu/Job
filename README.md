# Project Lighthouse

Project Lighthouse is a long-term AI-assisted career intelligence platform for Chenshuo Cui.

It is not a job scraper. It is not an ATS optimizer. It is a career decision system that monitors the US Bio + AI + Data job market, preserves official job descriptions, analyzes career fit, maintains application materials, and tracks long-term growth toward technical leadership.

## Core Principle

Don't build a job search tool. Build a career decision system. Every design decision should support long-term career growth rather than maximizing the number of applications.

The search space is not a short predefined company list. The search space is the full available US Bio + AI + Data job universe. Company lists are dynamic intelligence assets, not the boundary of the search.

## Roles

GPT acts as the career strategist:

- Career strategy
- JD analysis
- Lighthouse scoring
- Resume, CV, and cover letter strategy
- Interview preparation
- Weekly career and market reports

Codex acts as the software engineer:

- Repository structure
- Databases and CSV templates
- Job-universe collection workflows
- Parsing and normalization
- Tracker updates
- Report generation infrastructure
- Maintainable scripts and documentation

Codex should not make final career judgments. Career scoring, prioritization, and resume strategy remain GPT-first.

## Candidate Positioning

Biomedical engineer with expertise in AI, machine learning, and biological data science, experienced in translating complex scientific and technical challenges into practical solutions. Strong background in genomics, computational biology, and data engineering, with ability to work across research, engineering, customer, and stakeholder teams. Motivated by solving real-world problems rather than conducting isolated research, with a long-term goal of leading multidisciplinary teams that bridge science, technology, products, and customers.

The candidate is not trying to compete with PhD researchers on publication depth. The candidate's strongest value is solving complex problems, organizing work across teams, understanding customers and stakeholders, and connecting biology, AI/data, engineering, and product delivery.

## Search Philosophy

LinkedIn is a radar, not the source of truth.

Project Lighthouse uses LinkedIn, Indeed, BuiltIn, Wellfound, YC Jobs, and similar platforms for discovery. Every promising job should be verified against an official source whenever possible:

1. Company career page
2. Greenhouse
3. Lever
4. Workday
5. Ashby
6. SmartRecruiters
7. LinkedIn or other aggregators only when no official source is available

If LinkedIn and the official JD disagree, trust the official JD.

Title is only a discovery signal. The decision must come from the full JD.

## Priority Career Tracks

1. Technical Applications, Scientific Support, Scientific Solutions, Implementation, Customer Success
2. AI for Biology, Applied AI, Machine Learning, Foundation Models, LLM, Scientific AI
3. Scientific Software, Scientific Platform, Scientific Cloud, Workflow, Pipeline
4. Clinical Genomics, Variant Interpretation, Clinical Bioinformatics, Reporting, Curation
5. Scientific Product, Product Specialist, Associate Product Manager, Product Operations
6. Digital Manufacturing, Manufacturing Systems, Automation, MES, Process Analytics, MSAT

## Repository Structure

```text
companies/
  tier_s.csv
  tier_a.csv
  company_intelligence.csv

sources/
  job_sources.csv

tracker/
  jobs.csv
  applied.csv
  blacklist.csv

jobs/
  raw/
  normalized/

prompts/
  codex_search.md
  jd_analysis.md
  resume_strategy.md

reports/
  daily/
  weekly/

resume/
  applications/
  solutions/
  clinical/
  product/
  manufacturing/
  ai/

docs/
  project_lighthouse_prd.md
  candidate_profile.md
  career_tracks.md
  scoring_model.md
  source_strategy.md
  workflow.md

scripts/
```

## Lighthouse Score

Lighthouse Score is not an ATS score. It reflects long-term career fit.

| Dimension | Weight |
| --- | ---: |
| Problem Solving | 25 |
| Cross Functional | 15 |
| Customer Exposure | 15 |
| Leadership Growth | 15 |
| AI/Data | 10 |
| Biology | 10 |
| Technical Skills | 10 |

## Current Phase

Phase 1 initializes the repository, templates, and documentation.

No crawler is implemented in this phase. No LinkedIn automation is implemented in this phase. Job collection and parsing will be added in later tasks.

The current baseline is Project Lighthouse V2: the market is treated as a job universe, and the company database is treated as dynamic company intelligence.
