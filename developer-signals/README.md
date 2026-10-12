# Hacker News, npm & PyPI Developer Signals

Free sample output (4 rows, `sample.csv`) from the Apify actor **developer-signals**.

Actor page: https://apify.com/transparent_meteorite/developer-signals

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Track Hacker News mentions, Show HN and Launch HN posts, plus npm and PyPI package versions, repo links and download counts, in one dataset. Keyless public APIs. From $0.001 per item.

## Columns in sample.csv
`source`, `recordType`, `id`, `title`, `url`, `domain`, `createdAt`, `points`, `numComments`, `hnUrl`, `kind`, `query`, `queryType`, `packageName`, `latestVersion`, `description`, `license`, `homepage`, `repositoryUrl`, `keywords`, `downloadsLastDay`, `downloadsLastWeek`, `downloadsLastMonth`, `found`, `matchedQueries`

## Data source and privacy
Hacker News Algolia API, npm and PyPI registries; usernames removed.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
