# CS5228 Project: HDB Price Prediction

This project focuses on developing a predictive model for HDB resale prices with a data set of transaction records, spatial features / accessibility to essential living amenities, and other pertinent features to evaluate the factors influencing resale prices. 

## Main Files
The main files used in this project are organized into the following 3 folders. 

- **`preprocessing/`** – Contains the preprocessing and EDA code, specifically the `AuxDataClean.ipynb` notebook. 

- **`models/`** – Contains all modeling notebooks used for data mining.
  -  `hyperparameter_tuning.ipynb` contains our final predictive model which obtained the highest RMSE for this task.

- **`data/`** – Contains all datasets used for training, validation, and testing.  

## Repository Structure
The entire structure of the respository is as below.
```
├── analysis/.ipynb_checkpoints/
│   └── Figures-checkpoint.ipynb
|
├── data/
│   ├── .ipynb_checkpoints/
│   ├── cleaned_train.csv
│   ├── cleaned_train_with_amenities.csv
│   ├── loc_rank_with_mrt.csv
│   ├── sg-gov-hawkers.csv
│   ├── sg-hdb-block-details.csv
│   ├── sg-hdb-rpi.csv
│   ├── sg-mrt-stations.csv
│   ├── sg-primary-schools.csv
│   ├── sg-secondary-schools.csv
│   ├── sg-shopping-malls.csv
│   ├── test.csv
│   └── train.csv
│
├── models/
│   ├── .ipynb_checkpoints/
│   ├── catboost_info/
│   ├── Baseline_models.ipynb
│   ├── CatBoost.ipynb
│   ├── CatBoost_Ridge_Ensemble.ipynb
│   ├── GradBoost.ipynb
│   ├── KNN trees.ipynb
│   ├── XGBoost.ipynb
│   └── hyperparameter_tuning.ipynb
|
├── preprocessing/
│   ├── .ipynb_checkpoints/
│   ├── AuxDataClean.ipynb
│   └── Figures.ipynb
│
└── README.md
```

## How to Run (Reproducibility)
1. Run preprocessing/AuxDataClean.ipynb to generate cleaned data (set SAVE_FINAL_FILE=True).
2. Run Figures.ipynb for EDA.
3. Run model notebooks in order: baselines -> tuning -> specific models -> ensemble.

