# Analyzing Jobs Market 

# DataSearch: Data Science Job Market Insights

## 📋 Project Overview
DataSearch is a dynamic Power BI business intelligence solution designed to track, analyze, and uncover macroeconomic trends within the data science and tech employment sectors from 2017 through 2021. 

By analyzing thousands of job postings, this project provides actionable insights into salary shifts, global talent demand patterns, company distribution across major industries, and critical technical skills needed for roles such as Data Analysts, Data Engineers, and Data Scientists.

---

## 🚀 Key Features & Layout

The interactive dashboard is split into 4 core pages for seamless exploration:

### 1. Home Dashboard
![Home](Visuals/Home.png)
* A high-end central landing matrix utilizing custom vector UI tiles to route users seamlessly across specialized analytics modules (Jobs, Skills, and Company Overviews).

### 2. Jobs Overview
![Jobs Overview](Visuals/Jobs_Overview.png)
* **Market Distribution Matrix:** Incorporates an intricate hierarchical Treemap comparing major tech roles and their foundational skill sub-trees (e.g., matching SQL, Python, and Tableau to Data Analyst postings).
* **Volumetric Forecasting:** An area trend chart tracking historical hiring shifts over time, segmented dynamically by seniority levels (from Internships up to Executive positions).
* **Experience Correlation:** A clear bar chart mapping structural seniority against expected minimum industry experience metrics.

### 3. Skills Overview
![Skills Overview](Visuals/Skills_Overview.png)
* **Skill Density Matrix:** A specialized Pareto-style column chart identifying the top core technologies (SQL, Python, Cloud infrastructure) dominating modern tech listings.
* **Penetration Breakdown:** A dynamic cross-tabulated heatmap showing exactly how critical a skill is per role (e.g., showcasing that SQL appears in over 73% of Data Analyst postings and 90% of Data Architect listings).
* **Trend Over Time:** Trajectory line charts monitoring whether specific framework demands are rising or stabilizing year-over-year.

### 4. Company Overview
![Company Overview](Visuals/Company_Overview.png)
* **Market Aggregations:** Displays central KPI cards tracking average salaries alongside a distribution layout of market caps.
* **Industry Clusters:** A multi-dimensional bubble chart analyzing Average Years of Experience versus industry sectors, scaled proportionally by active posting volume.
* **Firmographic Distribution:** Scatter-trend mappings analyzing hiring activity patterns relative to company sizes (ranging from seed-stage startups to enterprises with 10K+ employees).

---

## 🛠️ Data Modeling & DAX Measures

To evaluate penetration density and salary distributions efficiently across high-volume job arrays, the model leverages specialized semantic metrics.

### Core DAX Measures Included:

* **Salary Standardization Baseline:**
```dax
Average Pay = ('Job Postings'[Maximum Pay] + 'Job Postings'[Minimum Pay]) / 2
