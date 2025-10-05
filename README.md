
## 📊 Project Overview

A comprehensive Power BI dashboard that analyzes diabetes patient data to uncover risk patterns, demographic trends, and correlations between key health metrics. Built with advanced DAX calculations, custom tooltips, and interactive visualizations for healthcare decision-making.

**Key Highlights:**
- 📈 **768 Patients** analyzed across 9 health variables
- 🎯 **34.9% Diabetes Rate** with detailed risk profiling
- 🔍 **3 Interactive Pages**: Overview, Detailed Analysis, Custom Tooltips
- 💡 **12+ Visualizations** with cross-filtering capabilities

---

## 🎯 Key Features

### Dashboard Pages

| Page | Purpose | Key Visuals |
|------|---------|-------------|
| **Overview** | High-level KPIs & distributions | 4 KPI Cards, Age/BMI/Glucose charts, Patient table |
| **Detailed Analysis** | Risk correlations & statistics | Scatter plot (BMI vs Glucose), Insulin trends, Blood pressure analysis |
| **Custom Tooltips** | Hover details | Patient-specific metrics with risk indicators |

### Interactive Elements
- ✅ **Smart Filters**: Age groups, BMI categories, diagnosis status
- ✅ **Cross-Filtering**: Click any visual to update entire dashboard
- ✅ **Custom Tooltips**: Hover for detailed patient information with risk levels
- ✅ **Navigation**: Seamless page transitions with back buttons

---

## 📸 Dashboard Preview

> **[View Complete Dashboard PDF](Diabetes%20Patient%20Analysis%20Dashboard.pdf)** - All 3 pages exported

**Page 1 - Overview:**
- Total Patients: 768 | Diabetic: 268 (34.9%) | Non-Diabetic: 500 (65.1%)
- Age distribution, glucose trends, BMI analysis, diagnosis breakdown

**Page 2 - Detailed Analysis:**
- BMI vs Glucose scatter plot (768 data points, color-coded by diagnosis)
- Insulin patterns, blood pressure distribution, pregnancy risk analysis
- Overall statistics: Avg BMI 31.99, Avg Glucose 120.89, Avg Age 33.24

**Page 3 - Custom Tooltip:**
- Displays on hover: Age, Glucose, BMI, Blood Pressure, Insulin, Outcome
- Risk indicators: ✓ Non-Diabetic (Green) | ⚠️ Diabetic (Red)
- BMI classification: Underweight/Normal/Overweight/Obese

---

## 🔍 Key Insights

1. **Age Correlation**: Glucose levels peak at ages 50-60 (140.28 mg/dL), lowest at 20-30 (113.74 mg/dL)
2. **BMI Impact**: Strong positive correlation between higher BMI and diabetes diagnosis
3. **Pregnancy Risk**: Higher pregnancy counts correlate with increased diabetes rates
4. **Demographics**: Average patient age 33.24 years, range 21-81 years
5. **Blood Pressure**: Most patients cluster in 60-80 mmHg range

---

## 🛠️ Technical Stack

**Tools:** Power BI Desktop (v2.139.2054.0) | DAX | Power Query  
**Dataset:** [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) - 768 records, 9 variables

**Key DAX Measures:**
```dax
Total Patients = COUNT(diabetes[Outcome])
Diabetic Patients = CALCULATE(COUNT(diabetes[Outcome]), diabetes[Outcome] = 1)
Diabetes Rate % = DIVIDE([Diabetic Patients], [Total Patients], 0) * 100
```

**Calculated Columns:**
- BMI Category (Underweight/Normal/Overweight/Obese based on WHO standards)
- Diagnosis (User-friendly "Diabetic"/"Non-Diabetic" labels)
- Age/BMI/Blood Pressure bins for grouped analysis

---

## 🚀 Quick Start

1. **Clone repository:**
   ```bash
   git clone https://github.com/Hamdaan-P/PowerBI--Diabetes-Patient-Analysis-Dashboard.git
   ```

2. **Open `Diabetes Patient Analysis Dashboard.pbix` in Power BI Desktop**

3. **Refresh data** (if needed): Home → Transform Data → Update path to `diabetes.csv`

4. **Explore:** Use slicers to filter, click visuals to cross-filter, hover for tooltips

---

## 📁 Repository Contents

```
PowerBI--Diabetes-Patient-Analysis-Dashboard/
├── Diabetes Patient Analysis Dashboard.pbix    # Power BI file
├── Diabetes Patient Analysis Dashboard.pdf     # Dashboard export (3 pages)
├── diabetes.csv                                # Source dataset
└── README.md                                   # Documentation
```

---

## 💡 Skills Demonstrated

- ✅ **Power BI Proficiency**: Advanced visualizations, DAX, Power Query
- ✅ **Data Analysis**: Statistical analysis, correlation identification
- ✅ **Healthcare Domain**: Medical data interpretation, risk assessment
- ✅ **Design**: User-centric layouts, color psychology, accessibility
- ✅ **Documentation**: Clear technical communication

---

## 📊 Project Metrics

| Metric | Value |
|--------|-------|
| Total Patients | 768 |
| Visualizations | 12+ |
| DAX Measures | 7 |
| Calculated Columns | 6 |
| Development Time | 3-4 hours |

---

## 👨‍💻 Author

**Hamdaan-P**

- 🐙 GitHub: [@Hamdaan-P](https://github.com/Hamdaan-P)
- 📂 Project: [PowerBI--Diabetes-Patient-Analysis-Dashboard](https://github.com/Hamdaan-P/PowerBI--Diabetes-Patient-Analysis-Dashboard)

---

## 📝 License

MIT License - Free to use with attribution

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

Made with ❤️ using Power BI Desktop

</div>