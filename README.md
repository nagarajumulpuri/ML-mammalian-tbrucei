# Project Title: Machine Learning-Driven Discovery of Selective Inhibitors Against Trypanosoma brucei Calcium Channels

## Project Background and Motivation
Trypanosoma brucei is a parasitic protozoan responsible for Nagana in cattle and human African trypanosomiasis (sleeping sickness) in humans. Existing treatments are limited by drug toxicity, the absence of an effective vaccine, and the emergence of drug resistance, highlighting the need for novel therapeutic targets. Voltage-gated calcium channels (VGCCs), which play important roles in cellular functions, represent an underexplored therapeutic target in parasitic organisms.

## Research Objectives
This project aims to develop machine learning models to identify compounds that selectively bind to the voltage-gated calcium channel of T. brucei. By comparing predicted binding affinities against the parasite and human calcium channels, we aim to identify selective inhibitors with reduced potential for off-target effects and host toxicity.

## Methodology
Data Collection: Compile compound structures and corresponding binding affinity data for parasite and human calcium channels. <br>
Data Preprocessing: Perform data cleaning, molecular standardization, and feature preparation. <br>
Feature Engineering: Generate molecular descriptors and molecular fingerprints using RDKit. <br>
Machine Learning: Develop and optimize models, including Random Forest, XGBoost, Support Vector Regression (SVR), CatBoost, and LightGBM. <br> 
Model Evaluation: Evaluate predictive performance using appropriate metrics, including ROC-AUC, PR-AUC, RMSE, MAE, and R², depending on the prediction task. <br>
Selectivity Prediction: Compare predicted binding affinities against parasite and human calcium channels to prioritize parasite-selective compounds. <br>
Future Validation: Apply molecular docking and molecular dynamics simulations to investigate prioritized compounds and their interactions with the target channels. <br>

## Repository Structure
### Random-Split-ML-All-Features
This folder contains machine learning models developed using a random train-test splitting strategy, in which the dataset is randomly divided into training and test sets. <br>
It includes three subfolders based on the input data used: <br>
tbrucei-only-data: Models trained and evaluated using only T. brucei data. <br>
mammalian-only-data: Models trained and evaluated using only mammalian calcium channel data. <br>
mammalian-tbrucei-data: Models trained and evaluated using combined mammalian and T. brucei data. <br>
All data preprocessing, feature engineering, model development, hyperparameter optimization, and evaluation procedures follow the methodology described in the Methodology section. <br>

### Scaffold-Split-ML-All-Features
This folder contains machine learning models developed using a scaffold-based train-test splitting strategy, in which compounds are divided based on their molecular scaffolds. This approach helps evaluate model generalizability to structurally distinct compounds and reduces the risk of overly optimistic performance estimates due to structural similarity between training and test sets. <br>

It includes three subfolders based on the input data used: <br>
tbrucei-only-data: Models trained and evaluated using only T. brucei data. <br>
mammalian-only-data: Models trained and evaluated using only mammalian calcium channel data. <br>
mammalian-tbrucei-data: Models trained and evaluated using combined mammalian and T. brucei data. <br>
All data preprocessing, feature engineering, model development, hyperparameter optimization, and evaluation procedures follow the methodology described in the Methodology section. <br>
