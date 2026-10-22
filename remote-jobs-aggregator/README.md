# Remote Jobs Aggregator: 6 Job Boards, Deduped, Salary Parsed

Free sample output (10 rows, `sample.csv`) from the Apify actor **remote-jobs-aggregator**.

Actor page: https://apify.com/transparent_meteorite/remote-jobs-aggregator

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Remote jobs from 6 official job-board APIs (Remotive, Remote OK, We Work Remotely, Himalayas, Jobicy, Arbeitnow) in one deduped dataset. Parsed salary with yearly USD, category, seniority, region and timezone filters, monitor mode that charges only new jobs. No login, no proxy.

## Columns in sample.csv
`id`, `title`, `company`, `companyUrl`, `source`, `sourceName`, `sourceUrl`, `applyUrl`, `postedAt`, `category`, `tags`, `jobType`, `experienceLevel`, `salaryMin`, `salaryMax`, `salaryCurrency`, `salaryPeriod`, `salaryText`, `salaryYearlyMaxUsd`, `locationRestriction`, `regions`, `timezones`, `dedupKey`, `alsoListedOn`, `sourcesCount`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
