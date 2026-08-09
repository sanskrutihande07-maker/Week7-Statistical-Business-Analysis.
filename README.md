# Week7-Statistical-Business-Analysis.
Statistical Business Analysis using Python, Pandas, SciPy, Seaborn and Scikit-learn. The project includes descriptive statistics, normality testing, correlation analysis, hypothesis testing, confidence intervals and linear regression.



# Statistical Business Analysis

## 📊 Project Overview

Statistical Business Analysis is a data science project that applies statistical techniques to business sales data.

The project analyzes sales performance using descriptive statistics, data distribution analysis, normality testing, correlation analysis, hypothesis testing, confidence intervals, and linear regression.

The main objective is to identify meaningful statistical relationships in sales data and translate the findings into actionable business insights.

---

## 🎯 Project Objectives

- Calculate descriptive statistics
- Analyze data distributions
- Perform normality testing
- Calculate Pearson correlation
- Perform hypothesis testing
- Compare sales across regions
- Calculate 95% confidence intervals
- Calculate margin of error
- Perform linear regression
- Calculate R-squared
- Interpret statistical results
- Provide business recommendations

---

## 📁 Dataset

The project uses a business sales dataset containing **100 records** and **7 columns**.

### Dataset Columns

| Column | Description |
|---|---|
| Date | Date of the transaction |
| Product | Product sold |
| Quantity | Number of units sold |
| Price | Price of the product |
| Customer_ID | Unique customer identifier |
| Region | Sales region |
| Total_Sales | Total sales value |

### Data Quality

- Total Records: **100**
- Total Columns: **7**
- Missing Values: **0**
- Duplicate Rows: **0**
- Regions: **East, North, South, West**

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- Jupyter Notebook

---

## 📈 Statistical Methods

### 1. Descriptive Statistics

The following statistics were calculated:

- Mean
- Median
- Mode
- Standard deviation
- Variance
- Minimum
- Maximum
- Quartiles

### 2. Distribution Analysis

The following visualizations were created:

- Histograms
- KDE density plots

### 3. Normality Testing

The **Shapiro-Wilk test** was used to determine whether numerical variables follow a normal distribution.

Significance level:

**α = 0.05**

### 4. Correlation Analysis

Pearson correlation was calculated between:

- Quantity and Price
- Quantity and Total_Sales
- Price and Total_Sales

### 5. Hypothesis Testing

Three hypothesis tests were performed:

1. One-Sample t-Test
2. Independent Two-Sample Welch t-Test
3. One-Way ANOVA

### 6. Confidence Interval

A **95% confidence interval** was calculated for Total_Sales.

### 7. Regression Analysis

Linear regression was performed using:

**Independent Variable:** Price

**Dependent Variable:** Total_Sales

---

## 📊 Key Statistical Results

### Descriptive Statistics

| Variable | Mean | Median | Standard Deviation |
|---|---:|---:|---:|
| Quantity | 4.78 | 5.00 | 2.5882 |
| Price | ₹25,808.51 | ₹24,192.00 | ₹13,917.63 |
| Total_Sales | ₹123,650.48 | ₹97,955.50 | ₹100,161.09 |

---

## 🔬 Normality Test Results

| Variable | Test Statistic | P-value | Result |
|---|---:|---:|---|
| Quantity | 0.9304 | 0.0001 | Not normally distributed |
| Price | 0.9475 | 0.0006 | Not normally distributed |
| Total_Sales | 0.8989 | <0.0001 | Not normally distributed |

Since all p-values are below 0.05, the null hypothesis of normality is rejected for all three variables.

---

## 🔗 Correlation Analysis

| Variable | Correlation with Total_Sales |
|---|---:|
| Quantity | 0.6881 |
| Price | 0.6461 |

### Interpretation

Quantity has a positive relationship with Total_Sales.

Price also has a positive relationship with Total_Sales.

The correlation between Quantity and Price is approximately **0.01**, indicating almost no linear relationship between them.

---

## 🧪 Hypothesis Testing Results

### One-Sample t-Test

**Business Question:**

Is the average Total_Sales significantly different from ₹100,000?

- Benchmark Mean: ₹100,000
- Sample Mean: ₹123,650.48
- t-statistic: 2.3612
- p-value: 0.020172

### Result

**Reject H₀**

The average Total_Sales is statistically significantly different from ₹100,000.

---

### Independent Two-Sample Welch t-Test

**Business Question:**

Is average Total_Sales significantly different between North and South?

| Region | Average Total_Sales |
|---|---:|
| North | ₹142,272.68 |
| South | ₹138,438.96 |

- t-statistic: 0.1299
- p-value: 0.897152

### Result

**Fail to reject H₀**

There is insufficient statistical evidence to conclude that average Total_Sales differs between North and South.

---

### One-Way ANOVA

**Business Question:**

Is there a statistically significant difference in average Total_Sales among East, North, South, and West?

- F-statistic: 2.1644
- p-value: 0.097237

### Result

**Fail to reject H₀**

There is insufficient statistical evidence to conclude that average Total_Sales differs significantly among the four regions.

---

## 📐 Confidence Interval

