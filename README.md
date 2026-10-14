# Public-data samples from my Apify actors

One folder per actor, each with a small `sample.csv` of real output and a README with the column list and data-source notes.

**Disclosure: I maintain all of these actors** (Apify account `transparent_meteorite`). The samples are free to use; the actors are paid pay-per-event tools at https://apify.com/transparent_meteorite

| Actor | Sample | What for |
|---|---|---|
| [fmcsa-new-carrier-leads](https://apify.com/transparent_meteorite/fmcsa-new-carrier-leads) | [fmcsa-new-carrier-leads/](./fmcsa-new-carrier-leads/) | FMCSA New Carrier Leads: New Authority Truckers, Email & Phone |
| [warn-layoff-alerts](https://apify.com/transparent_meteorite/warn-layoff-alerts) | [warn-layoff-alerts/](./warn-layoff-alerts/) | WARN Layoff Notices API: 7 States (TX CA WA OR MD VA NC) $3/1k |
| [website-tech-stack-detector](https://apify.com/transparent_meteorite/website-tech-stack-detector) | [website-tech-stack-detector/](./website-tech-stack-detector/) | Website Tech Stack Lookup: CMS, Frameworks, Hosting $0.002/site |
| [ats-open-roles](https://apify.com/transparent_meteorite/ats-open-roles) | [ats-open-roles/](./ats-open-roles/) | Career Site Jobs API: Greenhouse, Lever, Ashby & more | $2/1k |
| [city-council-agendas](https://apify.com/transparent_meteorite/city-council-agendas) | [city-council-agendas/](./city-council-agendas/) | City Council Agendas API: Legistar Items, Votes & PDFs | $1/1k |
| [company-enrichment-by-domain](https://apify.com/transparent_meteorite/company-enrichment-by-domain) | [company-enrichment-by-domain/](./company-enrichment-by-domain/) | Company Enrichment by Domain: Socials, Emails, Tech Stack $5/1k |
| [sec-form-d-funding-leads](https://apify.com/transparent_meteorite/sec-form-d-funding-leads) | [sec-form-d-funding-leads/](./sec-form-d-funding-leads/) | SEC Form D Funding Leads: Recently Funded Startups, $2.50/1k |
| [technical-seo-page-audit](https://apify.com/transparent_meteorite/technical-seo-page-audit) | [technical-seo-page-audit/](./technical-seo-page-audit/) | Technical SEO Page Audit: Broken Links, Hreflang, $3/1k |
| [domain-intelligence-lookup](https://apify.com/transparent_meteorite/domain-intelligence-lookup) | [domain-intelligence-lookup/](./domain-intelligence-lookup/) | Domain Intelligence: WHOIS/RDAP, DNS, Subdomains, SSL, $2/1k |
| [new-business-filings](https://apify.com/transparent_meteorite/new-business-filings) | [new-business-filings/](./new-business-filings/) | New Business Filings: New LLCs and Corporations, $4/1k |
| [app-store-reviews](https://apify.com/transparent_meteorite/app-store-reviews) | [app-store-reviews/](./app-store-reviews/) | App Store Reviews Scraper: Ratings, 150+ Countries, $0.50/1k |
| [website-contact-extractor](https://apify.com/transparent_meteorite/website-contact-extractor) | [website-contact-extractor/](./website-contact-extractor/) | Website Contact Extractor: Email & Phone Scraper, Socials $2/1k |
| [shopify-store-leads](https://apify.com/transparent_meteorite/shopify-store-leads) | [shopify-store-leads/](./shopify-store-leads/) | Shopify Store Leads: Apps, Products, Contacts $4/1k |
| [local-business-leads](https://apify.com/transparent_meteorite/local-business-leads) | [local-business-leads/](./local-business-leads/) | Local Business Leads: No-Website Finder (OpenStreetMap) $3/1k |
| [workday-jobs-scraper](https://apify.com/transparent_meteorite/workday-jobs-scraper) | [workday-jobs-scraper/](./workday-jobs-scraper/) | Workday Jobs Scraper: Any Career Site, 165+ Companies $1/1k |
| [company-news-monitor](https://apify.com/transparent_meteorite/company-news-monitor) | [company-news-monitor/](./company-news-monitor/) | Company News Monitor: Brand & Keyword News Alerts, $2/1k |
| [building-permits-leads](https://apify.com/transparent_meteorite/building-permits-leads) | [building-permits-leads/](./building-permits-leads/) | Building Permits Leads: US City Permits and Violations, $1.5/1k |
| [sitemap-link-inventory](https://apify.com/transparent_meteorite/sitemap-link-inventory) | [sitemap-link-inventory/](./sitemap-link-inventory/) | Sitemap Link Inventory: All URLs + Broken-Link Check, $1/1k |
| [developer-signals](https://apify.com/transparent_meteorite/developer-signals) | [developer-signals/](./developer-signals/) | Hacker News, npm & PyPI Developer Signals |
| [sanctions-screening](https://apify.com/transparent_meteorite/sanctions-screening) | [sanctions-screening/](./sanctions-screening/) | Sanctions Screening: OFAC SDN, EU, UN & UK Lists, Fuzzy Match |
| [federal-grants-contracts](https://apify.com/transparent_meteorite/federal-grants-contracts) | [federal-grants-contracts/](./federal-grants-contracts/) | Federal Grants & Contracts Finder: Grants.gov + USAspending |

Street addresses are removed in every sample (only city, state and a 3-digit ZIP prefix such as 805xx are kept, and coordinates are rounded to 2 decimals, about 1 km). Phone numbers keep only their last two digits and email addresses keep only the first letter and the domain. Record names are business names. Source licences are listed per folder (for example OpenStreetMap data is ODbL).

## Workflow templates

[`integrations/`](./integrations/) has n8n workflows, Make blueprints and Zapier-style recipes for eight of these actors (same disclosure applies: I maintain them). Tested with: n8n 2.42.6 (all 8 import; 2 run end to end with real rows), Make (all 8 import as valid scenarios; not run, account over its ops limit), Zapier (not importable; step-by-step guide only, not run). Details in the README inside.

Landing pages for all 21 actors: https://mamoo85.github.io/open-data-actors/
| [linkedin-public-jobs](https://apify.com/transparent_meteorite/linkedin-public-jobs) | [linkedin-public-jobs/](./linkedin-public-jobs/) | LinkedIn Public Jobs Scraper (no login) | Salary & Level |
| [meta-ad-library](https://apify.com/transparent_meteorite/meta-ad-library) | [meta-ad-library/](./meta-ad-library/) | Meta Ad Library Scraper: Facebook & Instagram Ads |
| [amazon-product-search](https://apify.com/transparent_meteorite/amazon-product-search) | [amazon-product-search/](./amazon-product-search/) | Amazon Product Search: prices, ratings, ASINs |
<!--od-latest-->
## Fresh data and data dictionaries

Ten folders also have `latest.csv` and `latest.json` (up to 60 rows, refreshed weekly, fixed raw URLs) and a `DATA_DICTIONARY.md` listing every column: [warn-layoff-alerts](./warn-layoff-alerts/DATA_DICTIONARY.md), [fmcsa-new-carrier-leads](./fmcsa-new-carrier-leads/DATA_DICTIONARY.md), [federal-grants-contracts](./federal-grants-contracts/DATA_DICTIONARY.md), [city-council-agendas](./city-council-agendas/DATA_DICTIONARY.md), [sec-form-d-funding-leads](./sec-form-d-funding-leads/DATA_DICTIONARY.md), [new-business-filings](./new-business-filings/DATA_DICTIONARY.md), [building-permits-leads](./building-permits-leads/DATA_DICTIONARY.md), [developer-signals](./developer-signals/DATA_DICTIONARY.md), [ats-open-roles](./ats-open-roles/DATA_DICTIONARY.md), [workday-jobs-scraper](./workday-jobs-scraper/DATA_DICTIONARY.md). Dataset pages, static JSON API, chart widgets and monthly stats: https://mamoo85.github.io/open-data-actors/datasets/
<!--/od-latest-->

## More ways to use the actors

All maintained by me (same disclosure as above):

- [open-data-actor-workflows](https://github.com/Mamoo85/open-data-actor-workflows): n8n workflows, Make blueprints and Zapier recipes for all 24 actors.
- [open-data-actor-notebooks](https://github.com/Mamoo85/open-data-actor-notebooks): executed Colab/Jupyter notebooks, one per actor.
- [open-data-actors-agent-tools](https://github.com/Mamoo85/open-data-actors-agent-tools): LangChain, LlamaIndex and CrewAI tools.
- [open-data-actors-mcp](https://github.com/Mamoo85/open-data-actors-mcp): MCP server (listed in the official MCP registry).
| [google-maps-places-scraper](https://apify.com/transparent_meteorite/google-maps-places-scraper) | [google-maps-places-scraper/](./google-maps-places-scraper/) | Google Maps Scraper: Places, Phones, Emails $1.50/1K |
| [tiktok-public-profile-scraper](https://apify.com/transparent_meteorite/tiktok-public-profile-scraper) | [tiktok-public-profile-scraper/](./tiktok-public-profile-scraper/) | TikTok Profile Scraper - Followers, Posts, Bio, Emails |
