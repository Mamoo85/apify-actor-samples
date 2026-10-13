# Data dictionary: City building permits (Chicago, Seattle, Austin)

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/building-permits-leads/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/building-permits-leads/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:32:31Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/building-permits-leads
Data origin: City open-data portals (Chicago, Seattle, Austin)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `permitId` | string | Permit identifier at the city. |
| `recordType` | string | permit or violation. |
| `cityCode` | string | Short city code used by the actor. |
| `city` | string | City name. |
| `state` | string | US state or territory (two-letter code). |
| `permitType` | string | Permit type. |
| `workClass` | string | Work class, for example new or reroof. |
| `description` | string | Free-text description from the source (truncated to 300 characters). |
| `status` | string | Status of the record at the source. |
| `applicationDate` | date | Application date. |
| `issueDate` | date | Issue date. |
| `recordDate` | date | Record date used for freshness filtering. |
| `valuation` | integer | Declared project valuation in USD. |
| `latitude` | number | Latitude rounded to 2 decimals (about 1 km). |
| `longitude` | number | Longitude rounded to 2 decimals (about 1 km). |
| `contractorBusiness` | string | Contractor business name as filed. |
| `sourceUrl` | url | URL of the source feed or portal page the row came from. |
| `sourcePortal` | string | City open-data portal and dataset id. |
| `scrapedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
