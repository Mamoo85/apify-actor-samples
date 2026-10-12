# FMCSA New Carrier Leads: New Authority Truckers, Email & Phone

Free sample output (12 rows, `sample.csv`) from the Apify actor **fmcsa-new-carrier-leads**.

Actor page: https://apify.com/transparent_meteorite/fmcsa-new-carrier-leads

**Disclosure: I maintain this actor.** This repo is a free sample of its real output so you can judge the columns before running it. Nothing here is a review or endorsement by a third party.

## What it does
New US trucking authorities with officer names and authority status on every row, tested by 141 automated checks. New USDOT/MC carriers from the official FMCSA census with filed email and phone. Filter by state and fleet size; deduped, so daily runs only bill new carriers.

## Columns in sample.csv
`legal_name`, `usdot`, `email`, `phone`, `city`, `state`, `zip`, `power_units`, `total_drivers`, `total_cdl`, `carrier_operation`, `carrier_operation_label`, `registered_date`, `safer_url`, `census_status`, `registered_date_iso`, `county_code`, `classification`, `hazmat`, `cargo_types`, `truck_units`, `bus_units`, `fleet_size_class`, `units_owned`, `units_term_leased`, `interstate_drivers`, `intrastate_drivers`, `mcs150_mileage`, `mcs150_mileage_year`

## Data source and privacy
US FMCSA census (public federal data). Street addresses, officer names and mobile numbers removed; emails/phones masked.
Personal data is removed or masked (emails look like `a***@domain`, phones like `xxx-xxx-xx12`). The sample was generated on 2026-10-11 and is a snapshot, not a maintained dataset. Use the actor for current data and check the source's terms for your use case.
