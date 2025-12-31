# 📊 Social Media Usage and Sleep Duration Analysis

## 📌 Project Overview
This project explores the relationship between **digital behavior**, **screen time**, and **sleep duration** using real-world observational data. Rather than attempting to prove causality, the analysis focuses on identifying meaningful patterns that emerge from everyday screen usage and how these patterns relate to sleep.

The project examines whether higher social media usage and prolonged screen exposure are associated with reduced sleep duration, using statistical testing and regression modeling.

A storytelling-style public report based on this analysis is available on Medium.

📖 *How Our Screens Steal Our Sleep*  
https://medium.com/@okt4vianus/how-our-screens-steal-our-sleep-388417e1a26d

---

## 📂 Dataset Information

**Source:**  
[Kaggle – Social Media & Mental Health Indicators Dataset](https://www.kaggle.com/datasets/sonalshinde123/social-media-mental-health-indicators-dataset)

**Description:**  
The dataset captures individual-level digital behavior and lifestyle factors, including screen usage, online interaction quality, demographic information, and sleep duration. It reflects everyday digital habits rather than controlled experimental conditions.

**Variables (15 total):**

| Column Name | Description |
|------------|-------------|
| person_name | Identifier of the individual |
| age | Age in years |
| date | Date of observation |
| gender | Gender (Male, Female, Other) |
| platform | Primary social media platform |
| daily_screen_time_min | Total daily screen time (minutes) |
| social_media_time_min | Time spent on social media per day (minutes) |
| negative_interactions_count | Number of negative online interactions |
| positive_interactions_count | Number of positive online interactions |
| sleep_hours | Total sleep duration per day (hours) |
| physical_activity_min | Daily physical activity (minutes) |
| anxiety_level | Anxiety level score |
| stress_level | Stress level score |
| mood_level | Mood level score |
| mental_state | Overall mental condition |

**Variable Types:**
- Numerical variables: **10**
- Categorical variables: **5**

---

## 🎯 Research Questions
1. Is there a statistically significant difference in sleep duration between users with low and high social media usage?
2. How does social media usage relate to sleep duration when treated as a continuous behavior?
3. When controlling for total screen time and demographics, which factors most strongly predict sleep duration?

---

## 🛠️ Tools & Libraries
- **Python**
- **Pandas & NumPy** – Data manipulation
- **Matplotlib & Seaborn** – Visualization
- **SciPy** – Statistical testing
- **Statsmodels** – Regression analysis

---

## 📁 Project Structure

    social-media-sleep-analysis/
    ├── presentation/                      # Final presentation slides
    ├── video_presentation/                # Recorded presentation
    ├── social_media_sleep_analysis.ipynb  # Main analysis notebook
    ├── social_media_mental_health.csv     # Dataset
    └── README.md                          # Project documentation

---

## 📈 Analysis Workflow

### 1. Data Overview
Initial exploration was conducted to understand dataset structure, variable types, and summary statistics. This step established a clear view of numerical and categorical variables before further analysis.

---

### 2. Data Quality Checks
To ensure analytical reliability, the following checks were performed:
- **Missing values:** None detected
- **Duplicate rows:** None detected
- **Outliers:** Identified using IQR and Z-score methods  

Outliers observed in age and screen-related variables represent realistic behavioral variation and were retained.

---

### 3. Exploratory Data Analysis (EDA)
Exploratory analysis included:
- Histograms and boxplots to inspect distributions
- Scatter plots to visualize relationships between screen behavior and sleep duration
- Correlation analysis to identify linear associations

EDA revealed a consistent negative relationship between screen exposure and sleep duration.

---

### 4. Statistical Testing
An **independent samples t-test** was used to compare sleep duration between low and high social media usage groups.

- Groups defined by median social media usage
- Outcome variable: `sleep_hours`
- Confidence level: 95%

The results show a statistically significant difference in average sleep duration, with higher social media users sleeping less on average.

---

### 5. Regression Analysis
Multiple regression models were built to quantify relationships and control for confounding variables:

- **Simple linear regression:**  
  Social media time vs. sleep duration
- **Multiple linear regression:**  
  Includes total screen time, interaction counts, and age
- **Interaction model (optional):**  
  Tested whether age modifies the effect of social media usage

Model evaluation included coefficient interpretation, adjusted R², and residual diagnostics.

---

## 📌 Key Findings
- Higher social media usage is associated with reduced sleep duration
- Total daily screen time has a stronger relationship with sleep than any single platform
- Online interaction quality plays a smaller role compared to overall screen exposure
- Sleep loss appears linked to cumulative digital behavior rather than isolated habits

---

## ⚠️ Limitations
- Observational data does not establish causality
- Not all lifestyle and mental health variables were included in regression models
- Potential unobserved confounders may influence results
- The dataset reflects a snapshot rather than long-term behavior

---

## 🌱 Future Work
- Incorporate additional mental health and physical activity variables
- Explore longitudinal or experimental study designs
- Test screen-time reduction or digital curfew interventions
- Conduct platform-specific behavioral analysis

---

## 📚 References
- Stine, R., & Foster, D. (2013). *Statistics for Business: Decision Making and Analysis*. Addison-Wesley.
- Gelman, A., Hill, J., & Vehtari, A. (2020). *Regression and Other Stories*.
