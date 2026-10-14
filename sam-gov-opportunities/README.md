# SAM.gov Scraper: Federal Contract Opportunities API

Free sample output (10 rows, `sample.csv`) from the Apify actor **sam-gov-opportunities**.

Actor page: https://apify.com/transparent_meteorite/sam-gov-opportunities

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Get open federal contracts and government bids from SAM.gov: solicitations, RFPs, RFQs, sources sought and award notices with contracting officer email and phone, NAICS, PSC, set-aside, deadlines, full text and attachments. No API key needed; daily new-only monitor mode.

## Columns in sample.csv
`noticeId`, `title`, `solicitationNumber`, `noticeType`, `postedDate`, `responseDeadline`, `department`, `office`, `naicsCode`, `pscCode`, `setAside`, `samUrl`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
