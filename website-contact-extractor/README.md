# Website Contact Extractor: Email & Phone Scraper, Socials $2/1k

Free sample output (5 rows, `sample.csv`) from the Apify actor **website-contact-extractor**.

Actor page: https://apify.com/transparent_meteorite/website-contact-extractor

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
$0.002 per website, not per page, with up to 5 contact pages crawled; verified by 110 passing tests. Bulk-extract emails, phone numbers and social profiles from business websites: role/named email tags, E.164 phones, 8 socials and address, one clean row per site.

## Columns in sample.csv
`inputUrl`, `domain`, `url`, `status`, `companyName`, `companyNameSource`, `emails`, `emailCount`, `primaryEmail`, `phones`, `phoneCount`, `primaryPhone`, `socials`, `contactPageUrl`, `pagesCrawled`, `pagesCrawledUrls`, `responded`, `scrapedAt`, `phonesList`, `linkedin`, `facebook`, `instagram`, `x`, `youtube`, `tiktok`, `pinterest`, `github`

## Data source and privacy
Public business websites; emails and phones masked.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
