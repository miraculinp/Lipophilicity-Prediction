
# Lipophilicity Prediction

## Table of Contents

- [Overview](#overview)
- [Data](#data)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Project Structure](#project-structure)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Evaluation](#evaluation)
- [Results](#results)
- [Contributing](#contributing)

## Overview

This project focuses on predicting the lipophilicity (LogP) of chemical compounds using machine learning and cheminformatics. Lipophilicity is an important property for drug design and discovery, and accurate prediction can significantly impact the pharmaceutical industry. In this repository, we use molecular descriptors and the XGBoost algorithm to create a predictive model for LogP.

## Data

We use a dataset containing chemical compounds and their corresponding LogP values. The data is stored in a CSV file, "Lipophilicitydata.csv."

## Getting Started

### Prerequisites

Before running the code, you need to ensure you have the following libraries and tools installed:

- RDKit
- Pandas
- NumPy
- Matplotlib
- Sklearn
- XGBoost
- Jupyter Notebook or Colab

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/miraculinp/lipophilicity-prediction.git
   cd lipophilicity-prediction
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook or Python script for your analysis.

## Project Structure

The project structure is organized as follows:

- `data/`: Contains the dataset "Lipophilicitydata.csv."
- `notebooks/`: Jupyter Notebooks for data analysis and model development.
- `scripts/`: Python scripts for data preprocessing, modeling, and evaluation.
- `results/`: Save model results, plots, and any other relevant output here.

## Data Preprocessing

- Converting SMILES strings into molecular structures using RDKit.
- Calculating various RDKit molecular descriptors for each compound.
- Handling outliers and missing values.

## Model Building

- Utilizing the XGBoost algorithm for regression.
- Normalizing descriptor values.
- Cross-validation for model assessment.

## Evaluation

- Assessing model performance using R-squared (R^2) and Root Mean Squared Error (RMSE).
- Visualizing predictions vs. actual values.

## Results

The lipophilicity prediction model has been developed and evaluated with the following results:

- **Average Cross-Validation Score (10 Folds):** 0.9478667778543899
- **R-squared (R^2) Score:** 0.9566719900592656
- **Root Mean Squared Error (RMSE):** 0.42224880326842185


Further analysis and insights can be found in the project's Jupyter Notebook and related scripts in the repository.


## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request with a description of your changes.
