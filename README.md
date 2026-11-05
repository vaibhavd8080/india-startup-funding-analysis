# India Startup Funding Analysis — Excel Dashboard

An end-to-end **Microsoft Excel** project analysing **3,044 Indian startup funding records** from 2 January 2015 to 13 January 2020. The workbook includes a documented cleaning process, PivotTables, PivotCharts and an executive dashboard.

## Dashboard Preview

![India Startup Funding Executive Dashboard](images/executive-dashboard.png)

## Project Objective

Explore reported startup funding activity in India and answer:

- How much funding was reported, and how did it change over time?
- Which industries, cities and startups received the most reported funding?
- How is funding distributed across investment types?
- Which investor entries appear most frequently?

## Dataset

- **Records:** 3,044 funding records
- **Period:** 2 January 2015 – 13 January 2020
- **Currency:** USD
- **Source:** [Indian Startup Funding Dataset — Kaggle](https://www.kaggle.com/datasets/sudalairajkumar/indian-startup-funding)

## Workbook Structure

| Sheet | Purpose |
|---|---|
| `Raw_Data` | Original source data, preserved separately |
| `Cleaned_Data` | Cleaned dataset and analysis helper columns |
| `Pivot_Analysis` | Seven PivotTables used for analysis |
| `Executive_Dashboard` | KPI cards, five PivotCharts and written insights |
| `Cleaning_Log` | Documented data-cleaning decisions |
| `Data_Dictionary` | Column definitions |

## Data Preparation

Cleaning decisions are documented in the workbook's `Cleaning_Log` sheet.

- Standardised column headers and preserved `Sr_No` as the source record identifier.
- Removed non-printing characters and normalised whitespace.
- Parsed dates and repaired eight malformed date strings.
- Standardised selected investment type, industry and city labels.
- Replaced missing categorical values with `Unknown`.
- Converted reported funding amounts to numeric values; unavailable amounts remain blank.
- Preserved the source qualifier for one amount in a separate field.
- Checked for duplicate identifiers and exact duplicate rows; repeated startup names were retained because they may represent separate funding rounds.

## Analysis

The workbook contains seven PivotTables:

1. Total reported funding
2. Year-wise funding
3. Top 10 industries by reported funding
4. Top 10 cities by reported funding
5. Top 10 funded startups
6. Funding by investment type
7. Most frequent investor entries

The executive dashboard presents KPI cards and five PivotCharts for the main comparisons.

## Key Findings

1. **Bengaluru leads** with approximately $18.5B, or 48.5% of reported funding.
2. **2017 was the peak year** at approximately $10.4B.
3. **Private Equity represents about 70%** of reported funding (approximately $26.7B).
4. The number of recorded deals declined after 2016, while the median reported deal size increased. Changes in reporting coverage may partly explain this pattern.
5. **Flipkart is the top funded startup** in this dataset at approximately $4.06B.

## Data Limitations

- **971 of 3,044 records (31.9%) have no reported amount.** Funding totals therefore describe only records with reported amounts.
- The 2020 data ends on 13 January 2020; it is not a complete year.
- The Rapido Bike Taxi $3.9B Series B entry appears unusual and may be a source-data error. It has been retained and affects related totals and rankings.
- Startup name variants such as Flipkart and Flipkart.com were not merged.

## Tools & Skills

Microsoft Excel, Power Query, PivotTables, PivotCharts, `GETPIVOTDATA`, `SUMPRODUCT`, `COUNTIF`, helper columns, dashboard design and data documentation.

## Repository Structure

```text
india-startup-funding-analysis/
├── README.md
├── India_Startup_Funding_Dashboard.xlsx
├── data/
│   └── startup_funding_raw.xlsx
├── docs/
│   └── India_Startup_Funding_Dashboard.pdf
└── images/
    └── executive-dashboard.png
```

## Open the Project

- [Download the Excel workbook](India_Startup_Funding_Dashboard.xlsx)
- [View the dashboard PDF](docs/India_Startup_Funding_Dashboard.pdf)
- [View the raw dataset file](data/startup_funding_raw.xlsx)

Open the workbook in **Microsoft Excel desktop** for the full PivotTable and PivotChart experience. Browser previews may not display all workbook features.

## Author

**Vaibhav Deshmukh**  
[GitHub Profile](https://github.com/vaibhavd8080)
