# YouTube Shorts Scraper: Views, Likes, Dates, $2 per 1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **youtube-shorts-scraper**.

Actor page: https://apify.com/transparent_meteorite/youtube-shorts-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape YouTube Shorts from channels or single Shorts URLs: views, likes, comment count, exact publish date, duration, hashtags, description and full channel stats. Sort by newest, popular or oldest, filter by date, monitor for new Shorts. No login, no API key, no proxy needed.

## Columns in sample.csv
`id`, `url`, `title`, `viewCount`, `likes`, `commentsCount`, `date`, `duration`, `durationSeconds`, `category`, `hashtags`, `channelName`, `channelHandle`, `channelUrl`, `numberOfSubscribers`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
