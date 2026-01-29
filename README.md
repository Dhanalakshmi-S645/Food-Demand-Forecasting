<div align="center">
  <h1>🍲 Food Demand Forecasting</h1>
  <h3>Predicting Meal Orders for Upcoming Weeks</h3>

  <img src="https://images.unsplash.com/photo-1555939594-58056f625634?w=800&auto=format&fit=crop&q=80" alt="Food Delivery Illustration" width="680" style="border-radius: 16px; margin: 24px 0; box-shadow: 0 8px 32px rgba(0,0,0,0.15);">

  <p style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto;">
    End-to-end Machine Learning project to forecast number of orders for the next 10 weeks — helping fulfillment centers reduce food waste and optimize inventory.
  </p>

  <p>
    <strong>Author</strong> • Dhanalakshmi<br>
    <strong>Location</strong> • Bengaluru, Karnataka<br>
    <strong>Date</strong> • January 2026
  </p>

  <p>
    <a href="https://github.com/Dhanalakshmi-S645/Food-Demand-Forecasting/stargazers">
      <img src="https://img.shields.io/github/stars/Dhanalakshmi-S645/Food-Demand-Forecasting?style=social" alt="GitHub stars">
    </a>
    <a href="https://github.com/Dhanalakshmi-S645/Food-Demand-Forecasting">
      <img src="https://img.shields.io/github/forks/Dhanalakshmi-S645/Food-Demand-Forecasting?style=social" alt="GitHub forks">
    </a>
  </p>
</div>

<br>

## 🎯 Project Goal

Forecast **num_orders** for upcoming 10 weeks so fulfillment centers can plan raw materials, reduce waste (~15–20%), and improve operations — a real problem faced by food delivery platforms like Zomato & Swiggy.

**Evaluation Metric**: RMSLE (Root Mean Squared Log Error) — lower is better

**Best Model**: LightGBM (tuned with Optuna)  
**Validation RMSLE**: **0.4461** (very strong result)

<br>

## 📊 Key Results at a Glance

| Metric                  | Value       | Note                              |
|-------------------------|-------------|-----------------------------------|
| Best Validation RMSLE   | 0.4461      | After Optuna tuning (30 trials)   |
| Top Predicted Food      | Rice Bowl (Indian) | Dominates peak weeks 150–155     |
| Highest Single Prediction | ~5,381 orders | Week 154, TYPE_A center, with promotion |
| Main Demand Driver      | Promotions  | Active in ~90% of top predictions |
| Best Center Type        | TYPE_A      | Highest average predicted demand  |

<br>

## 🗂️ What's Inside This Repository

| File / Folder                              | Description                                                                 |
|--------------------------------------------|-----------------------------------------------------------------------------|
| `Food_Demand_Forecasting_Dhanalakshmi.ipynb` | Complete notebook: EDA → Feature Engineering → Modeling → Optuna Tuning → Submission |
| `submission_lightgbm_optuna_best.csv`       | Final Kaggle submission file (id + predicted num_orders)                    |
| `enriched_predictions_for_presentation.csv` | Predictions enriched with category, cuisine, center_type, city_code, etc.  |
| `weekly_demand_predictions_146_156.csv`     | Weekly breakdown (only upcoming weeks 146–156)                              |
| `README.md`                                 | This beautiful overview                                                     |

<br>

## 🚀 How to Run Locally

1. Clone the repo
   ```bash
   git clone https://github.com/Dhanalakshmi-S645/Food-Demand-Forecasting.git
   cd Food-Demand-Forecasting
