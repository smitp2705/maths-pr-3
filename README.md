# Maths Project 3 – Inferential Statistics on Health Data

A Python-based statistics project that applies inferential statistics concepts to a real health dataset.

---

##  Project Files

| File | Description |
|------|-------------|
| `maths_3_project.ipynb` | Main Jupyter Notebook with theory and code |
| `health_dataset_changed.csv` | Health dataset used for analysis (1500 records) |

---

##  Dataset Overview

**File:** `health_dataset_changed.csv`  
**Rows:** 1500 patients  
**Columns:** 15

| Column | Type | Description |
|--------|------|-------------|
| `record_id` | Text | Unique ID for each patient |
| `age_group` | Category | Age group (18-25, 26-35, 36-45, 46-60, 60+) |
| `age` | Number | Patient age |
| `weight` | Number | Weight in kg |
| `gender` | Category | Male / Female |
| `region` | Category | Geographic region (North, South, East, West) |
| `smoking_status` | Category | Smoker / Non-Smoker / Former Smoker |
| `exercise_frequency` | Category | Daily / Weekly / Rarely / Never |
| `bmi` | Decimal | Body Mass Index |
| `blood_pressure` | Decimal | Blood pressure reading |
| `diabetes` | True/False | Whether patient has diabetes |
| `hypertension` | True/False | Whether patient has hypertension |
| `cholesterol_level` | Decimal | Cholesterol level |
| `glucose_level` | Decimal | Blood glucose level |
| `visit_date` | Date | Date of hospital visit |

---

##  What the Notebook Covers

### Part A – Theory
Short answers covering key statistics concepts:
- Inferential Statistics
- Hypothesis Testing (Null & Alternative Hypothesis, p-value, significance level)
- Confidence Interval & Critical Value
- Type I and Type II Errors
- z-test, t-test, Chi-Square, ANOVA
- Covariance and Correlation

### Part B – Practical Analysis (Python Code)

| Analysis | What it does |
|----------|-------------|
| **Confidence Interval** | Calculates 95% CI for age, weight, BMI, blood pressure, cholesterol, glucose |
| **Critical Value** | Finds critical value at 5% significance level |
| **t-test** | Compares BMI of Smokers vs Non-Smokers |
| **Chi-Square Test** | Checks if Smoking Status is related to Diabetes |
| **ANOVA Test** | Compares BMI across all 5 age groups |
| **Covariance & Correlation** | Measures relationship between numerical variables |

---

##  Libraries Used

```
pandas
numpy
scipy
statsmodels
seaborn
matplotlib
```

Install all at once:
```bash
pip install pandas numpy scipy statsmodels seaborn matplotlib
```

---

##  How to Run

1. Download both files into the same folder
2. Open `maths_3_project.ipynb` in Jupyter Notebook or VS Code
3. Update the CSV path in the notebook:
   ```python
   df = pd.read_csv("health_dataset_changed.csv")
   ```
4. Run all cells from top to bottom

---

## Key Concepts (Quick Reference)

- **p-value < 0.05** → Reject the Null Hypothesis (result is significant)
- **p-value ≥ 0.05** → Accept the Null Hypothesis (result is not significant)
- **Confidence Interval** → Range where the true value likely falls (95% means 95% of the time)
- **t-test** → Used when comparing two groups
- **ANOVA** → Used when comparing three or more groups
- **Chi-Square** → Used for categorical data relationships
