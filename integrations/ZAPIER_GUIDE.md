# Zapier step-by-step guide (NOT importable)

Zapier has no public zap import format, so these are click-by-click build instructions. Each Zap has 4 steps: Schedule, Webhooks (Custom Request), Looping, and your destination. Webhooks by Zapier needs a paid Zapier plan. I maintain these Apify actors (account `transparent_meteorite`).

Never paste your Apify token anywhere public. Token: Apify Console > Settings > API & Integrations.


## Apify ATS Open Roles on a schedule

Run the Apify actor transparent_meteorite/ats-open-roles (open jobs from Greenhouse, Lever, Ashby and other career sites (set monitorMode for new-or-changed)) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~ats-open-roles/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "companies": [
    "airbnb",
    "stripe",
    "https://jobs.lever.co/spotify"
  ],
  "maxJobsPerCompany": 25,
  "onlyNewSinceLastRun": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify Building Permits Leads on a schedule

Run the Apify actor transparent_meteorite/building-permits-leads (new or changed building permits from official city open-data portals) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~building-permits-leads/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "cities": [
    "CHI",
    "SEA",
    "AUS"
  ],
  "recordTypes": [
    "permit"
  ],
  "sinceDays": 7,
  "maxItems": 50,
  "monitorMode": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify FMCSA New Carrier Leads on a schedule

Run the Apify actor transparent_meteorite/fmcsa-new-carrier-leads (newly authorized US trucking carriers with contact data, new ones only each run) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~fmcsa-new-carrier-leads/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "mode": "newCarriers",
  "states": [
    "MI"
  ],
  "daysBack": 7,
  "maxResults": 25,
  "requireEmail": true,
  "onlyNewSinceLastRun": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify Local Business Leads on a schedule

Run the Apify actor transparent_meteorite/local-business-leads (local businesses (including ones without a website) from OpenStreetMap) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~local-business-leads/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "categories": [
    "dentist"
  ],
  "locations": [
    "Austin, TX"
  ],
  "maxItems": 50,
  "requireWebsite": false
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify SEC Form D Funding Leads on a schedule

Run the Apify actor transparent_meteorite/sec-form-d-funding-leads (recently funded startups from SEC Form D filings) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~sec-form-d-funding-leads/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "lookbackDays": 3,
  "maxResults": 25,
  "excludePooledFunds": true,
  "includeAmendments": false,
  "onlyNewSinceLastRun": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify WARN Layoff Alerts on a schedule

Run the Apify actor transparent_meteorite/warn-layoff-alerts (new WARN Act layoff notices from 7 states) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~warn-layoff-alerts/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "states": [
    "CA",
    "TX"
  ],
  "daysBack": 30,
  "maxResults": 50,
  "onlyNewSinceLastRun": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify Website Contact Extractor on a schedule

Run the Apify actor transparent_meteorite/website-contact-extractor (public business emails, phones and social links from websites) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~website-contact-extractor/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "startUrls": [
    {
      "url": "https://example.com"
    }
  ],
  "maxPagesPerSite": 5,
  "includeNamedEmails": true,
  "sameDomainOnly": true
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.

## Apify Website Tech Stack Detector on a schedule

Run the Apify actor transparent_meteorite/website-tech-stack-detector (CMS, frameworks, analytics and hosting for a list of websites) on a schedule and pass each result row to your next step.

1. **Trigger**: app `Schedule by Zapier`, event `Every Day`. Set: time_of_day = 7am, trigger_on_weekends = no.
2. **Action**: app `Webhooks by Zapier`, event `Custom Request`. Set Method = `POST`, URL = `https://api.apify.com/v2/acts/transparent_meteorite~website-tech-stack-detector/run-sync-get-dataset-items?timeout=240&format=json&clean=true`, Data Pass-Through = `no`, Unflatten = `yes`.
   - Data (paste as JSON in the Data box):

```json
{
  "urls": [
    "shopify.com",
    "vercel.com"
  ],
  "concurrency": 4
}
```

   - Headers: `Authorization` = `Bearer <your Apify token>`, `Content-Type` = `application/json`.
   - Click Test. You should see a list of result rows (an empty list just means no new rows for those filters).
3. **Action**: `Looping by Zapier`, `Create Loop From Line Items`. Map the fields you need from step 2 (the response is an array).
4. **Action**: your destination (Google Sheets, Slack, HubSpot, etc.). Map the looped fields.
5. Turn the Zap on. Check the actor's Store page for per-result pricing first.
