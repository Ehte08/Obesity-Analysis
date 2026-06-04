# Obesity Analysis

A statistical analysis of lifestyle and behavioral factors associated with obesity levels, done as a group project for AMS317 at Stony Brook. We pulled data from the UCI Machine Learning Repository — 2,111 records, 17 features, covering eating habits, physical activity, transportation modes, and family history — and tested two hypotheses against it.

---

## Hypotheses

**Hypothesis 1** — Lifestyle factors (caloric intake, physical activity, alcohol consumption, water intake) can significantly predict obesity level using logistic regression. We evaluated with ROC/AUC curves and interaction modeling to see which factors actually moved the needle.

**Hypothesis 2** — Lower physical activity frequency (FAF) and higher reliance on sedentary transportation (automobile vs. walking) are associated with significantly higher obesity levels. This one involved computing BMI from the raw height/weight data and running regression against the behavioral features.

---

## Dataset

[UCI ML Repository — Estimation of Obesity Levels](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition) (ID: 544)

2,111 individuals from Mexico, Peru, and Colombia. Features include family history of obesity, frequency of high-caloric food consumption, vegetable intake, meal frequency, water intake, alcohol consumption, physical activity frequency, hours of technology use, and primary transportation mode.

```python
from ucimlrepo import fetch_ucirepo
dataset = fetch_ucirepo(id=544)
```

---

## Running the notebook

```bash
pip install ucimlrepo pandas numpy matplotlib seaborn statsmodels scikit-learn
jupyter notebook AMS317GroupProject.ipynb
```

The notebook walks through data loading, descriptive statistics, hypothesis testing, and visualization in order.

---

## Files

```
Obesity-Analysis/
├── AMS317GroupProject.ipynb     # Full analysis notebook
└── AMS317 Group Presentation.pdf  # Slide deck from the final presentation
```
