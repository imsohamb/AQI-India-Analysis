# 🌫️ Air Quality Index Analysis — India (2015–2020)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerics-013243?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle)

> **Exploratory Data Analysis (EDA) project** analyzing daily air quality across major Indian cities from 2015 to 2020 — uncovering pollution trends, seasonal patterns, and city-wise comparisons using real government data.

---

## 📌 Project Overview

Air pollution is one of India's most critical public health challenges. This project analyzes **real daily AQI (Air Quality Index) measurements** from major Indian cities to answer:

- 🏙️ Which Indian city is the most polluted?
- 📅 How does Delhi's air quality change across seasons and years?
- 🌡️ What percentage of days did Delhi experience "Severe" or "Very Poor" air quality?
- 📊 How do Mumbai, Bengaluru, Chennai, and Kolkata compare to Delhi?

---

## 📊 Dataset

**Source:** [Air Quality Data in India — Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)

**Original Source:** Central Pollution Control Board (CPCB), Government of India

| Detail | Info |
|--------|------|
| File used | `city_day.csv` |
| Time Period | 2015 – 2020 |
| Cities covered | 26 Indian cities |
| Key columns | City, Date, PM2.5, PM10, NO2, CO, SO2, O3, AQI |

> AQI (Air Quality Index) is a standardized scale used by governments worldwide to communicate how polluted the air is. Higher AQI = worse air quality.

---

## 🏷️ AQI Categories (Indian Standards)

| AQI Range | Category | Health Impact |
|-----------|----------|---------------|
| 0 – 50 | Good | Minimal impact |
| 51 – 100 | Satisfactory | Minor breathing discomfort |
| 101 – 200 | Moderate | Discomfort for sensitive people |
| 201 – 300 | Poor | Breathing discomfort for most |
| 301 – 400 | Very Poor | Respiratory illness on prolonged exposure |
| 401+ | Severe | Affects healthy people; serious risk for sensitive groups |

---

## 🛠️ Libraries Used

| Library | Purpose |
|--------|---------|
| `Pandas` | Loading, cleaning, filtering, and grouping data |
| `NumPy` | Numerical operations |
| `Matplotlib` | Bar charts, line graphs, pie charts |

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/AQI-India-Analysis.git
cd AQI-India-Analysis
```

### 2. Install dependencies
```bash
pip install numpy pandas matplotlib
```

### 3. Download the dataset
Download `city_day.csv` from [Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india) and place it in the project folder.

### 4. Run the Jupyter Notebook
```bash
jupyter notebook AQI_India_Project.ipynb
```

---

## 🔍 Project Workflow

```
Load Dataset (city_day.csv)
        ↓
Understand Structure (columns, data types, shape)
        ↓
Clean Data (remove missing AQI values)
        ↓
Filter for 5 Major Cities
        ↓
Calculate Average AQI per City → Bar Chart
        ↓
Analyze Delhi AQI Over Time → Line Graph
        ↓
Categorize AQI Levels for Delhi → Pie Chart
        ↓
Identify Most & Least Polluted City
        ↓
Save Results to CSV
```

---

## 📈 Results & Findings

### 🏙️ City-wise Average AQI (2015–2020)

A bar chart comparing the average AQI of **Delhi, Mumbai, Bengaluru, Chennai, and Kolkata** reveals:

- **Delhi** has the highest average AQI — consistently in the "Poor" to "Very Poor" range
- **Bengaluru** and **Chennai** have relatively lower average AQI
- All cities show AQI values well above the "Good" threshold (≤ 50)

---

### 📅 Delhi AQI Over Time

The line graph of Delhi's daily AQI from 2015–2020 shows a clear **seasonal pattern**:

- AQI **spikes sharply every winter (October–January)** due to:
  - Crop stubble burning in neighboring states
  - Cold air trapping pollutants close to the ground (temperature inversion)
  - Reduced wind speeds
- AQI drops during **monsoon season (July–September)** as rain washes pollutants away
- This pattern repeats every year — a classic real-world periodic signal

---

### 🥧 Delhi AQI Category Distribution

The pie chart shows what percentage of days (2015–2020) Delhi fell into each AQI category:

- A **majority of days** fall in the "Poor", "Very Poor", or "Severe" categories
- Only a small fraction of days had "Good" or "Satisfactory" air quality
- This quantifies what residents experience but rarely see as hard data

---

## 💡 Key Concepts Used

- **Exploratory Data Analysis (EDA)** — understanding data before modeling
- **Data Cleaning** — handling missing values in real-world datasets
- **Groupby Operations** — aggregating data by city
- **Time Series Visualization** — plotting trends over time
- **Custom Functions** — building an AQI categorization function
- **Data Filtering** — isolating specific cities and conditions

---

## 🗂️ Project Structure

```
AQI-India-Analysis/
│
├── AQI_India_Project.ipynb     # Main Jupyter Notebook
├── city_day.csv                # Dataset (download from Kaggle)
├── avg_aqi_results.csv         # Exported results
└── README.md                   # This file
```

---

## 🌍 Why This Matters

According to the World Health Organization, **India has 14 of the world's 20 most polluted cities**. Data science tools like this project allow us to:

- Quantify pollution levels objectively using real measurements
- Identify which cities and seasons need the most urgent intervention
- Communicate complex environmental data to policymakers and the public through visualization

This is data science applied to a real, urgent public health problem.

---

## 👤 Author

**Soham Bhagwat**
- GitHub: [@imsohamb](https://github.com/imsohamb)
- 📍 Pune, Maharashtra

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---
