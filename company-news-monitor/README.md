# Company News Monitor: Brand & Keyword News Alerts, $2/1k

Free sample output (11 rows, `sample.csv`) from the Apify actor **company-news-monitor**.

Actor page: https://apify.com/transparent_meteorite/company-news-monitor

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Company news monitoring at $0.002 per article from 75 publisher RSS feeds (Bloomberg, CNBC, FT, TechCrunch, PR Newswire...) plus the GDELT news index when reachable. Track companies, domains or keywords. Deduped, event-tagged, delta mode for schedules.

## Columns in sample.csv
`title`, `url`, `domain`, `sourceName`, `publishedAt`, `language`, `country`, `matchedKeywords`, `snippet`, `imageUrl`, `eventTags`, `sentiment`, `provider`, `feedUrl`, `fetchedAt`

## Data source and privacy
Public news RSS and GDELT metadata; titles and links only, copyright stays with publishers.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
