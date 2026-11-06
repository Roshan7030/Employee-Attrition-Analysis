# HR Attrition Analysis

## Project Overview

The **HR Attrition Analysis** is an Excel-based HR analytics
project designed to summarize employee headcount, attrition, workforce
demographics, and department-level distribution. It converts
employee-level data into KPI cards, charts, and interactive slicers so
that users can explore the workforce and identify areas that may need
further HR attention.

## Business Problem

HR teams need a clear view of their workforce to monitor employee
retention and understand how the workforce is distributed across
departments and demographic groups. Reviewing employee records one by
one makes it difficult to identify patterns quickly.

This project organizes the HR data into an interactive dashboard that
helps answer questions such as:

-   How many employees are in the organization?
-   How many employees have left, and what is the overall attrition
    rate?
-   What is the average employee age?
-   How is the workforce distributed by department, gender, education,
    marital status, and age group?
-   Which employee segments may deserve closer investigation when
    studying attrition?

## Dashboard Preview

Add your dashboard screenshot to the repository (for example, in a
folder named `images`) and update the path below if your filename is
different.

![HR Employee Analytics Dashboard](images/hr_employee_dashboard.png)

## Key Performance Indicators (KPIs)

The dashboard displays the following headline metrics from the workbook:

  ------------------------------------------------------------------------
  KPI                                          Value Meaning
  --------------------- ---------------------------- ---------------------
  Total Employees                              1,470 Total employee
                                                     records in the
                                                     dataset

  Attrition Count                                237 Employees marked as
                                                     having left
                                                     (`Attrition = Yes`)

  Active Employees                             1,233 Employees marked as
                                                     current
                                                     (`Attrition = No`)

  Average Age                            36.92 years Average age of
                                                     employees

  Attrition Rate                                 16% Attrition count
                                                     divided by total
                                                     employees
  ------------------------------------------------------------------------

**KPI calculations**

-   **Active Employees** = Total Employees − Attrition Count
-   **Attrition Rate** = (Attrition Count ÷ Total Employees) × 100
-   **Average Age** = Average of the `Age` field

## Dashboard Visualizations and Filters

The dashboard includes the following visual elements:

  -----------------------------------------------------------------------
  Visual / Filter                     What it shows
  ----------------------------------- -----------------------------------
  Education-wise employee             Employee count across Bachelor's,
  distribution                        Master's, Associate's, High School,
                                      and Doctoral education categories

  Department-wise employee            Employee count in HR, R&D, and
  distribution                        Sales

  Marital-status distribution         Employee count for Divorced,
                                      Married, and Single employees

  Gender distribution                 Workforce split by Male and Female
                                      employees

  Age-group distribution              Employee count across the age bands
                                      shown in the dashboard

  Gender slicer                       Filters the dashboard by gender

  Marital Status slicer               Filters the dashboard by marital
                                      status

  Department slicer                   Filters the dashboard by department
  -----------------------------------------------------------------------

## Dataset Information

The Excel workbook contains **1,470 employee records and 48 columns** in
the `Data` sheet. The fields cover areas such as:

-   Employee and attrition information
-   Department, job role, and education field
-   Gender, age, and marital status
-   Business travel and overtime
-   Job satisfaction and environment satisfaction
-   Monthly income, daily rate, and salary hike
-   Years of experience and tenure-related fields

The workbook also contains supporting sheets for KPI calculations,
employee details, and category-wise summaries used by the dashboard.

> **Data-source note:** The uploaded workbook does not identify a
> verified original publisher or source URL. Add the original dataset
> citation here only if you can independently confirm it. Do not label
> the data as real company or hospital employee records without
> evidence.

## Tools and Techniques

-   **Microsoft Excel** -- data review, KPI calculations, pivot tables,
    charts, and dashboard creation
-   **Pivot Tables / Pivot Charts** -- summarizing employee data by
    categories
-   **Slicers** -- interactive filtering by gender, marital status, and
    department
-   **Excel formulas** -- KPI calculations such as active employee
    count, average age, and attrition rate
-   **Data visualization** -- presenting workforce metrics in an
    easy-to-read dashboard

## Key Findings from the Dataset

The following figures are calculated from the employee-level `Data`
sheet:

-   The dataset contains **1,470 employees**, including **237 employees
    with attrition** and **1,233 current employees**.
-   The overall attrition rate is approximately **16.1%** (displayed as
    16% on the dashboard).
-   The **R&D department** has the largest headcount (961 employees),
    followed by Sales (446) and HR (63).
-   The **25--34 age group** is the largest age segment in the source
    data (554 employees).
-   Single employees account for 120 of the 237 attrition cases; this is
    the largest attrition count among the marital-status groups.
-   Employees marked for overtime account for 127 attrition cases out of
    416 employees in that group.

These findings describe patterns in this dataset; they do not establish
the reasons why employees leave.

## Important Dashboard Validation Note

Some charts in the screenshot are titled **"Education wise Attrition,"
"Department wise Attrition," "Merital Status wise Attrition,"** and
**"Age Group wise Attrition."** However, the displayed category totals
correspond to overall employee counts (for example, department counts of
63, 961, and 446 add up to 1,470), not only the 237 employees who left.

For an accurate attrition comparison, use `Attrition = Yes` as a filter
or calculate attrition counts/rates for each category. Consider renaming
the current visuals to **"Employee Distribution by ..."** if they are
intended to show total headcount. Also verify the age-band labels
against the source data before publishing.

## Repository Structure

A suggested GitHub repository layout:

``` text
HR-Employee-Analytics/
│
├── images/
│   └── hr_employee_dashboard.png
│
├── HR DATA_Excel.xlsx
│
└── README.md
```

If you use different filenames, update the paths in this README
accordingly.

## How to Use the Project

1.  Download or clone this repository.
2.  Open the Excel workbook in Microsoft Excel.
3.  Go to the `dashboard` sheet to view the HR Employee Analytics
    Dashboard.
4.  Use the Gender, Marital Status, and Department slicers to filter the
    dashboard.
5.  Review the KPI cards and charts to explore workforce distribution
    and attrition metrics.

## Project Objective

The objective of this project is to demonstrate practical HR data
analysis and Excel dashboarding skills by transforming employee-level
data into meaningful workforce metrics and interactive visual summaries.

------------------------------------------------------------------------

**Note:** This is an analytical portfolio project. The results are based
on the supplied workbook and should not be treated as verified findings
about a specific real-world organization.