### 95% Confidence Interval for Total_Sales

- Sample Mean: ₹123,650.48
- Standard Error: ₹10,016.11
- Margin of Error: ₹19,874.13
- Lower Bound: ₹103,776.35
- Upper Bound: ₹143,524.61

### Confidence Interval

**₹103,776.35 to ₹143,524.61**

---

## 📉 Linear Regression

### Regression Model

**Independent Variable:** Price

**Dependent Variable:** Total_Sales

### Regression Equation

```text
Total_Sales = 3640.54 + (4.65 × Price)

---


##🧪 Statistical Testing Summary
One-Sample t-Test
Benchmark Mean: ₹100,000
Sample Mean: ₹123,650.48
t-statistic: 2.3612
p-value: 0.020172
Result: ✅ Reject H₀

The average Total_Sales is statistically significantly different from ₹100,000.

Independent Two-Sample t-Test

North vs South

North Average: ₹142,272.68
South Average: ₹138,438.96
t-statistic: 0.1299
p-value: 0.897152
Result: ✅ Fail to Reject H₀

There is no statistically significant difference in average Total_Sales between North and South.

One-Way ANOVA
F-statistic: 2.1644
p-value: 0.097237
Result: ✅ Fail to Reject H₀

There is no statistically significant difference in Total_Sales among the four regions.

###
📐 Confidence Interval
95% Confidence Interval for Total_Sales
Sample Mean: ₹123,650.48
Standard Error: ₹10,016.11
Margin of Error: ₹19,874.13
Lower Bound: ₹103,776.35
Upper Bound: ₹143,524.61
📌 Confidence Interval

₹103,776.35 to ₹143,524.61

# 📊 Visualizations

## 1. Quantity Histogram

![Quantity Histogram](visualizations/Quantity_histogram.png)

---

## 2. Price Histogram

![Price Histogram](visualizations/Price_histogram.png)

---

## 3. Total Sales Histogram

![Total Sales Histogram](visualizations/Total_Sales_histogram.png)

---

## 4. Price KDE Plot

![Price KDE Plot](visualizations/Price_kde.png)

---

## 5. Quantity KDE Plot

![Quantity KDE Plot](visualizations/Quantity_kde.png)

---

## 6. Total Sales KDE Plot

![Total Sales KDE Plot](visualizations/Total_Sales_kde.png)

---

## 7. Correlation Heatmap

![Correlation Heatmap](visualizations/correlation_heatmap.png)

---

## 8. Regional Sales Boxplot

![Regional Sales Boxplot](visualizations/regional_sales_boxplot.png)

---

## 9. Price vs Total Sales Regression Plot

![Price vs Total Sales Regression Plot](visualizations/regression_plot.png)

---

# 💡 Business Insights

### Key Findings

- 📌 Average **Total_Sales** is **₹123,650.48**.
- 📌 Average sales are significantly different from the **₹100,000 benchmark**.
- 📌 **Quantity** has a positive relationship with **Total_Sales**.
- 📌 **Price** has a positive relationship with **Total_Sales**.
- 📌 **North** has the highest observed average sales among the four regions.
- 📌 **West** has the lowest observed average sales.
- 📌 Regional differences are **not statistically significant at the 5% significance level**.
- 📌 Price explains approximately **41.75% of the variation in Total_Sales**.
- 📌 Quantity, Price, and Total_Sales do not follow a normal distribution according to the Shapiro-Wilk test.
- 📌 The average Total_Sales is statistically different from the **₹100,000 benchmark**.
- 📌 There is no statistically significant difference between North and South average sales.
- 📌 There is no statistically significant difference in sales among the four regions.

---

# 🚀 Business Recommendations

### Recommended Actions

### 1. Monitor Quantity and Price Together

Monitor Quantity and Price together when evaluating sales performance because both variables show positive relationships with Total_Sales.

### 2. Investigate High-Value Transactions

Investigate factors that influence high-value transactions because these transactions can significantly affect the overall average sales.

### 3. Avoid Region-Based Decisions Alone

Do not make major regional decisions based only on observed averages because the ANOVA result was not statistically significant.

### 4. Analyze Additional Business Factors

Future analysis should include:

- Product category
- Discounts
- Customer behaviour
- Marketing expenditure
- Seasonality

### 5. Use Multiple Regression

Use multiple regression in future analysis to include additional business variables and better understand the factors influencing sales.

### 6. Collect More Data

Collect a larger dataset to improve the reliability and generalizability of future statistical analysis.

---

# 🏁 Conclusion

This project demonstrates the practical application of **statistics in business data analysis**.

The analysis identified positive relationships between **Quantity, Price, and Total_Sales**.

The average Total_Sales was statistically significantly different from the **₹100,000 benchmark**, while regional differences were not statistically significant.

The regression analysis showed that **Price explains approximately 41.75% of the variation in Total_Sales**.

The analysis also showed that the numerical sales variables do not follow a normal distribution according to the Shapiro-Wilk test.

Overall, this project demonstrates how statistical analysis can support **data-driven business decisions**, identify important relationships in sales data, and highlight areas for further investigation.
---
