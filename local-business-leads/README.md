# Local Business Leads: No-Website Finder (OpenStreetMap) $3/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **local-business-leads**.

Actor page: https://apify.com/transparent_meteorite/local-business-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Local business leads at $0.003 per place, including businesses with no website listed. Name, phone, website, email, address, hours, socials and coordinates from OpenStreetMap open data. 75+ types, no-website, phone and website filters, optional email enrichment.

## Columns in sample.csv
`name`, `category`, `osmCategory`, `brand`, `phone`, `website`, `email`, `fullAddress`, `houseNumber`, `streetName`, `unit`, `city`, `state`, `postcode`, `openingHours`, `socials`, `facebook`, `wheelchair`, `lat`, `lon`, `googleMapsUrl`, `osmType`, `osmId`, `osmUrl`, `lastEdited`, `source`, `searchLocation`

## Data source and privacy
OpenStreetMap contributors, ODbL 1.0 (https://www.openstreetmap.org/copyright); phones masked.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
