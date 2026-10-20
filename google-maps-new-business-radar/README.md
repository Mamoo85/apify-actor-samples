# New Business Leads from Google Maps - $3/1K

Free sample output (5 rows, `sample.csv`) from the Apify actor **google-maps-new-business-radar**.

Actor page: https://apify.com/transparent_meteorite/google-maps-new-business-radar

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Find newly opened businesses on Google Maps in any city: no or few reviews, recent first review, no photos or hours yet. Newness score 0-100 with reasons, phone, website. Monitor mode returns only places new since the last run. No login, no API key. $3 per 1,000 new places.

## Columns in sample.csv
`placeId`, `name`, `category`, `city`, `state`, `postalCode`, `countryCode`, `rating`, `reviewsCount`, `photosCount`, `newnessScore`, `newnessSignals`, `signalCodes`, `hasOpeningHours`, `website`, `mapsUrl`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
