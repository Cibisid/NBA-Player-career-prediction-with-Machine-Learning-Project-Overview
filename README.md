🏀 NBA Player Career Prediction with Machine Learning
This project uses machine learning techniques to classify NBA players based on various performance metrics. Multiple algorithms were evaluated to determine the best model for predicting player success.

📊 Project Overview
The pipeline includes:

Data preprocessing (handling missing values, feature scaling)

Model training using:

K-Nearest Neighbors (KNN)

Random Forest

Logistic Regression

Artificial Neural Networks (ANN)

Model evaluation using 10-fold cross-validation and F1-score

Grid Search for hyperparameter tuning

🗂 Dataset
File: nba.csv

Format: CSV

Description: Contains various numerical statistics about NBA players

Target Column: TAR (converted to binary for classification)

Missing Values: Imputed using mean strategy

🛠 Installation and Dependencies
Ensure you have the following Python libraries installed:

pip install pandas numpy scikit-learn matplotlib
🔄 Data Preprocessing
Steps:

Loaded the dataset and checked for missing values

Dropped non-numeric columns (e.g., player names)

Converted TAR target variable to binary

Imputed missing values using mean imputation

Standardized numeric features for consistent model performance

🤖 Model Training & Evaluation
1. K-Nearest Neighbors (KNN)
n_neighbors = 5

Evaluated using 10-fold cross-validation and test dataset

2. Random Forest
n_estimators = 100 (optimized to 200 later)

Evaluated via cross-validation and tested separately

3. Logistic Regression
Explored penalties: None, l1, l2, elasticnet

Selected the best based on F1-score

4. Artificial Neural Network (ANN)
Architecture: hidden_layer_sizes=(64, 32)

Optimizer: adam

Early stopping: True

🔧 Hyperparameter Tuning
Random Forest: Grid search used to optimize n_estimators

Best Result: n_estimators = 200

📈 Model Comparison
A bar chart visualizes the F1-scores across different models

Best Model: Logistic Regression (l2)

F1-Score: 0.8056

▶️ How to Run
Upload the nba.csv file to your Google Colab environment.

Copy/paste the code from the notebook into Colab cells.

Run all cells:
Runtime > Run all

✅ Expected Output
Printed F1 scores for all models

Bar chart comparing model performance

📝 Notes
Ensure nba.csv is correctly formatted and uploaded.

Modify file paths in code if needed.

random_state = 42 is used for reproducibility.

👤 Author
Cibi Siddarth
University of North Florida
School of Computing
