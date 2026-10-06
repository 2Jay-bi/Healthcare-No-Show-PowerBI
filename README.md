# Healthcare Appointment and No-Show Operations Dashboard

![Healthcare Appointment and No-Show Operations Dashboard](images/Healthcare%20Appointments%20and%20No%20show%20Operations%20Dashboard.png)

## Project Overview

This Power BI dashboard analyzes patient appointment activity, attendance, no-shows, visit duration, waiting time, facility performance, and geographic utilization. It gives healthcare leaders an interactive view of operational performance and helps identify opportunities to improve scheduling, patient access, and facility capacity.

## Business Questions

The dashboard answers the following questions:

- How many appointments were scheduled, attended, and missed?
- What is the overall no-show rate?
- How are operational KPIs changing quarter over quarter?
- Which quarters experienced the largest changes in appointment performance?
- How do visit duration and waiting time vary by visit type?
- Which facilities combine high appointment volume with high no-show rates?
- Which visit types contribute to facility performance differences?
- How closely do scheduled time and actual waiting time align?
- Where are appointments geographically concentrated?
- Which facilities or services should leadership prioritize for operational improvement?

## Dataset Summary

| Metric | Result |
|---|---:|
| Original encounter records | 10,018 |
| Cleaned unique appointments | 10,000 |
| Dashboard reporting period | Q1 2023–Q4 2025 |
| Appointments in dashboard period | 9,757 |
| Attended appointments | 8,985 |
| No-shows | 772 |
| Overall no-show rate | 7.91% |
| Average visit duration | 48.30 minutes |
| Average wait time | 47.78 minutes |
| Synthetic patients | 3,811 |
| Providers | 120 |
| Facilities | 25 |

> This project uses fully synthetic data created for educational and portfolio purposes. It contains no real patient information, personally identifiable information, or protected health information.

## Dashboard KPIs

The dashboard presents six primary KPIs:

- Total Appointments
- Total Attended
- Average Visit Duration
- Total No-Shows
- No-Show Rate
- Average Wait Time

Each KPI includes a quarter-over-quarter sub-KPI and a directional arrow. KPI and sub-KPI colors match the corresponding chart metric when that metric is represented in a visual. Metrics not directly represented in a chart remain black. Red and green are reserved for directional arrows.

## Dashboard Visuals

### Quarterly Appointment Volume and QoQ Operational Performance

This combination chart displays Total Appointments by quarter together with quarter-over-quarter changes in:

- Total Attended
- Total No-Shows
- Average Wait Time

The visual helps leadership monitor appointment demand and identify quarters with significant operational changes.

### Visit Operations by Visit Type

This chart compares:

- Average Visit Duration
- Average Wait Time
- Total No-Shows QoQ %
- Average Visit Duration QoQ %

The chart shows how operational performance differs across follow-up, primary care, behavioral health, care coordination, urgent care, telehealth, preventive visits, and specialist consultations.

### Facility Volume vs. No-Show Performance

This scatter plot compares facilities using:

- **X-axis:** Total Appointments
- **Y-axis:** No-Show Rate
- **Bubble size:** Total No-Shows
- **Bubble color:** Visit Type
- **Label:** Facility or City

The visual identifies facilities that combine high appointment demand with elevated no-show rates. Users can drill up and down between city and facility levels for additional detail.

### Average Wait Time vs. Scheduled Time by Visit Type

This scatter plot compares average scheduled minutes with average wait time for each visit type. It helps identify services where waiting time may not align with the scheduled appointment duration.

### Facility Utilization Map

The map displays the geographic distribution of healthcare facilities. Bubble shading represents Total Appointments using a Low-to-High color gradient, making it easier to identify areas with higher facility utilization.

## Dashboard Interactivity

The dashboard includes:

- Quarter-Year filtering
- Cross-filtering between visuals
- Hover tooltips
- Drill-through from the facility scatter plot and map
- Drill up and drill down between city and facility
- Facility-level appointment and no-show details
- Consistent visit-type colors across related visuals

These features allow users to move from a high-level operational summary to more detailed facility and service-level analysis.

## Data Preparation

The dataset was prepared using Python, pandas, Power Query, and Power BI. The main preparation steps included:

1. Profiling missing values, duplicate records, and inconsistent data types.
2. Removing 18 duplicate encounter IDs.
3. Standardizing patient, provider, and facility identifiers.
4. Correcting inconsistent visit-type and visit-mode labels.
5. Converting numeric fields stored as text.
6. Recovering and standardizing mixed-format encounter dates.
7. Creating appointment-status and no-show target fields.
8. Creating date, quarter, month, and age-group attributes.
9. Creating a dedicated date dimension.
10. Building a star-schema data model.
11. Creating DAX measures for KPIs and quarter-over-quarter performance.
12. Validating dashboard totals against facility and quarterly validation tables.

## Tools and Skills Demonstrated

- Power BI Desktop
- Power Query
- DAX
- Python and pandas
- Data cleaning and transformation
- Star-schema data modeling
- KPI and QoQ calculations
- Interactive filtering
- Tooltips and drill-through
- Drill-up and drill-down navigation
- Geographic analysis
- Data validation
- Healthcare operations analysis
- Dashboard design and business storytelling

## Key Findings

- The dashboard contains 9,757 appointments for the Q1 2023–Q4 2025 reporting period.
- A total of 8,985 appointments were attended, while 772 resulted in no-shows.
- The overall no-show rate was 7.91%.
- Average visit duration was 48.30 minutes, while average wait time was 47.78 minutes.
- Appointment volume remained relatively stable across most quarters but showed noticeable quarter-over-quarter changes in attendance, no-shows, and waiting time.
- Visit duration and waiting time varied across visit types, indicating opportunities for service-specific scheduling improvements.
- Facility no-show rates varied even among facilities with similar appointment volumes.
- The facility scatter plot helps identify locations where high volume and elevated no-show rates create the greatest operational impact.
- Geographic utilization is concentrated across several major metropolitan areas, supporting location-based capacity and outreach planning.

## Business Recommendations

- Prioritize facilities that combine high appointment volume, high no-show rates, and large no-show counts.
- Use automated reminders for broad, lower-cost no-show prevention.
- Apply targeted outreach to higher-risk facilities and visit types.
- Review services where average waiting time is close to or greater than scheduled appointment duration.
- Compare quarterly performance after interventions to determine whether no-show rates and waiting times improve.
- Use drill-through details to investigate facility-specific scheduling and patient-access issues.

## Operational Value

The dashboard gives healthcare administrators, scheduling teams, facility managers, and patient-outreach coordinators a centralized view of appointment performance. It supports capacity planning, facility comparison, scheduling improvement, patient-access analysis, and data-driven prioritization of no-show reduction initiatives.

## Important Limitation

The dataset is synthetic, so the findings demonstrate data preparation, analytical reasoning, Power BI development, and healthcare operations analysis rather than the performance of a real healthcare organization. The dashboard identifies descriptive relationships and historical patterns but does not establish causation..
## Data Sources

* [Synthea Synthetic Patient Data](https://synthetichealth.github.io/synthea/)
* [CMS Provider Data](https://data.cms.gov/provider-data/)
* [CDC PLACES](https://www.cdc.gov/places/)

## Author

**Vestine Nimenya**

* [LinkedIn](https://www.linkedin.com/in/vestine-nimenya-17188b267/)
* [GitHub](https://github.com/2Jay-bi)
