# Workday Jobs Scraper: Any Career Site, 165+ Companies $1/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **workday-jobs-scraper**.

Actor page: https://apify.com/transparent_meteorite/workday-jobs-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Workday jobs from 165+ verified employers or any myworkdayjobs.com site, verified by 64 passing tests. Keyword, location and posted-date filters, full descriptions, salary ranges, remote/hybrid, and only-new-jobs delta mode. $1 per 1,000 jobs.

## Columns in sample.csv
`company`, `title`, `location`, `locations`, `locationsText`, `country`, `remoteType`, `timeType`, `postedOn`, `postedOnIsEstimate`, `postedOnText`, `postedDaysAgo`, `jobReqId`, `url`, `hiringEntity`, `careerSiteUrl`, `workdayTenant`, `workdaySite`, `jobId`, `scrapedAt`

## Data source and privacy
Public Workday career sites.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
