# 📊 Business Employment Trend Analysis Using Python (2011 - 2026)

> An end-to-end data analytics project that analyzes business employment trends across industries in New Zealand from 2011 to 2026 using Python.

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-2E8B57)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?logo=googlecolab)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)

---

## 📌 Project Overview

This project analyzes the **Business Employment Data** published by **Stats NZ (New Zealand Government)** to understand employment trends across industries between **2011 and 2026**.

The analysis focuses on identifying employment growth, industry-wise workforce distribution, long-term employment changes, and quarterly seasonal patterns using Python-based data analysis techniques.

The project demonstrates a complete Data Analytics workflow, including:

- 📂 Business Understanding
- 🧹 Data Cleaning & Preprocessing
- ⚙️ Feature Engineering
- 📊 Exploratory Data Analysis (EDA)
- 📈 Statistical Analysis
- 📉 Data Visualization
- 💡 Business Insights & Recommendations

  ---

  # ❓ Problem Statement

Business employment is a key indicator of a country's economic performance and workforce dynamics. Understanding how employment levels change across industries over time helps identify growing sectors, declining industries, and seasonal employment patterns that influence business and policy decisions.

The **Stats NZ Business Employment Dataset** contains quarterly employment information across multiple industries in New Zealand from **2011 to 2026**. However, the large volume of data makes it difficult to identify long-term trends, compare workforce participation across industries, and understand seasonal fluctuations without systematic analysis.

This project applies Python-based data analytics techniques to analyze employment trends, compare industry performance, evaluate long-term employment growth, and identify seasonal employment patterns. The insights generated can support workforce planning, economic analysis, and evidence-based business decision-making.

---

# 📂 Dataset

| **Attribute** | **Details** |
|---------------|-------------|
| **Dataset Name** | Business Employment Indicators |
| **Source** | Stats NZ (New Zealand Government) |
| **Time Period** | 2011 – 2026 |
| **File Format** | CSV |
| **Original Records** | 26,059 |
| **Records After Cleaning** | 23,220 |
| **Features (After Cleaning)** | 13 Columns |
| **Analysis Environment** | Google Colab |

### 📖 Dataset Description

The dataset contains quarterly business employment information across various industries in New Zealand. It includes employment-related indicators such as **Filled Jobs**, **Total Earnings**, employment categories, adjustment types (**Actual**, **Seasonally Adjusted**, and **Trend**), and time-related information.

After preprocessing, the dataset was cleaned by removing suppressed records, handling missing values, renaming columns, engineering new features, and preparing the data for statistical analysis and visualization.

---

# 📁 Project Files

This repository contains the following project files:

- 📄 Raw Dataset
- 📄 Cleaned Dataset
- 📓 Google Colab Notebook
- 🐍 Python Source Code
- 📊 Data Visualizations
- 📑 Project Report (PDF)
- 📄 README.md

---

# 🎯 Project Objectives

### Objective 1
Analyze quarterly business employment trends across industries from **2011 to 2026** to understand how employment levels have changed over time.

### Objective 2
Compare employment levels across different industries to identify sectors with the **highest** and **lowest** workforce participation.

### Objective 3
Examine long-term employment growth, decline, and stability across industries to identify consistent employment patterns.

### Objective 4
Identify seasonal and quarterly employment patterns using **Actual**, **Seasonally Adjusted**, and **Trend** data to distinguish seasonal fluctuations from long-term employment trends.

---

# 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Git
- GitHub

---

# 🧹 Data Preprocessing

The raw dataset was cleaned and transformed to improve data quality and ensure accurate analysis. Several preprocessing techniques were applied before performing statistical analysis and visualization.

## Data Cleaning

The following data cleaning steps were performed:

- Removed **suppressed records** to ensure reliable analysis.
- Checked for **missing values** and handled them appropriately.
- Removed unnecessary columns that did not contribute to the analysis.
- Renamed column names for better readability.
- Verified data types and converted columns where required.
- Checked for duplicate records.
- Prepared a clean dataset for further analysis.

### Data Cleaning Summary

| Step | Description |
|------|-------------|
| Missing Values | Checked and handled appropriately |
| Suppressed Records | Removed |
| Duplicate Records | Verified |
| Unnecessary Columns | Removed |
| Column Renaming | Completed |
| Data Type Validation | Completed |

