# Project Title: Machine Learning-Driven Discovery of Selective Inhibitors Against Trypanosoma brucei Calcium Channels

# Project Background and Motivation
Trypanosoma brucei is a parasitic protozoan responsible for Nagana in cattle and human African trypanosomiasis (sleeping sickness) in humans. Existing treatments are limited by drug toxicity, the absence of an effective vaccine, and the emergence of drug resistance, highlighting the need for novel therapeutic targets. Voltage-gated calcium channels (VGCCs), which play important roles in cellular functions, represent an underexplored therapeutic target in parasitic organisms.

# Research Objectives
This project aims to develop machine learning models to identify compounds that selectively bind to the voltage-gated calcium channel of T. brucei. By comparing predicted binding affinities against the parasite and human calcium channels, we aim to identify selective inhibitors with reduced potential for off-target effects and host toxicity.

# Methodology
Data Collection: Compile compound structures and corresponding binding affinity data for parasite and human calcium channels.
Data Preprocessing: Perform data cleaning, molecular standardization, and feature preparation.
Feature Engineering: Generate molecular descriptors and molecular fingerprints using RDKit.
Machine Learning: Develop and optimize models, including Random Forest, XGBoost, Support Vector Regression (SVR), CatBoost, and LightGBM.
Model Evaluation: Evaluate predictive performance using appropriate metrics, including ROC-AUC, PR-AUC, RMSE, MAE, and R², depending on the prediction task.
Selectivity Prediction: Compare predicted binding affinities against parasite and human calcium channels to prioritize parasite-selective compounds.
Future Validation: Apply molecular docking and molecular dynamics simulations to investigate prioritized compounds and their interactions with the target channels.

# Description of Each Folder
RandomizesSearch
