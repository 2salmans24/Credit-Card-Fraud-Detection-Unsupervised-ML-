# Credit Card Fraud Detection - Unsupervised ML Project

## Project Overview
This project explores the use of unsupervised learning techniques for detecting fraudulent credit card transactions. Initially, models like Isolation Forest and DBSCAN were implemented, but through feature engineering and model tuning, an autoencoder was found to perform significantly better.

The autoencoder was trained and optimized to achieve a high recall rate for fraudulent transactions, making it a suitable solution for real-world fraud detection problems.

## Key Results
- **Best Model**: Autoencoder
- **ROC AUC Score**: 0.874
- **Recall**: 80% of fraudulent transactions detected
- **Precision**: 3%

## Project Structure
- `Credit Card Fraud Detection-Unsupervised Learning Project.ipynb`: Jupyter notebook containing all the analysis, model implementation, and evaluation.
- `data/`: Not included due to size limitations.
- `images/`: Visuals and plots are all included in the notebook.
- `isolation_forest_model.pkl`: Saved Isolation Forest model for conceptual deployment (optional).

## How to Get the Dataset
The dataset used in this project is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), which contains anonymized credit card transactions made by European cardholders in September 2013. It is available for download on Kaggle.

### Steps to Download the Dataset:
1. Go to the [Kaggle Dataset Page](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
2. Click "Download" and extract the dataset to your local machine.
3. Place the dataset file (`creditcard.csv`) in the root directory or a `data/` folder in the repository.
4. Run the notebook after placing the dataset in the correct folder.

Make sure the dataset is named `creditcard.csv` for seamless loading in the notebook.

### Example: How to Load the Dataset in Your Notebook
```python 
import os
import pandas as pd

# Load the dataset from the data folder or the root directory
dataset_path = 'data/creditcard.csv' if os.path.exists('data/creditcard.csv') else 'creditcard.csv'
df = pd.read_csv(dataset_path)
