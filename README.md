# Global FDI Net Inflows Analysis

📌 Overview

This project analyzes Foreign Direct Investment (FDI) net inflows as a percentage of GDP using World Bank data from 2000–2025.

The analysis focuses on:

FDI/GDP trends over time

Association with five economic indicators

Decision-tree classification

K-means clustering

Comparison of FDI/GDP across two time periods

Evaluation of regression performance

🎯 Objectives

Analyze the historical trend of FDI/GDP.

Identify indicators associated with FDI/GDP.

Classify observations into lower- and higher-FDI groups.

Identify country-level economic profiles using clustering.

Compare FDI/GDP between two periods.

Evaluate the limitations of numeric prediction.

📊 Dataset

Data was retrieved from the World Bank World Development Indicators API.

Years: 2000–2025

Countries/Economies: 262

Rows: 6,812

Target: FDI net inflows (% of GDP)

FDI indicator: BX.KLT.DINV.WD.GD.ZS

Selected Indicators

Trade openness — Trade (% of GDP)

Population — Log transformed

Domestic credit to private sector (% of GDP)

Mobile cellular subscriptions per 100 people

GDP per capita — Log transformed

🔬 Methodology

Retrieve data from the World Bank API.

Merge and clean country-year data.

Calculate descriptive statistics.

Analyze Spearman correlations over five-year periods.

Visualize annual FDI/GDP trends.

Compare regression models using a chronological train/test split.

Train a Decision Tree Classifier for lower/higher FDI.

Apply K-means clustering to country profiles.

Use the Wilcoxon signed-rank test to compare two periods.

📈 Key Results

Annual median FDI/GDP decreased from 2.577% (2000) to 1.921% (2025).

Highest annual median: 4.495% in 2007.

Lowest annual median: 1.601% in 2020.

Trade openness showed the strongest and most consistent positive association with FDI/GDP.

Population showed a consistent negative association.

Regression models produced negative R² values, so reliable numeric prediction was not demonstrated.

The decision tree achieved 63.9% test accuracy for lower/higher FDI classification.

K-means identified 3 country-profile clusters.

The typical country's FDI/GDP was lower in 2013–2025 than in 2000–2012.

Correlation and machine-learning results indicate associations and patterns, not causation.

🛠️ Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

SciPy

Scikit-learn

World Bank API

▶️ Run the Project

Install the required libraries:

pip install requests pandas numpy matplotlib seaborn scipy scikit-learn

Then run the Jupyter Notebook or Python script containing the analysis.

📚 Data Source

World Bank — World Development Indicators

Data retrieval date: 11 October 2026

Primary indicator:

BX.KLT.DINV.WD.GD.ZS
FDI net inflows (% of GDP)

👤 Project

Global FDI Net Inflows: Exploratory and Classification Analysis Using Python
