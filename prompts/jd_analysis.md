# JD Analysis Prompt

Use this prompt when GPT analyzes a job description after Codex has collected it.

## Core Rule

Title is only a discovery signal. The decision must be based on the full JD.

Do not use keyword matching as the final decision method.

If a job was discovered through LinkedIn or another aggregator, analyze the official JD whenever available. LinkedIn is a radar. Official company or ATS pages are the source of truth.

## Candidate Lens

The candidate is strongest in:

- Problem solving
- Cross-functional communication
- Customer and stakeholder understanding
- Scientific understanding
- Bioinformatics, genomics, AI/ML, and biological data science
- Engineering thinking
- Long-term leadership potential

The candidate is not trying to compete with PhD candidates in pure research depth. Prioritize roles that develop technical leadership, product judgment, customer exposure, and ownership.

## Analysis Template

For each JD, produce:

1. Actual work breakdown
   - What will the person really do every week?
   - Approximate percentage split across customer, technical, product, research, data, operations, and documentation work.

2. Career track
   - Technical Applications
   - Scientific Support
   - Solutions / Implementation
   - AI for Biology
   - Scientific Software / Platform
   - Clinical Genomics
   - Product
   - Digital Manufacturing
   - Medical AI
   - Bio Data Science
   - Validation / Quality
   - Other

3. Must-have requirements
   - Separate hard requirements from nice-to-have requirements.

4. Candidate fit
   - Existing strengths
   - Transferable experience
   - Missing skills
   - Gaps that can be filled quickly
   - Gaps that are not worth filling

5. Lighthouse Score
   - Problem Solving: 25
   - Cross Functional: 15
   - Customer Exposure: 15
   - Leadership Growth: 15
   - AI/Data: 10
   - Biology: 10
   - Technical Skills: 10

6. Recommendation
   - Tier S: must apply
   - Tier A: strong apply
   - Tier B: strategic reach
   - Tier C: watchlist
   - Pass

7. Resume direction
   - Which resume library version to use
   - Which bullets should be emphasized
   - Whether a cover letter is useful

8. Leadership question
   - If the candidate works here for three years, will this role move him closer to technical leader, product leader, program leader, or director?

9. Source quality
   - Official JD
   - Verified from aggregator
   - Aggregator only
   - Needs source verification