---

## ⚙️ Feature Engineering

To make the dataset suitable for trend analysis, new features were created from the existing data.

The following features were engineered:

- 📅 **Year** extracted from the Period column.
- 📅 **Quarter** derived from the reporting period.
- 🏷️ Renamed **Series_title_1** to **Employment Variable**.
- 🏷️ Renamed **Series_title_2** to **Category**.
- 🏷️ Renamed **Series_title_3** to **Adjustment Type**.

These engineered features simplified the analysis and enabled year-wise, quarter-wise, and industry-wise comparisons.

---

# 📊 Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) was performed to understand the structure of the dataset, identify patterns, detect anomalies, and summarize important characteristics before applying statistical analysis.

The EDA process included:

- Dataset overview
- Data type inspection
- Missing value analysis
- Duplicate record verification
- Summary statistics
- Distribution analysis
- Category-wise exploration
- Time-based exploration
- Industry-wise analysis

---

# 📊 Statistical Analysis

Statistical analysis was performed to summarize the employment data and understand its overall distribution, variability, and trends. These statistical measures provide meaningful insights into workforce patterns across industries and support data-driven decision-making.

The following statistical techniques were applied:

- Measure of Central Tendency
- Variance
- Standard Deviation
- Skewness
- Kurtosis
- Outlier Detection

---

## 📌 Measure of Central Tendency

Measure of Central Tendency was used to identify the typical employment level in the dataset.

| Metric | Value |
|---------|------:|
| Mean | 74,018.02 |
| Median | 14,265.50 |
| Mode | 287.00 |

### 📈 Interpretation

- The **mean employment value** is **74,018.02**, representing the average employment across all observations.
- The **median (14,265.50)** is significantly lower than the mean, indicating that most observations have relatively lower employment values.
- The **mode (287)** represents the most frequently occurring employment value.
- The large difference between the mean and median suggests the presence of several industries with exceptionally high employment values.

<img width="1287" height="622" alt="Screenshot 2026-09-03 010623" src="https://github.com/user-attachments/assets/a70e18ef-9d50-4ba2-8b5f-0a8d867c88f0" />


```md
![Central Tendency](images/central_tendency.png)
```

---

## 📌 Variance & Standard Deviation

Variance and Standard Deviation were calculated to measure the spread of employment values.

| Metric | Value |
|---------|------:|
| Variance | 45,905,395,632.10 |g
| Standard Deviation | 214,255.44 |

### 📈 Interpretation

- The dataset has a **high standard deviation**, indicating considerable variation in employment levels across industries.
- The large variance reflects the wide gap between industries with low employment and those with very high workforce participation.
- This suggests that employment is not evenly distributed among industries.

---
## 📌 Distribution Analysis

Distribution analysis helps understand the shape of the employment data.

| Metric | Value |
|---------|------:|
| Skewness | 6.96 |
| Kurtosis | 57.55 |

### 📈 Interpretation

- The dataset is **highly positively skewed**, indicating that most industries have moderate employment levels while a few industries employ significantly larger workforces.
- The high kurtosis value indicates the presence of extreme values (outliers).
- Such a distribution is common in economic and employment datasets where a small number of industries dominate employment.

<img width="1317" height="627" alt="Screenshot 2026-08-24 222234" src="https://github.com/user-attachments/assets/4037de2e-745e-44fa-88f6-1b9707aef151" />


```md
![Distribution](images/distribution.png)
```

---

## 📌 Outlier Detection

Outliers were identified using the **Interquartile Range (IQR)** method.

| Metric | Value |
|--------|-------|
| Interquartile Range (IQR) | *(Your calculated IQR)* |
| Lower Bound | *(Your calculated lower limit)* |
| Upper Bound | *(Your calculated upper limit)* |
| Number of Outliers | **2,986** |

### 📈 Interpretation

- The IQR method identified **2,986 observations** as potential outliers.
- These observations mainly represent industries or employment categories with exceptionally high employment values.
- Since these values reflect genuine business and economic conditions rather than data entry errors, they were **retained** in the dataset.
- Keeping these observations ensures that the analysis accurately represents real-world employment patterns across industries.

<img width="911" height="536" alt="Screenshot 2026-09-03 010647" src="https://github.com/user-attachments/assets/ea580a72-3ca8-44db-8c2d-ccc6ed834ed5" />

