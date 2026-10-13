# Amazon Product Search: prices, ratings, ASINs

Free sample output (4 rows, `sample.csv`) from the Apify actor **amazon-product-search**.

Actor page: https://apify.com/transparent_meteorite/amazon-product-search

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Amazon product data at $0.004 per product, 20% below the alternative we tested (free plan), with 41 filled fields per product in that test. Search by keyword, URL or ASIN: price, list price, rating, reviews, Prime, badges, bought-in-past-month, images and specs. No login.

## Columns in sample.csv
`asin`, `title`, `brand`, `price`, `listPrice`, `currency`, `rating`, `reviewCount`, `isPrime`, `isSponsored`, `badges`, `boughtInPastMonth`, `monthlyPurchaseVolume`, `availability`, `url`, `marketplace`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
