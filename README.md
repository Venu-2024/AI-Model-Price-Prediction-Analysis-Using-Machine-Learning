# AI Model Price History — Machine Learning Project

An end-to-end machine learning notebook for exploring historical AI model pricing and modeling price-related patterns.

## Project goals

* Clean and inspect historical AI model pricing data.
* Perform exploratory data analysis (EDA) and visualize price distributions and relationships.
* Engineer time-based and price-related features.
* Train regression models to estimate log input price.
* Classify models into price tiers (Low / Medium / High).
* Explore groups of models with K-Means clustering.
* Tune a Ridge Regression model with `GridSearchCV`.
* Inspect feature importance from a Random Forest model.

## Notebook

Open `AI\_Model\_Price\_History\_ML\_Project.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.

## Dataset

The notebook expects a CSV file named `ai\_model\_price\_history.csv` in the working directory. The CSV was not included with the uploaded notebook, so add the dataset if you have permission to redistribute it, or document a reliable source/download procedure.

The notebook references fields such as `week\_start`, `model\_name`, `developer`, `provider`, `mode`, `input\_price\_per\_1m\_tokens`, `output\_price\_per\_1m\_tokens`, and `max\_input\_tokens`.

**Data note:** Check the source, license, and collection date of the dataset before publishing it. Do not commit private, restricted, or unlicensed data.

## Setup

Python 3.10+ is a reasonable starting point. Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Then open the notebook and run the cells from top to bottom. Update the CSV path in the data-loading cell if needed.

## Methods included

* Data cleaning and missing-value handling
* Exploratory data analysis with Pandas, Matplotlib, and Seaborn
* Feature engineering and preprocessing pipelines
* Linear Regression, Ridge Regression, and Random Forest Regression
* Logistic Regression and Random Forest Classification
* K-Means clustering with elbow and silhouette analysis
* PCA-based cluster visualization
* Cross-validation and hyperparameter tuning
* Random Forest feature-importance analysis

## Evaluation

The notebook is designed to report regression metrics such as MAE, RMSE, and R², plus cross-validation results and classification diagnostics. Run the notebook against the intended dataset and add the actual results here before presenting model performance claims.

## Important limitations

* Historical prices can change; this analysis should not be treated as a live price feed.
* Model names, providers, and pricing units may change over time. Validate data definitions before drawing conclusions.
* The selected clustering count (`k=4`) is a modeling choice in the notebook and should be justified using the resulting diagnostics.
* This repository currently contains the notebook and project documentation; the dataset is not bundled.

## Suggested next improvements

1. Add a data dictionary and a reproducible data acquisition step.
2. Save selected plots to an `images/` folder and include them in this README.
3. Compare model results in a single table and explain the best model using measured test metrics.
4. Add automated checks or a small script for data validation.
5. Add a clear license only after deciding what rights you want to grant.

## Repository structure

```text
AI-Model-Price-History-ML/
├── AI\_Model\_Price\_History\_ML\_Project.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Author

Venu Madalagi

https://github.com/Venu-2024

venu272002@gmail.com

