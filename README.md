# Personalized Offer Response Prediction - Starbucks Capstone

## Project Summary

This project builds a machine learning pipeline to predict whether a user will respond to a Starbucks marketing offer. It integrates user demographics, historical transaction behavior, and offer details to improve personalized targeting for promotions.

## Software and Libraries

The project was developed using the following tools and libraries:

- **Python** - 3.8+.
- **Pandas** - for loading, merging, and transforular data.
- **NumPY** - for numerical computations, arrays, and mathematical operations.
- **Matplotlib** and **Seaborn** – Utilized for exploratory data visualization, plotting ROC curves, and statistical graphics.
- **Scikit-learn** – Preprocessing tools, classification models (Logistic Regression, Random Forest), evaluation metrics, and hyperparameter tuning utilities like `RandomizedSearchCV`.
- **XGBoost** – Used to train and tune gradient boosting models for classification.
- **IPython.display** – For rendering DataFrames and outputs interactively within Jupyter.
- **Jupyter Notebook (Amazon SageMaker Studio)** – Development and experimentation environment for prototyping, analysis, and visualisation.

## Project Structure

- `data/`  
  Contains three original JSON datasets used in the project:
  - `portfolio.json` – Contains metadata about the marketing offers.
  - `profile.json` – Includes demographic and membership information for users.
  - `transcript.json` – Event log capturing user interactions (e.g., transactions, offer received/viewed/completed).

- `Starbucks_Capstone_notebook.ipynb`  
  Main Jupyter Notebook containing all code for data processing, EDA, feature engineering, modeling, and evaluation.

- `proposal.pdf`  
  Initial project proposal outlining goals, problem definition, and approach.

- `Starbucks project report.pdf`  
  Final project report summarizing the full project process, analysis, results, and recommendations.

- `README.md`  
  This file. Provides project overview, setup instructions, and structure reference.structions.

## How to Run

This project is designed to be run in **Amazon SageMaker Studio**. To replicate the results:

1. Upload the provided dataset (`portfolio.json`, `profile.json`, `transcript.json`) to your workin within a `data/` folderg directory.
2. Open the Jupyter notebook and run all cells sequentially.
3. You may need to install missing packages using pip, e.g.:
   ```python
   !pip install xgboost