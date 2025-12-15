# Network Traffic Based Intrusion Detection
This project started as an attempt to understand how machine learning models can be used to analyze network traffic for intrusion detection.
Instead of focusing on a single algorithm, multiple classical models were compared to observe the impact of feature selection and model choice.

## Dataset
The project uses a publicly available network traffic dataset obtained from Kaggle, containing labeled connection-level features for normal and attack traffic.

## What I did
- Cleaned and encoded network traffic features
- Removed redundant attributes from the dataset
- Used Recursive Feature Elimination (RFE) to select relevant features
- Trained and evaluated several ML models
- Combined selected models using a voting-based ensemble

## Models Used
Random Forest  
Decision Tree  
Gradient Boosting  
XGBoost  
CatBoost  
Support Vector Machine (RBF)  

## How evaluation was done
The data was split into training and test sets. Models were evaluated on a held-out test set to check for overfitting and consistency, and an ensemble was used to improve stability.

## Results
The ensemble model performed consistently better than individual models on the test set,
suggesting that combining different approaches can improve stability.

## Tools
Python, NumPy, Pandas, scikit-learn, XGBoost, CatBoost, Matplotlib, Seaborn

## How to run
This project was developed and tested using Google Colab.
To run it locally, a Python virtual environment is recommended.

Create and activate a virtual environment:
```
python3 -m venv venv
source venv/bin/activate
```
Install dependencies:
```
pip install -r requirements.txt
```
Run the notebook or script to reproduce the workflow.
