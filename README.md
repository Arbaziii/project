# project
Crop Yield Prediction Using Machine Learning
This project explores the use of machine learning models to predict crop yield based on environmental factors such as pesticide usage, temperature, and rainfall. The primary objective is to understand how these variables interact to influence agricultural productivity and develop accurate predictive models for crop yield forecasting.

Project Overview
The project uses historical crop yield data and environmental factors to train and evaluate multiple machine learning models. The models used include:

Linear Regression

Random Forest Regressor

Gradient Boosting Regressor

Stacking Regressor (combining predictions from multiple models)

Key Steps
Data Preprocessing:

Handling missing values using mean imputation.

Scaling features using StandardScaler to ensure consistency in input data.

Creating interaction terms (e.g., between pesticide usage and temperature) to capture non-linear relationships.

Adding a temporal trend feature to account for changes over time (e.g., year_diff).

Model Training and Tuning:

Models are trained and fine-tuned using GridSearchCV for Random Forest and Gradient Boosting models to optimize hyperparameters such as the number of estimators, maximum depth, and learning rate.

Model Stacking:

A Stacking Regressor is used to combine predictions from multiple models (Linear Regression, Random Forest, and Gradient Boosting) to improve performance.

Model Evaluation:

Performance metrics used to evaluate models include Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² (Coefficient of Determination).

Visualization:

Visualizations include heatmaps of missing values, scatter plots comparing actual vs. predicted crop yields, and residuals plots to assess model performance.

Feature importance is evaluated to understand the key variables influencing crop yield predictions.

Results
The Random Forest Regressor model showed the best performance, with an R² of 0.85, indicating its strong ability to explain the variance in crop yield.

Gradient Boosting Regressor performed well with an R² of 0.82, though it was slightly less effective for extreme crop yield cases.

Linear Regression, while offering high accuracy, had a lower R² of 0.60, indicating it was less effective in capturing complex relationships in the data.

Requirements
To run this project, you will need the following libraries:

pandas

numpy

seaborn

matplotlib

scikit-learn

google.colab (for file upload in this notebook)

How to Run the Code
Upload your dataset: The code expects a CSV file with crop yield and environmental data. You can upload the dataset using the file upload option in Google Colab.

Preprocessing: The data is preprocessed by handling missing values, scaling the features, and creating interaction terms and time-based trend features.

Model Training and Tuning: Models are trained using Random Forest and Gradient Boosting, with hyperparameter tuning performed via GridSearchCV.

Evaluation: The models' performance is evaluated using various metrics, and visualizations are generated to assess prediction accuracy.

Results and Future Work
This study shows that machine learning can provide valuable insights into crop yield prediction, with environmental factors like pesticide usage and temperature being crucial for forecasting. Future work could explore incorporating additional features such as soil health, irrigation patterns, and other external factors to further improve prediction accuracy.
