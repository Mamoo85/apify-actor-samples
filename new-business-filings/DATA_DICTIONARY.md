# Data dictionary: New business entity filings (CO, NY, OR, CT)

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/new-business-filings/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/new-business-filings/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:21:48Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/new-business-filings
Data origin: State open-data portals (Colorado, New York, Oregon, Connecticut)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `entityName` | string | Registered entity name. |
| `state` | string | US state or territory (two-letter code). |
| `stateName` | string | Full state name. |
| `filingDate` | date | Filing or formation date (ISO). |
| `entityType` | string | Normalised entity type (LLC, Corporation and so on). |
| `entityTypeRaw` | string | Entity type as published by the state. |
| `status` | string | Status such as Good Standing. |
| `jurisdiction` | string | Jurisdiction of formation. |
| `county` | string | County name. |
| `naicsCode` | string | Industry text or NAICS value when the state provides it. |
| `entityId` | string | State entity identifier. |
| `sourceUrl` | url | URL of the source feed or portal page the row came from. |
| `sourcePortal` | url | Open-data portal the row came from. |
| `scrapedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
