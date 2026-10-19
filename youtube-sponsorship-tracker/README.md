# YouTube Sponsorship Tracker - Brand Deals $2/1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **youtube-sponsorship-tracker**.

Actor page: https://apify.com/transparent_meteorite/youtube-sponsorship-tracker

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Find which YouTubers a brand sponsors, or every sponsor in a channel or niche. One row per video and sponsor: brand, domain, promo code, tracked link, ad timestamp, evidence and confidence. No login, no API key. $2 per 1,000 rows.

## Columns in sample.csv
`videoId`, `url`, `title`, `channelName`, `channelSubscribers`, `views`, `likes`, `publishedAt`, `sponsorBrand`, `sponsorDomain`, `promoCode`, `sponsorTimestamp`, `isPaidPromotionFlag`, `hasAdDisclosure`, `confidence`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
