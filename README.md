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

## Dependencies
The project requires the following Python libraries:
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn
- TensorFlow/Keras

You can install these dependencies using:
```bash
pip install -r requirements.txt
