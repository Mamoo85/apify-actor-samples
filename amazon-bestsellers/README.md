# Amazon Best Sellers Scraper - Top 100 Ranks, 21 Countries

Free sample output (10 rows, `sample.csv`) from the Apify actor **amazon-bestsellers**.

Actor page: https://apify.com/transparent_meteorite/amazon-bestsellers

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Amazon Best Sellers, New Releases, Movers & Shakers, Most Wished For and Gift Ideas ranks in 21 countries: rank, ASIN, title, price, rating, reviews, images, category path. Subcategory crawl, rank-change monitor, optional product details.

## Columns in sample.csv
`rank`, `asin`, `title`, `url`, `price`, `priceMax`, `currency`, `stars`, `reviewsCount`, `thumbnail`, `highResImage`, `listType`, `listName`, `category`, `categoryPath`, `categorySlug`, `categoryId`, `categoryUrl`, `countryCode`, `page`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
