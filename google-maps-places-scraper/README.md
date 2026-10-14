# Google Maps Scraper: Places, Phones, Emails $1.50/1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **google-maps-places-scraper**.

Actor page: https://apify.com/transparent_meteorite/google-maps-places-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape Google Maps places by keyword and location: name, address, phone, website, rating, review count, hours, categories, coordinates, place URL. Optional website emails and socials, up to 5 reviews. No login. $1.50 per 1,000 places.

## Columns in sample.csv
`title`, `categoryName`, `address`, `city`, `state`, `totalScore`, `reviewsCount`, `priceLevel`, `openNowText`, `permanentlyClosed`, `temporarilyClosed`, `claimedByOwner`, `description`, `placeId`, `url`, `searchString`, `rank`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
