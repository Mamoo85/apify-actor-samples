# Career Site Jobs API: Greenhouse, Lever, Ashby & more | $2/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **ats-open-roles**.

Actor page: https://apify.com/transparent_meteorite/ats-open-roles

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Career-site jobs at $0.002 each, with seniority, department and ready-made company presets. Open roles from the public job-board APIs of Greenhouse, Lever, Ashby, Workable, SmartRecruiters and Recruitee plus schema.org pages. One clean schema with salary, remote flag, apply URL.

## Columns in sample.csv
`company`, `companySlug`, `ats`, `jobId`, `title`, `department`, `location`, `postedAt`, `updatedAt`, `applyUrl`, `jobUrl`, `salaryMin`, `salaryMax`, `salaryCurrency`, `salaryPeriod`, `sourceUrl`, `seniority`, `scrapedAt`

## Data source and privacy
Public job boards of Greenhouse, Lever, Ashby and similar.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
