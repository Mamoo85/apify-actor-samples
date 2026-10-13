# Data dictionary: Developer signals: Hacker News, npm and PyPI

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/developer-signals/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/developer-signals/latest.json) (49 rows, refreshed weekly, last pull 2026-10-13T22:32:35Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/developer-signals
Data origin: Hacker News Algolia API, npm registry, PyPI JSON API
License: Free to use, source terms apply. These are facts about publicly posted items (jobs, stories, packages). Free to use for analysis; the text of postings belongs to the original publishers, so check the source terms before republishing it.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `source` | string | Source system of the row. |
| `recordType` | string | Kind of record in this row. |
| `id` | string | Hacker News item id (stories). |
| `title` | string | Title or headline of the record. |
| `url` | url | Link to the record at the source. |
| `domain` | string | Domain of the linked story. |
| `createdAt` | datetime | Story creation time (UTC). |
| `points` | integer | Hacker News points. |
| `numComments` | integer | Comment count. |
| `hnUrl` | url | Link to the Hacker News discussion. |
| `kind` | string | Story kind, for example showHn. |
| `textSnippet` | string | Start of the story text (truncated). |
| `query` | string | Search query that surfaced the story. |
| `queryType` | string | Type of query. |
| `packageName` | string | npm or PyPI package name. |
| `latestVersion` | string | Latest published version. |
| `description` | string | Free-text description from the source (truncated to 300 characters). |
| `license` | string | Declared package license. |
| `homepage` | url | Package homepage. |
| `repositoryUrl` | url | Source repository URL. |
| `keywords` | json-string | JSON list of package keywords. |
| `requiresPython` | string | Python version constraint (PyPI). |
| `latestReleaseAt` | datetime | Time of the latest release. |
| `downloadsLastDay` | integer | Downloads in the last day. |
| `downloadsLastWeek` | integer | Downloads in the last week. |
| `downloadsLastMonth` | integer | Downloads in the last month. |
| `found` | boolean | True when the package was found. |
| `matchedQueries` | json-string | JSON list of queries the row matched. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
