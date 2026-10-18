# Businesses Without Websites Leads Finder - $4/1K

Free sample output (4 rows, `sample.csv`) from the Apify actor **website-redesign-leads**.

Actor page: https://apify.com/transparent_meteorite/website-redesign-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Find local businesses on Google Maps with no website or a weak one (no HTTPS, not mobile-friendly, outdated, broken, parked, Facebook-only). Each lead gets a 0-100 opportunity score with plain-English reasons, phone and address. No login. $4 per 1,000 leads.

## Columns in sample.csv
`name`, `opportunityScore`, `leadTier`, `reasons`, `websiteStatus`, `category`, `city`, `state`, `rating`, `reviewsCount`, `claimedByOwner`, `mapsUrl`, `searchString`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
