# Master-s_Thesis_Apartment_Price_Prediction_Poland

## Overview

This repository contains the code and the dataset for my Master's thesis titled 'Multi-City Polish Property Price Prediction using Location Features', submitted as part of the Data Science and Society Program at Tilburg University, under the supervision of prof. dr. Afra Alishahi.

**Abstract:**  
This thesis presents a machine learning approach to apartment price prediction in Poland, comparing two ensemble learning methods—Random Forest Regressor and eXtreme Gradient Boosting—and one neural network model, a Multilayer Perceptron. The study investigates the accuracy of these models in predicting prices based on property characteristics and location features (including the 15 largest cities, latitude, longitude, and points of interest). The model performance was measured using $R^2$, MAE, and RMSE. To test the generalizability of the best model, a multi-city disperate-group analysis was conducted. Lastly, a SHapley Additive exPlanations analysis was used to analyze feature importance. Results show that Random Forest outperforms the other two models across all metrics, though eXtreme Gradient Boosting performs only slightly worse. Both models perform well across all 15 cities, with slight differences in which model scored best for each city. The most important features are the size of the property, longitude, and city. The findings of this study show that ensemble learning models, namely the Random Forest Regressor and eXtreme Gradient Boosting, perform best for this regression task on the Polish market; however, due to time constraints, future research should aim to improve the Multilayer Perceptron model through more thorough hyperparameter tuning. Regarding the features, location plays an important role in price prediction, however, the core property characteristics remain highly relevant.

## Repository Structure (Files)

```bash
├── apartment_price_prediction_kaminska.ipynb/             # The main notebook with all code
├── kaggle_dataset.csv/              # Dataset taken from https://www.kaggle.com/datasets/krzysztofjamroz/apartment-prices-in-poland
├── final_dataset.csv/        # Final (cleaned) dataset
├── bayesian_optimization_results.csv/          # Results from the Bayesian Optimization of the Multilayer Perceptron
├── output_bayesian_optimization.txt        # Output from the Bayesian Optimization of the Multilayer Perceptron
├── output_best_mlp.txt  # Output from the best Multilayer Perceptron trained + evaluation metrics
├── shap_analysis_output.txt  # Output from the Shap analysis
├── shap_values_subset.pkl  # Shap results stored in a pickle
├── shap_summary_bar_labeled.png  # Shap analysis visualization in a bar plot
├── shap_summary_beeswarm_labeled.png  # Shap analysis visualization in a beeswarm plot
└── README.md         # This file
