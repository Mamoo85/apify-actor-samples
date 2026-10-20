# Google Maps Listing Monitor: Rating, Hours, Closure Alerts

Free sample output (10 rows, `sample.csv`) from the Apify actor **maps-listing-change-monitor**.

Actor page: https://apify.com/transparent_meteorite/maps-listing-change-monitor

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Track a fixed set of Google Maps listings (clients, competitors or a category search) and get one row per change: closed, reopened, rating drop, review spike or stall, hours, phone, website or category changed, listing gone. Run 1 records a health baseline. No login.

## Columns in sample.csv
`rowType`, `eventType`, `severity`, `summary`, `setName`, `title`, `categoryName`, `status`, `rating`, `reviewsCount`, `field`, `oldValue`, `newValue`, `ratingDelta`, `reviewsDelta`, `city`, `state`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
