# Domain Intelligence: WHOIS/RDAP, DNS, Subdomains, SSL, $2/1k

Free sample output (8 rows, `sample.csv`) from the Apify actor **domain-intelligence-lookup**.

Actor page: https://apify.com/transparent_meteorite/domain-intelligence-lookup

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
Bulk domain lookup verified by 94 passing tests: RDAP registration (registrar, created, expires, age), DNS over HTTPS (A, AAAA, MX, NS, TXT with SPF and DMARC parsed), subdomains from certificate transparency, SSL expiry and HTTP security headers. $0.002 per domain.

## Columns in sample.csv
`domain`, `registrableDomain`, `checkedAt`, `registered`, `dns`, `hasSpf`, `hasDmarc`, `dmarcPolicy`, `ssl`, `sslIssuer`, `sslValidTo`, `sslDaysLeft`, `securityHeaders`, `securityHeadersScore`, `rdap`, `registrar`, `createdAt`, `expiresAt`, `updatedAt`, `ageDays`, `nameservers`, `status`, `answered`

## Data source and privacy
Public RDAP/DNS/TLS data.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
