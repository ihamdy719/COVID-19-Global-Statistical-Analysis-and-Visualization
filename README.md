# COVID-19 Global Data Analysis & Statistical Modeling

An end-to-end data analysis project examining global COVID-19 trends using Python and Power BI.  
This project demonstrates the complete data science workflow including data wrangling, exploratory data analysis (EDA), feature engineering, statistical modeling, hypothesis testing, and dimensionality reduction (PCA).

---

## 📌 Project Objective

The objective of this project is to analyze real-world COVID-19 data to:

- Identify infection and mortality trends
- Analyze recovery and fatality rates
- Examine vaccination and testing impact
- Study government stringency effects
- Apply statistical validation techniques
- Reveal latent country-level patterns using PCA

This project demonstrates mastery of the full data analysis lifecycle.

---

## 📂 Repository Structure

```

COVID-19-Global-Data-Analysis/
│
├── Datasets/
│   ├── owid-covid-data.csv              # Raw dataset (Our World in Data)
│   └──  cleaned_covid_data.csv           # Processed dataset
│
│
├── Docs/
│   ├── Data Analysis Report.pdf         # Final written report
│   └── Final_Project_Ideas_Detailed.pdf # Initial project proposal
│
├── PowerBI/
│   ├── covid_19.pbix                    # Interactive dashboard file
│   └── PowerBI_Photo/
│       ├── Overview.png
│       ├── Country_Deep_Dive.png
│       ├── Relationships.png
│       └── Ranking_Table.png
│
├── Data Analysis Project.ipynb      # Complete analysis notebook
|
└── README.md

```

---

## 🛠 Tools & Technologies

### Python Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scikit-learn (StandardScaler, Lasso, RFE, PCA)

### Visualization
- Power BI

### Dataset Source
- Our World in Data (OWID) COVID-19 Dataset

---

## 🔄 Project Workflow

1. Raw Data Inspection  
2. Exploratory Data Analysis (Before Cleaning)  
3. Data Cleaning & Preprocessing  
4. Outlier Handling (IQR Clipping)  
5. Feature Engineering  
6. Feature Selection (Lasso, RFE)  
7. Probability Distribution Fitting  
8. Hypothesis Testing  
9. Principal Component Analysis (PCA)  
10. Dashboard Visualization (Power BI)

---

## 🧹 Data Wrangling

- Converted date column to datetime format
- Removed aggregated records (World, continents, income groups)
- Handled missing values:
  - Numerical → Median
  - Categorical → Mode
- Applied IQR-based clipping for daily and rate-based variables
- Preserved cumulative totals to maintain time-series integrity

---

## 📊 Exploratory Data Analysis (EDA)

- Univariate and multivariate analysis
- Distribution visualization (Histograms)
- Correlation analysis
- Skewness detection
- Heavy-tailed behavior identification
- Missing data assessment

---

## ⚙ Feature Engineering

New features created:

- Case Fatality Rate (CFR)
- Growth Rate
- Active Case Proxies

Feature selection techniques:
- Lasso Regression
- Recursive Feature Elimination (RFE)

---

## 📈 Statistical Analysis

### Correlation Analysis
Used latest country-level observations to avoid time-series duplication bias.

### Probability Distribution Fitting
Fitted Normal and Lognormal distributions to daily case counts.

### Hypothesis Testing
Independent two-sample t-test applied to evaluate changes in government stringency over time.

---

## 📉 Dimensionality Reduction (PCA)

- Standardized features using StandardScaler
- Reduced dimensions to 2 principal components
- Visualized country clusters
- Interpreted explained variance ratio
- Identified latent pandemic patterns

---

## 📊 Power BI Dashboard

The interactive dashboard includes:

1. Global Overview
2. Country Deep Dive
3. Testing & Positivity Analysis
4. Ranking & Comparison Table

Features:
- Date filtering
- Country filtering
- Continent filtering
- Interactive comparisons

---

## 🔎 Key Insights

- COVID-19 indicators exhibit heavy-tailed distributions
- Testing intensity significantly affects reported case counts
- Policy stringency impact varies across regions
- PCA reveals clusters of countries with similar pandemic dynamics
- Feature selection highlights key predictors of mortality trends

---

## ⚠ Limitations

- Incomplete testing data for some countries
- Reporting inconsistencies across regions
- Aggregated indicators may hide sub-national variation
- Assumptions in statistical tests may not hold for all countries

---

## 👥 Team Members
### Ibrahim Hamdy
### Zeinab Ahmed

---

## 🚀 How to Run the Project

1. Clone the repository
2. Install required Python libraries
3. Open `Data Analysis Project.ipynb`
4. Run all cells sequentially
5. Open `covid_19.pbix` using Power BI Desktop for dashboard exploration

---

## 📚 References

- Our World in Data – COVID-19 Dataset
- James et al., *An Introduction to Statistical Learning*
- Montgomery & Runger, *Applied Statistics and Probability for Engineers*

---

## 🎯 Learning Outcomes

This project demonstrates the ability to:

- Clean and preprocess large real-world datasets
- Perform EDA using professional visualization techniques
- Engineer meaningful features
- Apply statistical validation and probability modeling
- Reduce dimensionality using PCA
- Present insights through interactive dashboards
- Collaborate effectively in a structured team environment

---
