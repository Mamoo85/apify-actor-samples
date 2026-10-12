# Building Permits Leads: US City Permits and Violations, $1.5/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **building-permits-leads**.

Actor page: https://apify.com/transparent_meteorite/building-permits-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
New building permits and code violations from official city open-data portals (Chicago, NYC, LA, SF, Seattle, Austin, Baton Rouge, Montgomery Co. MD, Cincinnati): type, status, dates, valuation, property address, contractor business if published, source link. Delta mode. $0.0015 per record.

## Columns in sample.csv
`permitId`, `recordType`, `cityCode`, `city`, `state`, `permitType`, `description`, `status`, `applicationDate`, `issueDate`, `recordDate`, `valuation`, `propertyAddress`, `latitude`, `longitude`, `contractorBusiness`, `sourceUrl`, `sourcePortal`, `scrapedAt`

## Data source and privacy
City open-data permit portals (public records).
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
