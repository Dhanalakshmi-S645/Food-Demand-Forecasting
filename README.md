# Food Demand Forecasting Project

Predicting meal orders for upcoming weeks using machine learning.

**Author**: Dhanalakshmi  
**Date**: January 2026  


## Project Goal
Forecast number of orders (num_orders) for 10 upcoming weeks to help fulfillment centers plan inventory and reduce food waste.

## Key Results
- Best model: LightGBM (Optuna tuned)
- Validation RMSLE: 0.4461
- Top predicted food: Rice Bowl (Indian) in TYPE_A centers
- Promotions strongly increase demand

## Files
- Food_Demand_Forecasting_Dhanalakshmi.ipynb → full notebook with EDA, modeling & tuning
- submission_lightgbm_optuna_best.csv → Kaggle submission file
- enriched_predictions_for_presentation.csv → predictions with category, cuisine, center details
- weekly_demand_predictions_146_156.csv → weekly breakdown (weeks 146–156)

## How to run
1. Install requirements: `pip install pandas numpy matplotlib seaborn lightgbm xgboost optuna`
2. Update file paths in notebook if needed
3. Run all cells

Made with ❤️ in Jupyter Notebook