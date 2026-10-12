# Company Enrichment by Domain: Socials, Emails, Tech Stack $5/1k

Free sample output (8 rows, `sample.csv`) from the Apify actor **company-enrichment-by-domain**.

Actor page: https://apify.com/transparent_meteorite/company-enrichment-by-domain

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Company enrichment from each company's own site and DNS only, verified by 73 passing tests. Domains in; name, logo, description, socials, careers/ATS, business emails and phones, email provider (MX) and tech stack out. No login, no data brokers. $0.005 per domain.

## Columns in sample.csv
`domain`, `input`, `finalUrl`, `status`, `companyName`, `companyNameSource`, `description`, `logoUrl`, `faviconUrl`, `language`, `countryHint`, `countryHintSource`, `address`, `emails`, `phones`, `linkedinCompanyUrl`, `x`, `facebook`, `instagram`, `youtube`, `github`, `tiktok`, `careersUrl`, `emailProvider`, `mxHosts`, `spfPresent`, `techStack`, `copyrightYear`, `pagesFetched`, `fetchedAt`

## Data source and privacy
Public company websites; contact data masked.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
