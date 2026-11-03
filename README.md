# Hotel Business Intelligence Dashboard

An interactive Hotel Business Intelligence solution developed using **Microsoft Power BI**, **Power Query** and **DAX** to analyse hotel performance, monitor key business metrics and support data-driven revenue management decisions.

## Project Overview

The project addresses the need for consolidated performance reporting to monitor hotel revenue, room occupancy and booking trends.

Hotel operational datasets were transformed, modelled and analysed to develop an interactive dashboard that provides visibility into key performance indicators (KPIs) and business performance trends.

### Business Problem

The need for consolidated performance reporting to monitor hotel revenue, room occupancy and booking trends, limiting the ability to effectively track performance and identify operational trends.

### Approach

Transformed and modelled hotel datasets using Power Query and a Star Schema data model. Developed DAX measures and calculated columns to analyse business performance and built an interactive dashboard with dynamic KPI filters.

### Outcome

Delivered an interactive reporting solution tracking Revenue, Occupancy Rate, Average Daily Rate (ADR), Revenue Per Available Room (RevPAR), Realisation and Daily Sellable Room Nights (DSRN), supporting operational and revenue management decisions.


## Technology Stack

| Technology | Application |
|---|---|
| Microsoft Power BI | Dashboard development and data visualisation |
| Power Query | Data extraction, cleaning and transformation |
| DAX | Calculated columns, measures and KPI calculations |
| Excel / CSV | Source data and supporting business metrics |

## Dataset Overview

The project uses five structured datasets:

| Dataset | Description |
|---|---|
| `dim_date.csv` | Date dimension for time-based analysis |
| `dim_hotels.csv` | Hotel properties and geographical information |
| `dim_rooms.csv` | Room identifiers and room classifications |
| `fact_bookings.csv` | Detailed hotel booking transactions |
| `fact_aggregated_bookings.csv` | Aggregated booking and room-capacity information |

Additional supporting files include hospitality metadata and an Excel metrics reference.

## Data Modelling

A Star Schema approach was implemented to organise the datasets and establish relationships between fact and dimension tables.

The model integrates hotel, room and date dimensions with booking and aggregated booking fact tables.


## Data Transformation and Analysis

### Power Query

- Imported structured CSV datasets into Power BI.
- Cleaned and transformed source data.
- Standardised column structures and data types.
- Prepared datasets for relational modelling and analysis.

### Data Modelling

- Implemented a Star Schema architecture.
- Established one-to-many relationships between dimension and fact tables.
- Connected date, hotel and room dimensions to the relevant fact tables.

### DAX Development

Developed calculated columns and measures to support business performance analysis.

Examples of calculated columns:

- Week Number: `WEEKNUM(dim_date[date])`
- Day Type: Categorised Friday and Saturday as weekends based on the hotel's business requirements.

Key measures and KPIs:

- Revenue
- Total Successful Bookings
- Occupancy %
- Average Daily Rate (ADR)
- Revenue Per Available Room (RevPAR)
- Realisation %
- Daily Sellable Room Nights (DSRN)

### Week-on-Week Analysis

Implemented Week-on-Week (WoW) change calculations to evaluate performance against the preceding week.

The analysis covers:

- Revenue WoW Change %
- Occupancy WoW Change %
- ADR WoW Change %
- RevPAR WoW Change %
- Realisation WoW Change %
- DSRN WoW Change %

These calculations support trend monitoring and comparison of hotel performance over time.

## Dashboard Features

- Interactive filtering by hotel city.
- Room category filtering.
- Monthly and weekly performance analysis.
- Dynamic KPI cards responding to selected filters.
- Hotel revenue and occupancy performance monitoring.
- Week-on-Week performance comparisons.

## Repository Structure

```text
hotel-business-intelligence-dashboard/
│
├── datasets/       # Source datasets and supporting metadata
├── dashboard/      # Power BI dashboard file
├── images/         # Dashboard preview and data model
├── report/         # Detailed project report
├── README.md
└── .gitignore
```

## Accessing the Project

1. Clone this repository.
2. Navigate to the `dashboard/` directory.
3. Open the `.pbix` file using Microsoft Power BI Desktop.
4. If prompted, configure the dataset source paths to match the local `datasets/` directory.

Refer to the `report/` directory for the detailed project documentation.

## Project Documentation

The accompanying report documents the business requirements, data preparation, data modelling, DAX development and dashboard implementation.

## Author

**Denis Kombe Karisa**

Data Analytics | Business Intelligence | ICT


---

*Developed as part of the Data and Artificial Intelligence programme, Cyber Shujaa, Week 4 Business Intelligence assignment. Learning resources: Codebasics.io.*
