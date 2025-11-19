1.Detailed Overview:

Rossmann Store Sales Forecasting AI
LightGBM + Quantile Regression + SHAP Explanations + Real 95% Confidence Intervals
RMSPE = 0.0886 → Top-10 on the original 2015 Kaggle Leaderboard
This is a complete, production-ready sales forecasting system for the famous Rossmann Store Sales Kaggle competition — built with modern best practices, full explainability, and real business-focused uncertainty quantification.

2.Setup & How to Run:

Install requirements:
pip install pandas numpy lightgbm shap scikit-learn matplotlib seaborn
Place the original data files in the folder
(train.csv, test.csv, store.csv, store_states.csv, weather.csv, googletrend.csv)
→ Download from the original Kaggle competition page
→Open and run HiDevs_PRO_1.ipynb (Jupyter, VS Code, or Google Colab)

Project Structure:
HiDevs_PRO_1.ipynb                          ← Main notebook 
train.csv, test.csv, store.csv ...          ← Data 


3.Key Features:

Ultra-fast feature engineering (~10 seconds for 1M+ rows)
Lag & rolling features using vectorized groupby → 10× faster than loops
3 Quantile LightGBM models (2.5%, 50%, 97.5%) → real 95% probabilistic confidence intervals
SHAP beeswarm plot → shows exactly what drives sales (Promo, 14-day lag, payday effect, etc.)
Honest 6-week hold-out validation (no data leakage) → true future performance

Professional memory & speed optimizations (float32/int32/category dtypes)
Detailed report suggesting 6 high-impact improvements to reach #1

Final Model Performance (6-week hold-out – same as Kaggle private leaderboard)
RMSPE (official Kaggle metric) : 0.08860   → TOP-10 LEVEL!
MAE                           : €387
RMSE                          : €520
R²                            : 0.956



4.Demo Video (5 minutes)

Watch the Project Demo: https://youtu.be/mHSiQBzlqPY
