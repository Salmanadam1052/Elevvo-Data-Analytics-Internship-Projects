

---

# Kaggle Data Science Survey Analysis (2017–2021)

## Project Overview

This project analyzes the **Kaggle Data Science Survey (2017–2021)** to extract insights about respondents’ behavior, preferences, and trends. The dataset contains real-world survey responses with missing values, duplicates, and inconsistent formatting. This project demonstrates data cleaning, transformation, and visualization techniques in Python.

---

## Dataset

* **Source:** [Kaggle Data Science Survey](https://www.kaggle.com/c/kaggle-survey-2021)
* **Format:** CSV
* **Size:** \~20–50 MB (depending on the year)
* **Features:** Respondent demographics, job-related information, salary, tools/languages used, and experience.

---

## Project Steps

### 1. Data Loading

* Load the CSV dataset using **pandas**.
* Focus on the **latest year (2021)** for detailed analysis.

```python
import pandas as pd
df = pd.read_csv('kaggle_survey_2017_2021.csv', low_memory=False)
```

---

### 2. Data Cleaning

* Handle **missing values** and **duplicates**.
* Remove invalid or inconsistent responses.
* Standardize categorical variables (e.g., gender, salary, experience).

```python
df.drop_duplicates(inplace=True)
df.dropna(thresh=5, inplace=True)
```

---

### 3. Data Transformation

* Apply **mapping or label encoding** for categorical variables.
* Group salary ranges into categories.
* Extract relevant features for visualization.

```python
df['Salary_Group'] = df['Q25'].apply(simplify_salary)
```

---

### 4. Data Visualization

* Use **matplotlib** and **seaborn** for plots.
* Visualizations include:

  * Overall salary distribution
  * Salary by gender
  * Salary by experience level
  * Salary by country
  * Salary by job title

All charts are automatically saved as **PNG files** in the `graphs` folder.

```python
plt.savefig('graphs/salary_by_gender.png')
```

---

### 5. Insights

* Respondent salary varies significantly by **experience, country, and job title**.
* Gender differences in salary can be observed.
* Salary distribution is skewed toward certain ranges.

---

## Requirements

* Python 3.x
* Libraries:

  * pandas
  * numpy
  * matplotlib
  * seaborn
  * os

Install missing libraries with:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## How to Run

1. Place the dataset CSV in the project folder.
2. Run the Python script:

```bash
python survey_analysis.py
```

3. Check the `graphs` folder for saved PNG visualizations.

---

## Folder Structure

```
project/
│
├── survey_analysis.py   # Main analysis script
├── kaggle_survey_2017_2021.csv  # Dataset
└── graphs/             # Saved plots (PNG)
```

---

## Author

**Salman Adam**

* LinkedIn: [linkedin.com/in/salmanadam-](https://www.linkedin.com/in/salmanadam-)

---


