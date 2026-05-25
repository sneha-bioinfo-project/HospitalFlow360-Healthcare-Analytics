# HospitalFlow360 | End-to-End Healthcare Analytics Project

HospitalFlow360 is an end-to-end healthcare analytics project built using **Python, SQL, Excel, and Power BI**.  
It simulates hospital operations through synthetic data and analyzes key business areas such as **appointments, admissions, billing, no-shows, readmissions, revenue leakage, department performance, and doctor efficiency**.

The project was designed to demonstrate a complete analytics workflow:
**data generation → data cleaning → SQL analysis → Excel dashboarding → Power BI modeling → executive reporting**.

---

## Project Objectives

- Build a realistic synthetic healthcare dataset for operational analytics
- Analyze appointment behavior, no-show patterns, and department performance
- Track admissions, readmissions, and length of stay
- Identify revenue leakage through billing and payment logic
- Create interactive dashboards in Excel and Power BI
- Apply data modeling, KPI development, and business intelligence techniques

---

## Dataset Overview

The project includes the following core tables:

- **Patients**: 5,000 records
- **Doctors**: 40 records
- **Departments**: 8 records
- **Calendar**: 3 years of dates
- **Appointments**: 12,000 records
- **Admissions**
- **Billing**

The datasets were generated using Python with realistic business rules and linked across tables for analysis.

---

## Tech Stack

- **Python**
  - pandas
  - NumPy
  - Faker
  - Matplotlib
  - Seaborn
  - ydata-profiling

- **SQL**
  - Joins
  - Aggregations
  - CTEs
  - Window Functions
  - Conditional Logic
  - Date Calculations

- **Excel**
  - Pivot Tables
  - Pivot Charts
  - Slicers
  - Timelines
  - VBA Macros
  - Dashboard Design

- **Power BI**
  - Star Schema Modeling
  - Fact and Dimension Tables
  - DAX Measures
  - Time Intelligence
  - KPI Dashboards

---

## Python: Data Generation & Preparation

Python was used to build the foundation of the project by creating synthetic hospital data and preparing it for analysis.

### What was done
- Generated hospital master and transactional tables
- Simulated appointment, admission, and billing behavior using business logic
- Created derived features such as:
  - Age bands
  - Time bands
  - Stay bands
  - Booking gap days
  - Weekend flags
  - Appointment month
  - Appointment day name
  - Revenue loss flag
- Performed data quality checks
- Removed duplicates
- Standardized text fields
- Exported raw and cleaned datasets
- Created a data dictionary
- Generated a profiling report for exploratory validation

### Key business logic modeled
- No-show probability based on patient and appointment patterns
- Readmission probability based on age, department, stay length, and admission type
- Billing logic with discounts, claim status, payment status, and revenue loss flags

---

## SQL: Operational Analytics

SQL was used to extract healthcare insights from the structured datasets.

### Analyses performed
- Missing insurance information check
- Negative length of stay validation
- Duplicate appointment detection
- Department-wise appointment volume analysis
- No-show rate analysis by department
- No-show rate analysis by appointment time band
- Readmission analysis using CTEs and window functions
- Revenue leakage analysis tied to appointment no-shows
- Doctor efficiency analysis using average length of stay

### SQL concepts used
- `SELECT`
- `WHERE`
- `JOIN`
- `GROUP BY`
- `HAVING`
- `CASE WHEN`
- `CTE`
- `LEAD`
- Aggregate functions
- Date calculations

---

## Excel: Dashboard & Automation

Excel was used to create an interactive business intelligence dashboard for healthcare operations analysis.

### What was done
- Built Pivot Tables and Pivot Charts
- Created dashboard visuals for operational metrics
- Added Slicers and Timelines for filtering
- Used formulas such as:
  - `IF`
  - `IFS`
  - `TEXT`
  - logical operators
- Created derived categories like age bands and appointment month labels
- Built VBA macros for:
  - Pivot refresh automation
  - Data validation checks
  - Length-of-stay anomaly checks
  - PDF export workflow

### Dashboard focus
- Appointment trends
- Department performance
- Patient segmentation
- Revenue leakage tracking
- Operational KPI reporting

---

## Power BI: Modeling & KPI Reporting

Power BI was used to structure the project into a clean analytical model and build executive-style reporting.

### Data modeling
A **star schema** was created using:
- **FactBilling**
- **FactAdmissions**
- **FactAppointments**
- **DimDoctor**
- **DimPatient**
- **DimDepartment**
- **DimCalendar**

A dedicated **_Measure** table was used to store DAX calculations in an organized way.

### DAX measures created
- Total Revenue
- Total Appointments
- Avg Billing per Admission
- Admissions YTD
- Appointments MoM Growth

### Power BI focus
- KPI cards
- Trend analysis
- Department-level insights
- Insurance distribution
- Revenue and appointment performance
- Time-intelligence calculations

---

## Key Insights Covered

- Appointment no-show patterns
- Readmission behavior
- Revenue leakage from operational gaps
- Department performance differences
- Doctor efficiency by length of stay
- Billing and claim behavior
- Patient demographic segmentation

---

## Project Structure

```text
HospitalFlow360/
├── python/
├── sql/
├── excel/
├── powerbi/
├── data/
├── docs/
├── screenshots/
└── README.md
