# YouTube Comments Scraper - Comments & Replies, $1/1K

Free sample output (10 rows, `sample.csv`) from the Apify actor **youtube-comments-scraper**.

Actor page: https://apify.com/transparent_meteorite/youtube-comments-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Scrape public YouTube comments and replies from videos, Shorts, channels, playlists or searches: text, author, likes, reply count, creator heart, pinned, date. Top or newest, keyword/likes/date filters, monitor mode. No login.

## Columns in sample.csv
`videoId`, `videoTitle`, `videoUrl`, `channelName`, `sortBy`, `commentId`, `text`, `likeCount`, `replyCount`, `hasCreatorHeart`, `isPinned`, `isEdited`, `publishedTimeText`, `isReply`, `parentCommentId`, `position`, `commentUrl`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
