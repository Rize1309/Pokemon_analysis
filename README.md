# 🔴 Pokémon Data Analysis — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

## 📖 About the Project

Exploratory Data Analysis (EDA) of a Pokémon dataset containing **800 Pokémon** across **6 generations** with 12 features including stats, types, and legendary status.

The goal is to uncover patterns in Pokémon stats, compare types and generations, and answer key analytical questions using Python data tools.

---

## 📂 Dataset

| Feature | Description |
|---|---|
| `#` | Pokémon ID |
| `Name` | Pokémon name |
| `Type 1` | Primary type |
| `Type 2` | Secondary type (if any) |
| `HP` | Hit Points |
| `Attack` | Attack stat |
| `Defense` | Defense stat |
| `Sp. Atk` | Special Attack |
| `Sp. Def` | Special Defense |
| `Speed` | Speed stat |
| `Generation` | Generation (1–6) |
| `Legendary` | Is Legendary (True/False) |

---

## 🛠️ Tools & Libraries

- **Python 3.11**
- **Pandas** — data cleaning and analysis
- **Matplotlib** — visualizations
- **Seaborn** — statistical plots

---

## 📊 Analysis Structure

### 1. Data Cleaning
- Filled missing values in `Type 2` with `"None"`
- Identified Mega-form duplicates (same `#`, different stats)
- Verified correct data types for all columns

### 2. Univariate Analysis
- Distribution of `Speed` — histogram
- Distribution of Pokémon types — bar chart

### 3. Bivariate & Correlation Analysis
- Heatmap of correlations between all numeric stats
- Scatter plot: `Attack` vs `Defense` colored by `Legendary` status

### 4. Type & Generation Deep-Dive
- Average `Attack` by Type 1 — bar chart
- `HP` distribution by Generation — box plot
- Top-50 Pokémon by `Total` stats breakdown

### 5. Key Questions Answered
- Which Generation 1 Pokémon have `Attack > 100`?
- Is there a significant difference in `Total` between Legendary and regular Pokémon?
- Which type appears most often in the Top-50 Pokémon by `Total`?

---

## 🔍 Key Findings

- 🐉 **Dragon** is the strongest type by average Attack (112 vs ~74 overall average) and dominates the Top-50 with **11 appearances**
- ⭐ **Legendary Pokémon** have a `Total` stat **34.5% higher** than regular Pokémon (637 vs 417 on average)
- 💊 **HP is stable across generations** — median stays at 60–70 in all 6 generations
- ⚠️ **Note:** Mega-forms share the same `#` as their base form and were excluded from type-based analysis to avoid skewed results

---

## 🚀 How to Run

```bash
git clone https://github.com/Rize1309/Pokemon_analysis.git
cd Pokemon_analysis
jupyter notebook pokemon_eda.ipynb
```

---

## 📁 Project Structure

```
Pokemon_analysis/
│
├── pokemon_data.csv       # Dataset (800 Pokémon, 12 features)
├── pokemon_eda.ipynb      # Main analysis notebook
└── README.md              # Project description
```
