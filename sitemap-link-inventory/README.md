# Sitemap Link Inventory: All URLs + Broken-Link Check, $1/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **sitemap-link-inventory**.

Actor page: https://apify.com/transparent_meteorite/sitemap-link-inventory

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Find every sitemap for a domain (robots.txt, nested indexes, .gz, .txt, common paths) and return all URLs with lastmod, priority, images, hreflang, path groups and duplicates. Optional broken-link, redirect, noindex checks. Partial results never fail the run. $0.001 per sitemap file / link checked.

## Columns in sample.csv
`recordType`, `site`, `url`, `changefreq`, `priority`, `sourceSitemap`, `sitemapDepth`, `pathGroup`, `pathDepth`, `hasQuery`, `imageCount`, `videoCount`, `hreflangCount`, `robotsDisallowed`, `isDuplicate`, `checked`

## Data source and privacy
Public sitemaps.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
