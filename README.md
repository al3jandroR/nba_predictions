# NBA Game Prediction Model

This project is a machine learning powered NBA game prediction system designed to simulate real-world sports betting models, with a focus on data-driven feature engineering and real-time data integration.

## Overview

The goal of this project is to accurately predict the winner of NBA games using recent team performance, advanced statistical features, and real-time injury data scraping.

This system was built from the ground up with an emphasis on:

- Real-world feature engineering
- API data extraction and cleaning
- Model evaluation best practices
- Sports analytics concepts used in betting models
- Clean daily prediction outputs for future expansion into dashboards or automation

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python (Pandas, Scikit-Learn) | Data analysis, machine learning models |
| nba_api | Pull official NBA game, team, and player data |
| ESPN Web Scraping (Pandas) | Auto-fetch injury reports for daily matchups |
| Random Forest Classifier | Initial baseline model for classification |
| GridSearchCV | Hyperparameter tuning for best model parameters |
| Walk-Forward Validation | Accurate model testing across seasons |

---

## Features Used in Prediction

| Feature | Description |
|---------|-------------|
| Rolling 5-Game Averages | Team offensive/defensive stats over last 5 games |
| Streak Score | Current win streak over last N games |
| Efficiency Score | FG% combined with PTS for offensive strength |
| Defense Score | DREB + STL + BLK metrics |
| AST/TOV Ratio | Playmaking efficiency |
| Back-to-Back Games | Determines if a team is on short rest |
| Days Rest | Time between games for a team |
| Home/Away Indicator | Captures home-court advantage |
| Net Metrics | Compares team vs opponent directly (Net Efficiency, Net Form Score) |
| Injury Impact | Auto-scraped injuries per team added contextually to output |

---

## Model Performance

| Split | Accuracy |
|-------|----------|
| Training Accuracy | ~81% |
| Testing Accuracy | ~80% |
| Daily Predictions | Model has successfully performed well against the Vegas lines on multiple test days so far |

---

## Example Daily Output

| Matchup   | Predicted Winner | Home Injuries | Away Injuries |
|-----------|------------------|---------------|----------------|
| BOS @ ORL | ORL              | Kristaps Porzingis (Q), Jrue Holiday (Out) | None |
| LAL @ DAL | LAL              | LeBron James (Q), Austin Reaves (Out) | None |

---

## Future Plans / Improvements

- Auto-scrape player injuries & expected minutes missed for predictions
- Expand feature set with individual player metrics and pace factors
- Add opponent matchup-specific stats
- Deploy predictions API for front-end use

---

## Why This Project?

Sports analytics is a growing industry and this project is designed to simulate the real-world challenges of working with dynamic data environments.

This project demonstrates skills in:
- Machine learning modeling
- API consumption & data engineering
- Real-time data scraping
- Feature engineering
- Model validation strategies beyond random train/test splits

---

## How To Run

1. Clone Repository  
2. Run `nba_predictions.ipynb` for daily predictions  

---
