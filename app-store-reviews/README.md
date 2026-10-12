# App Store Reviews Scraper: Ratings, 150+ Countries, $0.50/1k

Free sample output (9 rows, `sample.csv`) from the Apify actor **app-store-reviews**.

Actor page: https://apify.com/transparent_meteorite/app-store-reviews

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Apple App Store reviews at $0.50 per 1,000, verified by 85 passing tests. Review text, stars, app version, date, votes, plus rating, rating count, price, genre and release notes. 150+ countries, keyword search, date and star filters, delta mode.

## Columns in sample.csv
`type`, `appId`, `appName`, `country`, `bundleId`, `developer`, `developerId`, `genre`, `genres`, `price`, `currency`, `formattedPrice`, `ratingAverage`, `ratingCount`, `ratingAverageCurrentVersion`, `ratingCountCurrentVersion`, `version`, `currentVersionReleaseDate`, `releaseDate`, `releaseNotes`, `sizeBytes`, `sizeMB`, `contentRating`, `minimumOsVersion`, `languages`, `description`, `iconUrl`, `sellerUrl`, `url`, `reviewId`, `title`, `text`, `rating`, `date`, `voteSum`, `voteCount`

## Data source and privacy
Apple public App Store listings and review feeds; reviewer names removed, text truncated. Review text remains the authors' copyright; sample is for illustration only.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
