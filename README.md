# 📊 Social Media Usage and Sleep Duration Analysis

## 📌 Project Overview
This project analyzes the relationship between **social media usage**, **screen time behavior**, and **sleep duration** using statistical analysis and regression modeling. The goal is to understand whether increased digital engagement significantly affects sleep hours and overall daily behavior patterns.

The analysis follows a structured data analysis workflow, including data cleaning, exploratory data analysis (EDA), hypothesis testing, and regression modeling.

---

## 📂 Dataset Information
**Source:**  
[Kaggle – Social Media & Mental Health Indicators Dataset](https://www.kaggle.com/datasets/sonalshinde123/social-media-mental-health-indicators-dataset)

**Description:**  
The dataset captures individual-level digital behavior and lifestyle factors such as:
- Daily screen time
- Social media usage duration
- Positive and negative online interactions
- Demographic information
- Sleep duration (hours)

**Variables:**
- Total variables: **10**
- Numerical variables: **6**
- Categorical variables: **4**

---

## 🎯 Research Questions
1. Is there a significant difference in sleep duration between users with low and high social media usage?
2. How strong is the relationship between screen time and sleep hours?
3. Which digital behavior variables most strongly predict sleep duration?

---

## 🛠️ Tools & Libraries
- **Python**
- **Pandas & NumPy** – Data manipulation
- **Matplotlib & Seaborn** – Visualization
- **SciPy** – Statistical testing
- **Statsmodels** – Regression analysis

---

## 🔍 Project Structure (temporary)
social-media-sleep-analysis/
│
├── social_media_sleep_analysis.ipynb # Main analysis notebook
├── social_media_mental_health.csv # Dataset
├── README.md # Project documentation


---

## 📈 Analysis Workflow
### 1. Data Overview
- Dataset shape, data types, and summary statistics
- Identification of numerical and categorical variables

### 2. Data Quality Checks
- Missing value detection
- Duplicate row detection
- Outlier identification using the IQR method

### 3. Exploratory Data Analysis (EDA)
- Histograms and boxplots
- Scatter plots
- Correlation matrix

### 4. Statistical Testing
- Independent t-test
- Comparison of mean sleep hours between low and high social media usage groups
- 95% confidence intervals and p-values

### 5. Regression Analysis
- Simple and multiple linear regression models
- Interpretation of coefficients, p-values, and standard errors
- Model fit evaluation using Adjusted R²
- Residual diagnostics

---

## 📌 Key Findings
- Users with **higher social media usage tend to sleep fewer hours on average**
- Screen time shows a **statistically significant negative relationship** with sleep duration
- Regression models explain a substantial portion of variance in sleep hours
- Model assumptions are reasonably satisfied based on residual analysis

---

## 📚 References
- Kaggle Dataset: Social Media & Mental Health Indicators
- Udacity Data Analysis Nanodegree Project Structure  
  https://github.com/patiegm/Udacity_Data_Analysis_Nanodegree

---
