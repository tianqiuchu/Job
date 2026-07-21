# Project Lighthouse

Project Lighthouse is a long-term AI-assisted career operating system for Chenshuo Cui.

It is not a job scraper. It is a career decision system that helps collect opportunities, preserve job descriptions, analyze career fit, maintain application materials, and track long-term growth toward technical leadership.

## Core Principle

Don't build a job search tool. Build a career decision system. Every design decision should support long-term career growth rather than maximizing the number of applications.

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
- Job collection workflows
- Parsing and normalization
- Tracker updates
- Report generation infrastructure
- Maintainable scripts and documentation

Codex should not make final career judgments. Career scoring, prioritization, and resume strategy remain GPT-first.

## Candidate Positioning

Biomedical engineer with expertise in AI, machine learning, and biological data science, experienced in translating complex scientific and technical challenges into practical solutions. Strong background in genomics, computational biology, and data engineering, with ability to work across research, engineering, customer, and stakeholder teams. Motivated by solving real-world problems rather than conducting isolated research, with a long-term goal of leading multidisciplinary teams that bridge science, technology, products, and customers.

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

tracker/
  jobs.csv
  applied.csv
  blacklist.csv

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
