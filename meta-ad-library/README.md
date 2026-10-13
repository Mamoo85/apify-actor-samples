# Meta Ad Library Scraper: Facebook & Instagram Ads

Free sample output (4 rows, `sample.csv`) from the Apify actor **meta-ad-library**.

Actor page: https://apify.com/transparent_meteorite/meta-ad-library

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Image or video URL on 100% of ads vs 70% in our side-by-side test, at $0.00065 per ad. Search the public Meta Ad Library by keyword, advertiser Page id or library URL. No login. Flat rows: ad text, headline, link, CTA, media URLs, ISO dates, platforms, variations.

## Columns in sample.csv
`adArchiveId`, `pageId`, `pageName`, `isActive`, `startDate`, `endDate`, `platforms`, `bodyText`, `title`, `linkUrl`, `ctaText`, `mediaType`, `imageUrls`, `videoUrls`, `variationsCount`, `libraryUrl`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
