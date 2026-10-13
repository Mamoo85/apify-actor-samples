# Data dictionary: Jobs from Workday career sites

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/workday-jobs-scraper/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/workday-jobs-scraper/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:32:48Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/workday-jobs-scraper
Data origin: Public Workday career-site job feeds
License: Free to use, source terms apply. These are facts about publicly posted items (jobs, stories, packages). Free to use for analysis; the text of postings belongs to the original publishers, so check the source terms before republishing it.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `company` | string | Employer name. |
| `title` | string | Title or headline of the record. |
| `location` | string | Location text as published. |
| `locations` | json-string | JSON list of locations. |
| `locationsText` | string | Locations joined as text. |
| `country` | string | Country. |
| `remoteType` | string | Remote or onsite type as given by Workday. |
| `timeType` | string | Full time or part time. |
| `postedOn` | date | Posting date (ISO). Estimated when postedOnIsEstimate is true. |
| `postedOnIsEstimate` | boolean | True when the date was computed from relative text. |
| `postedOnText` | string | Posting age as shown on the site. |
| `postedDaysAgo` | integer | Days since posting. |
| `jobReqId` | string | Requisition id. |
| `url` | url | Link to the record at the source. |
| `salaryText` | string | Salary text as published. |
| `salaryMin` | integer | Lower end of the posted salary range (number, in salaryCurrency per salaryPeriod). Empty when not disclosed. |
| `salaryMax` | integer | Upper end of the posted salary range. Empty when not disclosed. |
| `salaryCurrency` | string | ISO currency code of the salary range. |
| `salaryPeriod` | string | Period the salary range covers (for example year or hour). |
| `hiringEntity` | string | Hiring legal entity. |
| `careerSiteUrl` | url | Career site URL. |
| `workdayTenant` | string | Workday tenant name. |
| `workdaySite` | string | Workday site name. |
| `jobId` | string | Job identifier at the source platform. |
| `scrapedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
