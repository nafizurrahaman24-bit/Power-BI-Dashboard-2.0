# Power BI Dashboard 2.0
# Power BI Data Jobs Dashboard

An interactive **Power BI dashboard for exploring the data-job market**, with a focus on job demand, salaries, skills, and job titles.

The dashboard is designed to answer practical questions such as:

- Which skills appear most frequently in data-related job postings?
- Which skills are associated with higher median yearly salaries?
- Which data job titles have the highest demand?
- Which data job titles have the highest median salary?
- How do the results change when filtering by country, job title, or skill?


## Dashboard Overview

The Power BI report contains three main pages:

### 1. Dashboard 2.0

 ## Dashboard Preview 
![alt text](<Power BI DashBoard 2.0.gif>)

The main interactive dashboard provides a high-level view of the data-job market.

**Key metrics include:**

- **Job Count** – number of job postings in the current filter context
- **Median Yearly Salary** – median annual salary
- **Median Hourly Salary** – median hourly salary
- **Skills Per Job** – average/derived number of skills associated with jobs

**Interactive filters include:**

- Job country
- Job title
- Skill
- Job-related parameter selections

The page also includes visualizations for:

- Top-paying jobs in data
- Top skills in data
- Job demand by skill
- Salary by skill

### 2. Skill Stats

This page focuses specifically on the relationship between **skills, job demand, and salary**.

It includes:

- **Top skills in data by job count**
- **Median yearly salary of the top 20 skills**

The skill visuals are sorted to make the most relevant skills easier to identify.

### 3. Measures

This page provides additional analytical views using Power BI measures and job/skill dimensions.

It includes comparisons such as:

- Top job titles by job count
- Top skills by job count
- Median salary by job title
- Median salary by skill

This page is useful for exploring the underlying measures and understanding how demand and compensation differ across the data-job market.

## Key Business Questions

The dashboard is built around four major analytical questions:

### Job Demand

**Which jobs and skills are most in demand?**

Job-posting counts are used to identify the job titles and skills appearing most frequently in the dataset.

### Salary Analysis

**Which jobs and skills have higher median salaries?**

Median yearly salary is used instead of the average to reduce the influence of unusually high or low salary values.

### Skill Analysis

**Which skills are associated with both demand and compensation?**

The dashboard allows skills to be compared based on their frequency in job postings and their median salary.

### Geographic Analysis

**How does the data-job market vary by country?**

The country slicer allows the analysis to be narrowed to a specific job market.

## Interactive Features

The report uses Power BI slicers and field parameters to make the dashboard interactive.

### Country Filter

Filter the analysis by **job country**.

### Job Title Filter

Select specific job titles to examine their demand and salary characteristics.

### Skill Filter

Select a skill to investigate its relationship with job postings and compensation.

### Dynamic Parameters

The report includes Power BI field parameters that allow selected measures/fields to be used dynamically in visualizations.

## Data Model

The report uses a job-postings-oriented data model containing entities such as:

- `job_postings_fact`
- `skills_dim`
- `_measures`
- `Select Job Parameters`
- `Select Skill Parameter`

The model separates job-posting information from skill information and uses dedicated measures for the main KPIs.

### Important fields

| Field | Purpose |
|---|---|
| `job_title_short` | Job-title category |
| `job_country` | Country associated with the job posting |
| `skills` | Individual skill |
| `Job Count` | Number of job postings |
| `Median Yearly Salary` | Median annual salary |
| `Median Hourly Salary` | Median hourly salary |
| `Skill Per Job` | Skill-related job metric |

## Power BI Measures

The dashboard uses dedicated measures for its main calculations, including:

- **Job Count**
- **Median Yearly Salary**
- **Median Hourly Salary**
- **Skill Per Job**

Using measures allows the dashboard to respond dynamically to slicers and other filter selections.

## Tools & Technologies

- **Microsoft Power BI Desktop**
- **DAX**
- **Power BI Field Parameters**
- **Power BI Slicers**
- **Data Modeling**
- **Interactive Data Visualization**

## Dashboard Structure

```text
Power BI Data Jobs Dashboard
│
├── Dashboard 2.0
│   ├── KPI Cards
│   ├── Country Filter
│   ├── Job Title Filter
│   ├── Skill Filter
│   ├── Top Paying Jobs
│   └── Top Skills
│
├── Skill Stats
│   ├── Top Skills by Job Count
│   └── Median Salary by Skill
│
└── Measures
    ├── Job Demand Analysis
    ├── Skill Analysis
    ├── Salary Analysis
    └── Job Title Analysis
``

## How to Use

1. Download or clone this repository.
2. Open `Dashboard 2.0.pbix` using **Power BI Desktop**.
3. Allow the dataset to load or refresh if required.
4. Use the slicers to filter the dashboard.
5. Hover over charts to view detailed values.
6. Select data points to cross-filter other visuals.
7. Use the different report pages to explore demand, skills, and salary patterns.

> **Note:** Power BI Desktop is required to open and interact with the `.pbix` file.

## Insights You Can Explore

The dashboard can be used to investigate questions such as:

- What are the most frequently requested skills in data jobs?
- What skills have the highest median yearly salaries?
- Which data job titles have the largest number of postings?
- Which job titles have the highest median yearly salaries?
- How do job-market patterns change by country?
- How does the number of skills associated with jobs relate to the job market?

## Project Purpose

This project demonstrates practical skills in:

- Data visualization
- Data analysis
- Power BI dashboard development
- DAX measure creation
- Data modeling
- Interactive reporting
- Business-oriented analytical thinking

It can be used as a **data analytics portfolio project** to demonstrate the ability to transform job-market data into an interactive business intelligence dashboard.

## File

```text
Dashboard 2.0.pbix
```

**Format:** Power BI Desktop file (`.pbix`)

## Author

**Nafizur Rahaman**

Data Analytics | Finance | Business Intelligence



