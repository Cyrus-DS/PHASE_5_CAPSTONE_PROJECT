# 🌧️ AI-Powered Rainfall Prediction

Predicting rainfall using machine learning to support smarter decision-making in agriculture, infrastructure, and climate resilience.



## Project Overview

This project predicts whether it will rain using meteorological data such as:

* Temperature
* Humidity
* Wind speed
* Sunshine
* Cloud cover
* Air pressure

The system outputs the **probability of rainfall**, enabling data-driven planning and preparation.

This project began as a group capstone in my Data Science program. After completion, I independently refined and improved the model, strengthened the pipeline, and benchmarked its performance in a Kaggle competition.

🔗 **Kaggle Competition:**
[https://www.kaggle.com/competitions/playground-series-s5e3/submissions](https://www.kaggle.com/competitions/playground-series-s5e3/submissions)



## Business Relevance

Accurate rainfall prediction supports:

* 🌾 Agricultural irrigation planning
* 🏙️ Urban flood preparedness
* ⚡ Energy demand forecasting
* 🌍 Climate resilience initiatives

Rainfall forecasting is not just a weather problem — it directly impacts operational and economic decisions.



## Dataset

* Source: Kaggle Playground Series
* Training Data: 2,190 rows × 25 features
* Test Data: 1,464 rows
* Target Variable: `rainfall` (Binary: 0 = No Rain, 1 = Rain)

The model was trained on historical weather data and evaluated on unseen data to ensure generalization.



## Project Workflow

### 1️⃣ Data Cleaning & Exploration

* Checked for missing values and inconsistencies
* Analyzed class imbalance
* Explored feature distributions and correlations

### 2️⃣ Feature Engineering

* Temperature range (max − min)
* Cyclical date encoding (`sin` / `cos`)
* Interaction features
* Correlation filtering
* Mutual Information feature selection

### 3️⃣ Preprocessing Pipeline

* Outlier handling
* Feature scaling
* Categorical encoding
* Automated transformation pipeline
* Prevented data leakage

### 4️⃣ Model Development

Multiple models were tested, including:

* Logistic Regression
* Random Forest
* Gradient Boosting
* XGBoost
* LightGBM

The final selected model demonstrated the best balance between performance and generalization.



## 🏆 Kaggle Results

After refining the model independently, I submitted it to Kaggle and achieved:

*  **Public ROC-AUC:** 0.85974 *(live leaderboard ranking)*
*  **Private ROC-AUC:** 0.89368 *(final evaluation score)*

The higher private score indicates strong model generalization and robustness on unseen data.



## Model Performance (Validation)

* Accuracy ≈ 0.86
* ROC-AUC ≈ 0.88
* Strong recall on rainfall class
* Well-calibrated probability outputs



## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* LightGBM
* Joblib



## Reproducibility

The project includes:

* Saved preprocessing pipeline
* Saved trained model (`.joblib`)
* Submission-ready prediction workflow

The pipeline ensures consistent transformations between training and test data and is ready for deployment.



## Future Improvements

* Advanced ensemble stacking
* Time-series cross-validation
* Integration of satellite/geospatial data


## Conclusion

This project demonstrates:

* End-to-end machine learning development
* Feature engineering and model optimization
* Competition benchmarking
* Reproducible and deployment-ready pipelines

It reflects both technical rigor and practical application in solving real-world problems.

