# Data dictionary: Open jobs from Greenhouse, Lever and Ashby boards

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/ats-open-roles/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/ats-open-roles/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:21:57Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/ats-open-roles
Data origin: Public Greenhouse, Lever and Ashby job-board APIs
License: Free to use, source terms apply. These are facts about publicly posted items (jobs, stories, packages). Free to use for analysis; the text of postings belongs to the original publishers, so check the source terms before republishing it.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `company` | string | Company name. |
| `companySlug` | string | Company slug on the ATS board. |
| `ats` | string | ATS platform: greenhouse, lever or ashby. |
| `jobId` | string | Job identifier at the source platform. |
| `title` | string | Title or headline of the record. |
| `department` | string | Department or team. |
| `location` | string | Location text as published. |
| `remote` | boolean | True when the posting is flagged remote. |
| `workplaceType` | string | onsite, hybrid or remote where given. |
| `employmentType` | string | Employment type such as FULL_TIME. |
| `postedAt` | datetime | Posting time (UTC). |
| `updatedAt` | datetime | Last update time (UTC). |
| `applyUrl` | url | Application link. |
| `jobUrl` | url | Public job page link. |
| `salaryMin` | integer | Lower end of the posted salary range (number, in salaryCurrency per salaryPeriod). Empty when not disclosed. |
| `salaryMax` | integer | Upper end of the posted salary range. Empty when not disclosed. |
| `salaryCurrency` | string | ISO currency code of the salary range. |
| `salaryPeriod` | string | Period the salary range covers (for example year or hour). |
| `descriptionText` | string | Start of the job description (truncated to 300 characters). |
| `sourceUrl` | url | URL of the source feed or portal page the row came from. |
| `seniority` | string | Seniority level inferred from the title. |
| `scrapedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
