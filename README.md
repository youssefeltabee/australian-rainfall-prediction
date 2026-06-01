# Australian Rainfall Prediction

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.8-F7931E?logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green)

Machine learning project that predicts whether it will rain tomorrow in Australia based on weather data.

## Project Overview

This project builds an end-to-end ML pipeline to predict rainfall using historical Australian weather data. It demonstrates:
- Complete data preprocessing with scikit-learn Pipeline
- Feature engineering (date to season conversion)
- GridSearchCV hyperparameter tuning
- Model comparison (RandomForest vs LogisticRegression)
- ~84% accuracy on test set

## Results

| Model | CV Accuracy | Test Accuracy |
|-------|:-----------:|:-------------:|
| RandomForest | ~84% | 84% |
| LogisticRegression | ~83% | 83% |

## Quick Start

```bash
pip install -r requirements.txt
jupyter notebook australian_rainfall_prediction.ipynb
```

## Dataset

Historical weather observations from the Australian Bureau of Meteorology with features including temperature, rainfall, wind speed, humidity, and pressure.
