# CrimeCast: Forecasting Crime Categories

This repository contains the code for the Kaggle competition **"CrimeCast: Forecasting Crime Categories."** The goal of this competition is to build predictive models to determine the type of crime based on the provided dataset.

## Competition Overview

In this competition, you will analyze a dataset filled with information about crime incidents, including details such as incident locations, victim demographics, and other key attributes. The objective is to use this data to predict the crime category for each incident.

## Dataset

The dataset consists of the following files:

- **train.csv**: The training set, which includes the target variable `crime_category` along with various feature attributes.
- **test.csv**: The test set, which contains the feature attributes but excludes the target variable `crime_category`. The task is to predict this variable.
- **sample_submission.csv**: A sample submission file in the correct format required for the competition.

### Columns Description

The dataset contains the following columns:

- **Location**: Street address of the crime incident.
- **Cross_Street**: Cross street of the rounded address.
- **Latitude**: Latitude coordinates of the crime incident.
- **Longitude**: Longitude coordinates of the crime incident.
- **Date_Reported**: Date the incident was reported.
- **Date_Occurred**: Date the incident occurred.
- **Time_Occurred**: Time the incident occurred (24-hour military time).
- **Area_ID**: LAPD's Geographic Area number.
- **Area_Name**: Name designation of the LAPD Geographic Area.
- **Reporting_District_no**: Reporting district number.
- **Part 1-2**: Crime classification.
- **Modus_Operandi**: Activities associated with the suspect.
- **Victim_Age**: Age of the victim.
- **Victim_Sex**: Gender of the victim.
- **Victim_Descent**: Descent code of the victim.
- **Premise_Code**: Code indicating the location of the crime.
- **Premise_Description**: Description of the premise code.
- **Weapon_Used_Code**: Weapon code indicating the type of weapon used.
- **Weapon_Description**: Description of the weapon code.
- **Status**: Status of the case.
- **Status_Description**: Description of the status code.
- **Crime_Category**: The target variable, representing the category of the crime.

## Solution Overview

The solution follows a structured approach consisting of multiple steps:

1. **Exploratory Data Analysis (EDA)**: 
   - Conducted EDA using various graphs, heatmaps, etc., to explore the entire dataset.
   - Classified data into categorical and numerical columns and derived important insights to guide the model-building process.

2. **Feature Engineering and Data Preprocessing**:
   - Created new features and ensured class balance for necessary columns.
   - Preprocessed the data using pipelines and transformers, which included imputing missing values and applying necessary transformations.
   - Incorporated encoding techniques to handle categorical variables efficiently.

3. **Model Building**:
   - Experimented with different classifier models, including K-Nearest Neighbors (KNN) Classifier and Decision Tree Classifier.
   - Selected and implemented the Gradient Boosting Classifier, an ensemble model, as the final model based on its superior performance.

4. **Hyperparameter Tuning**:
   - Performed hyperparameter tuning using GridSearch to optimize model parameters and improve accuracy.

5. **Evaluation**:
   - Evaluated models using cross-validation and performance metrics such as accuracy, F1-score, and confusion matrix.

6. **Submission**:
   - Generated predictions for the test set and formatted them according to the submission guidelines.

## Getting Started

To run the code locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crimecast-forecasting.git
