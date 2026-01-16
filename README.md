Credit Card Default Prediction
This project aims to predict the probability of a credit card client defaulting on their payment in the following month. It utilizes a dataset of 30,000 clients, incorporating various demographic and financial features to build a robust predictive model.

📊 Dataset Overview
The dataset contains 25 features, including:

ID: ID of each client.

LIMIT_BAL: Amount of given credit (includes individual and family/supplementary credit).

SEX: Gender (1 = male; 2 = female).

EDUCATION: Education level (1 = graduate school; 2 = university; 3 = high school; 4 = others).

MARRIAGE: Marital status (1 = married; 2 = single; 3 = others).

AGE: Age in years.

PAY_0 to PAY_6: History of past payments (September to April).

BILL_AMT1 to BILL_AMT6: Amount of bill statement (September to April).

PAY_AMT1 to PAY_AMT6: Amount of previous payment (September to April).

default payment next month: The target variable (1 = yes; 0 = no).

🛠️ Project Workflow
Data Loading & Exploration: Initial inspection of the data using pandas and seaborn.

Data Cleaning: Checking for missing values (none found in this dataset).

Feature Analysis: Examining data distribution, skewness, and kurtosis to understand feature characteristics.

Model Building: Implementing various machine learning algorithms to identify the most effective predictor.

Hyperparameter Tuning: Using RandomizedSearchCV to optimize model performance.

🚀 Best Performing Model
The GradientBoostingClassifier was identified as the most effective algorithm for this task.

Optimized Parameters:

learning_rate: 0.05

n_estimators: 200

min_samples_leaf: 4

subsample: 0.8

Final Accuracy: 0.822 (82.2%).

💻 Dependencies
To run this project, you will need the following libraries:

pandas

numpy

seaborn

scikit-learn

📂 File Structure
mini_project.ipynb: The main Jupyter Notebook containing all data analysis, visualization, and modeling code.

default_of_credit_card_clients.csv: The source dataset.
