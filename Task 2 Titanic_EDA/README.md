

---

# Titanic Dataset - Exploratory Data Analysis (EDA)

## Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Titanic dataset using Python libraries **Pandas, NumPy, Matplotlib, and Seaborn**.
The goal is to analyze patterns of survival based on passenger demographics, ticket class, and other features.

---

## Dataset

* Source: Seaborn library (`sns.load_dataset('titanic')`)
* Key Columns:

  * `survived`: 0 = Died, 1 = Survived
  * `pclass`: Passenger Class (1 = 1st, 2 = 2nd, 3 = 3rd)
  * `sex`: Gender of passenger
  * `age`: Age of passenger
  * `sibsp`: Number of siblings/spouses aboard
  * `parch`: Number of parents/children aboard
  * `fare`: Ticket fare
  * `embarked`: Port of Embarkation
  * `embark_town`: Name of embark town

---

## Steps Performed

### 1. Data Loading

* Loaded Titanic dataset using Seaborn.
* Imported necessary libraries: `pandas`, `numpy`, `matplotlib.pyplot`, `seaborn`.

### 2. Handling Missing Values

* Dropped missing values for `embarked` and `embark_town`.
* Filled missing `age` values with the median age.

### 3. Feature Engineering

* `family_size` = `sibsp` + `parch` + 1
* `alone` = 1 if `family_size` = 1 else 0

### 4. Visualizations

#### Survival Analysis

* Count plot for overall survival.
* Bar plot for survival rate by gender.
* Count plots for survival by passenger class and embark town.

#### Age and Fare

* Histogram and boxplot for age distribution and survival by age.
* Histogram and boxplot for fare distribution and survival by fare.

#### Family Features

* Count plot for survival of passengers traveling alone vs with family.

#### Correlation and Relationships

* Heatmap of numeric feature correlations.
* Pairplot of key features (`age`, `fare`, `pclass`, `survived`) colored by survival.

---

## Key Insights

* **Gender:** Females had a higher survival rate than males.
* **Class:** 1st class passengers had a higher survival rate than 2nd and 3rd class.
* **Embark Town:** Passengers from certain embarkation towns had higher survival rates.
* **Family/Alone:** Passengers traveling with family had different survival patterns compared to those alone.
* **Age & Fare:** Younger passengers and higher fare payers tended to have higher survival rates.

---

## Libraries Used

* pandas
* numpy
* matplotlib
* seaborn

---

## Output

All plots were visualized in the notebook and can be optionally saved as images for reporting purposes.

---

## Author

**Salman Adam**

* LinkedIn: [www.linkedin.com/in/salmanadam](https://www.linkedin.com/in/salmanadam)

--