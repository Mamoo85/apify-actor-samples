# Sanctions Screening: OFAC SDN, EU, UN & UK Lists, Fuzzy Match

Free sample output (6 rows, `sample.csv`) from the Apify actor **sanctions-screening**.

Actor page: https://apify.com/transparent_meteorite/sanctions-screening

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Screen names of people, companies and vessels against the official OFAC SDN, OFAC Consolidated, UN, EU and UK sanctions lists. Fuzzy match handles diacritics, transliteration, word order and aliases; optional DOB and country. Screening aid, not legal advice. $0.004 per name.

## Columns in sample.csv
`recordType`, `inputName`, `inputType`, `status`, `bestScore`, `matchCount`, `minScore`, `topMatchName`, `topMatchList`, `topMatchPrograms`, `topMatchEntryId`, `topMatchSourceUrl`, `matches`, `nearestBelowThreshold`, `listsChecked`, `listPublishDates`, `disclaimer`

## Data source and privacy
US OFAC SDN list (public domain). Matches shown are listed entities, not conclusions about anyone.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
