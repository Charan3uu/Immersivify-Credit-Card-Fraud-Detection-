# Immersivify-Credit-Card-Fraud-Detection-

## Overview  
This project focuses on detecting fraudulent credit card transactions using machine learning. Fraud detection is crucial for financial institutions to prevent unauthorized access and monetary loss.

## Dataset  
The dataset includes anonymized credit card transactions with the following key features:  
- **Time**: Seconds elapsed between this transaction and the first transaction in the dataset.  
- **V1, V2, ..., V28**: PCA-transformed features for confidentiality.  
- **Amount**: Transaction amount.  
- **Class**: Target variable (1 for fraudulent transactions, 0 for legitimate transactions).  

The dataset file is named `fraudTest.csv`.

## Workflow

### 1. Data Exploration and Visualization:
- Analyze the data distribution.
- Visualize the class imbalance.

### 2. Data Preprocessing:
- Handle class imbalance using techniques like oversampling (SMOTE).
- Scale the Amount feature using `StandardScaler`.
- Split the data into training and testing sets.

### 3. Model Building:
- Use **Random Forest Classifier** for predictive modeling.
- Perform **GridSearchCV** to tune hyperparameters.
- Train the model on sparse matrices to handle memory constraints.

### 4. Evaluation:
- Assess model performance using precision, recall, F1-score, and a confusion matrix.
- Visualize metrics to understand the model’s performance.

## Installation  
Install the required Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib imbalanced-learn
```

## Usage

### Clone the repository:

```bash
git clone https://github.com/Charan3uu/Immersivify-Credit-Card-Fraud-Detection-
```

### Run the Python script:

```bash
python FRAUD-DETECTION.py
```

## Results

- **Model Performance**: The model achieved high accuracy and precision on test data, minimizing false positives and false negatives.
- **Insights**: Class imbalance addressed through SMOTE significantly improved recall for fraudulent transactions.

## Files

- `FRAUD-DETECTION.py`: Main script for data preprocessing, modeling, and evaluation.
- `fraudTest.csv`: Dataset file. (The dataset was too big to upload. So, I did'nt)
- `README.md`: Documentation for the project.
- `random_forest_fraud_detection.pkl.gz`: Trained model file.

## Visualization

Key visualizations include:
- Distribution of legitimate vs. fraudulent transactions.
- Precision-recall curves and confusion matrix.

## Contributing  
Contributions are welcome. Fork the repository and submit pull requests for improvements or suggestions.

## Acknowledgments  
Thanks to the open-source datasets and the machine learning community for resources and inspiration.
