# Healthcare & Road Accident Data Analysis

An end-to-end data analysis project on two real-world datasets: hospital patient encounters (diabetes care) and road accidents. The goal is to turn raw, messy data into clear, evidence-based insights.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Business Questions](#business-questions)
3. [Datasets](#datasets)
4. [Tools & Technologies](#tools--technologies)
5. [Project Structure](#project-structure)
6. [Methodology](#methodology)
7. [Key Findings](#key-findings)
8. [Recommendations](#recommendations)
9. [Limitations](#limitations)
10. [How to Run](#how-to-run)
11. [Author](#author)

---

## Project Overview

This project covers the full analytics workflow: defining questions, cleaning data, exploratory analysis, deeper statistical analysis, visualization, and recommendations.

- **Part 1: Healthcare Analysis.** What drives hospital readmission and length of stay for diabetic patients?
- **Part 2: Accident Analysis.** When, where and under what conditions do road accidents occur, and what makes them severe?

---

## Business Questions

### Healthcare
1. Which patient groups (age, diagnosis, number of medications) have the highest 30-day readmission rate?
2. What factors are associated with a longer hospital stay?
3. Is there a relationship between medication changes and readmission?

### Accidents
1. At what hours, days and months do accidents peak?
2. How do weather and visibility relate to accident severity?
3. Which states or cities are accident hotspots?

---

## Datasets

| Dataset | Source | Size | Description |
|---|---|---|---|
| Diabetes 130-US Hospitals | [UCI ML Repository](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008) | ~100,000 rows | Hospital encounters, diagnoses, medications, readmission |
| US Accidents | [Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents) | ~7M rows (sampled) | Accident location, time, weather, severity |

> Raw data is **not** included in this repository because of file size. Download it from the links above and place it in `data/raw/`.

---

## Tools & Technologies

- **Python:** pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook
- **Optional:** SQL, Power BI / Tableau for the dashboard

---

## Project Structure

```
data-analysis-project/
│
├── data/
│   ├── raw/              # Original files (never modified)
│   └── clean/            # Cleaned datasets
├── notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   └── 04_analysis.ipynb
├── reports/
│   └── figures/          # Exported charts
├── README.md
└── requirements.txt
```

---

## Methodology

1. **Data loading and profiling:** shape, data types, missing values, duplicates.
2. **Data cleaning:** handling missing values, fixing data types, removing duplicates, treating outliers. Every decision is documented in the cleaning log below.
3. **Exploratory data analysis:** distributions, trends, correlations.
4. **Deep-dive analysis:** answering each business question with evidence.
5. **Visualization:** charts and dashboard.
6. **Insights and recommendations.**

### Cleaning Log

| Column | Issue | Action | Reason |
|---|---|---|---|
| *(example)* weight | ~97% missing | Dropped | Too sparse to be useful |
| *(add your own)* | | | |

---

## Key Findings

> Fill this section in after your analysis, using real numbers from your results.

### Healthcare
- Finding 1: *(e.g. Patients aged 70–80 had the highest readmission rate at X%)*
- Finding 2:
- Finding 3:

### Accidents
- Finding 1: *(e.g. Accident counts peak between 7–9 AM and 4–6 PM on weekdays)*
- Finding 2:
- Finding 3:

*(Add 2–3 of your best charts here: `![Chart title](reports/figures/chart1.png)`)*

---

## Recommendations

- *(Healthcare)* Example: Prioritise follow-up care for the highest-risk patient groups identified above.
- *(Accidents)* Example: Increase traffic monitoring during identified peak hours and locations.

---

## Limitations

- Findings show **associations, not causation**.
- The healthcare data covers 1999–2008 and US hospitals only, so it may not reflect current practice.
- The accident data may have reporting bias and missing weather values.
- Analysis is based on a sample of the accident dataset.

This analysis is for educational purposes and is not medical or policy advice.

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download datasets into data/raw/ (see Datasets section)

# 4. Launch Jupyter and run the notebooks in order
jupyter notebook
```

`requirements.txt`:
```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## Author

**ABHISHEK RATHOD**
- GitHub: https://github.com/abhirathod2001/
- LinkedIn: https://www.linkedin.com/in/abhishek-rathod-0264b9212/
- Email: ar5091188@gmail.com

---

*If you found this project useful, consider giving it a star.*
