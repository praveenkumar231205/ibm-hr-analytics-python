# 📊 IBM HR Analytics — Employee Attrition EDA

A comprehensive Exploratory Data Analysis (EDA) on the IBM HR Attrition dataset
to uncover key workforce trends, attrition patterns and actionable business 
recommendations for employee retention.

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `01_eda_and_insights.ipynb` | Main EDA Notebook |
| `IBM_HR_dataset.csv` | Dataset |
| `README.md` | Project Documentation |

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core Programming Language |
| Pandas | Data Manipulation & Cleaning |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualizations |
| Google Colab | Development Environment |

---

## 📌 Dataset Overview

- **Source**: IBM HR Analytics Dataset
- **Total Records**: 1,470 employees
- **Total Features**: 35 columns (7 irrelevant columns removed)
- **Target Variable**: Attrition (Yes/No)

---

## 🔍 Project Workflow

### 1. Data Cleaning
- Removed irrelevant columns (`EmployeeCount`, `EmployeeNumber`, 
  `StandardHours`, `Over18`, `HourlyRate`, `DailyRate`, `MonthlyRate`)
- Performed Type Coercion on integer columns to detect hidden missing values
- Stripped whitespace and replaced empty strings across object columns
- Confirmed zero missing values and zero duplicate rows

### 2. Univariate Analysis
- Plotted histograms for all numerical columns
- Mapped ordinal integer columns (`JobSatisfaction`, `Education`, 
  `WorkLifeBalance` etc.) to meaningful labels and plotted countplots
- Analyzed target variable distribution — 84% No Attrition vs 16% Attrition

### 3. Bivariate Analysis
- Analyzed 8 categorical variables vs Attrition using countplots
- Analyzed 6 numerical variables vs Attrition using histplots with hue
- Consistently tracked both **attrition rate** and **absolute volume** 
  for every variable

### 4. Correlation Heatmap
- Initial heatmap on numerical columns to identify multicollinearity
- Final heatmap with Attrition encoded as numeric to identify 
  correlation with target variable

---

## 🔑 Key Business Findings

### 🔴 High Risk Attrition Factors
- **Overtime** is the strongest attrition driver — employees working 
  overtime leave at `30.5%` rate, nearly **triple** the rate of 
  non-overtime employees (`10.4%`)
- **Young employees aged 18–22** show the highest turnover rate of 
  `47.4%` — almost every 1 in 2 young employees is leaving
- **Low income employees earning $1,000–$3,000** account for nearly 
  **half** of all departures (`107 out of 237`) with an attrition 
  rate of `29.3%`
- **Sales Representatives** exhibit the highest role-based attrition 
  rate of `~39.8%` posing a direct risk to company revenue

### 🟡 Moderate Risk Factors
- **HR Department** has an alarming attrition rate of `41%` which is 
  unsustainable for a department responsible for managing the 
  entire workforce
- **Single employees** leave at `~25.5%` rate — double that of 
  married employees
- **Freshers with 0–4 years** of experience account for the highest 
  volume of departures (`122 out of 237`) with a `26%` attrition rate
- **Long distance commuters** travelling beyond `13 miles` show 
  noticeably higher attrition rates peaking at `26.9%`

### 🟢 Positive Retention Indicators
- **High earners above $15,000** show `0%` attrition — compensation 
  is a strong retention tool
- **Employees with 4+ years** at the company show dramatically 
  improved retention dropping below `13%` attrition rate
- **~70%** of employees are highly involved in their work indicating 
  a largely engaged and productive workforce
- **Research Directors and Managers** show the lowest role-based 
  attrition at `~2.5%` and `~4.9%` respectively

---

## 📋 Recommendations

- Revisit **overtime policies** — the data strongly suggests burnout 
  is a primary attrition driver
- Introduce **early career retention programs** targeting employees 
  in their first 4 years
- Review **compensation structure** for lower income brackets and 
  Sales Representatives
- Address **HR department burnout** as losing HR staff creates a 
  compounding retention problem across the entire organization

---

## ▶️ How to Run

1. Clone the repository
```bash
git clone https://github.com/yourusername/IBM-HR-Analytics.git
```

2. Install required libraries
```bash
pip install pandas numpy matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook 01_eda_and_insights.ipynb
```

Or simply open directly in **Google Colab**

---

## 👤 Author

**Praveenkumar Chettiyar**  
B.Tech Artificial Intelligence  
GH Raisoni College of Engineering, Nagpur
  [LinkedIn](www.linkedin.com/in/praveenkumar-chettiyar-8b4a193a9) |  
[GitHub](https://github.com/praveenkumar231205)

---

⭐ If you found this project helpful, feel free to star the repository!
