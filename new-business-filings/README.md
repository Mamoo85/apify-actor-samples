# New Business Filings: New LLCs and Corporations, $4/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **new-business-filings**.

Actor page: https://apify.com/transparent_meteorite/new-business-filings

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
New LLCs and corporations from official state open data (CO, NY, OR, CT), verified by 57 passing tests. Name, filing date, type, status, registered agent, public address, source link. Filter by state, type, keyword; deduped across runs. No login. $0.004 per filing.

## Columns in sample.csv
`entityName`, `state`, `stateName`, `filingDate`, `entityType`, `entityTypeRaw`, `status`, `address`, `addressType`, `jurisdiction`, `entityId`, `sourceUrl`, `sourcePortal`, `scrapedAt`

## Data source and privacy
State business-registry open data; registered-agent names removed.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
