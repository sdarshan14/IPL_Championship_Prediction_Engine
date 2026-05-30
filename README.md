# IPL Championship Prediction Engine

## Overview

The IPL Championship Prediction Engine is a sports analytics research project designed to identify the key factors that contribute to winning the Indian Premier League (IPL). Unlike traditional IPL projects that focus on player statistics, this project investigates the relationship between league-stage performance and championship success.

The project analyzes playoff teams from IPL seasons 2011–2025 and studies how league position, points, net run rate (NRR), and playoff qualification patterns influence title-winning probabilities.

The ultimate goal is to develop a Championship Readiness Index (CRI) and build a championship prediction framework based on historical IPL data.

---

## Research Questions

This project attempts to answer the following questions:

1. Does finishing in the Top 2 significantly increase championship chances?
2. How important is winning Qualifier 1?
3. Does a higher Net Run Rate increase title probability?
4. Which league position has historically produced the most champions?
5. Is there a measurable relationship between points table performance and title success?
6. Can a Championship Readiness Index (CRI) effectively identify championship-caliber teams?

---

## Dataset Information

Dataset Name:

```text
IPL_Championship_Research_Dataset.xlsx
```

Period Covered:

```text
2011–2025
```

Reason:

```text
IPL playoff format was introduced in 2011.
```

Dataset Includes:

- All playoff teams from 2011–2025
- League standings
- Points
- Net Run Rate (NRR)
- Match results
- Champions
- Runner-Ups

Total Seasons:

```text
15
```

Total Playoff Team Records:

```text
60
```

---

## Dataset Features

| Column | Description |
|----------|----------|
| Season | IPL Season |
| Team | Team Name |
| LeaguePosition | Position after League Stage |
| Matches | Matches Played |
| Wins | Matches Won |
| Losses | Matches Lost |
| NoResult | No Result Matches |
| Points | League Stage Points |
| NRR | Net Run Rate |
| C | Champion Flag (1 = Champion, 0 = Not Champion) |
| RU | Runner-Up Flag (1 = Runner-Up, 0 = Not Runner-Up) |

---

## Technologies Used

### Programming

- Python

### Data Analysis

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn

### Notebook Environment

- Google Colab

### Version Control

- GitHub

---

## Project Structure

```text
IPL-Championship-Prediction-Engine/
│
├── data/
│   └── IPL_Championship_Research_Dataset.xlsx
│
├── charts/
│
├── output/
│
├── IPL_Championship_Prediction_Engine.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## Project Workflow

### Phase 1: Data Collection

- Collect IPL playoff team data from 2011–2025.
- Record league positions and playoff outcomes.

### Phase 2: Data Cleaning

- Validate team records.
- Handle missing values.
- Standardize dataset structure.

### Phase 3: Exploratory Data Analysis

- League Position Analysis
- Champion Analysis
- Runner-Up Analysis
- NRR Analysis
- Points Analysis

### Phase 4: Championship Readiness Index

Develop a custom metric to estimate a team's championship readiness.

### Phase 5: Predictive Analytics

Future enhancement involving machine learning models for championship probability prediction.

---

## Analyses Performed

### League Position Analysis

Investigates title-winning frequencies across:

- Position 1
- Position 2
- Position 3
- Position 4

### Champion Analysis

Studies historical champions and their league-stage performance.

### Runner-Up Analysis

Examines runner-up trends and league positions.

### Net Run Rate Analysis

Evaluates the relationship between NRR and title success.

### Points Analysis

Measures the impact of league-stage points on championship outcomes.

### Team Success Analysis

Compares title counts across franchises.

### Correlation Analysis

Studies relationships among:

- League Position
- Points
- NRR
- Championship Status
- Championship Readiness Index

---

## Championship Readiness Index (CRI)

The Championship Readiness Index is a custom metric developed for this project.

Formula:

```text
CRI =
((5 - LeaguePosition) × 20)
+
(Points × 2)
+
(NRR × 20)
```

Higher CRI values indicate stronger championship readiness.

---

## Generated Outputs

### Visualizations

```text
titles_by_position.png
runnerups_by_position.png
team_titles.png
champion_vs_nrr.png
champion_vs_points.png
correlation_matrix.png
top_cri_teams.png
```

### Exported Files

```text
cleaned_ipl_dataset.csv
ipl_research_output.csv
```

---

## Key Insights to Investigate

- Championship distribution by league position.
- Success rate of Top 2 teams.
- Impact of NRR on title-winning probability.
- Historical performance trends of IPL champions.
- Relationship between league-stage dominance and championship success.

---

## Future Enhancements

### Playoff Analysis

Add:

- Qualifier 1 Results
- Qualifier 2 Results
- Eliminator Results

### Team Factors

Add:

- Captain
- Coach
- Previous Titles
- Playoff Experience

### Advanced Metrics

Develop:

- Championship Probability Score
- Team Dominance Score
- Momentum Index

### Machine Learning Models

- Logistic Regression
- Random Forest
- XGBoost

### Dashboard Development

- Streamlit Dashboard
- Power BI Dashboard

---

## Expected Outcomes

The project aims to determine whether specific league-stage characteristics consistently predict IPL championship success and whether a custom Championship Readiness Index can be used as an indicator of title-winning potential.

---

## Author

Bhashyam Sree Darshan

---

## License

This project is intended for educational, analytical, and research purposes.
