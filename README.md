# Soccer Player Market Value Prediction

## Project Structure

- Soccer-Market-Value/
  - data/
    - predicting-the-market-value-of-soccer-players.zip
    - soccer_player.csv
  - notebooks/
    - Predicted_Soccer_Market_Values.ipynb
  - plots/
    - gradient_descent_convergence.png
    - actual_vs_predicted+Messi2012andRonaldo2017.png
  - scripts/
    - create_summary.ipynb
  - summary/
    - Messi&Ronaldo_market_value_analysis.md
    - project_overview.md
  - requirements.txt
  - README.md

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

> `passes_blocked` was excluded due to missing data for some players.

---

## Installation


```bash
# Create a virtual environment
python3 -m venv venv

# Activate the virtual environment
source venv/bin/activate  # Mac/Linux
# venv\Scripts\activate   # Windows

# Install required packages
pip install -r requirements.txt
```
## Usage
1. Open the notebook to view predictions and plots:
   notebooks/Predicted_Soccer_Market_Values.ipynb
2. Run the script to generate markdown summaries:
   scripts/create_summary.ipynb → outputs to summary/.
3. Visualizations are saved in the plots/ folder.

## Evaluation Metrics
The model is evaluated using the following metrics:
* R² Score – explains how well the variance in market value is captured.
* Mean Absolute Error (MAE) – average absolute difference between predicted and actual values.
* Root Mean Squared Error (RMSE) – penalizes larger errors.
* Mean Absolute Percentage Error (MAPE) – percentage-based error for relative accuracy.
Metrics are calculated in the notebook using the gradient descent implementation.

