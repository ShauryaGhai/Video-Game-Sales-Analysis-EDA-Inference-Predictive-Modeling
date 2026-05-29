# Video Game Sales: A Complete Data Science Pipeline

End to end analysis of U.S. video game sales across five major consoles 
(2004–2010), covering the full data science workflow from exploratory 
analysis through statistical inference to predictive modeling.

## Overview

The central question is deceptively simple: which consoles produced the 
best selling games during this era? But total sales are inflated by how 
many titles a console has in the dataset — median sales per game tell a 
more honest story. And once you ask why some games sell more than others, 
regression models quickly reveal that the features we can measure explain 
very little of what actually drives commercial success.

## Notebooks

**01 — EDA and Visualization**
Exploratory analysis comparing sales distributions across five consoles 
using boxplots, summary statistics, and grouped aggregations — separating 
typical per-game performance from total volume.

**02 — Statistical Inference**
Bootstrap confidence interval estimating the proportion of games with 
online features, and a hypothesis test on whether true mean U.S. sales 
exceeded 0.3 million copies.

**03 — Predictive Modeling**
Linear regression predicting U.S. sales and logistic regression predicting 
blockbuster status (>1M copies), evaluated on an 80/20 train-test split 
with adjusted classification threshold for class imbalance.

## Key Findings

- PS3 and Nintendo Wii had the highest median per game sales; X360 led in 
  total volume partly due to having more titles in the dataset
- 35.4% of games included online features — 95% CI: [0.332, 0.377]
- Hypothesis test rejected true mean = 0.3M (p ≈ 0, observed mean = 0.48M)
- Linear regression R² = 0.032, RMSE = 1.09M — release year, perspective, 
  and online features explain very little of sales variance
- Logistic regression AUC = 0.615, sensitivity = 62.9% — modest predictive 
  ability, limited by missing variables like critic scores and franchise status

## Dataset

1,770 game titles from the University of Portsmouth Research Portal, 
curated by Dr. Joe Cox. To run: download `video_games.csv` from 
https://researchportal.port.ac.uk/en/datasets/video-games-dataset and 
place it in the same directory as the notebooks.

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, StatsModels

## Acknowledgements
Developed collaboratively as part of STAT 207 (Data Science Exploration) 
at the University of Illinois Urbana-Champaign.
