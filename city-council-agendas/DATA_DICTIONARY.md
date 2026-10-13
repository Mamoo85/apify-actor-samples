# Data dictionary: City council agenda items and votes

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/city-council-agendas/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/city-council-agendas/latest.json) (60 rows, refreshed weekly, last pull 2026-10-13T22:32:24Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/city-council-agendas
Data origin: Legistar public web API (city clerk records)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `city` | string | City and state. |
| `client` | string | Legistar client slug of the city. |
| `body` | string | Council body or committee. |
| `meetingDate` | date | Meeting date (ISO). |
| `meetingTime` | string | Meeting time as published. |
| `location` | string | Meeting location. |
| `agendaStatus` | string | Agenda status such as Final. |
| `agendaItemNumber` | string | Agenda item number. |
| `agendaSequence` | integer | Order of the item on the agenda. |
| `title` | string | Agenda item title. |
| `matterFile` | string | Legislative file number. |
| `matterType` | string | Matter type, for example Resolution or Bill. |
| `matterStatus` | string | Status of the matter. |
| `action` | string | Action taken on the item. |
| `voteResult` | string | Pass, Fail or empty. |
| `agendaNote` | string | Agenda note text (truncated). May contain names of officials as published in the public agenda. |
| `attachmentUrls` | json-string | JSON list of attachment links. |
| `agendaPdfUrl` | url | Link to the agenda PDF. |
| `minutesPdfUrl` | url | Link to the minutes PDF. |
| `meetingUrl` | url | Link to the meeting page. |
| `eventId` | integer | Legistar event id. |
| `eventItemId` | integer | Legistar event item id. |
| `matterId` | integer | Legistar matter id. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