```md
![Box Plot](images/boxplot.png)
```

---

# 🎯 Objective 1: Analyze Quarterly Business Employment Trends (2011–2026)

## 📌 Objective

Analyze quarterly business employment trends across industries from **2011 to 2026** to understand how employment levels have changed over time.

---

## 📊 Analysis Performed

The following analyses were conducted to understand employment trends over time:

- Year-wise employment trend analysis
- Quarter-wise employment trend analysis
- Year and Quarter comparison
- Employment trend visualization
- Trend interpretation and business insights

---

## 📈 Visualizations

### 1️⃣ Year-wise Business Employment Trend

<img width="1303" height="595" alt="Screenshot 2026-09-03 010821" src="https://github.com/user-attachments/assets/9239bd4b-8b5b-4fed-a1b6-57d0091fff8a" />

```markdown
![Year-wise Employment Trend](images/yearwise_employment_trend.png)
```

### 🔍 Key Insights

- Business employment showed an overall increasing trend from **2011 to 2025**.
- Employment growth accelerated after **2021**, indicating strong post-pandemic workforce recovery.
- **2023 and 2024** recorded the highest employment levels in the dataset.
- The slight reduction observed in **2025** is marginal and does not indicate a long-term decline.
- **2026** includes only **Quarter 1** data and was excluded from trend interpretation to ensure a fair year-wise comparison.

---

### 2️⃣ Quarter-wise Employment Distribution

<img width="1061" height="616" alt="Screenshot 2026-09-03 010922" src="https://github.com/user-attachments/assets/e82aa02a-21da-4fef-b0d2-3b5c70f41dc6" />

```markdown
![Quarter-wise Employment](images/quarterwise_employment.png)
```

### 🔍 Key Insights

- Employment levels remain relatively consistent across all four quarters.
- Quarter 4 recorded slightly higher employment compared to the other quarters.
- No quarter experienced a significant drop in employment, indicating stable workforce demand throughout the year.
- Quarterly fluctuations are relatively small, suggesting limited seasonal variation at the overall business level.

---

## 💡 Business Insights

- Business employment in New Zealand has shown steady long-term growth over the study period.
- The consistent increase in employment reflects positive workforce expansion across industries.
- Quarterly employment remained relatively stable, indicating that most industries maintain workforce levels throughout the year.
- The findings suggest a resilient labor market with limited seasonal fluctuations in overall employment.

---

## ✅ Recommendation

- Continue monitoring employment trends on a quarterly basis to identify emerging changes in workforce demand.
- Use long-term employment trends to support workforce planning and strategic business decisions.
- Future studies can extend the analysis by examining employment trends at the individual industry level to identify sector-specific growth opportunities.

---

# 🎯 Objective 2: Compare Employment Levels Across Industries

## 📌 Objective

Compare employment levels across different industries to identify sectors with the **highest**  workforce participation.

---

## 📊 Analysis Performed

The following analyses were conducted:

- Industry-wise employment comparison
- Top 10 industries by employment
- Bottom 10 industries by employment
- Industry ranking
- Workforce distribution analysis

---

## 📈 Visualizations

### 1️⃣ Top 10 Industries by Employment

<img width="1497" height="721" alt="Screenshot 2026-09-03 010901" src="https://github.com/user-attachments/assets/18846f7e-5c7f-4e1e-92bb-7c6bbc61a7c3" />

```markdown
![Top 10 Industries](images/top10_industries.png)
```

### 🔍 Key Insights

- **Health Care and Social Assistance** emerged as one of the largest employers.
- **Manufacturing** consistently maintained a high level of workforce participation.
- **Retail Trade** and **Construction** employed a significant number of workers, highlighting their importance to the economy.
- The top industries together account for a substantial share of total employment.

---

## 💡 Business Insights

- Service-oriented industries contribute significantly to national employment.
- Manufacturing and retail continue to play a vital role in providing employment opportunities.
- Capital-intensive industries operate efficiently with comparatively smaller workforces.
- Understanding industry-wise employment helps businesses and policymakers identify sectors with strong labor demand.

---

## ✅ Recommendation

- Prioritize workforce development and skill enhancement programs in high-employment industries.
- Encourage innovation and investment in industries with lower employment potential to improve productivity and create new opportunities.
- Monitor employment trends regularly to support strategic workforce planning and informed policy decisions.

