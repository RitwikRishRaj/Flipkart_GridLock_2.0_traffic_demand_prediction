# Flipkart GridLock 2.0 Traffic Demand Prediction

This repository contains the solution developed for the Flipkart GridLock 2.0 traffic demand prediction challenge.

## Project Summary

- Data sources: `data/dataset/train.csv`, `data/dataset/test.csv`
- Notebook analysis and modeling work is under the `notebooks/` folder
- Final submission files are stored in the `submissions/` folder

## Approach

- Model training and feature engineering were performed primarily in the notebooks
- Key components include geohash decoding, time-based cyclic features, lag features, target encoding, and multiple ensemble models
- Final predictions were produced by blending LightGBM, ExtraTrees, CatBoost, and XGBoost outputs with a linear meta-model

## Result

- Achieved an online validation score of approximately **92.03% R²**
- Qualified for the first round of the challenge

## Output

- Final submission output written to `submissions/submission_v10.csv`

## Notes

- If you want to reproduce the results, run the main notebook for the modeling pipeline and ensure the data files are in `data/dataset/`
- The notebooks include detailed feature engineering and model training steps
