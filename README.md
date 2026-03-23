# KetSDA_data_entry

`KetSDA_data_entry` is a Shiny app designed for Kettering Seventh-day Adventist Church deacons to enter weekly attendance data by church service and classroom.

The app writes data to existing Google Sheets and supports separate entry for:

- Church services
- Adult Sabbath School classes
- Children’s Sabbath School classes

It is built for mobile-friendly use and is intended to allow multiple deacon teams to submit attendance without creating duplicate daily rows.

## Notes

This repository contains a public-safe version of the app.

The live production app uses:

- links to password-protected Google Sheets that store the actual attendance data
- service-account authentication credentials for Google Sheets access
- deacon login credentials for app access

Those production credentials and private data sources are **not included** in this repository.

## Features

- Mobile-friendly Shiny interface
- Writes to two Google Sheets
- Updates a single row per date
- Automatically calculates attendance totals
- Includes app-level login protection
- Auto-refreshes saved values periodically
- Supports concurrent data entry with duplicate-row safeguards

## Security

Sensitive information such as:

- Google service-account JSON files
- private sheet links
- real usernames and passwords

has been excluded from this repository.
