# U.S. Higher Education Institutional Analysis

## Project Overview

This project analyzes U.S. higher education institutions using 2024 IPEDS data to examine enrollment patterns, financial aid participation, and student outcomes across different institution types and levels.

The project combines SQL-based data preparation and analysis with an interactive Power BI dashboard that allows users to explore national patterns and individual institutions.

## Research Questions

1. How do enrollment patterns differ across institution types and sizes?
2. How does financial aid participation vary across institution types?
3. How do graduation outcomes differ across institution types and institutional levels?
4. How do graduation rates vary across levels of Pell Grant participation?

## Tools Used

- SQL Server
- Power BI
- Power Query
- DAX
- IPEDS 2024 Data


## Methodology
Four IPEDS datasets were integrated using the institution-level `UNITID` identifier:

- **HD2024 – Institutional Characteristics:** institution name, state, control, level, and size
- **DRVEF2024 – Fall Enrollment:** total, full-time, and part-time enrollment
- **SFA2324 – Student Financial Aid:** Pell Grant, grant aid, and federal student loan participation
- **DRVGR2024 – Graduation Rates:** graduation and transfer-out rates

The datasets were profiled and validated before analysis. SQL Server was used to assess data coverage, join the four datasets, filter IPEDS special/missing values, and create a reusable analytical view for Power BI.

The analysis then examined enrollment patterns, financial aid participation, graduation and transfer-out outcomes, and differences in graduation rates across levels of Pell Grant participation.


## Key Findings
### -- 1) Enrollment Patterns
Average enrollment increased substantially with institution size across all institution types. Among the largest institutions, average total enrollment was 35,072 at public institutions, 45,907 at private nonprofits, and 50,405 at private for-profits. Public institutions also showed a larger part-time enrollment presence across several size categories.

### --2) Financial Aid Participation
Average Pell Grant participation was 33.7% at public institutions, 37.3% at private nonprofits, and 55.6% at private for-profits. Private for-profit institutions also had the highest average federal student loan participation, while private nonprofits had the highest average grant-aid participation.

### --3) Graduation and Transfer-Out Outcomes
Graduation and transfer-out outcomes varied by both institution type and level. Among four-year institutions, average graduation rates were 45.4% for public, 53.4% for private nonprofit, and 42.0% for private for-profit institutions. This differed from the aggregate results, demonstrating how institutional composition can affect comparisons.

### --4) Pell Participation and Graduation
Institutions with lower Pell participation averaged a 62.1% graduation rate, compared with 54.1% for moderate-Pell institutions and 59.5% for higher-Pell institutions. The pattern was not linear, suggesting that Pell participation alone does not explain differences in institutional graduation outcomes.

## Dashboard

The interactive Power BI dashboard includes:

- Total enrollment and institution counts
- Average Pell Grant participation
- Average graduation rates
- Full-time and part-time enrollment by institution type
- Financial aid participation by institution type
- Graduation rates by Pell participation
- Graduation rates by institution type and level
- Filters for state, institution type, and institution level
- An institution-level detail page

### [View Interactive Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNTU3NTEyY2QtYjMwMy00MjEyLThmMGUtNTcxMzdjNzA3NDhiIiwidCI6Ijk1ZjA3NGI4LWFiZWQtNGZkZC05MTk4LWIwN2I4YmQ0ZGJjOSIsImMiOjZ9)

## Data Source

Data was obtained from the U.S. Department of Education's Integrated Postsecondary Education Data System (IPEDS), using the 2024 institutional dataset.

## Repository Contents

- SQL queries used for data preparation and analysis
- Power BI dashboard
- Project documentation

## Author

Verse Iyorkar
