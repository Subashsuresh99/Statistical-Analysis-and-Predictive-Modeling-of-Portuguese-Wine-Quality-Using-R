# 🍷 Statistical Analysis and Predictive Modeling of Wine Quality

This project applies **data science and statistical modeling techniques** to explore, analyze, and predict the quality and characteristics of wines using chemical and sensory data.
It was developed as part of the *Introduction to Data Sciences* course under Prof. Dr.-Ing. Joachim Schwarz (Submission Date: June 30, 2025).

---

## 📘 Overview

The study investigates relationships between wine properties and perceived quality using a mix of **statistical tests**, **regression modeling**, **machine learning classification**, and **factor analysis** in **R**.

The dataset contains **6,497 observations** (1,599 red and 4,898 white wines) with 11 numerical attributes such as acidity, sulphates, alcohol, and pH.

---

## 🧠 Objectives

1. Perform **exploratory data analysis (EDA)** to summarize and visualize data distributions.
2. Test hypotheses using **t-tests** to compare wine types.
3. Develop a **linear regression model** to predict red-wine quality.
4. Train a **classification model** to distinguish “good” vs “bad” wines.
5. Build a **logistic regression model** to predict wine colour.
6. Apply **factor analysis** to reduce dimensionality of chemical features.

---

## 📊 Methods & Models

| Task  | Method / Technique                                   | Key Outcome                                                                                                        |
| ----- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| **1** | Descriptive statistics, skewness & outlier detection | No missing data; several right-skewed variables identified.                                                        |
| **2** | Welch’s t-test                                       | White wines show slightly higher mean alcohol content (p = 0.0043).                                                |
| **3** | Multiple linear regression                           | 36% variance in quality explained; alcohol & sulphates increase quality, volatile acidity & chlorides decrease it. |
| **4** | Random Forest classification                         | 90% accuracy, AUC = 0.94 in predicting good vs bad wines.                                                          |
| **5** | Logistic regression                                  | 98.9% accuracy, AUC = 0.998 in classifying red vs white wines.                                                     |
| **6** | Factor analysis (PAF, oblimin rotation)              | Three latent factors explain 61% of total variance.                                                                |

---

## 🧩 Tools & Libraries

* **Language:** R (R Core Team, 2024)
* **Main Packages:**
  `ggplot2`, `dplyr`, `tidyr`, `psych`, `mosaic`, `e1071`, `car`, `caret`, `pROC`, `GGally`, `factoextra`, `FactoMineR`, `lmtest`

---

## 📂 Project Structure

```
├── data/
│   └── wine.csv
├── scripts/
│   └── wine_analysis.R
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── results/
├── report/
│   └── wine_quality_report.pdf
└── README.md
```

---

## ⚙️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/wine-quality-analysis.git
   cd wine-quality-analysis
   ```

2. Open `wine_analysis.R` in RStudio or VSCode with R extension.

3. Install dependencies:

   ```R
   install.packages(c("ggplot2","dplyr","tidyr","psych","mosaic",
                      "e1071","car","caret","pROC","GGally",
                      "factoextra","FactoMineR","lmtest"))
   ```

4. Run the script step by step or execute all chunks:

   ```R
   source("scripts/wine_analysis.R")
   ```

5. Results (figures, tables, and summaries) will appear in the console and `outputs/` folder.

---

## 📈 Key Insights

* Alcohol and sulphate levels are the strongest predictors of wine quality.
* Volatile acidity and chlorides negatively impact perceived quality.
* Machine-learning models can classify wine type and quality with high accuracy.
* Three latent factors—**Acidity**, **Sweetness/Sulphur**, and **Alcohol/Volatility**—capture the majority of variance across features.

---

## 🤖 AI Tool Declaration

ChatGPT (OpenAI, 2025) was used **only** for phrasing, formatting assistance, and code automation within R (e.g., automating loops for skewness and outlier detection).
No analytical or statistical decision-making was delegated to AI.

---

## 🧾 References

Cortez et al. (2009). *Modelling wine preferences by data mining from physicochemical properties.* Decision Support Systems, 47(4), 547–553.
Atalay et al. (2021). *Wine quality prediction with machine-learning techniques.* Food Science and Technology, 41(Suppl 1), 83–90.
Vidal et al. (2015). *Application of factor analysis to wine chemistry.* Food Chemistry, 169, 237–243.
Field, A. (2013). *Discovering Statistics Using R.* Sage.
R Core Team (2024). *R: A language and environment for statistical computing.*

---

## 👥 Authors

* **Subash Karapparambu Suresh Kumar** — Matr.-Nr.: 7026794

---

**License:** Academic / Educational use only.
