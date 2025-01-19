# Credit Card Fraud Detection with Sampling Techniques and Model Evaluation


## Project Highlights

- Data Balancing: Used SMOTE to handle class imbalance in the dataset.

- Sampling Techniques: Evaluated different sampling techniques, including random sampling and systematic sampling.

- Machine Learning Models: Evaluated models such as Logistic Regression, Decision Tree, Random Forest, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN).

- Performance Evaluation: Compared the accuracy of models for different sampling techniques and identified the best combination.


## Dataset

The dataset used is a credit card fraud dataset, with features representing various transactions and a binary target variable (Class) indicating whether a transaction is fraudulent (1) or not (0).

### Preprocessing

- Features (X): All columns except Class.

- Target (y): The Class column.


## Approach

1. Data Balancing

The dataset is highly imbalanced, so we use SMOTE to generate synthetic samples for the minority class, ensuring a balanced dataset for training.

2. Sampling Techniques

We use five different sampling techniques to create sample datasets from the SMOTE-resampled data:

Sampling1: Random sampling with a fixed random seed.

Sampling2: Random sampling with a different seed.

Sampling3: Systematic sampling (every nth record).

Sampling4: Random sampling with another fixed seed.

Sampling5: Random sampling with yet another seed.

The sample size is calculated using the confidence interval formula with a 95% confidence level and a 5% margin of error.

3. Machine Learning Models

The following machine learning models are trained and evaluated:

- Logistic Regression

- Decision Tree Classifier

- Random Forest Classifier

- Support Vector Machine (SVM)

- K-Nearest Neighbors (KNN)

4. Performance Evaluation

Each model is evaluated on the sampled datasets using accuracy as the performance metric. Results are presented in a matrix format and saved to a CSV file.


## Results

- Accuracy Matrix: A table showing the accuracy of each model for each sampling technique.

- Best Sampling Technique for Each Model: Identifies the sampling technique that gives the best accuracy for each model.

Results are saved in sampling_results.csv for further analysis.


