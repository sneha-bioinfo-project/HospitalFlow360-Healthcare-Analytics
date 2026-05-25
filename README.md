# HospitalFlow360

## End-to-End Healthcare Analytics Project

<p align="center">
  <img src="screenshots/powerbi_dashboard.png" alt="HospitalFlow360 dashboard preview" width="950">
</p>

<p align="center">
  <b>Python • SQL • Excel • Power BI • DAX • Healthcare Analytics</b>
</p>

---

## Project Overview

**HospitalFlow360** is an end-to-end healthcare analytics project built with **Python, SQL, Excel, and Power BI**. It simulates hospital operations through synthetic data and analyzes core business areas such as **appointments, admissions, billing, no-shows, readmissions, department performance, and revenue leakage**.

The project demonstrates a complete analytics workflow:

**Data Generation → Data Cleaning → SQL Analysis → Excel Dashboarding → Power BI Modeling → Executive Reporting**

---

## Business Objectives

* Create a realistic synthetic healthcare dataset for analytics practice and portfolio presentation
* Analyze appointment behavior, no-show patterns, and department performance
* Track admissions, readmissions, and length of stay
* Identify revenue leakage through billing and payment logic
* Build interactive dashboards in Excel and Power BI
* Apply data modeling, KPI development, and business intelligence techniques

---

## Tech Stack

| Category        | Tools & Technologies |
| --------------- | -------------------- |
| Programming     | Python               |
| Data Analysis   | pandas, NumPy        |
| Data Generation | Faker                |
| Visualization   | Matplotlib, Seaborn  |
| Profiling       | ydata-profiling      |
| Querying        | SQL                  |
| Dashboarding    | Excel, Power BI      |
| BI Modeling     | DAX, Star Schema     |
| Automation      | VBA Macros           |

---

## Dataset Overview

The project includes the following core tables:

| Table        | Purpose                                    |
| ------------ | ------------------------------------------ |
| Patients     | Patient demographics and insurance details |
| Doctors      | Doctor details and department mapping      |
| Departments  | Hospital department structure              |
| Calendar     | Date dimension for reporting               |
| Appointments | Appointment transactions                   |
| Admissions   | Admission records                          |
| Billing      | Financial and payment records              |

### Generated Scale

* **5,000** patient records
* **40** doctor records
* **8** department records
* **3 years** of calendar dates
* **12,000** appointment records
* Admission and billing records linked for operational analysis

---

## Repository Structure

```text
HospitalFlow360/
├── python/
│   ├── HospitalFlow360_DataGeneration.ipynb
│   ├── appointments_profile_report.html
│   └── requirements.txt
├── sql/
│   ├── data_quality_analysis.sql
│   ├── department_performance_analysis.sql
│   ├── no_show_analysis.sql
│   ├── readmission_analysis.sql
│   ├── revenue_leakage_analysis.sql
│   └── doctor_efficiency_analysis.sql
├── excel/
│   └── HospitalFlow360_ExcelDashboard.xlsx
├── powerbi/
│   └── HospitalFlow360.pbix
├── data/
│   ├── raw/
│   └── cleaned/
├── docs/
│   └── data_dictionary.csv
├── screenshots/
│   ├── excel_dashboard.png
│   ├── powerbi_dashboard.png
│   └── data_model.png
└── README.md
```

---

## Python: Data Engineering & Preparation

Python was used to build the foundation of the project by generating, validating, and preparing the healthcare datasets.

### What was done

* Generated synthetic healthcare tables
* Linked patients, doctors, departments, appointments, admissions, and billing records
* Created derived fields for analytics
* Performed data cleaning and validation
* Removed duplicates
* Standardized text fields
* Exported raw and cleaned datasets
* Built a data dictionary
* Created a profiling report for exploratory validation

### Features engineered

* Age bands
* Time bands
* Stay bands
* Booking gap days
* Weekend flags
* Appointment month
* Appointment day name
* Revenue loss flag

### Business logic simulated

* Appointment no-show probability
* Booking gap influence
* Insurance influence
* Follow-up appointment behavior
* Readmission probability
* Length of stay generation
* Billing discounts
* Payment status logic
* Insurance claim status logic

