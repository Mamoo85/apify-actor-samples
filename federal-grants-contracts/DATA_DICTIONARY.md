# Data dictionary: Federal grants and contract awards

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/federal-grants-contracts/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/federal-grants-contracts/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:32:47Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/federal-grants-contracts
Data origin: Grants.gov and USAspending.gov (U.S. federal open data)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `source` | string | grants.gov or usaspending.gov. |
| `recordType` | string | opportunity (open grant) or award (contract award). |
| `opportunityNumber` | string | Grants.gov opportunity number. |
| `title` | string | Title or headline of the record. |
| `description` | string | Free-text description from the source (truncated to 300 characters). |
| `agency` | string | Top-level agency. |
| `subAgency` | string | Sub-agency or office. |
| `agencyCode` | string | Agency code. |
| `status` | string | Status of the record at the source. |
| `postedDate` | date | Date the opportunity was posted. |
| `closeDate` | date | Application close date. |
| `daysUntilClose` | integer | Days from retrieval to close date. |
| `archiveDate` | date | Date the opportunity is archived. |
| `amountCeiling` | integer | Maximum award in USD (opportunities). |
| `amountFloor` | integer | Minimum award in USD (opportunities). |
| `estimatedFunding` | integer | Total estimated funding in USD. |
| `numberOfAwards` | integer | Expected number of awards. |
| `costSharing` | boolean | True when cost sharing is required. |
| `assistanceListings` | json-string | JSON list of Assistance Listing numbers. |
| `fundingInstruments` | json-string | JSON list: grant, cooperative agreement and so on. |
| `fundingCategories` | json-string | JSON list of funding categories. |
| `eligibleApplicants` | json-string | JSON list of eligible applicant types. |
| `url` | url | Link to the record at the source. |
| `apiReference` | url | API call that returns the full record. |
| `matchedKeyword` | string | Search keyword that surfaced the row. |
| `retrievedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