---

---

# 🎯 Objective 3: Examine Long-Term Employment Growth, Decline, and Stability Across Industries

## 📌 Objective

Examine long-term employment growth, decline, and stability across industries to identify sectors with consistent growth, declining employment, and stable workforce patterns over time.

---

## 📊 Analysis Performed

The following analyses were conducted:

- Industry-wise employment growth analysis
- Percentage growth calculation (2011–2025)
- Top growing industries
- Stable employment trend analysis
- Long-term workforce pattern evaluation

---

## 📈 Visualizations

### 1️⃣ Top Growing Industries (2011–2025)

<img width="1274" height="707" alt="Screenshot 2026-09-03 010947" src="https://github.com/user-attachments/assets/a3a13f57-de83-4442-b467-5021f5f1ffa5" />

```markdown
![Top Growing Industries](images/top_growing_industries.png)
```

### 🔍 Key Insights

- **Construction** experienced one of the highest employment growth rates during the study period.
- **Health Care and Social Assistance** showed strong and consistent workforce expansion.
- **Professional, Scientific and Technical Services** recorded substantial long-term growth.
- Growth in these industries reflects increasing economic activity, infrastructure development, and demand for skilled professionals.

---

### 3️⃣ Industry Growth Comparison

<img width="1139" height="592" alt="Screenshot 2026-09-03 011126" src="https://github.com/user-attachments/assets/0aabab4e-091e-4e68-bcef-729b79d55770" />

```markdown
![Industry Growth Comparison](images/industry_growth_comparison.png)
```

### 🔍 Key Insights

- Employment growth varied considerably across industries.
- Service-oriented industries generally demonstrated stronger long-term workforce expansion.
- Traditional and capital-intensive industries exhibited relatively stable or moderate growth.
- The analysis highlights differences in workforce demand across sectors over time.

---

## 💡 Business Insights

- Long-term employment trends indicate that workforce growth is concentrated in industries experiencing sustained economic expansion.
- Industries with stable employment demonstrate resilience and consistent labor demand.
- Growth-oriented industries present greater opportunities for employment, investment, and workforce development.
- Declining or slow-growing industries may benefit from innovation, technology adoption, and workforce reskilling initiatives.

---

## ✅ Recommendation

- Focus workforce planning and skill development initiatives on industries with strong long-term growth potential.
- Encourage investment and innovation in industries experiencing slower employment growth.
- Regularly monitor industry employment trends to support strategic planning and evidence-based decision-making.
- Promote reskilling and upskilling programs to help workers transition into expanding industries.

---

---

# 🎯 Objective 4: Identify Seasonal and Quarterly Employment Patterns

## 📌 Objective

Identify seasonal and quarterly employment patterns using **Actual**, **Seasonally Adjusted**, and **Trend** data to evaluate how employment varies across quarters and distinguish seasonal fluctuations from long-term employment trends.

---

## 📊 Analysis Performed

The following analyses were conducted:

- Quarter-wise employment trend analysis
- Comparison of Actual, Seasonally Adjusted, and Trend employment data
- Seasonal variation analysis
- Long-term employment trend evaluation
- Quarterly workforce pattern comparison

---

## 📈 Visualizations

### 1️⃣ Quarterly Employment Distribution

<img width="1402" height="655" alt="Screenshot 2026-09-03 011228" src="https://github.com/user-attachments/assets/0ddf8561-1b64-4915-83df-b93ef4c7f721" />

```markdown
![Quarter-wise Employment Distribution](images/quarterwise_employment_distribution.png)
```

### 🔍 Key Insights

- Employment levels remained relatively stable across all four quarters.
- Quarter 4 recorded a slightly higher employment level compared to the other quarters.
- Quarterly differences were relatively small, indicating consistent workforce demand throughout the year.
- No quarter experienced a significant decline in employment.

---

### 2️⃣ Actual vs Seasonally Adjusted vs Trend employment across industries

<img width="1553" height="724" alt="Screenshot 2026-09-03 020121" src="https://github.com/user-attachments/assets/a1bb0850-5c89-4b2d-b910-8e2b5b1d4d96" />

```markdown
![Adjustment Type Comparison](images/adjustment_type_comparison.png)
```

