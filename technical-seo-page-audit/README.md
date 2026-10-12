# Technical SEO Page Audit: Broken Links, Hreflang, $3/1k

Free sample output (5 rows, `sample.csv`) from the Apify actor **technical-seo-page-audit**.

Actor page: https://apify.com/transparent_meteorite/technical-seo-page-audit

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Technical SEO audit verified by 130 passing tests: title, meta, canonical, H1-H3, internal/external and broken links, missing alt, Open Graph, hreflang, JSON-LD, redirect chain, TTFB, and a prioritised issues list with a score. Respects robots.txt. $0.003 per page.

## Columns in sample.csv
`url`, `finalUrl`, `statusCode`, `score`, `redirectChain`, `redirectCount`, `ttfbMs`, `responseTimeMs`, `contentType`, `htmlBytes`, `title`, `titleLength`, `metaDescription`, `metaDescriptionLength`, `canonical`, `canonicalCount`, `robotsMeta`, `lang`, `viewport`, `charset`, `h1`, `h1Count`, `h2Count`, `h3Count`, `emptyHeadings`, `headings`, `wordCount`, `internalLinks`, `externalLinks`, `nofollowLinks`, `emptyAnchorLinks`, `uniqueLinks`, `imagesTotal`, `imagesMissingAlt`, `imagesEmptyAlt`, `openGraph`, `twitterCard`, `hreflang`, `jsonLdTypes`, `jsonLdBlocks`, `jsonLdInvalid`, `canonicalIsSelf`, `linksChecked`, `brokenLinkCount`, `brokenLinkCheckSkipped`, `linksNotChecked`, `issues`, `issueCounts`, `auditedAt`, `robotsAllowed`, `indexable`

## Data source and privacy
Public pages you point it at.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
