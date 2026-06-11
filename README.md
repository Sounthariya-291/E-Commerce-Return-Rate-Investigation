# E-Commerce Return Rate Investigation

## Project Overview

This project focuses on analyzing e-commerce transaction data to identify factors influencing product return behavior. The analysis was performed using Python, Pandas, NumPy, Matplotlib, Seaborn, and SciPy. Various statistical and exploratory data analysis techniques were applied to understand return patterns and provide business recommendations.

---

## Objectives

* Analyze e-commerce transaction data.
* Identify factors affecting product returns.
* Investigate the impact of delivery duration, discounts, and product categories on returns.
* Perform correlation analysis and hypothesis testing.
* Segment customers based on return behavior.
* Provide business recommendations to reduce return rates.

---

## Dataset Description

The dataset contains e-commerce transaction records with customer, product, sales, and shipping information.

### Dataset Summary

* Total Records: 51,290
* Total Features: 16
* Missing Values: 8
* Duplicate Records: 0

### Features

* Order_Date
* Time
* Aging
* Customer_Id
* Gender
* Device_Type
* Customer_Login_type
* Product_Category
* Product
* Sales
* Quantity
* Discount
* Profit
* Shipping_Cost
* Order_Priority
* Payment_method

---

## Data Cleaning and Preprocessing

The following preprocessing steps were performed:

* Loaded the dataset using Pandas.
* Checked dataset dimensions and structure.
* Identified missing values.
* Verified duplicate records.
* Generated descriptive statistics.
* Created a return indicator variable for analysis.

### Missing Values

* Aging – 1
* Sales – 1
* Quantity – 2
* Discount – 1
* Shipping_Cost – 1
* Order_Priority – 2

### Duplicate Records

* Duplicate Records Found: 0

---

## Exploratory Data Analysis (EDA)

### Return Rate Analysis

* Total Orders: 51,290
* Returned Orders: 14,385
* Return Rate: 28.05%

### Category-wise Return Rate

| Product Category   | Return Rate (%) |
| ------------------ | --------------- |
| Home & Furniture   | 29.99           |
| Auto & Accessories | 29.61           |
| Electronic         | 28.03           |
| Fashion            | 26.42           |

### Observations

* Home & Furniture products show the highest return rate.
* Fashion products show the lowest return rate.
* Return behavior varies across categories.

---

## Correlation Analysis

Correlation analysis was performed among numerical variables.

### Key Findings

* Aging and Returned = 0.791
* Sales and Profit = 0.917
* Sales and Shipping Cost = 0.917

### Observation

Delivery duration (Aging) has the strongest relationship with return behavior.

---

## Outlier Analysis

Outliers were detected using boxplots.

### Identified Outliers

* High Sales transactions
* Long Delivery Duration records
* High Shipping Cost transactions

These outliers may influence return trends and business performance.

---

## Hypothesis Testing

### Null Hypothesis (H₀)

Delivery delay has no impact on return behavior.

### Alternative Hypothesis (H₁)

Delivery delay significantly impacts return behavior.

### Results

* T-Statistic = NaN
* P-Value = NaN

Although the T-Test did not produce a valid result, correlation analysis indicates a strong relationship between delivery duration and return behavior.

---

## Customer Segmentation

High-return customers were identified using return frequency.

### Sample High-Return Customers

* Customer ID 82069
* Customer ID 96431
* Customer ID 82256
* Customer ID 82604
* Customer ID 71200

---

## Key Findings

* Overall return rate is 28.05%.
* Home & Furniture has the highest return rate.
* Fashion has the lowest return rate.
* Aging (delivery duration) is the most influential factor associated with returns.
* Sales, Profit, and Shipping Cost are highly correlated.
* No duplicate records were found.
* Only 8 missing values were present in the dataset.

---

## Business Recommendations

* Improve delivery efficiency and reduce delays.
* Monitor high-return product categories.
* Improve product descriptions and quality control.
* Track customers with frequent returns.
* Implement predictive analytics for return prevention.

---

## Conclusion

The analysis revealed that delivery duration plays a significant role in return behavior. Product categories such as Home & Furniture and Auto & Accessories exhibit relatively higher return rates. Improving delivery performance and customer experience can help reduce return rates and enhance business profitability.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Google Colab

---

## Project Structure

E-Commerce-Return-Rate-Investigation/

├── data/
│   └── E-commerce Dataset.csv

├── notebooks/
│   └── Task_5ecommerce_return_rate_investigation.ipynb

├── reports/
│   └── Final_Report.pdf

├── images/
│   ├── sales_distribution.png
│   ├── return_by_category.png
│   └── heatmap.png

├── README.md

└── requirements.txt

## Author


Sounthariya
