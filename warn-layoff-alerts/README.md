# WARN Layoff Notices API: 7 States (TX CA WA OR MD VA NC) $3/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **warn-layoff-alerts**.

Actor page: https://apify.com/transparent_meteorite/warn-layoff-alerts

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
WARN Act layoff notices from 7 official state sources (TX, CA, WA, OR, MD, VA, NC), verified by 89 passing tests. Clean rows: employer, workers affected, city, notice and layoff dates. Deduped across runs for scheduled alerts. CSV, JSON, API or webhook. $0.003 per notice.

## Columns in sample.csv
`company`, `city`, `county`, `state`, `layoff_count`, `notice_date`, `layoff_date`, `received_date`, `layoff_type`, `source_state`, `source_url`, `enriched`

## Data source and privacy
State WARN-notice postings (public government records).
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
