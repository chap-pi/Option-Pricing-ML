## 📊 Machine Learning for Option Pricing:

# Application to European Call Options on Apple (AAPL)

The base data file is compressed in a ZIP archive because it's too large to include in the Git repository. Before manipulating the code, remember to extract this ZIP file to retrieve the original CSV file.

Project Overview:
This project investigates the use of machine learning models for pricing European call options, using real market data on Apple (AAPL) options between 2021 and 2023.

The project follows a progressive and structured methodology:
- Data cleaning and feature engineering,
- Linear regression as an interpretable baseline,
- Random Forest to capture non-linear effects,
- Gradient Boosting as a more refined non-linear model.
All results are documented and analyzed in a final PDF report generated with LaTeX.

Project Structure:
├── data/
│   ├── raw/
│      └── aapl_2021_2023.csv 
│
├── notebooks/
    ├── data/
    │    ├── processed/
│   │            └── aapl_calls_ml_dataset.csv
│   ├── 01_Data Clean.ipynb
│   ├── 02_Linear Regression.ipynb
│   ├── 03_Random Forest.ipynb
│   └── 04_GradientBoosting.ipynb
│
├── report/
│    ├── figures/
│    ├── report.md
│    ├── template.tex
│
├── requirements.txt
└── README.md

Dataset:
The raw dataset contains historical option market data for Apple (AAPL), including prices, implied volatility, maturities, strikes...
Source:
https://www.kaggle.com/datasets/kylegraupe/aapl-options-data-2016-2020
(only the aapl_2021_2023.csv file is used in this project)

▶️ How to Run the Project:
Place the raw dataset in: data/raw/aapl_2021_2023.csv

Run the notebooks in order:
1) 01_data_preparation.ipynb
2) 02_linear_regression.ipynb
3) 03_random_forest.ipynb
4) 04_gradient_boosting.ipynb

📌 Notes: 
- The project focuses on methodology and interpretability, not black-box optimization.
- All modeling choices are justified and discussed in the report.
- Results should be interpreted in the context of real market data limitations.

