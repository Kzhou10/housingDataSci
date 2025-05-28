# 🏙️ Rental Housing Price Analysis: Vancouver vs. Calgary

## 📌 Project Overview

This project investigates rental housing prices in two major Canadian cities—**Vancouver** and **Calgary**. The goal is to explore market differences and identify key factors that contribute to rental price variations. Vancouver is known for its high cost of living and limited housing supply, while Calgary offers more affordable options driven by different economic factors. Understanding the dynamics between these cities can help inform public policy, urban planning, and investment decisions.

---

## 🎯 Objectives

- Determine whether rental prices differ significantly between Vancouver and Calgary.
- Identify key predictors of rental prices (e.g., number of beds, square footage, furnishing).
- Compare the influence of these predictors between the two cities.
- Visualize and interpret market trends and patterns in rental data.

---

## 📂 Project Structure


# 🏙️ Rental Housing Price Analysis: Vancouver vs. Calgary

## 📌 Project Overview

This project investigates rental housing prices in two major Canadian cities—**Vancouver** and **Calgary**. The goal is to explore market differences and identify key factors that contribute to rental price variations. Vancouver is known for its high cost of living and limited housing supply, while Calgary offers more affordable options driven by different economic factors. Understanding the dynamics between these cities can help inform public policy, urban planning, and investment decisions.

---

## 🎯 Objectives

- Determine whether rental prices differ significantly between Vancouver and Calgary.
- Identify key predictors of rental prices (e.g., number of beds, square footage, furnishing).
- Compare the influence of these predictors between the two cities.
- Visualize and interpret market trends and patterns in rental data.

---

## 📂 Project Structure

rental-price-analysis/
├── data/
│ └── rent_data.csv # Original dataset from RentFaster or Kaggle
├── scripts/
│ └── analysis.R # R script for cleaning, EDA, modeling, and visualization
├── output/
│ ├── summary_statistics.csv # Summary stats by city
│ ├── visualizations/ # Plots (boxplots, histograms, etc.)
├── README.md # Project overview and instructions
└── report.pdf # Final project report with interpretation of results

markdown
Copy
Edit

---

## 🧪 Methodology

1. **Data Cleaning & Preprocessing**
   - Filter for listings in Vancouver and Calgary.
   - Remove irrelevant or inconsistent entries.
   - Convert categorical variables (e.g., furnishing, smoking) into usable formats.
   - Drop variables like `availability_date` due to low relevance and inconsistent formatting.

2. **Descriptive Analysis**
   - Compare price distributions using summary statistics and boxplots.
   - Explore relationships among features (beds, baths, square footage, etc.).
   - Compute correlation matrix for numerical variables.

3. **Inferential Statistics**
   - Perform two-sample t-tests to assess price differences.
   - Run chi-square tests for associations with categorical features.

4. **Modeling**
   - Fit multiple linear regression models for each city.
   - Use model diagnostics (R², RMSE, VIF) to evaluate fit and check for multicollinearity.
   - Consider Ridge/LASSO if needed.

5. **Interpretation**
   - Discuss which features most impact price.
   - Analyze whether those impacts vary by city.
   - Reflect on implications for renters, landlords, and policymakers.

---

## 📈 Sample Visuals

- Boxplots comparing rental prices between cities
- Histograms showing price distributions
- Correlation heatmaps of numerical features

---

## 📦 Dependencies

This project uses the following R packages:

```r
install.packages(c(
  "dplyr",
  "ggplot2",
  "summarytools",
  "corrplot",
  "car",
  "leaps"
))
