# Video-Game-Sales-Analysis-EDA-Inference-Predictive-Modeling
End to end data science pipeline on 1,770 U.S. video game titles (2004–2010) — exploratory analysis, bootstrap inference, and regression modeling in Python.

## Project Structure

| Notebook | Focus | Key Techniques |
|---|---|---|
| `01_EDA_and_Visualization.ipynb` | Understanding sales distributions by console | Boxplots, summary statistics, groupby analysis |
| `02_Statistical_Inference.ipynb` | Drawing population level conclusions from sample data | Bootstrap confidence intervals, hypothesis testing |
| `03_Predictive_Modeling.ipynb` | Predicting sales and blockbuster status | Linear regression, logistic regression, train-test split, ROC-AUC |

## Dataset
Video Games Sales dataset (2004–2010) from the University of Portsmouth Research Portal, curated by Dr. Joe Cox. Contains 1,770 game titles across 166 variables including console, U.S. sales (millions), release year, and gameplay features.

**To run these notebooks:** Download `video_games.csv` from https://researchportal.port.ac.uk/en/datasets/video-games-dataset and place it in the same directory as the notebooks.

## Key Findings
- PS3 and Nintendo Wii had the highest median per-game sales; X360 led in total volume (partly due to having more titles in the dataset)
- 35.4% of games in this era included online features — 95% CI: [33.2%, 37.7%]
- True mean U.S. sales significantly exceeded 0.3M copies (p ≈ 0)
- Release year, online features, and perspective type explain only ~3% of sales variance — blockbuster status depends largely on factors outside this dataset (franchise recognition, marketing, critic reviews)

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, StatsModels

## Acknowledgements
Developed with Granth Bangard as part of STAT 207 (Data Science Exploration) at the University of Illinois Urbana-Champaign.
