# 🦟 Malaria Treatment Analytics Dashboard

##  Project Overview

This project demonstrates an end-to-end healthcare analytics workflow developed to analyze longitudinal malaria treatment administration data. The analysis transforms raw clinical records into meaningful operational insights through data cleaning, exploratory data analysis (EDA), feature engineering, KPI development, SQL integration, and interactive dashboard visualization in Power BI.

The objective is to support healthcare professionals and program managers in monitoring treatment adherence, medication exposure, treatment duration, and documentation quality to improve patient care and data-driven decision-making.

---

## 📊 Dashboard Preview

### Executive Overview
![Executive Overview](image/Trearment%20program_Executive%20Overview.png)

### Treatment Adherence Analysis
![Treatment Adherence Analysis](image/Treatment%20Adherence%20Analysis.png)

### Data Quality Assessment
![Data Quality Assessment](image/Data%20Quality%20Assessment.png)

>  Additional dashboard views (Exposure Analysis, Treatment Trends, 
> Key Insights, Strategic Recommendations) are available in the 
> [`image/`](image/) folder.
---

##  Business Problem

Healthcare facilities generate large volumes of medication administration data, but raw records alone provide limited operational value.

This project addresses key questions such as:

* Are participants completing their prescribed treatment protocol?
* Which participants receive the highest medication exposure?
* Are treatment durations consistent across participants?
* How complete and reliable is the clinical documentation?
* What operational insights can be derived to support healthcare decision-making?

---

##  Dataset Summary

| Attribute               | Value                                |
| ----------------------- | ------------------------------------ |
| Dataset Type            | Longitudinal Healthcare Dataset      |
| Total Treatment Records | **730**                              |
| Total Participants      | **195**                              |
| Level of Analysis       | Dose-level medication administration |
| Database                | PostgreSQL                           |

Each record represents a medication administration event for a participant undergoing malaria treatment.

---

#  Technology Stack

| Tool       | Purpose                                                               |
| ---------- | --------------------------------------------------------------------- |
| Python     | Data analysis and feature engineering                                 |
| Pandas     | Data manipulation                                                     |
| NumPy      | Numerical computations                                                |
| PostgreSQL | Central data integration layer connecting Python pipeline to Power BI |
| SQLAlchemy | Python-to-PostgreSQL connectivity for automated data loading          |
| Power BI   | Dashboard development and storytelling                                |
| Matplotlib | Exploratory visualizations                                            |

---

#  Analytics Workflow

The project follows a structured healthcare analytics pipeline:

1. Data cleaning
2. Data profiling
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. KPI Development
6. **PostgreSQL as Integration Layer** — Cleaned and engineered data is loaded from Python into PostgreSQL, which serves as the central data store connecting the Python pipeline to the Power BI dashboard.
7. Interactive Power BI Dashboard Development
8. Business Insights & Recommendations

---

#  Feature Engineering

The following analytical features were developed to support participant-level analysis:

* Total doses administered
* Treatment protocol completion status
* Incomplete treatment indicator
* Extended treatment indicator
* Total medication exposure
* Average ordered dose
* Average treatment duration
* Maximum treatment duration
* Missing end-date indicator
* Missing duration indicator

---

#  Dashboard Pages

### 1. Executive Overview

Provides a high-level summary of operational KPIs, participant statistics, treatment completion, and medication exposure.

---

### 2. Treatment Adherence Analysis

Evaluates treatment protocol completion, incomplete treatments, extended treatment cases, and participant adherence trends.

---

### 3. Exposure Analysis

Analyzes participant medication exposure, identifies high-exposure participants, and visualizes exposure distribution.

---

### 4. Data Quality Dashboard

Assesses documentation completeness through:

* End-date completeness
* Missing end-date rate
* Treatment duration completeness

---

### 5. Treatment Activity Trends

Visualizes treatment activity and dosage patterns over time to identify operational trends.

---

### 6. Insights & Recommendations

Summarizes the major findings from the analysis and provides practical recommendations to improve treatment monitoring and healthcare data quality.

---

#  Key Findings

The analysis identified several important operational insights:

* Treatment protocol completion rate was **75.9% indicating high adherence to medication**
* 1.54% of participants had an extended treatment beyond the 4 dose standard protocol 
* Medication exposure varied across participants, indicating the importance of exposure monitoring.
* Documentation completeness was generally high with 74.1% although 25.9% missing treatment end dates affected a portion of the records.
* Participant-level KPIs enabled more meaningful operational reporting than dose-level summaries alone.

---

# Recommendations

Based on the analysis:

* Strengthen follow-up procedures for participants with incomplete treatment.
* Monitor the participants with unusually high medication exposure.
* Improve clinical documentation practices to reduce missing end dates.
* Implement routine dashboard monitoring to support operational decision-making.
* Perform regular healthcare data quality assessments before reporting and analysis.

---

#  Repository Structure

```text
malaria_treatment_analytics/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_data_data_profiling.ipynb
│   ├── 03_eda_analysis.ipynb
│   ├── 04_feature_engineering.ipynb
│   └── 05_kpi_development.ipynb
│
├── dashboard/
│   └── malaria_treatment_dashboard.pbix
│
├── images/
│   ├── executive_overview.png
│   ├── treatment_adherence.png
│   ├── exposure_analysis.png
│   ├── data_quality.png
│   ├── treatment_activity_trends.png
│   └── insights_recommendations.png
│
└── sql/
    └── README.md           
```

---

#  Running the Project

1. Clone the repository.

2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Create a PostgreSQL database.

4. Update the database connection string in the notebooks to match your local PostgreSQL configuration.

5. Execute the notebooks in the following order:

* 01_data_cleaning
* 02_data_profiling
* 03_eda_analysis
* 04_feature_engineering
* 05_kpi_development

6. Refresh the Power BI dashboard to load the latest data from PostgreSQL.

---

#  Skills Demonstrated

This project demonstrates practical experience in:

* Healthcare Data Analytics
* Data Cleaning & Validation
* Exploratory Data Analysis (EDA)
* Feature Engineering
* KPI Development
* SQL Database Integration
* Power BI Dashboard Development
* Data Storytelling
* Healthcare Operational Reporting

---

##  Author

**Jentrix Semo**

Healthcare Data Analyst with hands-on experience in malaria treatment adherence research, clinical data pipelines, and operational dashboard development using Python, SQL, and Power BI.

This repository was developed as a portfolio project to demonstrate practical end-to-end healthcare data analytics skills using real-world analytical workflows.
