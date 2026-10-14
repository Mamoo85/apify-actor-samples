# TikTok Profile Scraper - Followers, Posts, Bio, Emails

Free sample output (5 rows, `sample.csv`) from the Apify actor **tiktok-public-profile-scraper**.

Actor page: https://apify.com/transparent_meteorite/tiktok-public-profile-scraper

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
TikTok public profiles and latest posts: followers, likes, video count, bio, bio link, emails and links in bio, verified, business category, plus each recent video's plays, likes, comments, shares, saves, hashtags, music and engagement rate. Video URLs too. No login.

## Columns in sample.csv
`type`, `id`, `text`, `webVideoUrl`, `createTimeISO`, `playCount`, `diggCount`, `commentCount`, `shareCount`, `collectCount`, `repostCount`, `isPinned`, `isSponsored`, `hashtags`, `engagementRate`, `authorMeta`, `scrapedAt`

## Data source and privacy
Public web pages and public ad/job/product listings. Personal data is removed or masked (emails look like `a***@domain`). The sample was generated on 2026-10-12 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use.
