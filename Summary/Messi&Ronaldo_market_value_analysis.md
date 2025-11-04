
# Soccer Player Market Value Analysis

This document analyzes predicted vs. actual market values for top soccer players across different seasons using a linear regression model with performance-based features.

---

## Features Used in the Model

- xG Per Avg Match  
- Shots  
- OnTarget  
- Shots Per Avg Match  
- On Target Per Avg Match  
- goals  
- goals_per_shot  
- assists  
- passes_completed  
- assisted_shots  
- touches  
- height  
- games_starts  
- minutes  

> **Note:** `passes_blocked` was not included due to missing data for some players.

---

## 1. Messi

### Prime Season: 2011-2012

| Feature | Value |
|---------|-------|
| xG Per Avg Match | 1.35 |
| Shots | 278 |
| OnTarget | 135 |
| Shots Per Avg Match | 4.63 |
| On Target Per Avg Match | 2.25 |
| goals | 73 |
| goals_per_shot | 0.263 |
| assists | 30 |
| passes_completed | 3700 |
| assisted_shots | 125 |
| touches | 2008 |
| height | 170 |
| games_starts | 37 |
| minutes | 3269 |

- **Actual Market Value:** 150-200 Million Euros  
- **Predicted Market Value:** 258.57 Million Euros  
- **Observation:** This was Messi's peak season. The model should reflect a very high market value due to exceptional goal-scoring and assists.

### 2019-2020 Season

| Feature | Value |
|---------|-------|
| xG Per Avg Match | 0.63 |
| Shots | 39 |
| OnTarget | 19 |
| Shots Per Avg Match | 4.5 |
| On Target Per Avg Match | 2.19 |
| goals | 25 |
| goals_per_shot | 0.13 |
| assists | 21 |
| passes_completed | 1700 |
| assisted_shots | 86 |
| touches | 2614 |
| height | 170 |
| games_starts | 32 |
| minutes | 2880 |

- **Actual Market Value:** 112 Million Euros  
- **Predicted Market Value:** 106.10 Million Euros  
- **Observation:** The model may underestimate Messi's value due to missing context-based features, e.g., influence in key matches.

---

## 2. Ronaldo

### Prime Season: 2017-2018

| Feature | Value |
|---------|-------|
| xG Per Avg Match | 0.7 |
| Shots | 260 |
| OnTarget | 111 |
| Shots Per Avg Match | 4.81 |
| On Target Per Avg Match | 2.06 |
| goals | 44 |
| goals_per_shot | 0.169 |
| assists | 8 |
| passes_completed | 1210 |
| assisted_shots | 53 |
| touches | 1174 |
| height | 188 |
| games_starts | 44 |
| minutes | 3670 |

- **Actual Market Value:** ~135 Million Euros  
- **Predicted Market Value:** 220.62 Million Euros  
- **Observation:** Ronaldo's prime season shows high goal-scoring efficiency; model predictions should reflect his market value peak.

### 2019-2020 Season

| Feature | Value |
|---------|-------|
| xG Per Avg Match | 1.27 |
| Shots | 26 |
| OnTarget | 13 |
| Shots Per Avg Match | 6.22 |
| On Target Per Avg Match | 3.11 |
| goals | 31 |
| goals_per_shot | 0.1 |
| assists | 5 |
| passes_completed | 1086 |
| assisted_shots | 50 |
| touches | 1761 |
| height | 187 |
| games_starts | 33 |
| minutes | 2917 |

- **Actual Market Value:** 60 Million Euros  
- **Predicted Market Value:** 69.69 Million Euros  
- **Observation:** The model slightly overestimates Ronaldo's market value — despite strong goal stats, his lower assists, reduced passing volume, and age likely caused his real-world market value to drop.

---

## 3. Analysis Observations

- Players’ **prime seasons** generally result in higher predicted market value due to better stats (goals, assists, xG, etc.).  
- Model may **underestimate value in shorter or injury-affected seasons** (e.g., 2019-2020 for Messi or Ronaldo).  
- Adding features like **team influence, competition level, or key match performance** could improve prediction accuracy.
