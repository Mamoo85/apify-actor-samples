# Data dictionary: SEC Form D private placement filings

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/sec-form-d-funding-leads/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/sec-form-d-funding-leads/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:21:54Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/sec-form-d-funding-leads
Data origin: SEC EDGAR Form D filings
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `accessionNumber` | string | EDGAR accession number. |
| `filingDate` | date | Filing date (ISO). |
| `formType` | string | D or D/A. |
| `isAmendment` | boolean | True for amended filings. |
| `cik` | string | SEC Central Index Key of the issuer. |
| `entityName` | string | Issuer name. |
| `entityType` | string | Legal entity type. |
| `jurisdictionOfIncorporation` | string | Jurisdiction of incorporation. |
| `yearOfIncorporation` | integer | Year of incorporation. |
| `businessCity` | string | Issuer business city. |
| `issuerState` | string | Issuer business state. |
| `industryGroup` | string | Industry group selected on the form. |
| `revenueRange` | string | Revenue range selected on the form. |
| `federalExemptions` | json-string | JSON list of federal exemptions claimed (for example 06b is Rule 506(b)). |
| `dateOfFirstSale` | date | Date of first sale. |
| `firstSaleYetToOccur` | boolean | True when no sale has occurred yet. |
| `totalOfferingAmount` | integer | Total offering amount in USD. |
| `totalAmountSold` | integer | Amount sold so far in USD. |
| `totalRemaining` | integer | Amount remaining in USD. |
| `offeringIsIndefinite` | boolean | True when the offering amount is indefinite. |
| `minimumInvestment` | integer | Minimum investment accepted in USD. |
| `numberOfInvestors` | integer | Investors who have invested. |
| `salesCommissionsUsd` | integer | Sales commissions in USD. |
| `findersFeesUsd` | integer | Finders fees in USD. |
| `filingUrl` | url | Link to the filing index on sec.gov. |
| `primaryDocUrl` | url | Link to the primary document on sec.gov. |
| `scrapedAt` | datetime | UTC timestamp when the actor fetched the row. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
