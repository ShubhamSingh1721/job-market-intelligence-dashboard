# Job Market Intelligence Dashboard

A Power BI and SQL analytics project exploring 30,000 LinkedIn job postings to understand hiring demand, company activity, location trends, compensation patterns, applications, and remote-work opportunities.

## Project Overview

The goal of this project is to turn raw job-posting data into useful business insights using MySQL, SQL, and Microsoft Power BI.

The planned dashboard structure contains four analytical pages:

1. **Executive Dashboard** — overall hiring activity, job types, experience levels, companies, and locations.
2. **Salary & Compensation Insights** — recorded salary comparisons across companies, locations, experience levels, and employment types.
3. **Company & Location Analysis** — job postings and application activity by company and location.
4. **Remote & Job Market Trends** — remote-work indicators, applications by work type and experience level, and internship opportunities.

*Project status: Page 1 is complete; the remaining pages are in progress.*

## Dataset

- **Source:** LinkedIn job postings dataset
- **Records:** 30,000
- **Format:** CSV
- **Key fields:** Company, job title, location, work type, experience level, applications, salary fields, and remote-work indicator.

Dataset redistribution is subject to the original source's license and terms.

## Tools & Technologies

- **MySQL / SQL** — querying, aggregation, and exploratory analysis
- **Microsoft Power BI** — interactive dashboard development
- **DAX** — KPI measures and calculations
- **CSV** — dataset import

## Key Metrics

The project includes or plans to include these KPIs, depending on dashboard completion:

- Total Jobs
- Total Companies
- Total Applications
- Average Applications per Job
- Remote Jobs and Remote Job Percentage
- Average Salary
- Highest Salary
- High Salary Jobs

## Analytical Questions

- Which companies publish the most job postings?
- Which locations have the highest hiring activity?
- How do applications vary by company, work type, and experience level?
- Which companies have remote-work or internship postings?
- How does recorded compensation vary across job categories?

## Methodology

1. Imported the 30,000-row CSV dataset into MySQL for SQL analysis.
2. Used SQL queries to analyse job postings, applications, companies, locations, work types, and experience levels.
3. Examined missing values and duplicate job IDs.
4. Created DAX measures for key dashboard metrics.
5. Built the Executive Dashboard in Power BI and began developing the remaining report pages.
6. Identified salary outliers and missing remote-work classifications as data-quality limitations.

## Data Quality Notes

- Salary fields contain suspicious and extreme values. Salary results require further validation before being treated as definitive.
- Some records have missing salary, company, experience-level, and skills information.
- The remote-work indicator contains missing values. Missing classifications should not automatically be treated as confirmed on-site jobs.
- The dataset contains 30,000 rows in the current Power BI report. This does not mean all data-quality issues have been resolved.

## Planned Repository Structure

- `dashboard/` — final Power BI report
- `sql/` — SQL analysis queries
- `screenshots/` — dashboard page previews
- `docs/` — project documentation

*These folders and files should be listed as repository contents only after they have been created and added to GitHub.*

## Future Improvements

- Validate salary values and handle outliers.
- Improve the treatment of missing remote-work classifications.
- Complete the remaining Power BI pages.
- Add trend analysis if the posting-date data can be reliably interpreted.
- Develop a companion web application for exploring job-market insights.

## Author

**Shubham Singh**

MBA in Business Analytics | Aspiring Data Analyst / Business Analyst

**Skills demonstrated:** SQL, MySQL, Power BI, DAX, data analysis, data visualization, and business intelligence.
