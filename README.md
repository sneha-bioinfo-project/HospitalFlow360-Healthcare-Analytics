<h1 align="center">🏥 HospitalFlow360</h1>
<p align="center"><strong>End-to-End Healthcare Analytics Project</strong></p>
<p align="center">Python • SQL • Excel • Power BI • DAX</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Analytics-blue?style=for-the-badge&logo=python" alt="Python Badge" />
  <img src="https://img.shields.io/badge/SQL-Operational_Analytics-black?style=for-the-badge&logo=mysql" alt="SQL Badge" />
  <img src="https://img.shields.io/badge/Excel-Dashboarding-green?style=for-the-badge&logo=microsoft-excel" alt="Excel Badge" />
  <img src="https://img.shields.io/badge/Power_BI-DAX-yellow?style=for-the-badge&logo=powerbi" alt="Power BI Badge" />
</p>

<p align="center">
  <em>Built to demonstrate healthcare data engineering, analytics, dashboarding, and executive reporting across the full workflow.</em>
</p>

---

## 📌 Project Snapshot

| Metric         | Details                                                          |
| -------------- | ---------------------------------------------------------------- |
| Domain         | Healthcare Analytics                                             |
| Core Tools     | Python, SQL, Excel, Power BI                                     |
| Main Focus     | Appointments, Admissions, Billing, Readmissions, Revenue Leakage |
| Modeling Style | Star Schema in Power BI                                          |
| BI Outputs     | Excel Dashboard + Power BI Dashboard                             |
| Data Type      | Synthetic hospital operations data                               |

---

## 🔄 Analytics Workflow

```text
Python Data Generation
        ↓
Data Cleaning & Validation
        ↓
SQL Operational Analysis
        ↓
Excel Dashboarding & Automation
        ↓
Power BI Modeling & DAX
        ↓
Executive KPI Reporting
```

---

## 🧠 What This Project Covers

HospitalFlow360 simulates hospital operations and analyzes the performance of a healthcare system through structured datasets and BI outputs.

### Core analytical areas

* Appointment behavior
* No-show patterns
* Admissions and readmissions
* Billing and payment logic
* Revenue leakage
* Department performance
* Doctor efficiency

---

## 📊 Dataset Overview

| Table        | Purpose                                    |
| ------------ | ------------------------------------------ |
| Patients     | Patient demographics and insurance details |
| Doctors      | Doctor information and department mapping  |
| Departments  | Hospital department structure              |
| Calendar     | Date dimension for analysis                |
| Appointments | Appointment transactions                   |
| Admissions   | Admission records                          |
| Billing      | Financial and payment records              |

### Generated scale

* 5,000 patient records
* 40 doctor records
* 8 departments
* 3 years of calendar dates
* 12,000 appointment records
* Admissions and billing linked for downstream analysis

---

## 🐍 Python: Data Engineering & Preparation

Python was used to build the foundation of the project by generating and preparing the hospital datasets.

### What was done

* Created synthetic healthcare tables
* Linked patients, doctors, departments, appointments, admissions, and billing records
* Engineered derived fields for analysis
* Performed duplicate removal and data validation
* Standardized text fields
* Exported raw and cleaned datasets
* Created a data dictionary
* Generated a profiling report for exploratory validation

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

## 🗄️ SQL: Operational Analytics

SQL was used to evaluate healthcare operations and extract business insights from the structured datasets.

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

## 📈 Excel: Dashboard & Automation

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

---

## 📊 Power BI: Modeling & KPI Reporting

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

---

## 🔍 Key Analyses Covered

| Analysis                     | Purpose                                       |
| ---------------------------- | --------------------------------------------- |
| Appointment No-show Patterns | Understand missed appointment behavior        |
| Readmission Behavior         | Track repeat admissions within 30 days        |
| Revenue Leakage              | Estimate financial loss from operational gaps |
| Department Performance       | Compare workload across departments           |
| Doctor Efficiency            | Analyze average length of stay                |
| Billing & Claim Behavior     | Review payment and insurance outcomes         |
| Patient Segmentation         | Study demographic and insurance patterns      |

---

## 🧰 Skills Demonstrated

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

## 📁 Repository Structure

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
```

---

## 📦 Files Included

* Python notebook for synthetic data generation and preparation
* SQL scripts for healthcare analytics
* Excel dashboard workbook
* Power BI report file
* Data dictionary
* Dashboard screenshots
* Profiling report

---

## 📝 Notes

* This project uses **synthetic healthcare data** created for portfolio and learning purposes.
* No real patient information is included.
* The project demonstrates an end-to-end analytics workflow across multiple tools.

---

## 👤 Author

**Sneha S**

Healthcare Analytics | Data Analytics | Business Intelligence
