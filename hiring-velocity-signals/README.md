# Hiring Velocity Signals: Company Hiring Trends from Jobs

Free sample output (5 rows, `sample.csv`) from the Apify actor **hiring-velocity-signals**.

Actor page: https://apify.com/transparent_meteorite/hiring-velocity-signals

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
One row per company: open roles, new roles in 7/30 days, hiring trend vs the prior window, department and seniority mix, new cities and regions, and a 0-100 hiring score. Reads public ATS boards (Greenhouse, Lever, Ashby, Workable, SmartRecruiters, Recruitee) and LinkedIn guest job search. No login.

## Columns in sample.csv
`company`, `status`, `atsVendor`, `careersUrl`, `signal`, `openRoles`, `newRoles7d`, `newRoles30d`, `velocityPerWeek`, `trendPct`, `trend`, `countsAreLowerBound`, `hiringScore`, `lookbackDays`, `checkedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
