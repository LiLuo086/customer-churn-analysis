# Customer Churn Analysis in Excel

## Project Overview

**Churn rate**, also known as customer attrition rate or customer churn, is a business metric that calculates the percentage of customers who stop using a product or service during a given period. It is particularly relevant in subscription-based business models, telecommunications where customer retention is a key factor.

As acquiring new customers often costs more than retaining existing ones, **Customer churn** is a critical metric for telecom companies.
In this project, I performed an exploratory churn analysis on the Databel Telecom dataset using Excel. The goal was to uncover churn patterns, calculate KPIs, and provide actionable insights for retention strategies.

## Objectives

- Analyze customer churn rate and trends.

- Identify key factors that influence churn.

- Build an interactive Excel dashboard to summarize findings.

- Provide business recommendations based on insights.

## Dataset

Source: [Databel Telecom Customer Churn Dataset](https://www.kaggle.com/datasets/muftau/investigating-customer-churn)

The dataset contains 6,687 customer records with 29 columns regarding customer status, demographic, contract information, and subscription details.

This dataset is a snapshot of the database at a specific time, so there is no time dimension in the dataset.

The metadata about this dataset is stored in the file `metadata.xlsx`.

## Methodology

Steps taken in Excel:

1. Data Cleaning:

    - **Remove duplicates** using customer ID as a unique key → 0 rows removed.  

    - **Handle missing values** in `Churn Category` (replaced blanks with `Other`) and `Churn Reason` (replaced blanks with `Don't know`).

    - **Convert columns**:
        - convert columns to numerical: `Account Length (in months)`, `Local Calls`, `Local Mins`, `Intl Calls`, `Intl Mins`, `Avg Monthly GB Download`, `Age`, `Number of customers in a group`, `Customer Service Calls`.
        - convert columns to currency columns: `Extra International Charges`, `Extra Data Charges`, `Monthly Charges`, `Total Charges`.
        - convert columns to text columns: other columns.
            - remove whitespace in text values.
            - convert text strings to lowercase.

    - **Standardize column names**: replace spaces between column names with underscore `_`, e.g. `Total Charges` → `Total_Charges`.

2. Exploratory Analysis:

    - Calculated churn rate.

    - Created PivotTables for churn distribution (by contract type, tenure, payment method, etc.).

    - Applied conditional formatting to highlight churn risks.

3. Visualization & Dashboard:

    - Built interactive Excel dashboard using slicers, PivotCharts, and KPIs.

    - Added trendline charts to show churn drivers.

## Key Insights

## Dashboard Preview

## Recommendations

## How to Use This Project

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/muftau/investigating-customer-churn)

2. Open the Excel workbook (Churn_Analysis_Dashboard.xlsx).

3. Use the slicers and filters to explore churn by customer attributes.
