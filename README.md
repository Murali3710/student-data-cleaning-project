# 📊 Student Data Cleaning Project

## 📌 Project Overview

This project focuses on cleaning and preprocessing a raw student dataset using Python. The goal is to handle missing values, standardize data, detect and treat outliers, and prepare the dataset for further analysis.

---

## 📂 Dataset Description

The dataset contains information about students such as:

- Student ID
- Name
- Age
- Gender
- Marks
- Department
- Join Date

---

## ⚙️ Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

--

## 🧹 Data Cleaning Steps Performed

### 1. Data Inspection
- Checked dataset structure using `info()` and `describe()`

### 2. Data Standardization
- Standardized values in:
  - **Gender** column (Male/Female consistency)
  - **Department** column (CSE, IT, ECE format)

### 3. Checking Duplicate Values
- Identified duplicate records using `duplicated()`
- Analyzed duplicate entries to verify whether they were exact duplicates

### 4. Handling Duplicate Values
- Removed duplicate records using `drop_duplicates()`
- Retained only unique observations in the dataset

### 5. Handling Missing Values
- Filled missing values in numerical columns using **median**
- Handled missing categorical values using **mode**
  
### 6. Date Conversion
- Converted `Join_Date` into proper datetime format
- Handled invalid date values

### 7. Outlier Detection
- Used box plots and IQR method
- Identified outliers in:
  - Age
  - Marks

### 8. Outlier Treatment
- Removed unrealistic values (e.g., Age = 200, 300, Marks = 300)
- Retained realistic values like Age = 18, Marks = 60

### 9. Final Dataset Check
- Verified cleaned dataset using `info()`, `describe()`, and null checks

---

## 📊 Final Outcome

- ✅ Clean and structured dataset
- ✅ No missing values
- ✅ No duplicates
- ✅ Outliers handled properly
- ✅ Data ready for analysis or visualization

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `student_dataset_dirty.csv` | Raw dataset with missing values, inconsistencies, and outliers |
| `cleaned_student_data.csv` | Final cleaned and preprocessed dataset |
| `student_data_cleaning.ipynb` | Jupyter Notebook with all cleaning steps |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Murali3710/student-data-cleaning.git
   ```

2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Open the notebook:
   ```bash
   jupyter notebook student_data_cleaning.ipynb
   ```

