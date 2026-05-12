# 📊 Product Retention & Funnel Analysis

> Which user cohorts drop off fastest — and what does the data say about fixing it?

![Status](https://img.shields.io/badge/Status-In_Progress-orange)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

## Business Problem
Most apps lose 60–80% of new users within the first week.
Without understanding *where* users drop off and *which cohorts* retain best,
product teams are optimising blind — spending budget on acquisition instead of fixing leaks.

## Objective
- Map the full user funnel (view → signup → activate → purchase) and calculate drop-off % at each stage
- Build day-1, day-7, day-30 cohort retention curves by signup week
- Run an A/B hypothesis test comparing two onboarding flows
- Publish a live Tableau dashboard with funnel + cohort heatmap + KPI cards

## Dataset
App user behaviour / event-level dataset — Kaggle  
~200,000+ event records | Columns: `user_id`, `event_date`, `event_name`, `session_id`

## Tools
SQL (PostgreSQL) · Python (Pandas, Scipy, Seaborn, Matplotlib) · Tableau Public

## Project Structure
```
product-retention-analysis/
├── data/               # Raw & cleaned CSVs (not tracked in git)
├── notebooks/          # Jupyter notebooks — EDA, funnel, cohort, A/B test
├── sql/                # SQL queries — active users, funnels, session analysis
├── dashboard/          # Tableau workbook + screenshot exports
└── requirements.txt    # Python dependencies
```

## Week-by-Week Build Plan

| Week | Focus | Deliverable |
|------|-------|-------------|
| 1 | Explore + SQL Setup | Schema review, load to PostgreSQL, 5 core queries |
| 2 | Funnel Analysis | Drop-off % per stage in SQL + Python |
| 3 | Cohort Retention | Day-1/7/30 curves + cohort heatmap (Seaborn) |
| 4 | A/B Test | Hypothesis test, p-value, written conclusion |
| 5 | Tableau Dashboard | Live published dashboard with 4 chart types |
| 6 | README + Polish | Business findings, 3 recommendations, clean notebooks |

## Key Questions This Project Answers
1. At which funnel stage do we lose the most users?
2. Do users who sign up on weekends retain differently than weekday signups?
3. Is the difference in onboarding flow A vs B statistically significant?
4. Which signup cohort has the best 30-day retention?

## Status
🔄 Analysis in progress — findings updated weekly

---
*Part of my DA portfolio → [github.com/SAFARKHAN-S](https://github.com/SAFARKHAN-S)*
