# Project Title:- ## Machine Learning-Driven Discovery of Selective Inhibitors Against Trypanosoma brucei Calcium Channels

## Project Background and Motivation
Trypanosoma brucei is a parasitic protozoan responsible for Nagana in cattle and human African trypanosomiasis (sleeping sickness) in humans. Existing treatments are limited by drug toxicity, the absence of an effective vaccine, and the emergence of drug resistance, highlighting the need for novel therapeutic targets. Voltage-gated calcium channels (VGCCs), which play important roles in cellular functions, represent an underexplored therapeutic target in parasitic organisms.

## Research Objectives
This project aims to develop machine learning models to identify compounds that selectively bind to the voltage-gated calcium channel of T. brucei. By comparing predicted binding affinities against the parasite and human calcium channels, we aim to identify selective inhibitors with reduced potential for off-target effects and host toxicity.

## Methodology
𝐃𝐚𝐭𝐚 𝐂𝐨𝐥𝐥𝐞𝐜𝐭𝐢𝐨𝐧: Compile compound structures and corresponding binding affinity data for parasite and human calcium channels. <br>
𝐃𝐚𝐭𝐚 𝐏𝐫𝐞𝐩𝐫𝐨𝐜𝐞𝐬𝐬𝐢𝐧𝐠: Perform data cleaning, molecular standardization, and feature preparation. <br>
𝐅𝐞𝐚𝐭𝐮𝐫𝐞 𝐄𝐧𝐠𝐢𝐧𝐞𝐞𝐫𝐢𝐧𝐠: Generate molecular descriptors and molecular fingerprints using RDKit. <br>
𝐌𝐚𝐜𝐡𝐢𝐧𝐞 𝐋𝐞𝐚𝐫𝐧𝐢𝐧𝐠: Develop and optimize models, including Random Forest, XGBoost, Support Vector Regression (SVR), CatBoost, and LightGBM. <br> 
𝐌𝐨𝐝𝐞𝐥 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧: Evaluate predictive performance using appropriate metrics, including ROC-AUC, PR-AUC, RMSE, MAE, and R², depending on the prediction task. <br>
𝐒𝐞𝐥𝐞𝐜𝐭𝐢𝐯𝐢𝐭𝐲 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧: Compare predicted binding affinities against parasite and human calcium channels to prioritize parasite-selective compounds. <br>
𝐅𝐮𝐭𝐮𝐫𝐞 𝐕𝐚𝐥𝐢𝐝𝐚𝐭𝐢𝐨𝐧: Apply molecular docking and molecular dynamics simulations to investigate prioritized compounds and their interactions with the target channels. <br>

## Repository Structure
### Random-Split-ML-All-Features
This folder contains machine learning models developed using a random train-test splitting strategy, in which the dataset is randomly divided into training and test sets. <br>

It includes three subfolders based on the input data used: <br>
𝐭𝐛𝐫𝐮𝐜𝐞𝐢-𝐝𝐚𝐭𝐚-𝐨𝐧𝐥𝐲: Models trained and evaluated using only T. brucei data. <br>
𝐦𝐚𝐦𝐦𝐚𝐥𝐢𝐚𝐧-𝐝𝐚𝐭𝐚-𝐨𝐧𝐥𝐲: Models trained and evaluated using only mammalian calcium channel data. <br>
𝐦𝐚𝐦𝐦𝐚𝐥𝐢𝐚𝐧-𝐭𝐛𝐫𝐮𝐜𝐞𝐢-𝐜𝐨𝐦𝐛𝐢𝐧𝐞𝐝-𝐝𝐚𝐭𝐚: Models trained and evaluated using combined mammalian and T. brucei data. <br>
All data preprocessing, feature engineering, model development, hyperparameter optimization, and evaluation procedures follow the methodology described in the Methodology section. <br>

### Scaffold-Split-ML-All-Features
This folder contains machine learning models developed using a scaffold-based train-test splitting strategy, in which compounds are divided based on their molecular scaffolds. This approach helps evaluate model generalizability to structurally distinct compounds and reduces the risk of overly optimistic performance estimates due to structural similarity between training and test sets. <br>

It includes three subfolders based on the input data used: <br>
𝐭𝐛𝐫𝐮𝐜𝐞𝐢-𝐝𝐚𝐭𝐚-𝐨𝐧𝐥𝐲: Models trained and evaluated using only T. brucei data. <br>
𝐦𝐚𝐦𝐦𝐚𝐥𝐢𝐚𝐧-𝐝𝐚𝐭𝐚-𝐨𝐧𝐥𝐲: Models trained and evaluated using only mammalian calcium channel data. <br>
𝐦𝐚𝐦𝐦𝐚𝐥𝐢𝐚𝐧-𝐭𝐛𝐫𝐮𝐜𝐞𝐢-𝐜𝐨𝐦𝐛𝐢𝐧𝐞𝐝-𝐝𝐚𝐭𝐚: Models trained and evaluated using combined mammalian and T. brucei data. <br>
All data preprocessing, feature engineering, model development, hyperparameter optimization, and evaluation procedures follow the methodology described in the Methodology section. <br>
