
# Soccer Player Market Value Prediction – Project Summary

This project explores predicting soccer players’ market values using performance statistics from various seasons. The main goal is to understand how measurable on-field performance can explain or estimate a player’s monetary value in the transfer market.

---

## 1. Objective

- Predict the market value of top soccer players based on key performance metrics.  
- Compare predicted values to actual market values to identify patterns and discrepancies.  
- Analyze the effect of prime seasons versus less productive seasons on market valuation.

---

## 2. Data

- Player data sourced from `soccer_player.csv`.  
- Seasons analyzed include Messi 2011-2012, Messi 2019-2020, Ronaldo 2017-2018, Ronaldo 2019-2020, Lewandowski 2019-2020, and Harry Kane 2019-2020.  
- Features used in the model:
  - xG Per Avg Match  
  - Shots, OnTarget  
  - Shots Per Avg Match, On Target Per Avg Match  
  - Goals, Goals per Shot, Assists  
  - Passes Completed, Assisted Shots, Touches  
  - Height, Games Started, Minutes Played  

> **Note:** `passes_blocked` was not included due to missing data for several players.

---

## 3. Methodology

- A **linear regression model** was implemented using gradient descent from scratch.  
- Players’ feature vectors were normalized using mean and standard deviation from the dataset.  
- Predictions were computed and compared against actual market values.

---

## 4. Key Observations

- **Prime seasons** result in higher predicted market values due to strong statistics (e.g., Messi 2011-2012, Ronaldo 2017-2018).  
- The model tends to **overestimate market values** when a player has exceptional goal-scoring efficiency but lower context-based metrics like assists or passes.  
- The model tends to **underestimate market values** for shorter seasons or injury-affected seasons (e.g., Harry Kane 2019-2020).  
- Metrics like R², MAE, RMSE, and MAPE indicate moderate predictive performance, which is reasonable given the linear nature of the model and limited features.

---

## 5. Limitations & Future Work

- Only linear regression was used; other models (e.g., random forest, XGBoost, or neural networks) may capture non-linear relationships better.  
- Important contextual features like team influence, competition level, and key match performance are missing.  
- Expanding the dataset to include more seasons and players could improve model accuracy.  
- Visualization of predictions vs. actual values helps identify over- and under-estimations clearly.

---

## 6. Deliverables

- **Plots** comparing predicted vs. actual market values for top players.  
- **Markdown reports** summarizing predictions, observations, and analysis.  
- **Evaluation metrics** to quantify model performance.  

---

## 7. Model Evaluation Metrics

The following metrics were calculated on the dataset:

- **R² Score:** 0.438  
- **Mean Absolute Error (MAE):** 15,841,811.81 Euros  
- **Root Mean Squared Error (RMSE):** 21,637,107.99 Euros  
- **Mean Absolute Percentage Error (MAPE):** 336.31%  

> **Observation:** The linear model captures some trends but struggles with extreme values (e.g., prime seasons), explaining why high-performing players like Messi 2011-2012 have predicted values far above actual market value.


This project provides a foundation for understanding how performance metrics translate into market value and serves as a stepping stone for more advanced player valuation models.
