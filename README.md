# Employee Sentiment Analysis

## Overview
This repository contains an end-to-end solution for labeling, analyzing, ranking, and modeling employee sentiment from email messages. It follows the project tasks: Sentiment Labeling, EDA, Employee Scoring, Ranking, Flight Risk Detection, and Predictive Modeling.

## Files & Folders
- `employee_sentiment_analysis.ipynb` - Main notebook (all tasks and visualizations).
- `test(in).csv` - Raw dataset (input).
- `labeled_dataset.csv` - Output from Task 1 (includes `Sentiment`).
- `employee_monthly_scores.csv` - Task 3 outputs.
- `employee_rankings.csv` - Task 4 outputs.
- `flight_risk_employees.csv` - Task 5 outputs.
- `visualizations/` - PNG images produced during EDA and modeling.
- `requirements.txt` - Python package requirements.

## How to run (local)
1. Create environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS / Linux
   venv\Scripts\activate      # Windows
   pip install -r requirements.txt

Run dashboard:
```bash
streamlit run dashboard.py
