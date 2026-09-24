# Molecular Solubility Prediction Using Machine Learning and Cheminformatics

## Overview

This project predicts the aqueous solubility of drug-like molecules using machine learning and cheminformatics.

Molecular structures are represented using SMILES strings, and RDKit is used to calculate simple molecular descriptors. Two regression models were trained and compared:

- Linear Regression
- Random Forest Regressor

The project demonstrates how molecular properties can be used to estimate aqueous solubility in a simple and beginner-friendly machine-learning workflow.

---

## Objective

The main objective of this project is to predict the aqueous solubility of molecules using molecular descriptors and regression models.

The project also compares the performance of Linear Regression and Random Forest.

---

## Dataset

The Delaney ESOL dataset was used for this project.

The dataset contains:

- 1128 molecules
- SMILES representations
- Measured log solubility values

After checking the dataset:

- Missing SMILES values: 0
- Missing solubility values: 0
- Invalid molecules: 0
- Final molecules used: 1128

---

## Molecular Descriptors

The following molecular descriptors were calculated using RDKit:

- Molecular Weight
- LogP
- Topological Polar Surface Area
- Hydrogen-Bond Donors
- Hydrogen-Bond Acceptors
- Rotatable Bonds
- Ring Count

These descriptors were used as input features for the machine-learning models.

---

## Machine-Learning Models

Two regression models were used:

### Linear Regression

Linear Regression was used as a simple baseline model.

### Random Forest Regressor

Random Forest was used as a non-linear regression model to compare performance with Linear Regression.

---

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error
- Root Mean Squared Error
- R² Score

The Linear Regression model achieved:

- MAE: 0.8115
- RMSE: 1.0693
- R² Score: 0.7581

The Random Forest model was also evaluated using the same metrics.

---

## Visualizations

The project includes:

- Actual vs Predicted Solubility plot
- Random Forest Feature Importance plot

These visualizations help show model performance and the relative importance of molecular descriptors.

---

## Workflow

Dataset Loading  
↓  
Data Checking and Cleaning  
↓  
SMILES Conversion using RDKit  
↓  
Molecular Descriptor Calculation  
↓  
Train/Test Split  
↓  
Linear Regression  
↓  
Random Forest Regression  
↓  
Model Evaluation  
↓  
Result Comparison  
↓  
Visualization  

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- RDKit
- scikit-learn
- Matplotlib
- Google Colab

---

## Files in This Repository

- `Molecular_Solubility_Prediction.ipynb`
- `solubility_model_results.csv`
- `README.md`

---

## Key Skills Demonstrated

This project demonstrates basic practical experience with:

- Cheminformatics
- SMILES handling
- RDKit
- Molecular descriptor calculation
- Data preprocessing
- Regression analysis
- Linear Regression
- Random Forest
- Model evaluation
- Scientific visualization

---

## Conclusion

In this project, aqueous solubility was predicted using molecular descriptors and two machine-learning models: Linear Regression and Random Forest.

The results show that simple molecular properties can be useful for estimating solubility.

This project demonstrates a simple application of cheminformatics and machine learning in molecular property prediction.

---

## Limitations

- The dataset is relatively small.
- Only a limited number of molecular descriptors were used.
- Solubility can be influenced by experimental conditions that are not represented in the model.
- Model predictions should not be treated as experimental measurements.

---

## Future Improvements

Possible future improvements include:

- Testing additional regression models
- Using molecular fingerprints
- Adding more molecular descriptors
- Hyperparameter tuning
- Using scaffold-based train/test splitting
- External validation with another dataset

---

## Purpose

This project was developed as a beginner-to-intermediate cheminformatics and machine-learning portfolio project.

It demonstrates how molecular descriptors can be combined with simple regression models to predict an important drug-related molecular property.

---

## Disclaimer

This project is intended for educational and research-training purposes only.

The predicted solubility values should not be considered experimental or clinical evidence.
