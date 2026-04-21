# Car Price Prediction

Simple machine learning project that predicts used car selling price from historical car listing features.

## Project Files

- `CarPricePrd.ipynb`: Main notebook for data loading, preprocessing, model training, and prediction.
- `cardata.csv`: Input dataset.
- `requirements.txt`: Python dependencies.

## Dataset

The dataset includes these columns:

- `Car_Name`
- `Year`
- `Selling_Price` (target)
- `Present_Price`
- `Kms_Driven`
- `Fuel_Type`
- `Seller_Type`
- `Transmission`
- `Owner`

## What The Notebook Does

1. Imports libraries: pandas, matplotlib, seaborn, scikit-learn.
2. Loads `cardata.csv`.
3. Explores data shape, info, null checks, and category counts.
4. Encodes categorical columns (`Fuel_Type`, `Seller_Type`, `Transmission`) into numeric values.
5. Splits features/target and creates train/test sets.
6. Trains and evaluates:
   - Linear Regression
   - Lasso Regression
7. Plots actual vs predicted prices.
8. Runs sample prediction input.

## Setup

### 1. Create and activate virtual environment

Windows (PowerShell):

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Windows (Command Prompt):

```bat
python -m venv .venv
.venv\Scripts\activate.bat
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run notebook

Open `CarPricePrd.ipynb` in VS Code or Jupyter and run cells from top to bottom.

## Notes

- Make sure `cardata.csv` stays in the project root folder.
- If you update package versions, also update `requirements.txt`.
- Model quality can improve with additional feature engineering and hyperparameter tuning.
