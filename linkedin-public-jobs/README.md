# LinkedIn Public Jobs Scraper (no login) | Salary & Level

Free sample output (4 rows, `sample.csv`) from the Apify actor **linkedin-public-jobs**.

Actor page: https://apify.com/transparent_meteorite/linkedin-public-jobs

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
28 filled fields per LinkedIn job vs 23 in our side-by-side test, at a lower price per job. Search public guest job listings with no login or cookies: keywords, location, date, remote/hybrid, level, type, company. Title, company, salary, seniority, industries, full description. Deduped.

## Columns in sample.csv
`jobId`, `title`, `company`, `companyUrl`, `location`, `postedAt`, `applicantsText`, `salaryText`, `seniority`, `employmentType`, `industries`, `workplaceType`, `applyType`, `jobUrl`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
