# Federal Grants & Contracts Finder: Grants.gov + USAspending

Free sample output (12 rows, `sample.csv`) from the Apify actor **federal-grants-contracts**.

Actor page: https://apify.com/transparent_meteorite/federal-grants-contracts

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Open and forecasted federal grant opportunities from Grants.gov plus contract and grant awards from USAspending.gov, in one unified schema: deadlines, ceilings, amounts, agency, NAICS/PSC, recipient, and a link to the official record. No API key. $0.002 per opportunity, $0.0015 per award.

## Columns in sample.csv
`source`, `recordType`, `opportunityNumber`, `title`, `agency`, `subAgency`, `agencyCode`, `status`, `postedDate`, `closeDate`, `daysUntilClose`, `assistanceListings`, `url`, `apiReference`, `matchedKeyword`, `retrievedAt`

## Data source and privacy
Grants.gov and USAspending.gov (US public domain).
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
