Sallah Call Center Performance Analysis

A Power BI dashboard project for analyzing call center operations across February, March, and April 2022. The repository includes the Power BI report and the monthly CSV files used as its source data.

## Project Files

- `Sallah-project.pbix` — Power BI report and data model.
- `Sallah Call Center Data Base - Feb.csv` — February 2022 call center records.
- `Sallah Call Center Data Base - Mar .csv` — March 2022 call center records.
- `Sallah Call Center Data Base -Apr.csv` — April 2022 call center records.
- `images/` — project images and screenshots.

## Analysis Scope

The data contains daily records for Project A, with agent-level information and operational call metrics. The available fields include:

- Forecasted calls and calls offered.
- Calls handled and calls handled within threshold.
- Abandoned calls.
- ASA (Average Speed of Answer) and answer time.
- Agent name, project, date, and month.

These fields can be used to review demand versus forecast, call handling, service levels, abandonment, and agent activity over time.

## Requirements

- Microsoft Power BI Desktop to open and interact with the `.pbix` report.
- A spreadsheet application or text editor to inspect the CSV source files.

## Open the Report

1. Clone or download this repository.
2. Open `Sallah-project.pbix` in Power BI Desktop.
3. If prompted, review the report's data source settings and point them to the CSV files in your local copy of the repository.
4. Refresh the data if needed, then use the report filters and visuals to explore the results.

## Data Format

Each monthly CSV file uses the same columns:

| Column | Description |
|---|---|
| `Project` | Project or call center group |
| `Date` | Date of the daily record |
| `Month` | Reporting month |
| `Forecasted Calls` | Forecasted call volume |
| `Calls Offered` | Calls offered to the call center |
| `Calls Handled` | Calls handled by agents |
| `Calls Handled With in Thrshold` | Calls handled within the configured service threshold (column name as supplied in the source data) |
| `Calls Abandon` | Calls abandoned before being handled |
| `ASA` | Average Speed of Answer |
| `Answer Time` | Answer time value recorded in the source data |
| `Agent Name` | Agent associated with the record |

## Notes

- The CSV files are the source data for the February–April 2022 reporting period.
- Column names are preserved as they appear in the supplied data, including `Calls Handled With in Thrshold`.
- The report's exact calculations and units should be checked in Power BI before interpreting ASA, answer time, or service-threshold results.
