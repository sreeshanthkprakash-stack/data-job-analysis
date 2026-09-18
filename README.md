# 📊 Global Data Jobs Analysis & Salary Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-Desktop_Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Dataset](https://img.shields.io/badge/Dataset-478.9K+_Job_Postings-blue?style=for-the-badge)](https://github.com/sreeshanthkprakash-stack/data-job-analysis)
[![DAX](https://img.shields.io/badge/DAX-Calculated_Measures-orange?style=for-the-badge)](https://learn.microsoft.com/en-us/dax/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

An interactive, multi-page business intelligence dashboard developed in **Power BI** to analyze over **478,000+ data job postings** globally throughout 2024. The project uncovers compensation benchmarks, job posting trends, work-from-home adoption, benefit availability, degree requirements, and portal distributions across diverse tech and data roles.

---

## 📑 Table of Contents
- [Executive Summary & High-Level KPIs](#-executive-summary--high-level-kpis)
- [Dashboard Architecture & Pages](#-dashboard-architecture--pages)
  - [Page 1: Data Jobs Dashboard (Overview)](#page-1-data-jobs-dashboard-overview)
  - [Page 2: Job Title Drill-Through Analysis](#page-2-job-title-drill-through-analysis)
- [Comprehensive Role & Salary Benchmark Matrix](#-comprehensive-role--salary-benchmark-matrix)
- [Key Business Insights & Findings](#-key-business-insights--findings)
- [Data Model & DAX Metrics](#-data-model--dax-metrics)
- [Dataset Schema](#-dataset-schema)
- [Installation & How to Run](#-installation--how-to-run)
- [Repository Structure](#-repository-structure)
- [Author & License](#-author--license)

---

## 📈 Executive Summary & High-Level KPIs

| KPI Metric | Value | Description |
|---|---|---|
| **Total Job Postings** | **478.90K** (478,895) | Analyzed records across data & engineering roles |
| **Overall Median Yearly Salary** | **$113.25K** ($113,250.00 USD) | Benchmark median annual compensation |
| **Overall Median Hourly Salary** | **$47.62 / hr** | Benchmark median hourly compensation rate |
| **Salary Star Rating** | ★★☆☆☆ | Normalized rating metric comparing market salary ranges |

---

## 🖥️ Dashboard Architecture & Pages

The Power BI report consists of two synchronized, interactive views with drill-through functionality:

### Page 1: Data Jobs Dashboard (Overview)
A high-level command center displaying macro-level market trends, role rankings, and salary distributions:

1. **Job Posting Trend in 2024 (Monthly Line Chart):**
   * Tracks monthly posting volumes from **Jan 2024 to Nov 2024**, identifying seasonal hiring surges and contraction periods.
2. **Highest Paying Jobs in Data (Horizontal Bar Chart):**
   * Ranks roles by median annual salary, spotlighting top-tier compensation roles like *Senior Data Scientist* and *Machine Learning Engineer*.
3. **Hourly vs. Yearly Salary Distribution (Scatter Plot):**
   * Maps median hourly pay against median yearly salary across roles to reveal compensation alignment and contracting premiums.
4. **Role Benchmark Matrix with Sparkline Trends:**
   * Summarizes job counts, annual salaries, hourly wages, and miniature monthly job trend lines per role.

---

### Page 2: Job Title Drill-Through Analysis
A granular, role-specific drill-through page allowing deep-dive analysis on any individual position (e.g., *Senior Data Scientist*, *Data Engineer*, *Data Analyst*):

1. **Salary Gauges:**
   * **Median Yearly Salary Gauge:** Displays role median vs. maximum range benchmark (e.g., $155.50K on a $311.00K scale for Senior Data Scientists).
   * **Median Hourly Salary Gauge:** Displays role hourly wage gauge (e.g., $49.90 / hr on a $99.79 scale).
2. **Work Arrangement & Perks (Donut Charts):**
   * **Work From Home %:** Percentage of remote vs. on-site postings (e.g., 13.94% Remote / 3.03K vs. 86.06% On-site / 18.7K).
   * **No Degree Required %:** Ratio of job postings not requiring a traditional degree (e.g., 7.2% No Degree / 1.57K vs. 92.8% Degree Required / 20.1K).
   * **Job Health Insurance %:** Prevalence of employer-provided health coverage (e.g., 19.22% Health Coverage / 4.18K vs. 80.78% / 17.55K).
3. **Global Job Distribution Map:**
   * Interactive bubble map powered by Bing Maps / OpenStreetMap pinpointing hiring concentration across North America, Europe, Asia, South America, and Australia.
4. **Hiring Platforms & Job Types:**
   * **Job Portal (Bar Chart):** Volume distribution across recruitment portals (*via LinkedIn, via BeBee, via Indeed, LinkedIn direct, via ZipRecruiter, via Jooble, via Recruit.net, via GrabJobs, etc.*).
   * **Job Type Distribution (Treemap):** Proportion of Full-time, Contractor, Part-time, and Internship opportunities.

---

## 📊 Comprehensive Role & Salary Benchmark Matrix

The dashboard consolidates the global data job market into the following breakdown:

| Job Title | Job Count | Median Yearly Salary | Median Hourly Salary | Market Share |
|---|:---:|:---:|:---:|:---:|
| **Data Engineer** | 128,994 | $126,268.00 | $59.16 | 26.94% |
| **Data Analyst** | 112,866 | $90,000.00 | $32.50 | 23.57% |
| **Data Scientist** | 97,664 | $125,000.00 | $43.03 | 20.39% |
| **Senior Data Engineer** | 30,608 | $146,500.00 | $58.68 | 6.39% |
| **Business Analyst** | 28,584 | $95,350.00 | $43.00 | 5.97% |
| **Software Engineer** | 23,402 | $145,000.00 | $60.00 | 4.89% |
| **Senior Data Scientist** | 21,731 | $155,500.00 | $49.90 | 4.54% |
| **Senior Data Analyst** | 15,347 | $107,310.00 | $39.45 | 3.20% |
| **Machine Learning Engineer** | 12,860 | $155,000.00 | $60.75 | 2.69% |
| **Cloud Engineer** | 6,839 | $113,838.00 | $50.00 | 1.43% |
| **Total / Overall** | **478,895** | **$113,250.00** | **$47.62** | **100.00%** |

---

## 💡 Key Business Insights & Findings

1. **Top Volume Roles:** **Data Engineer** (128.9K) and **Data Analyst** (112.8K) make up over **50% of all data job postings**, highlighting high organizational demand for data pipeline infrastructure and business reporting.
2. **Top Earning Positions:**
   * **Senior Data Scientist** ($155.5K) and **Machine Learning Engineer** ($155.0K) lead annual compensation.
   * **Machine Learning Engineer** commands the highest median hourly rate at **$60.75 / hr**, followed closely by **Software Engineer** ($60.00 / hr) and **Data Engineer** ($59.16 / hr).
3. **Seniority Premium:** Moving from *Data Analyst* ($90.0K) to *Senior Data Analyst* ($107.3K) represents a **+19.2%** salary jump, while *Data Scientist* ($125.0K) to *Senior Data Scientist* ($155.5K) yields a **+24.4%** premium.
4. **Remote Work & Education Landscape:**
   * For specialized roles like Senior Data Scientists, **~14%** offer full remote work.
   * **Over 92%** of senior listings explicitly require formal degree credentials.
   * LinkedIn and aggregated portals (*via LinkedIn, via BeBee, via Indeed*) account for the vast majority of postings.

---

## 🧮 Data Model & DAX Metrics

Key DAX measures implemented in the `.pbit` model include:

```dax
// Total Job Count
Job Count = COUNTROWS('job_postings_flat')

// Median Annual Salary
Median Yearly Salary = MEDIAN('job_postings_flat'[salary_year_avg])

// Median Hourly Rate
Median Hourly Salary = MEDIAN('job_postings_flat'[salary_hour_avg])

// Work From Home Percentage
WFH % = 
DIVIDE(
    CALCULATE(COUNTROWS('job_postings_flat'), 'job_postings_flat'[job_work_from_home] = TRUE()),
    COUNTROWS('job_postings_flat'),
    0
)

// Degree Not Mentioned / Required Percentage
No Degree % = 
DIVIDE(
    CALCULATE(COUNTROWS('job_postings_flat'), 'job_postings_flat'[job_no_degree_mention] = TRUE()),
    COUNTROWS('job_postings_flat'),
    0
)

// Health Insurance Coverage Percentage
Health Insurance % = 
DIVIDE(
    CALCULATE(COUNTROWS('job_postings_flat'), 'job_postings_flat'[job_health_insurance] = TRUE()),
    COUNTROWS('job_postings_flat'),
    0
)
```

---

## 🗂️ Dataset Schema

| Column Name | Data Type | Description |
|---|---|---|
| `job_title_short` | Text | Standardized role category (*Data Analyst, Data Engineer, etc.*) |
| `job_title` | Text | Full title from the original job listing |
| `job_location` | Text | Geographic location / city / state |
| `job_country` | Text | Country of posting |
| `job_via` | Text | Source platform / job board |
| `job_schedule_type` | Text | Employment type (*Full-time, Part-time, Contract, Internship*) |
| `job_work_from_home`| Boolean | `TRUE` if remote work is permitted, else `FALSE` |
| `job_posted_date` | DateTime | Timestamp when the job listing was published |
| `job_no_degree_mention` | Boolean | `TRUE` if no degree requirement is listed |
| `job_health_insurance` | Boolean | `TRUE` if health insurance benefits are included |
| `salary_rate` | Text | Rate unit (*year, hour*) |
| `salary_year_avg` | Decimal | Annual normalized salary in USD |
| `salary_hour_avg` | Decimal | Hourly normalized wage in USD |
| `company_name` | Text | Hiring employer name |
| `job_skills` | Text | List of technical skills extracted from posting |
| `job_type_skills` | Text | Categorized skills dictionary (analyst tools, programming, cloud) |

---

## 🚀 Installation & How to Run

### Prerequisites
* [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Latest version recommended)
* Git

### Step-by-Step Setup
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/sreeshanthkprakash-stack/data-job-analysis.git
   cd data-job-analysis
   ```

2. **Extract Dataset:**
   * Extract `job_postings_flat - Copy.zip` into the repository folder to unpack the complete CSV dataset.

3. **Open the Power BI Template:**
   * Double-click [`data_job_analysis.pbit`](file:///c:/Users/SREESHANTH_K/Desktop/job_analysis/data_job_analysis.pbit) in Power BI Desktop.
   * When prompted with parameters, browse to the extracted `job_postings_flat.csv` file.
   * Power BI will load the data into the pre-built data model, relationships, DAX measures, and dashboard visuals.

---

## 📁 Repository Structure

```text
├── .gitattributes                 # Git LFS & line ending attributes
├── .gitignore                      # Git ignore rules for large raw files
├── README.md                       # Full documentation & project walkthrough
├── data_job_analysis.pbit         # Power BI Template (Pages, DAX & visual layouts)
└── job_postings_flat - Copy.zip    # Compressed dataset archive (478K+ job postings)
```

---

## 👤 Author & Acknowledgments

* **Created by:** [Sreeshanth K](https://github.com/sreeshanthkprakash-stack)
* **Dataset & Context:** Global Tech & Data Job Postings dataset (Luke Barousse data ecosystem).
* **Tools:** Microsoft Power BI, Power Query, DAX.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) - feel free to use it for data analytics portfolios, research, and learning.
