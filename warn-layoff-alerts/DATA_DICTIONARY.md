# Data dictionary: WARN layoff notices (7 states)

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/warn-layoff-alerts/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/warn-layoff-alerts/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:21:36Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/warn-layoff-alerts
Data origin: State WARN notice postings (TX, CA, WA, OR, MD, VA, NC workforce agencies)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `company` | string | Employer named in the WARN notice. |
| `city` | string | City name. |
| `county` | string | County name. |
| `state` | string | US state or territory (two-letter code). |
| `layoff_count` | integer | Number of workers affected (integer). |
| `notice_date` | date | Date on the notice (ISO date). |
| `layoff_date` | date | First effective layoff or closure date (ISO date). |
| `received_date` | date | Date the state agency received the notice. |
| `wda` | string | Workforce Development Area, where the state reports it. |
| `source_state` | string | State agency the notice came from. |
| `layoff_type` | string | Closure, layoff, permanent or temporary, as labelled by the state. |
| `source_url` | url | State dataset or page the row came from. |
| `enriched` | boolean | True when the row was enriched with employer domain data. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
