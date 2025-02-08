# Expected Goals (xG) Model Training Using Opta Event Data

## Overview  
Expected Goals (xG) is a statistical metric used in football (soccer) to estimate the probability of a shot resulting in a goal. It is based on various factors such as shot location, angle, assist type, and defensive pressure. Higher xG values indicate higher chances of scoring.

This project trains an Expected Goals (xG) model using Opta event data with five different machine learning approaches.

## Models Used  
1. **Logistic Regression** (with Binary Cross-Entropy loss)  
2. **Logistic Regression** (Pytorch Binary Cross-Entropy loss) 
3. **XGBoost**  
4. **Random Forest**  
5. **Neural Network**  

## Requirements  
- Python (>=3.8)  
- Libraries:  
  - `pandas`  
  - `numpy`  
  - `matplotlib`
  - `scikit-learn`  
  - `xgboost`  
  - `torch`  
  - `pytorch`
  - `mplsoccer`

## Results & Conclusion  
While the models demonstrate reasonable predictive performance, the results indicate that they are **not suitable for real-world use**. When comparing the predicted xG values to established models (e.g., Understat), the predictions show significant differences, highlighting the challenges of accurately modeling xG using event data alone. Mainly our models flaws lie in unavalibility of xG value in training data. 
