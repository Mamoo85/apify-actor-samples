# City Council Agendas API: Legistar Items, Votes & PDFs | $1/1k

Free sample output (12 rows, `sample.csv`) from the Apify actor **city-council-agendas**.

Actor page: https://apify.com/transparent_meteorite/city-council-agendas

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
City council agenda items from 18 US cities via the official Legistar Web API, verified by 93 passing tests. Meeting date, body, matter, status, action, vote result, attachment and agenda PDF links. Keyword filters, deduped alerts. $0.001 per item.

## Columns in sample.csv
`city`, `client`, `body`, `meetingDate`, `meetingTime`, `location`, `agendaStatus`, `agendaItemNumber`, `agendaSequence`, `title`, `agendaNote`, `minutesNote`, `agendaPdfUrl`, `minutesPdfUrl`, `meetingUrl`, `eventId`, `eventItemId`

## Data source and privacy
Public Legistar city-council agenda data.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
