# 🏡 Ames Housing Data Cleaning Project

This project focuses on cleaning and preparing the **Ames Housing Dataset**, 
which provides rich information on residential property sales in Ames, 
Iowa, USA, between 2006 and 2010. The dataset contains 80+ features, including structural attributes,
quality ratings, and sale prices. The objective is to clean and preprocess the data so it's ready for deeper analysis and machine learning applications.

---

## 🎯 Objectives

- 📥 Load and inspect the dataset (`.tsv` format)
- 🔍 Identify and handle missing, inconsistent, and duplicate data
- 🧼 Apply appropriate cleaning strategies (imputation, removal, type conversion)
- 📊 Explore feature relationships and correlation with `SalePrice`
- 🔄 Normalise and transform skewed variables
- 🧮 Encode categorical variables
- 💾 Export a clean dataset suitable for modelling

---

## 🧰 Tools & Technologies Used

| Tool / Library     | Purpose                               |
|--------------------|----------------------------------------|
| **Python**         | Programming language                   |
| **Pandas**         | Data manipulation and preprocessing    |
| **NumPy**          | Numerical operations                   |
| **Matplotlib**     | Data visualization                     |
| **Seaborn**        | Statistical data visualization         |
| **Scikit-learn**   | Feature scaling and preprocessing      |
| **SciPy**          | Statistical transformations            |
| **Jupyter Notebook** | Interactive environment for analysis |

---

## 📁 Dataset

- **File name:** `Ames_Housing_Data1.tsv`
- **Source:** Ames Assessor's Office (hosted on IBM Cloud)
- **Format:** Tab-separated values
- **Rows:** 2,930 properties
- **Columns:** 80+ features related to home sales

---

## 🔧 Cleaning & Preprocessing Workflow

### 1. **Load Dataset**
- Read `.tsv` file using `pandas.read_csv()` with tab separator.
- Checked for basic structure, column types, and summary statistics.

### 2. **Handle Missing Values**
- Identified missing values using `.isnull().sum()`
- Applied various strategies:
  - Numerical features: imputed with median or mean
  - Categorical features: filled with mode or "None"
  - Dropped features with too many missing values (e.g., > 80%)

### 3. **Remove Duplicates and Inconsistencies**
- Checked for and removed duplicate rows.
- Ensured correct data types across all columns (e.g., dates, integers, categories).

### 4. **Explore Target Variable (`SalePrice`)**
- Assessed distribution of `SalePrice`
- Applied log transformation to reduce skewness

### 5. **Correlation Analysis**
- Used Pearson correlation to identify features most strongly related to `SalePrice`
- Visualized correlation matrix using Seaborn heatmaps

### 6. **Feature Engineering**
- Transformed skewed numeric variables using log1p
- One-hot encoded categorical variables as needed

### 7. **Feature Scaling**
- Applied `StandardScaler` and `MinMaxScaler` to normalize numeric variables

### 8. **Export Cleaned Dataset**
- Saved final dataset to `cleaned_data.csv` for future analysis or modeling
---
👩‍💻 Author
Orjiude Esther Obianuju
🎓 Data Analyst | Skilled in Python, Power BI, SQL & Excel
📧 Email: orjiudeesther@gmail.com
🔗 LinkedIn: www.linkedin.com/in/orjiude-esther
