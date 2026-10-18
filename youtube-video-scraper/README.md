# YouTube Scraper: Videos, Views, Likes, Tags, $2 per 1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **youtube-video-scraper**.

Actor page: https://apify.com/transparent_meteorite/youtube-video-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape YouTube videos from searches, channels, playlists, hashtags or URLs: views, likes, comment count, exact date, duration, description, tags, chapters, subtitle languages and channel stats. YouTube search filters. No login, no API key, no quota. $2 per 1,000 videos.

## Columns in sample.csv
`id`, `url`, `title`, `channelName`, `numberOfSubscribers`, `viewCount`, `likes`, `commentsCount`, `date`, `duration`, `durationSeconds`, `hashtags`, `tags`, `category`, `isShort`, `hasSubtitles`, `subtitleLanguages`, `fromSource`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
