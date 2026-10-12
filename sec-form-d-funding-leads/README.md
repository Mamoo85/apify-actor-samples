# SEC Form D Funding Leads: Recently Funded Startups, $2.50/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **sec-form-d-funding-leads**.

Actor page: https://apify.com/transparent_meteorite/sec-form-d-funding-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
SEC Form D funding leads at $0.0025 per filing, verified by 102 passing tests. Newly filed Form D notices from official EDGAR: issuer, industry, offering size, amount sold, investors, first-sale date, officers. Filter by industry, state, size; exclude pooled funds; dedupe. No login.

## Columns in sample.csv
`accessionNumber`, `filingDate`, `formType`, `isAmendment`, `cik`, `entityName`, `entityType`, `jurisdictionOfIncorporation`, `yearOfIncorporation`, `businessStreet`, `businessCity`, `issuerState`, `businessZip`, `businessPhone`, `industryGroup`, `revenueRange`, `federalExemptions`, `dateOfFirstSale`, `firstSaleYetToOccur`, `totalOfferingAmount`, `totalAmountSold`, `totalRemaining`, `offeringIsIndefinite`, `minimumInvestment`, `numberOfInvestors`, `salesCommissionsUsd`, `findersFeesUsd`, `filingUrl`, `primaryDocUrl`, `scrapedAt`

## Data source and privacy
SEC EDGAR Form D filings (US public domain); phones masked, related persons removed.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
