# Project Summary — Job Market Intelligence Dashboard

## 1. Project Overview

The Job Market Intelligence Dashboard is a data analytics project built using MySQL, SQL, DAX, and Microsoft Power BI. It analyses 30,000 LinkedIn job postings to identify hiring patterns, company activity, location-based demand, salary trends, application activity, and remote-work opportunities.

The project focuses on converting raw job-posting data into meaningful insights through SQL queries, KPI calculations, and interactive visualizations.

## 2. Project Objectives

- Analyse job-posting demand across companies and locations.
- Identify companies with the highest number of job postings.
- Compare hiring patterns across employment types and experience levels.
- Explore salary patterns across companies, locations, and job categories.
- Analyse application activity across different job categories.
- Examine remote-work indicators and internship opportunities.
- Present findings through a four-page interactive Power BI dashboard.

## 3. Dataset Details

- **Dataset:** LinkedIn Job Postings
- **Total Records:** 30,000
- **Source Format:** CSV
- **SQL Table:** `postings`
- **Analysis Tools:** MySQL and Power BI

### Important Fields

- `job_id` — job posting identifier
- `company_name` — company associated with a posting
- `title` — job title
- `location` — job location
- `formatted_work_type` — employment type
- `formatted_experience_level` — experience category
- `applies` — recorded application count
- `remote_allowed` — remote-work indicator
- `min_salary`, `med_salary`, `max_salary` — salary fields
- `normalized_salary` — normalized compensation field

## 4. Tools and Technologies

| Tool | Purpose |
|---|---|
| MySQL | Database storage and SQL execution |
| SQL | Data exploration, aggregation, ranking, and quality checks |
| Microsoft Power BI | Interactive dashboard development |
| DAX | KPI measures and calculations |
| CSV | Dataset import and exchange |

## 5. SQL Analysis Performed

SQL queries were used to explore the dataset and answer business questions.

The analysis included:

1. Inspecting the database table structure and validating the record count.
2. Checking duplicate job IDs.
3. Examining missing values in important columns.
4. Analysing job counts by work type and experience level.
5. Identifying the top companies and locations by job-posting count.
6. Comparing application counts across work types and companies.
7. Exploring average compensation by work type, experience level, company, and location.
8. Inspecting extreme salary values.
9. Analysing remote-marked job postings and companies.
10. Identifying companies with internship postings.
11. Exploring common job titles and posting domains.
12. Examining location suffixes and posting-year information.
13. Using aggregation, sorting, filtering, and ranking techniques to extract insights.

These queries support exploratory analysis. They do not imply that every data-quality issue has been resolved.

## 6. Power BI Dashboard Structure

The report contains four analytical pages with a consistent blue-and-white visual theme.

### Page 1 — Executive Dashboard

Provides a high-level overview of job-market activity.

Key elements:
- Total Jobs
- Total Companies
- Total Applications
- Remote Jobs
- Remote Job Percentage
- Average Salary
- Jobs by Work Type
- Jobs by Experience Level
- Top 10 Companies Hiring
- Top 10 Hiring Locations
- Highest-Paying Locations
- Average Salary by Work Type

### Page 2 — Salary & Compensation Insights

Focuses on recorded salary comparisons.

Planned analytical elements include:
- Highest Salary
- Salary comparisons by company
- Salary comparisons by location
- Salary by Experience Level
- Salary by Work Type
- High Salary Jobs
- Key Salary Insights

The raw Lowest Salary KPI requires a validated salary filter because the source data contains suspicious low values.

### Page 3 — Company & Location Analysis

Focuses on company-level hiring activity and location-based demand.

Planned analytical elements include:
- Companies with the most job postings
- Companies ranked by application activity
- Locations with the most job postings
- Locations ranked by application activity
- Company-level hiring comparisons
- Location-level demand comparisons

### Page 4 — Remote & Job Market Trends

Focuses on remote-work indicators and broader job-market patterns.

Planned analytical elements include:
- Remote-work classification
- Applications by Work Type
- Jobs by Experience Level
- Applications by Experience Level
- Companies with remote-marked postings
- Companies with internship postings

## 7. KPI Measures

The Power BI model includes measures such as:

- **Total Jobs** — counts rows in the dataset.
- **Total Companies** — counts distinct company names.
- **Total Applications** — sums recorded applications.
- **Average Salary** — calculates the average of `normalized_salary`.
- **Remote Jobs** — sums the numeric `remote_allowed` indicator.
- **Remote Job %** — calculates the remote indicator total divided by total jobs.

Additional measures, including Average Applications per Job and High Salary Jobs, can be documented as completed once they have been created and verified in the report.

## 8. Data Quality and Limitations

The dataset was inspected for missing values, duplicate job IDs, and suspicious salary values.

Important limitations include:

- Salary fields contain extreme or suspicious values.
- Salary units and pay periods require validation before compensation results can be treated as definitive.
- Some company, salary, experience-level, skills, and remote-work fields contain missing values.
- Missing remote-work classifications should not automatically be interpreted as on-site jobs.
- Location suffix extraction is a text-based analysis and is not a fully validated geographic mapping.
- Posting-date analysis depends on validating the timestamp units and meaning of the date field.

The original data should be preserved until documented cleaning rules have been applied and verified.

## 9. Skills Demonstrated

- SQL querying and aggregation
- MySQL database analysis
- Data-quality assessment
- DAX measures
- Power BI dashboard design
- KPI development
- Business intelligence
- Data visualization
- Exploratory data analysis
- Communicating analytical findings

## 10. Future Improvements

- Validate salary units and pay periods.
- Develop documented rules for handling salary outliers.
- Improve treatment of missing remote-work classifications.
- Validate posting-date information before extending trend analysis.
- Add further analysis where the source data supports reliable conclusions.
- Develop a companion web application for exploring job-market insights.

## 11. Author

**Shubham Singh**

MBA in Business Analytics | Aspiring Data Analyst / Business Analyst

**Project Stack:** MySQL, SQL, Power BI, DAX, CSV
