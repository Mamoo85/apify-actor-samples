# Threads Scraper: Profiles, Posts, Views, Likes, $1.50 per 1K

Free sample output (11 rows, `sample.csv`) from the Apify actor **threads-profile-scraper**.

Actor page: https://apify.com/transparent_meteorite/threads-profile-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape public Threads profiles and posts without login: post text, views, likes, replies, reposts, quotes, media URLs, hashtags, links, exact date, plus followers, bio and verified flag. Filter by date, monitor for new posts. No API key, no cookies. Flat price, no start fee.

## Columns in sample.csv
`type`, `code`, `url`, `text`, `createdAt`, `likeCount`, `replyCount`, `repostCount`, `quoteCount`, `viewCount`, `mediaType`, `hashtags`, `isReply`, `isPinned`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