---

## SQL: Operational Analytics

SQL was used to evaluate healthcare operations and derive business insights from the structured dataset.

### Analyses performed

* Missing insurance information check
* Negative length of stay validation
* Duplicate appointment detection
* Department-wise appointment volume analysis
* No-show rate by department
* No-show rate by appointment time band
* Readmission analysis using CTEs and window functions
* Revenue leakage estimation from no-shows
* Doctor efficiency analysis using average length of stay

### SQL concepts used

* `SELECT`
* `WHERE`
* `JOIN`
* `GROUP BY`
* `HAVING`
* `CASE WHEN`
* `CTE`
* `LEAD`
* Aggregate functions
* Date calculations

---

## Excel: Dashboard & Automation

Excel was used to create an interactive healthcare operations dashboard.

### What was done

* Built Pivot Tables and Pivot Charts
* Created dashboard visuals for operational metrics
* Added Slicers and Timelines for filtering
* Used formulas such as `IF`, `IFS`, `TEXT`, and logical operators
* Created derived categories such as age bands and appointment month labels
* Built VBA macros for automation tasks

### VBA automation included

* Pivot refresh automation
* Data validation checks
* Length-of-stay anomaly checks
* One-click PDF export workflow

### Dashboard focus

* Appointment trends
* Department performance
* Patient segmentation
* Revenue leakage tracking
* Operational KPI reporting

<p align="center">
  <img src="screenshots/excel_dashboard.png" alt="Excel dashboard preview" width="950">
</p>

---

## Power BI: Modeling & KPI Reporting

Power BI was used to structure the project into a clean analytical model and build executive-style reporting.

### Data modeling

A **star schema** was built using:

**Fact Tables**

* FactBilling
* FactAdmissions
* FactAppointments

**Dimension Tables**

* DimDoctor
* DimPatient
* DimDepartment
* DimCalendar

A dedicated **_Measure** table was used to store DAX calculations in an organized way.

### DAX measures created

* Total Revenue
* Total Appointments
* Avg Billing per Admission
* Admissions YTD
* Appointments MoM Growth

### Power BI focus

* KPI cards
* Trend analysis
* Department-level insights
* Insurance distribution
* Revenue and appointment performance
* Time-intelligence calculations

<p align="center">
  <img src="screenshots/data_model.png" alt="Power BI data model preview" width="950">
</p>

---

## Key Analyses Covered

* Appointment no-show patterns
* Readmission behavior
* Revenue leakage from operational gaps
* Department performance differences
* Doctor efficiency by length of stay
* Billing and claim behavior
* Patient demographic segmentation

---

## Skills Demonstrated

### Data Engineering

* Data Cleaning
* Feature Engineering
* Synthetic Data Generation
* Data Validation
* CSV Export

### SQL Analytics

* Operational Analytics
* KPI Analysis
* Window Functions
* CTEs
* Joins
* Aggregations

### Business Intelligence

* Dashboard Development
* Data Modeling
* DAX
* KPI Reporting
* Interactive Visualizations

### Healthcare Analytics

* No-show Analysis
* Readmission Tracking
* Revenue Leakage Analysis
* Department Performance Monitoring
* Doctor Efficiency Analysis

---

## Screenshots

### Excel Dashboard

<p align="center">
  <img src="screenshots/excel_dashboard.png" alt="Excel dashboard screenshot" width="950">
</p>

### Power BI Dashboard

<p align="center">
  <img src="screenshots/powerbi_dashboard.png" alt="Power BI dashboard screenshot" width="950">
</p>

### Data Model

<p align="center">
  <img src="screenshots/data_model.png" alt="Power BI data model screenshot" width="950">
</p>

---

## Files Included

* Python notebook for synthetic data generation and preparation
* SQL scripts for healthcare analytics
* Excel dashboard workbook
* Power BI report file
* Data dictionary
* Dashboard screenshots
* Profiling report

---

## Notes

* This project uses **synthetic healthcare data** created for portfolio and learning purposes.
* No real patient data is included.
* The project demonstrates an end-to-end analytics workflow across multiple tools.

---

## Contact

**Sneha S**

Healthcare Analytics | Data Analytics | Business Intelligence
