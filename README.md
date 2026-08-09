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
###.
🧪 Statistical Testing Summary
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


---


### visualizations/
    ├── Quantity_histogram.png

<img width="1181" height="620" alt="Quantity_histogram" src="https://github.com/user-attachments/assets/f1fede91-4d1d-420f-9004-f977cb2710ae" />

   
    ├── Price_histogram.png
****<img width="1138" height="631" alt="Price_histogram" src="https://github.com/user-attachments/assets/d1034814-84bc-42f3-bb28-e5aaf3504458" />

    ├── Total_Sales_histogram.png

<img width="1072" height="616" alt="Total_Sales_histogram" src="https://github.com/user-attachments/assets/47c2c91a-7570-4462-b808-ce7be9073a36" />

    ├── Price_kde.png
<img width="1147" height="635" alt="Price_kde" src="https://github.com/user-attachments/assets/b43ae6ee-cf16-4d08-9008-c6f93cc9aac3" />

    ├── Quantity_kde.png
<img width="1081" height="611" alt="Quantity_kde" src="https://github.com/user-attachments/assets/7094ad61-6e1e-4f2c-8fe9-e3089b352695" />

    
    ├── Total_Sales_kde.png

<img width="1157" height="627" alt="Total_Sales_kde" src="https://github.com/user-attachments/assets/a8d02099-e9d4-47fe-848b-d21b7413a929" />

    ├── correlation_heatmap.png

<img width="736" height="589" alt="correlation_heatmap" src="https://github.com/user-attachments/assets/74afbfd9-dbe5-4ee5-a98c-ac285e7cf6d9" />

    ├── regional_sales_boxplot.png
<img width="889" height="590" alt="regional_sales_boxplot" src="https://github.com/user-attachments/assets/27462fba-179c-42ee-9b5b-179d0ae6664d" />

    └── regression_plot.png
<img width="889" height="590" alt="regression_plot" src="https://github.com/user-attachments/assets/8b416d5b-0a53-49cc-91c3-95d550695159" />

.
###
💡 Business Insights
Average Total_Sales is ₹123,650.48.
Average sales are significantly different from the ₹100,000 benchmark.
Quantity has a positive relationship with Total_Sales.
Price has a positive relationship with Total_Sales.
North has the highest observed average sales among the four regions.
West has the lowest observed average sales.
Regional differences are not statistically significant at the 5% significance level.
Price explains approximately 41.75% of the variation in Total_Sales.
The sales variables do not follow a normal distribution according to the Shapiro-Wilk test.


###🚀 Business Recommendations
Monitor Quantity and Price together when evaluating sales performance.
Investigate factors that influence high-value transactions because they affect the overall average sales.
Do not make major regional decisions based only on observed averages because the ANOVA result was not statistically significant.
Analyze additional factors such as product category, discounts, customer behaviour, marketing expenditure, and seasonality.
Use multiple regression in future analysis to include additional business variables.
Collect a larger dataset to improve the reliability of future statistical analysis.




### 🏁 Conclusion

This project demonstrates the practical application of statistics in business data analysis.

The analysis identified positive relationships between Quantity, Price, and Total_Sales. The average Total_Sales was significantly different from the ₹100,000 benchmark, while regional differences were not statistically significant.

The regression analysis showed that Price explains approximately 41.75% of the variation in Total_Sales.

Overall, the project demonstrates how statistical analysis can support data-driven business decisions and identify areas for further investigation.
