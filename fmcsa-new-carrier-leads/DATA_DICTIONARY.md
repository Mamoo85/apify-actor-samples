# Data dictionary: New US trucking carriers (FMCSA census)

Files: [`latest.csv`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/fmcsa-new-carrier-leads/latest.csv) and [`latest.json`](https://raw.githubusercontent.com/Mamoo85/apify-actor-samples/main/fmcsa-new-carrier-leads/latest.json) (19 rows, refreshed weekly, last pull 2026-11-17T11:40:09Z). The older [`sample.csv`](./sample.csv) is kept as it was.

Source actor (Apify Store): https://apify.com/transparent_meteorite/fmcsa-new-carrier-leads
Data origin: FMCSA Motor Carrier Census (U.S. DOT)
License: CC0 1.0 (public domain dedication for our compilation). The underlying records are public records or open government data. We dedicate our selection and formatting to the public domain under CC0 1.0.

Contact details (emails, phones), street addresses and personal-name fields are removed before publishing. Coordinates are rounded to 2 decimals. Text fields are truncated to 300 characters.

| Column | Type | Description |
|---|---|---|
| `legal_name` | string | Registered legal name of the carrier. |
| `dba_name` | string | Doing-business-as name, if any. |
| `usdot` | string | USDOT number (carrier identifier). |
| `city` | string | City name. |
| `state` | string | US state or territory (two-letter code). |
| `power_units` | integer | Number of power units (trucks and tractors). |
| `total_drivers` | integer | Total drivers reported. |
| `total_cdl` | integer | Drivers holding a CDL. |
| `carrier_operation` | string | Operation code: A interstate, B intrastate hazmat, C intrastate non-hazmat. |
| `carrier_operation_label` | string | Plain-language label of carrier_operation. |
| `registered_date` | string | Registration date as YYYYMMDD. |
| `safer_url` | url | Link to the public FMCSA SAFER company snapshot. |
| `census_status` | string | Census status of the carrier. |
| `registered_date_iso` | date | Registration date as ISO date. |
| `county_code` | string | County code reported in the census. |
| `classification` | string | Carrier classification text, for example private property or authorized for hire. |
| `hazmat` | boolean | True when the carrier hauls hazardous materials. |
| `cargo_types` | json-string | JSON list of cargo classes. |
| `truck_units` | integer | Number of trucks. |
| `bus_units` | integer | Number of buses. |
| `fleet_size_class` | string | Fleet size bucket. |
| `units_owned` | integer | Owned units. |
| `units_term_leased` | integer | Term-leased units. |
| `interstate_drivers` | integer | Interstate drivers. |
| `intrastate_drivers` | integer | Intrastate drivers. |
| `mcs150_mileage` | integer | Annual mileage on the MCS-150. |
| `mcs150_mileage_year` | integer | Year the mileage refers to. |
| `duns_number` | string | D-U-N-S number on the census record. |
| `operation_type` | string | Value as published by the source. |
| `age_in_days` | integer | Value as published by the source. |
| `lead_score` | integer | Value as published by the source. |

Disclosure: I maintain the actor above (paid, pay-per-event). This file is a free sample.
