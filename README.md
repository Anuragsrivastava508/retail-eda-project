# Project 1: Exploratory Data Analysis (EDA)

## Retail Customer Sales Dataset

**Name:** Anurag Srivastava
**Roll Number / Unique ID:** 2026M01410026
**Program:** HCL / Career Shaper Data Analyst Training

## Project Overview

This project explores a dataset of approximately 7,000 retail
transactions from India covering 2023-2024. The goal was to look beyond
raw numbers and understand what was happening in the business: how
customers buy, which products generate the most value, and whether the
data reveals any areas that need attention.

The work follows the complete EDA process, from checking and cleaning
the source data to analysing sales patterns and presenting practical
business findings. Python, Pandas, NumPy, Matplotlib, and Seaborn were
used throughout the analysis.

## Repository Structure

```text
Project1-EDA/
|-- RollNo_Name_Project1_EDA.ipynb   # Analysis, code, charts, and outputs
|-- data/
|   `-- retail_customer_sales_dataset.csv
|-- outputs/
|   `-- cleaned_retail_customer_sales.csv
|-- figures/
|   `-- Generated charts and visualisations
|-- report/
|   |-- Retail_Customer_Sales_Insights_Report.docx
|   `-- Retail_Customer_Sales_Insights_Report.pdf
`-- requirements.txt
```

## Dataset Details

| Detail          | Description                           |
| --------------- | ------------------------------------- |
| Domain          | Retail customer and transaction sales |
| Period          | 2023-2024                             |
| Geography       | Four regions of India                 |
| Raw dataset     | 7,084 rows and 24 columns             |
| Cleaned dataset | 7,000 rows                            |
| Data format     | CSV                                   |

## Project Objectives

1. Inspect the structure, dimensions, columns, and data types.
2. Check for missing values, duplicate records, inconsistent categories,
   invalid numbers, and date-format problems.
3. Clean the data using methods that are clear and easy to explain.
4. Review numerical and categorical distributions through descriptive
   statistics.
5. Identify outliers using the IQR and Z-score methods.
6. Create useful features such as `Profit_Margin`, `Delivery_Days`, and
   `Revenue_per_Customer`.
7. Answer business questions using grouping and aggregation.
8. Present the important findings in a clear, practical report.

## How to Run the Project

### 1. Requirements

- Python 3.10 or later
- Jupyter Notebook / JupyterLab
- The libraries listed in `requirements.txt`

### 2. Install dependencies

Open a terminal at the project root and run:

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the analysis

Open `RollNo_Name_Project1_EDA.ipynb`, then choose
**Kernel > Restart & Run All** or **Run All**.

> **Tip:** Start Jupyter from the repository root. This ensures that the
> notebook can correctly find the `data`, `outputs`, and `figures`
> folders.

## Analysis Workflow

1. **Setup and inspection:** Loaded the CSV and reviewed the shape,
   columns, data types, and sample records.
2. **Data-quality audit:** Checked missing values, duplicates,
   inconsistent labels, impossible values, and date-format issues.
3. **Data cleaning:** Standardised categories, handled missing and
   invalid values, removed duplicate transactions, and documented each
   decision.
4. **Descriptive statistics:** Calculated measures such as mean, median,
   mode, standard deviation, variance, quartiles, and IQR.
5. **Univariate analysis:** Examined numerical distributions and
   categorical frequencies.
6. **Outlier analysis:** Applied IQR and Z-score methods and reviewed
   flagged observations.
7. **Feature engineering:** Created `Profit_Margin`, `Delivery_Days`,
   `Revenue_per_Customer`, and useful analytical groups.
8. **Business analysis:** Used `groupby()` and aggregation to answer ten
   business questions.
9. **Key findings:** Turned the results into a concise set of insights
   and recommendations.

## Key Data-Quality Results

The source data was usable, but it needed several corrections before
analysis:

- Removed **84 duplicate transactions**.
- Standardised **8 gender variants** and **12 region variants**.
- Parsed **4 date formats** into consistent date fields.
- Reviewed and handled **12 impossible values**.
- Flagged **15 records** where the delivery date was earlier than the
  order date.

The cleaned dataset now contains 7,000 transactions. The notebook
includes the detailed audit, cleaning decisions, and validation checks.

## Key Business Results

| Metric                               |            Result |
| ------------------------------------ | ----------------: |
| Total sales                          |     ₹76.7 million |
| Total profit                         |     ₹25.1 million |
| Overall profit margin                |             32.7% |
| Return rate                          |             12.6% |
| Sales from Electronics and Furniture | Approximately 83% |

### Major Insights

1. **Sales are concentrated in a few categories.** Electronics and
   Furniture account for roughly 83% of total sales, so they deserve
   close attention in forecasting and inventory planning.
2. **Profit margins are fairly similar across categories.** Differences
   in sales contribution appear to be driven more by volume and product
   mix than by a large gap in category margin.
3. **Higher discounts do not appear to increase purchase quantity.**
   Before changing the discount strategy, it would be useful to test
   whether discounts affect customer behaviour through promotions or
   controlled experiments.
4. **Delivery-mode performance needs review.** In this dataset,
   Express and Same-Day delivery do not show faster delivery times than
   Standard delivery. The service definitions and delivery promises may
   need closer examination.
5. **Customer ratings and returns may be connected.** Lower ratings are
   associated with higher return rates. Return reasons and product or
   service-quality information would help explain this relationship.

> These findings describe patterns in the supplied dataset. They do not
> establish cause and effect.

## Project Deliverables

| Deliverable                                           | Location                                                       |
| ----------------------------------------------------- | -------------------------------------------------------------- |
| Jupyter notebook with code, outputs, and explanations | `RollNo_Name_Project1_EDA.ipynb`                               |
| Original raw dataset                                  | `data/retail_customer_sales_dataset.csv`                       |
| Cleaned dataset                                       | `outputs/cleaned_retail_customer_sales.csv`                    |
| Charts and visualisations                             | `figures/`                                                     |
| Written insights report                               | `report/Retail_Customer_Sales_Insights_Report.docx` and `.pdf` |

## Conclusion

This project shows how EDA can turn raw retail transactions into a more
consistent and useful view of business performance. The work combines
data-quality checks, documented cleaning, statistical profiling,
outlier review, feature engineering, and grouped analysis.

The main takeaways are the importance of Electronics and Furniture to
sales, the need to review delivery performance and discount
effectiveness, and the possible link between customer feedback and
product returns.

**Project:** Project 1 --- Exploratory Data Analysis (Retail Customer Sales)

**Training Program:** HCL / Career Shaper Data Analyst Training

**Prepared by:** Anurag Srivastava
