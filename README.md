

## Project Overview

This project uses Power BI to examine patient appointment no-shows.The dashboard supports quarter-over-quarter monitoring of appointment volume, attendance, no-shows, no-show rate, and average wait time. Monthly trends reveal fluctuations in demand and missed appointments, while facility comparisons help identify locations that combine high appointment volume with elevated no-show rates. Visit-mode distribution and the historical no-show breakdown provide additional context for understanding how no-shows vary by visit type, diagnosis, payer, facility, transportation barriers, and food insecurity.
## Dashboard Overview

![Healthcare_Noshow_Operations Analysis](images/Healthcare_Noshow_Operations Analysis.png)

## Business Problem

Patient no-shows create unused provider capacity, scheduling inefficiencies, revenue losses, and delays in patient care.

## Project Objective

Identify the appointments, facilities, and time periods that should be prioritized to reduce patient no-shows and improve healthcare operations.

## Tools Used

* Power BI
* Power Query
* DAX
* SQL
* Python
* Google Colab
* Excel
* Azure Maps

## Project Workflow

1. Extracted and reviewed the healthcare data.
2. Cleaned, filtered, and transformed the data.
3. Removed duplicates and handled missing values.
4. Created fact and dimension tables.
5. Established relationships using a star schema.
6. Developed DAX measures and calculated columns.
7. Prepared and evaluated a patient no-show prediction model.
8. Built an interactive Power BI dashboard.
9. Generated business insights and recommendations.

## Dashboard Features

* Date, facility, visit type, and payer slicers
* KPI cards
* Azure Map
* Year, quarter, and month drill-down
* Decomposition tree
* Facility performance matrix
* Conditional formatting
* Cross-filtering
* Drill-through
* Report-page tooltips
* Predictive risk analysis

## Dataset

This project uses a custom synthetic healthcare dataset inspired by publicly available information from Synthea, CMS, and CDC. It contains no real patient-identifying information and is intended for educational and portfolio purposes.

## Data Sources

* [Synthea Synthetic Patient Data](https://synthetichealth.github.io/synthea/)
* [CMS Provider Data](https://data.cms.gov/provider-data/)
* [CDC PLACES](https://www.cdc.gov/places/)

## Author

**Vestine Nimenya**

* [LinkedIn](https://www.linkedin.com/in/vestine-nimenya-17188b267/)
* [GitHub](https://github.com/2Jay-bi)
