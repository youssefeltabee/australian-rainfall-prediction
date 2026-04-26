# Australian Rainfall Prediction

Machine learning project that predicts whether it will rain tomorrow in Australia based on weather data.

## Project Overview

This project builds an end-to-end ML pipeline to predict rainfall using historical Australian weather data. It demonstrates:
- Complete data preprocessing with Scikit-learn Pipeline
- Feature engineering (date to season conversion)
- GridSearchCV hyperparameter tuning
- Model comparison (RandomForest vs LogisticRegression)
- ~84% accuracy on test set

## Features

- **Data Preprocessing**: 
  - Handling missing values
  - Categorical encoding (OneHotEncoder)
  - Feature scaling (StandardScaler)
- **Feature Engineering**:
  - Date to Season conversion
  - RainToday/RainTomorrow shift
- **Models**:
  - RandomForestClassifier (best: ~84% accuracy)
  - LogisticRegression (~83% accuracy)
- **Evaluation**:
  - GridSearchCV with StratifiedKFold cross-validation
  - Confusion matrix, classification report
  - Feature importance analysis

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Open the notebook in Jupyter:
```bash
jupyter notebook australian_rainfall_prediction.ipynb
```

Run all cells to:
1. Load and explore data
2. Preprocess features
3. Train models with GridSearchCV
4. Evaluate and compare results

## Results

| Model | CV Accuracy | Test Accuracy |
|-------|-------------|--------------|
| RandomForest | ~84% | 84% |
| LogisticRegression | ~83% | 83% |

## Dataset Features

| Feature | Description |
|---------|-------------|
| Location | Australian location |
| MinTemp, MaxTemp | Temperature |
| Rainfall | Rainfall amount |
| Evaporation | Evaporation |
| Sunshine | Sunshine hours |
| WindGustDir | Wind gust direction |
| WindSpeed9am/3pm | Wind speed |
| Humidity9am/3pm | Humidity |
| Pressure9am/3pm | Pressure |
| Cloud9am/3pm | Cloud cover |
| Temp9am/3pm | Temperature |
| RainToday | Did it rain today? |
| RainTomorrow | Target: Will it rain tomorrow? |

## Requirements

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## License

MIT