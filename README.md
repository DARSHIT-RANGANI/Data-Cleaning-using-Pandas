# Employee-Data-Cleaning

# 👥 Employee Data Cleaning

**Transform messy HR data into production-ready analytics** with this complete Pandas notebook. Converts 1,020 records of raw employee data into clean, structured CSV for dashboards, ML models, and databases.

---

## 📋 Problem Solved

**Input:** `Messy_Employee_dataset.csv` - Real-world dirty data with:
* Missing Age & Salary values
* Malformed dates (MMDDYYYY format)
* Combined Department-Region fields
* Text performance scores (Poor/Excellent → 1-5 numeric)
* Negative phone numbers
* Duplicates & inconsistencies

**Output:** `CleanEmployeeDataset.csv` - Perfect analytics-ready data

---

## ✨ What It Does (Step-by-Step)

Messy Data → Missing Value Imputation → Date Parsing →
Text Cleaning → Column Splitting → Numeric Mapping →
Deduplication → Clean CSV Output

---


**Key Cleaning Operations:**
* 🧮 **Age/Salary**: Median imputation (Age: 32, Salary: ~$85K)
* 📅 **Dates**: `pd.to_datetime()` with error handling
* 📍 **DepartmentRegion**: Split by "-" → separate columns
* 🎯 **Performance**: {"Poor":1, "Average":2, "Good":3, "Very Good":4, "Excellent":5}
* ☎️ **Phone**: Convert negatives to positive
* 🗑️ **Duplicates**: Removed automatically

---

## 📊 Results Preview

| **Metric** | **Before** | **After** |
|------------|------------|-----------|
| Total Rows | 1,020 | 1,020 (no data loss) |
| Missing Age | 211 | 0 |
| Missing Salary | 24 | 0 |
| Data Types | Mixed | Consistent |
| Ready for | ❌ | ✅ Dashboards/ML/DB |


---

## 🛠 Tech Stack

| **Component** | **Details** |
|---------------|-------------|
| **Language** | Python 3.x |
| **Core Library** | Pandas |
| **Input File** | `Messy_Employee_dataset.csv` |
| **Output File** | `CleanEmployeeDataset.csv` |
| **Rows Processed** | 1,020 records |

---

### 📁 Repository Structure

├── Cleaning_pandas.ipynb # Main cleaning notebook
├── Messy_Employee_dataset.csv # Input (INCLUDED)
└── CleanEmployeeDataset.csv # Output (auto-generated)

---


### Steps
1. **Download** both files to same folder
2. **Open** `Cleaning_pandas.ipynb` in Jupyter/Colab/VSCode
3. **Run All Cells** → **Done!**
4. Find `CleanEmployeeDataset.csv` ready for use

---


## 👨‍💻 Author

**Darshit Rangani**  
*B.Tech Computer Engineering*  
*CodeInYourSelf*  
