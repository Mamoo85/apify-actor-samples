# Workflow templates for Apify public-data actors (n8n, Make, Zapier)

Ready-to-adapt templates that call eight of my Apify actors on a schedule through the Apify API and hand the rows to the next step in your automation.

**Disclosure: I maintain all of these actors** (Apify account `transparent_meteorite`). The templates are free to use. The actors are paid pay-per-event Apify tools; Apify's free plan credit covers a trial. Check each actor's Store page for current pricing before you schedule anything.

| Actor | What it returns |
|---|---|
| [fmcsa-new-carrier-leads](https://apify.com/transparent_meteorite/fmcsa-new-carrier-leads) | newly authorized US trucking carriers (new ones only each run) |
| [warn-layoff-alerts](https://apify.com/transparent_meteorite/warn-layoff-alerts) | WARN Act layoff notices, 7 states |
| [ats-open-roles](https://apify.com/transparent_meteorite/ats-open-roles) | open jobs from Greenhouse, Lever, Ashby and more |
| [local-business-leads](https://apify.com/transparent_meteorite/local-business-leads) | local businesses from OpenStreetMap |
| [website-contact-extractor](https://apify.com/transparent_meteorite/website-contact-extractor) | public business emails, phones, socials from websites |
| [sec-form-d-funding-leads](https://apify.com/transparent_meteorite/sec-form-d-funding-leads) | recently funded startups (SEC Form D) |
| [building-permits-leads](https://apify.com/transparent_meteorite/building-permits-leads) | new or changed building permits (monitor mode) |
| [website-tech-stack-detector](https://apify.com/transparent_meteorite/website-tech-stack-detector) | CMS, frameworks, analytics, hosting per site |

## Files

- `n8n/<actor>.json`: n8n workflow (Schedule trigger, HTTP Request, Set, placeholder destination, setup sticky note). Import via **Workflows > Import from file**.
- `make/<actor>.json`: Make scenario blueprint (HTTP "Make a request" module plus an Iterator). Import via **Scenario > ... > Import Blueprint**.
- `zapier/<actor>.json`: Zapier-style recipe. Zapier has no public zap-import file format, so this is a step-by-step spec with exact field values to paste into a Schedule, Webhooks by Zapier (Custom Request) and Looping step. It is not importable.

## How every template works

`POST https://api.apify.com/v2/acts/transparent_meteorite~<actor>/run-sync-get-dataset-items` with your filters as the JSON body and `Authorization: Bearer <your Apify token>` as a header. The response is a JSON array of result rows. The call is synchronous (Apify allows about 5 minutes); for bigger jobs use the async run endpoint and read the dataset afterwards.

## Credentials

No secrets are in these files. Replace the placeholders yourself:

- n8n: create a *Header Auth* credential (`Authorization` = `Bearer YOUR_APIFY_API_TOKEN`) and select it on the *Run actor* node (the credential id `REPLACE_WITH_YOUR_CREDENTIAL` is a placeholder).
- Make and Zapier: replace `YOUR_APIFY_API_TOKEN` in the Authorization header.
- Your token: Apify Console > Settings > API & Integrations.

## Tested with (2026-10-11)

- **n8n 2.42.6 (self-hosted, local): tested.** All 8 workflows imported with `n8n import:workflow` without error. Two (`website-tech-stack-detector`, `warn-layoff-alerts`) were executed end to end with a real Apify token via the Test run (manual) trigger: both nodes finished with status success, HTTP 200, and result rows came back (4 and 100 rows, tagged with `_source`). The other six were import-tested only, not executed. Finding fixed: the files now carry a top-level workflow `id` (the CLI import refused them without it) and a manual "Test run" trigger.
- **Make (us2 zone, free plan): imported, not run.** All 8 blueprints were created through the Make API as scenarios and Make reported them valid (not invalid). A live run could not be done because that Make team was over its operations limit (error IM310), so the HTTP module and Iterator were not executed. The test scenarios were deleted afterwards.
- **Zapier: not importable, not tested.** Zapier has no zap import format. See [ZAPIER_GUIDE.md](ZAPIER_GUIDE.md) for click-by-click build steps; the `zapier/*.json` files are the same steps as data. Nothing was run in Zapier.
- Node and module versions in these tools drift; if an import complains, rebuild the two steps by hand from the values in the file.
