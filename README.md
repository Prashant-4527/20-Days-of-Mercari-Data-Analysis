# 📦 20 Days of Mercari Data Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.24-013243?style=flat&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-11557C?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0?style=flat)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-f59e0b?style=flat)
![Days](https://img.shields.io/badge/Progress-16%20of%2020%20Days-6366f1?style=flat)

**A structured 20-day learning challenge — one concept per day, applied directly to 50,000 rows of real Mercari e-commerce data.**

[View Notebooks](#-day-by-day-breakdown) • [Dataset](#-dataset) • [Key Insights](#-key-findings-from-the-data) • [SQL Twin Repo](#-related-repositories) • [Author](#-author)

</div>

---

## 🎯 What This Is

This repository documents a **20-day structured Pandas + Visualization learning challenge** built on the Mercari Price Suggestion dataset. Every day covers one core concept — from Series and DataFrames through advanced Seaborn visualizations — applied immediately to real industry data.

This is **Phase 1** of a larger roadmap targeting the METI Japan internship (2027) and a Mercari AI Engineer role (2028).

> **Learning philosophy**: No toy datasets. Every concept is practiced on real Mercari listings — 50,000 rows, 8 columns, messy nulls, skewed distributions, and real business questions to answer.

---

## 📊 Dataset

**Source**: [Kaggle — Mercari Price Suggestion Challenge](https://www.kaggle.com/c/mercari-price-suggestion-challenge/data)  
**Size**: 50,000 listings · 8 columns  
**Domain**: Japanese e-commerce (secondhand marketplace)

| Column | Type | Notes |
|--------|------|-------|
| `name` | string | Item listing title |
| `category_name` | string | 3-level hierarchy (e.g. Women/Tops/T-shirts) |
| `brand_name` | string | 43% missing — key cleaning decision |
| `price` | float | Target variable · heavily right-skewed |
| `item_condition_id` | int | 1=New, 2=Like New, 3=Good, 4=Fair, 5=Poor |
| `shipping` | int | 1=seller pays, 0=buyer pays |
| `item_description` | string | Free text · 5.7% are placeholder "No description yet" |

---

## 📅 Day-by-Day Breakdown

### Week 1 — Pandas Core

| Day | Topic | Key Concepts |
|-----|-------|-------------|
| [Day 1](Day1_First%20Look.ipynb) | Series & DataFrames | 5-line dataset greeting · dtype inspection · boolean masking |
| [Day 2](Day2_loc_iloc.ipynb) | .loc & .iloc | Label vs position access · boolean filtering pattern · ML feature split |
| [Day 3](Day3_Cleaning.ipynb) | Data Cleaning | dropna decisions · fillna strategies · duplicate detection |
| [Day 4](Day4_Featuring.ipynb) | String Operations | str.split · map() · apply() · feature engineering from raw text |
| [Day 5](Day5_Groupby-Analysis.ipynb) | groupby & agg | split-apply-combine · named aggregation · multi-column groupby |
| [Day 6](Day6_merging-concat.ipynb) | merge & concat | Join types · ignore_index · category metadata enrichment |
| [Day 7](Day7_pivot_table-crosstab.ipynb) | pivot_table & crosstab | 2D summaries · margins · normalize for % distributions |

### Week 2 — Advanced Pandas + NumPy

| Day | Topic | Key Concepts |
|-----|-------|-------------|
| [Day 8](Day8_sort-ranking.ipynb) | sort & rank | nlargest/nsmallest · rank(dense) · price_rank_in_category feature |
| [Day 9](Day9_Numpy_on_Mercari.ipynb) | NumPy on Real Data | np.log1p transformation · IQR outlier detection · np.where |

### Week 3 — Visualization

| Day | Topic | Key Concepts |
|-----|-------|-------------|
| [Day 10](Day10_Basic_Charts.ipynb) | Matplotlib Basics | hist · bar · scatter · style_ax() · COLORS system |
| [Day 11](Day11_Advanced_Charts.ipynb) | Matplotlib Advanced | subplots · fig/ax pattern · value labels · reference lines |
| [Day 12](Day12_Seaborn_Charts_basic.ipynb) | Seaborn Basics | countplot · barplot with CI · histplot + KDE · hue parameter |
| [Day 13](Day13_Heatmap_Pairplot.ipynb) | Heatmap & Pairplot | Correlation matrix · coolwarm cmap · pairplot with sampling |
| [Day 14](Day14_Advance_charts_using_seaborn.ipynb) | Seaborn Advanced | boxplot · violinplot · stripplot · box+strip combined |

### Week 4 — Project Completion

| Day | Topic | Key Concepts |
|-----|-------|-------------|
| [Day 15](Day15_EDA_Visual_Story.ipynb) | EDA Visual Story | 6 publication-quality charts telling one coherent story |
| [Day 16](Day16_Challenge.ipynb) | Unguided Challenge | Full pipeline from scratch · no hints · business insights |
| Day 17 | Statistical Analysis | Outlier detection · IQR method · skewness · kurtosis · normality tests |
| Day 18 | Correlation & Business Insights | Pearson/Spearman correlation · feature importance · actionable conclusions |
| Day 19 | Mini Dashboard | Combined subplot story · multi-chart layout · publication-ready figures |
| Day 20 | Capstone Notebook | End-to-end EDA report · clean pipeline · final business summary |

> Days 17–20 coming soon.

---

## 🧠 Concepts Covered

<table>
<tr>
<td valign="top" width="50%">

**Pandas**
- Series · DataFrames · dtypes
- .loc and .iloc (label vs position)
- dropna · fillna · drop_duplicates
- str.split · str.lower · str.contains
- map() · apply() · lambda functions
- groupby · agg · size vs count
- merge (inner/left/right) · concat
- pivot_table · crosstab · normalize
- sort_values · nlargest · rank(dense)

</td>
<td valign="top" width="50%">

**NumPy**
- np.log1p (price transformation)
- np.percentile (IQR outlier detection)
- np.where (fast vectorized if-else)

**Matplotlib + Seaborn**
- hist · bar · scatter · line · barh
- subplots · fig/ax pattern
- countplot · barplot · histplot + KDE
- heatmap · pairplot · boxplot
- violinplot · stripplot · combined

</td>
</tr>
</table>

---

## 💡 Key Findings from the Data

Working through this challenge revealed five meaningful insights about the Mercari platform:

1. **Price requires log transformation** — Raw price is severely right-skewed (skewness ≈ 8.2). Log₁ₚ compression produces a near-normal distribution suitable for regression models.

2. **Category is the strongest price signal** — Electronics items average nearly 2× the platform mean of $26.65. Category explains more price variance than condition, brand, or description quality.

3. **Brand premium is real but concentrated** — Luxury brands (Celine, Canada Goose, Valentino) average 5–20× the platform mean. But these represent under 1% of all listings.

4. **Seller shipping behavior is strategic** — Handmade sellers absorb shipping costs 63% of the time to compete on service. Electronics sellers pay only 41% of the time.

5. **Description impact varies by category** — A description adds meaningful price premium in Vintage & Collectibles but almost none in Beauty. Blanket prompts are less effective than category-targeted ones.

---

## 🔗 Related Repositories

This repo is one half of a two-track Mercari data project:

| Repo | Focus | Stack |
|------|-------|-------|
| **📓 This repo** — [20-Days-of-Mercari-Data-Analysis](https://github.com/Prashant-4527/20-Days-of-Mercari-Data-Analysis) | Python EDA · Visualization · Feature Engineering | Pandas · NumPy · Matplotlib · Seaborn |
| **🗄️ SQL twin** — [mercaridb-sql](https://github.com/Prashant-4527/mercaridb-sql) | Database design · Business SQL · Analytics queries | MySQL · Window Functions · CTEs |

> Together, these repos represent a full-stack data analysis approach to the Mercari marketplace — querying from the database layer through Python visualization.

---

## 🗂 Folder Structure

```
20-Days-of-Mercari-Data-Analysis/
│
├── Day1_First Look.ipynb
├── Day2_loc_iloc.ipynb
├── Day3_Cleaning.ipynb
├── Day4_Featuring.ipynb
├── Day5_Groupby-Analysis.ipynb
├── Day6_merging-concat.ipynb
├── Day7_pivot_table-crosstab.ipynb
├── Day8_sort-ranking.ipynb
├── Day9_Numpy_on_Mercari.ipynb
├── Day10_Basic_Charts.ipynb
├── Day11_Advanced_Charts.ipynb
├── Day12_Seaborn_Charts_basic.ipynb
├── Day13_Heatmap_Pairplot.ipynb
├── Day14_Advance_charts_using_seaborn.ipynb
├── Day15_EDA_Visual_Story.ipynb
└── Day16_Challenge.ipynb
```

> **Dataset not included** — download `train.tsv` from [Kaggle](https://www.kaggle.com/c/mercari-price-suggestion-challenge/data) and save as `mercari_sample.csv` in the repo root.

---

## ⚙️ Setup

```bash
# Clone the repo
git clone https://github.com/Prashant-4527/20-Days-of-Mercari-Data-Analysis.git
cd 20-Days-of-Mercari-Data-Analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch Jupyter
jupyter notebook
```

Open any `DayN_*.ipynb` to follow along.

---

## 🗺 Roadmap Context

This challenge is **Phase 1** of an 8-phase AI engineering roadmap:

| Phase | Timeline | Focus |
|-------|----------|-------|
| **Phase 1** 🔄 | Apr 2026 | Pandas · NumPy · Matplotlib · Seaborn · MySQL |
| Phase 2 | May–Jun 2026 | Math for ML · Japan Trade Analysis |
| Phase 3 | Jul–Aug 2026 | ML Models · XGBoost · Scikit-learn |
| Phase 4 | Sep 2026 | FastAPI · Docker · REST APIs |
| Phase 5 | Oct–Dec 2026 | GenAI · RAG · Japanese NLP |
| Phase 6 | Jan–Feb 2027 | Deep Learning · PyTorch · LSTM |
| Phase 7 | Mar–Apr 2027 | METI Prep · Portfolio Polish |
| Phase 8 | Jul 2027–Jul 2028 | MLOps · AWS · Mercari Application |

**Target**: METI Japan Internship (May–Jun 2027) → Mercari AI Engineer (Jul 2028)

---

## 👤 Author

**Prashant Sulaniya**  
BCA Student · Maharaja Government College, Jaipur  
Self-training toward AI Engineer @ Mercari Tokyo

[![GitHub](https://img.shields.io/badge/GitHub-Prashant--4527-181717?style=flat&logo=github)](https://github.com/Prashant-4527)
[![JLPT](https://img.shields.io/badge/Japanese-JLPT%20N4%20%E2%86%92%20N3-red?style=flat)](https://www.jlpt.jp/e/)

---

<div align="center">
<sub>Built with 20 days of consistent daily work · April–May 2026</sub>
</div>
