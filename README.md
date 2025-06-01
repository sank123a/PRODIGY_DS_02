# PRODIGY_DS_02
Titanic dataset EDA project
Task 02 -Perform data cleaning and exploratory data analysis (EDA) on a dataset of your choice, such as the Titanic dataset from Kaggle. Explore the relationships between variables and identify patterns and trends in the data

# 🛳️ Titanic Dataset – Exploratory Data Analysis (EDA)

This project performs data cleaning and exploratory data analysis (EDA) on the famous Titanic dataset from Kaggle. The goal is to explore relationships between variables and identify patterns that influenced survival.

---

## 📁 Dataset

- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- File Used: `train.csv`
- Description: Contains information on the passengers aboard the Titanic, including demographics, ticket fare, class, and survival outcome.

---

## 🧪 Tools Used

- **Python**
- **Pandas** for data manipulation
- **Matplotlib** and **Seaborn** for data visualization
- **Jupyter Notebook** for development

---

## 🔄 Process Overview

### 1. **Data Loading**
- Imported `train.csv` using Pandas.

### 2. **Initial Inspection**
- Checked dataset structure using `.info()`, `.head()`, and `.describe()`.
- Identified missing values in `Age`, `Cabin`, and `Embarked`.

### 3. **Data Cleaning**
- Imputed missing `Age` values with median.
- Filled missing `Embarked` values with mode.
- Dropped `Cabin` due to excessive missing values.
- Dropped non-informative columns: `PassengerId`, `Name`, and `Ticket`.
- Converted categorical variables to `category` dtype for easier analysis.

### 4. **Exploratory Data Analysis (EDA)**
- **Univariate analysis** on `Survived`, `Sex`, `Age`, `Pclass`, `Embarked`.
- **Bivariate analysis** using plots like:
  - Bar charts (`Survived` vs `Sex`, `Pclass`, `Embarked`)
  - Histograms (age distribution)
  - Boxplots (`Age` vs `Survived`)
  - Correlation heatmaps for numerical features

---

## 📊 Key Insights

1. **Gender and Survival**:
   - Females had a much higher survival rate than males.

2. **Passenger Class**:
   - Passengers in 1st class were more likely to survive compared to those in 2nd or 3rd class.

3. **Age Distribution**:
   - Younger passengers had slightly better survival odds; children were prioritized.

4. **Port of Embarkation**:
   - Most passengers boarded from port 'S'; survival rates varied slightly by port.

5. **Correlation**:
   - Survival was positively correlated with `Fare` and negatively correlated with `Pclass`.

---

## 📁 Folder Structure

```

Titanic-EDA/
│
├── train.csv
├── PRODIGY_DS_02.ipynb       # Jupyter Notebook with full code
├── README.md               # Project summary and insights

```

---

## ✅ Future Work

- Perform feature engineering (e.g., extract titles from names).
- Train machine learning models to predict survival.
- Deploy using a simple web interface or dashboard.

---

## 🙌 Acknowledgements

Thanks to [Kaggle](https://www.kaggle.com/c/titanic/data) for providing the Titanic dataset for public use.

