# Air Quality Analysis for Policy Recommendations: Hypothesis Testing

## 📌 Project Overview
This repository contains a data analysis project completed for the environmental think tank **Repair Our Air (ROA)**. The objective is to leverage the Environmental Protection Agency's (EPA) Air Quality Index (AQI) data to guide and prioritize strategic national and regional policy recommendations. 

An AQI value close to 0 signals "little to no" public health concern, while higher values indicate an increased risk to public health. This analysis evaluates three major policy and operational questions using rigorous statistical hypothesis testing.

---

## 📊 Research Questions & Hypotheses

All tests are conducted using a **5% level of significance ($\alpha = 0.05$)**. For two-sample tests, **Welch's t-test** is utilized to account for potentially unequal variances between groups.

### 1. Metropolitan Strategy (California)
* **Objective:** Determine if the mean AQI in Los Angeles County is statistically different from the rest of California to evaluate a metropolitan-focused approach.
* **Null Hypothesis ($H_0$):** There is no difference in the mean AQI between Los Angeles County and the rest of California.
* **Alternative Hypothesis ($H_A$):** There is a difference in the mean AQI between Los Angeles County and the rest of California.
* **Test Type:** Two-sample independent t-test (Two-tailed).

### 2. Regional Office Expansion (New York vs. Ohio)
* **Objective:** Choose between New York and Ohio for a new regional office based on which state has lower AQI levels.
* **Null Hypothesis ($H_0$):** The mean AQI of New York is greater than or equal to that of Ohio.
* **Alternative Hypothesis ($H_A$):** The mean AQI of New York is below that of Ohio.
* **Test Type:** Two-sample independent t-test (One-tailed, `alternative='less'`).

### 3. Policy Impact Assessment (Michigan)
* **Objective:** Determine if Michigan will be affected by a new policy targeting states with a mean AQI of 10 or greater.
* **Null Hypothesis ($H_0$):** The mean AQI of Michigan is less than or equal to 10.
* **Alternative Hypothesis ($H_A$):** The mean AQI of Michigan is greater than 10.
* **Test Type:** One-sample t-test (One-tailed, `alternative='greater'`).

---

## 🛠️ Tech Stack & Libraries
* **Python 3**
* **Pandas:** Data manipulation and subsetting.
* **NumPy:** Numerical operations.
* **SciPy (stats):** Statistical functions and t-test execution.

---
