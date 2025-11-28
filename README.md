# Titanic Dataset – Handling Missing Values (Imputation)

## 📘 Project Overview
This assignment focuses on identifying and resolving missing data in the Titanic dataset.  
Imputation techniques were used to replace NaN values with logical and meaningful estimates.

---

## 🔍 Tasks Completed

### 1️⃣ Dataset Loading
- Imported the Titanic CSV file from an online GitHub source.
- Loaded the dataset into a Pandas DataFrame for processing.

### 2️⃣ Missing Value Analysis
- Used `isnull().sum()` to check how many values were missing in each column.
- Identified that the **Age** column had the highest number of missing entries.

### 3️⃣ Age Imputation Using Grouped Medians
The Age column was filled using two strategies:

#### ✔ Imputation Based on Sex  
- Calculated median age for:
  - Male passengers  
  - Female passengers  
- Replaced missing Age values using the median of the passenger’s Sex group.

#### ✔ Imputation Based on Passenger Title  
- Extracted titles such as *Mr, Miss, Mrs, Master* from the `Name` column.
- Combined rare titles like *Capt, Col, Rev, Countess* into a “Rare” category.
- Computed median Ages for each Title category.
- Used these values to impute any Age data still missing.

---

## 🧠 Why Imputation Matters
- Removes gaps in data that may cause errors in analysis.
- Makes the dataset more complete and consistent.
- Using grouping (Sex + Title) results in **more realistic** and **context-based** imputation.

---

## 📂 Files Included
- **titanic_imputation.ipynb** – Jupyter Notebook with all code and outputs  
- **README.md** – Explanation of the assignment steps

---

## 📊 Dataset Source
- Titanic dataset taken from a publicly available GitHub repository.

---

## 🛠 Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Jupyter Notebook  

---


