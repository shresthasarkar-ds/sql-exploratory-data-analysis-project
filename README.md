# SQL Exploratory Data Analysis Project

A portfolio-focused collection of SQL scripts for exploring relational data, calculating useful measures, identifying patterns, and supporting business reporting. The project is organised as a practical analytical roadmap—from understanding the database to producing reusable reporting outputs.

## Project Overview

Exploratory data analysis (EDA) is the foundation of reliable analytics. This project demonstrates how SQL can be used to inspect a database, understand its entities and measures, investigate time-based behaviour, and communicate findings through structured reporting.

The queries are grouped by analytical purpose so that data analysts and BI professionals can quickly adapt the approach to their own relational databases.

## Objectives

- Explore the structure, contents, and relationships of a relational database.
- Profile dimensions, dates, and numerical measures before deeper analysis.
- Use SQL to identify scale, rankings, trends, changes, and performance patterns.
- Apply advanced analytical patterns such as cumulative totals, contribution analysis, and segmentation.
- Prepare clean, repeatable query outputs that can support BI dashboards and reports.

## Project Requirements

The project is designed for analysts who need a structured way to turn raw relational data into decision-ready information.

### Functional requirements

- Access to a relational database containing transactional and/or master data.
- SQL scripts that can inspect database objects and explore available fields.
- Queries for validating dimensions, dates, measures, and data ranges.
- Analytical queries for aggregation, comparison, ranking, trend analysis, and segmentation.
- Reusable outputs that can be used as source tables or datasets for BI reporting.

### Analytical requirements

- Identify the business entities and attributes available for analysis.
- Establish relevant date coverage and time periods.
- Calculate meaningful measures and compare them across dimensions.
- Detect major contributors, high- and low-performing items, and material changes over time.
- Present findings at appropriate levels of detail while maintaining clear, readable SQL.

> **Note:** This repository is intentionally dataset-agnostic. Adapt table names, column names, filters, and metric definitions to match your own database and business context.

## Analysis Roadmap

### 1. Exploratory Data Analysis

| Analysis area | Purpose |
| --- | --- |
| Database exploration | Understand the available databases, schemas, tables, columns, and relationships. |
| Dimensions exploration | Inspect categorical attributes and the values available for grouping and filtering. |
| Date exploration | Review date ranges, coverage, and useful reporting periods. |
| Measures exploration | Summarise and validate numerical fields and calculated metrics. |
| Magnitude analysis | Measure scale through totals, averages, counts, and other aggregations. |
| Ranking analysis | Identify leading and trailing entities using ordered measures. |

### 2. Advanced Analytics

| Analysis area | Purpose |
| --- | --- |
| Cumulative analysis | Calculate running totals and cumulative contributions. |
| Change-over-time trends | Compare periods to reveal growth, decline, and seasonal patterns. |
| Performance analysis | Evaluate results against a chosen benchmark, target, or prior period where available. |
| Part-to-whole analysis | Measure the contribution of each category or entity to an overall total. |
| Data segmentation | Group records into meaningful segments for focused analysis. |
| Reporting | Deliver structured, reusable query results for business intelligence and reporting. |

## BI & Reporting

The SQL outputs in this project can serve as a dependable analytical layer for reporting tools such as Power BI, Tableau, Excel, or other BI platforms. Rather than embedding a specific dashboard design, the project focuses on producing clear, reusable datasets that reporting tools can consume.

Typical reporting uses include:

- Executive summaries of key measures and high-level trends.
- Time-based reports showing period-over-period movement and cumulative performance.
- Dimension-level breakdowns for categories, products, customers, locations, or other available entities.
- Top and bottom rankings to highlight major contributors and areas requiring attention.
- Segmented views that support focused analysis and business decision-making.

For reliable reporting, keep metric definitions consistent, document assumptions, validate totals before publishing, and design query outputs at the same grain required by the report.

## Technologies

- **SQL** — database exploration, data transformation, aggregation, and analytical queries.
- **Relational database** — the source for the project data; syntax may need adjustment for the selected platform.
- **BI and visualisation tools** — optional consumers of the SQL query results, including Power BI, Tableau, or Excel.

## Suggested Repository Structure

```text
sql-exploratory-data-analysis-project/
├── README.md
├── sql/
│   ├── 00_init_database.sql
|   ├──01_database_exploration.sql
│   ├── 02_dimensions_exploration.sql
│   ├── 03_date_exploration.sql
│   ├── 04_measures_exploration.sql
│   ├── 05_magnitude_analysis.sql
│   ├── 06_ranking_analysis.sql
│   ├── 07_cumulative_analysis.sql
│   ├── 08_change_over_time_analysis.sql
│   ├── 09_performance_analysis.sql
│   ├── 10_data_segmentation.sql
│   ├── 11_part_to_whole_analysis.sql
│   |── 12_report_customers.sql
|   └── 13_report_products.sql
└── docs/
    └── Project_Roadmap.png
```

Rename or reorganise the folders as needed; the numbered script format simply makes the analytical workflow easier to follow.

## SQL Analysis Themes

The scripts can use common SQL techniques such as:

- `SELECT`, `WHERE`, `GROUP BY`, `HAVING`, and `ORDER BY` for exploration and summarisation.
- `JOIN` operations to combine related entities.
- `CASE` expressions to create business-friendly groups and segments.
- Date functions for calendar-based analysis.
- Window functions such as `ROW_NUMBER()`, `RANK()`, `LAG()`, and cumulative `SUM()` for advanced analysis.
- Common table expressions (CTEs) to keep multi-step logic readable and maintainable.

## Workflow

1. Review the schema, tables, and available columns.
2. Explore dimensions, date fields, and numerical measures for completeness and relevance.
3. Establish baseline aggregates and validate them against the underlying data.
4. Analyse magnitude and rankings to identify significant entities.
5. Extend the analysis with trends, cumulative measures, performance comparisons, contribution analysis, and segmentation.
6. Shape the final query outputs for reporting and visualisation.
7. Document metric definitions, assumptions, and any database-specific syntax changes.

## Best Practices

- Start with small exploratory queries before writing complex transformations.
- Use explicit column names instead of `SELECT *` in reusable scripts.
- Give calculated fields clear, meaningful aliases.
- Keep joins intentional and check for unexpected duplicate rows.
- Validate row counts, totals, date ranges, and null values throughout the process.
- Use comments to explain business logic, assumptions, and non-obvious calculations.
- Format SQL consistently so others can review and reuse it.
- Parameterise or clearly isolate filters that may change between reporting periods.

## Getting Started

1. Clone or download this repository.
2. Connect to a compatible relational database.
3. Review each script and replace placeholder object names, where applicable, with those from your database.
4. Run the scripts in roadmap order, validating results as you go.
5. Load the resulting query outputs into your preferred reporting or visualisation tool, if needed.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share it with appropriate attribution.

## About Me

Hi, I’m **Shrestha Sarkar**, an aspiring Data Analyst and Finance professional with a background in Mathematics, Finance, Business Analytics, and Data Science.

I’m interested in SQL, data analytics, business intelligence, financial analytics, and AI. I enjoy turning raw data into meaningful insights that support better business decisions. Through projects and continuous learning, I’m developing practical skills in SQL, Python, R, Power BI, Tableau, Excel, and data visualisation.

---

If you find this project useful, consider starring the repository.
