<div align="center">

# 📊 HR Data Analysis with Python

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-EDA-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Charts-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical-4C72B0?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![HR Analytics](https://img.shields.io/badge/HR-Analytics-ff6b6b?style=for-the-badge)

<br/>

> A complete **Exploratory Data Analysis (EDA)** project on a real-world HR dataset —
> uncovering workforce trends, salary patterns, attrition rates, and performance insights
> through **15 targeted business questions**.

<br/>

| 🔢 Questions | 📦 Libraries | 📈 Visualisations | 🔍 Method |
|:---:|:---:|:---:|:---:|
| **15** | **5+** | **10+** | **EDA** |

</div>

---

## 📁 Project Structure

```
hr-data-analysis-with-python/
│
├── hr-data-analysis-with-python.ipynb   ← Main Jupyter Notebook
├── HR_Data.csv                           ← Source Dataset
├── new_chart.png                         ← Exported chart (Q6)
└── README.md                             ← This file
```

---

## 📌 About the Project

A full **Exploratory Data Analysis (EDA)** pipeline built on `HR_Data.csv` — from raw data cleaning to visual storytelling — answering critical HR business questions using Python.

| | |
|---|---|
| 📊 **Dataset** | `HR_Data.csv` — Employee records with Department, Salary (INR), Status, Experience, Performance Rating, Work Mode, Hire Date, Job Title, Location |
| 🎯 **Objective** | Answer 15 targeted HR business questions to surface actionable workforce insights |
| 🔧 **Approach** | Data Loading → Cleaning → EDA with GroupBy & Aggregations → Visualisation |
| 💡 **Key Techniques** | GroupBy, Correlation Heatmaps, Lambda functions, Attrition Rate, `nlargest()`, Time-series |

---

## 🗂️ Dataset — Column Reference

| Column | Type | Description |
|--------|------|-------------|
| `Employee_ID` | `object` | Unique identifier for each employee |
| `Department` | `object` | Employee's department (Finance, IT, HR, etc.) |
| `Job_Title` | `object` | Role / designation of the employee |
| `Salary_INR` | `float64` | Annual salary in Indian Rupees |
| `Status` | `object` | Active, Resigned, Retired, or Terminated |
| `Work_Mode` | `object` | Remote or On-site |
| `Hire_Date` | `datetime64` | Date hired — parsed from string in notebook |
| `Experience_Years` | `int64` | Years of professional experience |
| `Performance_Rating` | `float64` | Numeric performance score |
| `Location` | `object` | City, Country — Country extracted via `lambda` |

---

## ⚙️ Analysis Pipeline

```
STEP 1 — Library Import & Setup
         pandas · matplotlib · seaborn · random · %matplotlib inline

STEP 2 — Data Loading & Inspection
         read_csv() · df.info() · .unique() · .value_counts() · .nunique()

STEP 3 — Data Cleaning & Preprocessing
         drop('Unnamed: 0') · to_datetime(Hire_Date) · insert(Year) · lambda → Country

STEP 4 — Exploratory Data Analysis (EDA)
         groupby() · agg() · corr() · nlargest() · filter by Status · attrition rate %

STEP 5 — Data Visualisation
         Pie charts · Bar charts · Count plots · Heatmaps · Horizontal bar · savefig()
```

---

## ❓ 15 Business Questions Answered

| # | Question | Visualisation |
|:---:|----------|:-------------:|
| Q 01 | Distribution of Employee Status (Active, Resigned, Retired, Terminated) | 🥧 Pie Chart |
| Q 02 | Distribution of Work Modes — On-site vs Remote | 🥧 Pie Chart |
| Q 03 | How many employees are in each Department & Job Title? | 📊 Count Plot |
| Q 04 | Average Salary by Department (in thousands INR) | 📊 Bar Chart |
| Q 05 | Which Job Title has the highest average salary? | 📊 Bar Chart |
| Q 06 | Average salary across Departments segmented by Job Title | ↔️ Horizontal Bar |
| Q 07 | Count of Resigned & Terminated employees per Department | 📊 Grouped Bar Chart |
| Q 08 | How does Salary vary with Years of Experience? | 📋 GroupBy Table |
| Q 09 | Average Performance Rating by Department | 📊 Bar Chart |
| Q 10 | Which Countries have the highest concentration of employees? | 📋 value_counts() |
| Q 11 | Correlation between Performance Rating and Salary | 🔥 Heatmap |
| Q 12 | How has the number of hires changed year over year? | 📈 Time-series Bar |
| Q 13 | Salary difference between Remote vs On-site employees | 📋 GroupBy Mean |
| Q 14 | Top 10 highest-paid employees in each Department | 📋 nlargest() Table |
| Q 15 | Departments with the highest attrition rate (Resigned %) | 📋 Sorted DataFrame |

---

## 🛠️ Technologies & Libraries

| Tool | Role |
|------|------|
| ![Python](https://img.shields.io/badge/-Python_3-3776AB?logo=python&logoColor=white&style=flat-square) | Core programming language |
| ![Jupyter](https://img.shields.io/badge/-Jupyter_Notebook-F37626?logo=jupyter&logoColor=white&style=flat-square) | IDE / Interactive environment |
| ![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white&style=flat-square) | Data loading, cleaning & wrangling |
| ![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?style=flat-square) | Base charting & plotting |
| ![Seaborn](https://img.shields.io/badge/-Seaborn-4C72B0?style=flat-square) | Statistical visualisations |
| `random` | Random colour generation (Q6 chart) |
| `HR_Data.csv` | Source HR dataset |

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/hr-data-analysis-with-python.git
cd hr-data-analysis-with-python

# 2. Install required libraries
pip install pandas matplotlib seaborn jupyter

# 3. Launch Jupyter Notebook
jupyter notebook hr-data-analysis-with-python.ipynb
```

> ⚠️ Make sure `HR_Data.csv` is in the **same directory** as the notebook before running.

---

## 📬 Contact

<div align="center">

### Kartik Yadav
*Data Analyst · Python Developer*

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kartik_Yadav-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kartik-yadav-4b25553b0)
[![Email](https://img.shields.io/badge/Email-kartikyadav798261@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kartikyadav798261@gmail.com)
[![Phone](https://img.shields.io/badge/Phone-+91_7982612231-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](tel:+917982612231)

</div>

---

<div align="center">

*Crafted with ❤️ by **Kartik Yadav** · HR Data Analysis with Python · EDA Project*

</div>