### 🔍 Key Insights

- The **Actual** series captures observed employment values, including seasonal fluctuations.
- The **Seasonally Adjusted** series smooths recurring seasonal effects, making underlying employment changes easier to interpret.
- The **Trend** series highlights the long-term direction of employment growth by removing short-term fluctuations.
- All three series indicate an overall increase in employment over the study period.

---

## 💡 Business Insights

- Business employment remained relatively stable across all quarters, demonstrating a resilient labour market.
- Seasonal fluctuations were present but did not significantly affect long-term employment growth.
- Trend analysis confirms sustained workforce expansion across the study period.
- Comparing Actual, Seasonally Adjusted, and Trend data provides a clearer understanding of short-term fluctuations and long-term employment patterns.

---

## ✅ Recommendation

- Continue monitoring quarterly employment trends to identify emerging seasonal changes.
- Use Seasonally Adjusted and Trend data for strategic workforce planning and long-term decision-making.
- Businesses should combine short-term employment monitoring with long-term trend analysis when forecasting workforce requirements.
- Future analysis can investigate seasonal employment patterns within individual industries to identify sector-specific workforce dynamics.

---

---

# 💡 Overall Findings

The analysis of the **Business Employment Indicators** dataset provided valuable insights into employment trends across industries in New Zealand from **2011 to 2025**.

### Key Findings

- Business employment demonstrated an overall upward trend throughout the study period.
- Service-oriented industries such as **Health Care and Social Assistance**, **Retail Trade**, and **Construction** accounted for a significant share of total employment.
- Employment growth varied across industries, with some sectors experiencing rapid expansion while others maintained relatively stable workforce levels.
- Quarterly employment patterns showed only minor seasonal fluctuations, indicating consistent workforce demand throughout the year.
- Statistical analysis confirmed that the dataset is highly positively skewed due to a small number of industries with exceptionally high employment values.
- Outlier analysis revealed genuine business observations rather than data quality issues, so these records were retained for accurate analysis.

---

# 📌 Conclusion

This project successfully analyzed quarterly business employment trends using Python by applying data cleaning, feature engineering, statistical analysis, and exploratory data analysis techniques.

The findings revealed long-term employment growth across multiple industries, highlighted differences in workforce participation, and demonstrated that seasonal variations had a relatively limited impact on overall employment trends. The analysis also showed that employment distribution varies considerably across industries, reflecting differences in economic activity and workforce demand.

Overall, the project demonstrates how data analytics can transform raw employment data into meaningful business insights that support workforce planning, industry analysis, and evidence-based decision-making.

---

# ✅ Recommendations

Based on the analysis, the following recommendations are proposed:

- Monitor employment trends regularly to support strategic workforce planning.
- Focus workforce development initiatives on industries demonstrating strong long-term growth.
- Encourage reskilling and upskilling programs for industries experiencing slower employment growth.
- Use Seasonally Adjusted and Trend data for long-term planning rather than relying solely on Actual values.
- Extend future analysis by incorporating additional economic indicators such as GDP, inflation, or unemployment rates to gain deeper insights into employment dynamics.

---

# 🚀 Future Enhancements

This project can be further enhanced by:

- Developing an interactive dashboard using **Power BI** or **Tableau**.
- Building predictive models to forecast future employment trends using Machine Learning.
- Expanding the analysis to include regional and demographic employment patterns.
- Integrating additional economic datasets for more comprehensive workforce analysis.
- Automating the data analysis workflow using scheduled data pipelines.

---

# 📂 Project Structure

```text
Business-Employment-Trend-Analysis/
│
├── 📁 data/
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── 📁 notebooks/
│   └── Business_Employment_Trend_Analysis.ipynb
│
├── 📁 images/
│   └── charts and visualizations
│
├── 📁 report/
│   └── Project_Report.pdf
│
├── README.md
└── requirements.txt
```

---

# 👩‍💻 Author

**Suganya K**

Aspiring Data Analyst passionate about transforming data into actionable business insights using Python, SQL, Excel, and Power BI.

- 💼 LinkedIn: (https://www.linkedin.com/in/suganya-karuppusamy/)
- 💻 GitHub: https://github.com/suganyakaruppusamy-tech/business-employment-trends-analysis/edit/main/README.md

---
