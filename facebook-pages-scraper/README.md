# Facebook Pages Scraper: Emails, Phones, Followers $3/1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **facebook-pages-scraper**.

Actor page: https://apify.com/transparent_meteorite/facebook-pages-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape public Facebook Pages without login: name, category, followers, following, email, phone, address, website, social links, rating, price range, hours, page ID, creation date, ad status, verified flag. No cookies, no API key. Missing pages never charged.

## Columns in sample.csv
`pageUrl`, `pageName`, `pageId`, `category`, `followers`, `followings`, `verified`, `website`, `rating`, `ratingCount`, `priceRange`, `creation_date`, `ad_status`, `isRunningAds`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
