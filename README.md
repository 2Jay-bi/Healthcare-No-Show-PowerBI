# Healthcare Appointment and No-Show Operations Dashboard

![Healthcare Appointment and No-Show Operations Dashboard](Healthcare_Noshow_Operations%20Analysis.png)

## Business Questions

The dashboard answers the following questions:

- How many appointments were scheduled, attended, and missed?
- What is the overall no-show rate?
- How are the KPIs changing quarter over quarter?
- How do appointment volume and no-show rate change over time?
- Which facilities have higher appointment volumes and no-show rates?
- How are appointments distributed across visit modes?
- Which visit types, diagnoses, payers, facilities, and access barriers appear most frequently among historical no-shows?
- Where should healthcare leaders focus scheduling and patient-access improvements?

## Dataset Summary

| Metric | Result |
|---|---:|
| Original encounter records | 10,018 |
| Cleaned unique appointments | 10,000 |
| Synthetic patients | 3,811 |
| Providers | 120 |
| Facilities | 25 |
| Attended appointments | 9,202 |
| No-shows | 798 |
| Overall no-show rate | 7.98% |
| Average wait time | 47.7 minutes |
| Historical period | Dec. 2022–Dec. 2025 |

> This project uses fully synthetic data created for educational and portfolio purposes. It contains no real patient information, personally identifiable information, or protected health information.

## Dashboard KPIs

The dashboard presents the following primary KPIs:

- Total Appointments
- Total Attended
- Total No-Shows
- No-Show Rate
- Average Wait Time

Each KPI includes a quarter-over-quarter sub-KPI and a directional arrow. KPI values use neutral colors, while green and red are used only for arrows that indicate improvement or decline.

## Dashboard Visuals

### Monthly Appointment Volume and No-Show Rate

A combination chart compares monthly appointment volume with the historical no-show rate. It helps identify demand changes, seasonal patterns, and months with elevated missed-appointment rates.

### Facility Volume and No-Show Performance

A scatter chart compares facility appointment volume with no-show rate. It helps identify facilities with high demand, high no-show rates, or both.

### Appointment Distribution by Visit Mode

A donut chart shows the distribution of appointments across in-person, telehealth, and home-visit services.

### Historical No-Show Breakdown

A decomposition tree allows users to analyze historical no-shows by:

- Visit type
- Diagnosis
- Visit mode
- Payer
- Facility
- Transportation barrier
- Food-insecurity status

### Quarter-Year Filter

The Quarter-Year slicer filters the dashboard and supports historical and quarter-over-quarter analysis.

## Data Preparation

The dataset was prepared using Python, pandas, Power Query, and Power BI. Major preparation steps included:

1. Profiling missing values, duplicates, and inconsistent data types.
2. Removing 18 duplicate encounter IDs.
3. Standardizing identifiers and categorical values.
4. Correcting inconsistent visit-type and visit-mode labels.
5. Converting numeric fields stored as text.
6. Recovering and standardizing mixed-format encounter dates.
7. Creating an appointment-status field.
8. Creating date, quarter, month, and age-group attributes.
9. Building a star-schema data model in Power BI.
10. Validating dashboard totals against the cleaned source data.

## Tools and Skills Demonstrated

- Power BI Desktop
- Power Query
- DAX
- Data modeling and star-schema design
- Python and pandas
- Data cleaning and transformation
- KPI and QoQ calculations
- Interactive filtering
- Data validation
- Healthcare operations analysis
- Dashboard design and storytelling

## Key Findings

- The dataset contains 10,000 historical appointments.
- A total of 9,202 appointments were attended.
- There were 798 no-shows, producing an overall no-show rate of 7.98%.
- The average patient wait time was 47.7 minutes.
- Appointment volume and no-show rates varied across months and facilities.
- Visit mode, visit type, payer, diagnosis, facility, and access barriers provide useful dimensions for investigating historical no-show patterns.

## Operational Value

The dashboard gives healthcare leaders a centralized historical view of appointment performance. It can support scheduling reviews, capacity planning, facility comparisons, patient-access analysis, and the identification of areas where reminder processes or operational support may need improvement.

## Important Limitation

The data is synthetic, so the findings demonstrate analytical and Power BI development capabilities rather than performance at a real healthcare organization. The dashboard identifies descriptive relationships and historical patterns but does not establish causation.
## Data Sources

* [Synthea Synthetic Patient Data](https://synthetichealth.github.io/synthea/)
* [CMS Provider Data](https://data.cms.gov/provider-data/)
* [CDC PLACES](https://www.cdc.gov/places/)

## Author

**Vestine Nimenya**

* [LinkedIn](https://www.linkedin.com/in/vestine-nimenya-17188b267/)
* [GitHub](https://github.com/2Jay-bi)
