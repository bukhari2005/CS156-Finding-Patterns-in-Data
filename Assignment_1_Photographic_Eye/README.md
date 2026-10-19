# Assignment 1 — Can Machine Learning Learn My Photographic Eye?

## Project Overview

This project investigates whether machine learning can predict which photographs I would select for my personal photography portfolio.

I labeled 100 photographs from five locations and compared four classification approaches: a dummy baseline, raw-pixel logistic regression, PCA with logistic regression, and frozen pretrained ResNet18 features with logistic regression.

## Main Results

- Best development model: ResNet18 + Logistic Regression
- Mean cross-validation balanced accuracy: 0.654
- Held-out Berlin balanced accuracy: 0.600
- Validation: 3-fold StratifiedGroupKFold using photography sessions

## Files

`CS156_A1_Photographic_Eye.ipynb` contains the complete experiment, explanations, mathematical equations, visualizations, and appendices.

## Dataset

Photographs, metadata, and access instructions:

https://drive.google.com/drive/folders/1gmDHo0JDfF2qD9de_57G209mXdkD70Fl?usp=sharing

## How to Reproduce

1. Download or open the notebook in Google Colab.
2. Access the dataset using the Google Drive link above.
3. Place the project folder in Google Drive under `MyDrive/CS156_Photographic_Eye`, or update the `project` path in the notebook.
4. Run the Main Assignment cells in order, beginning with dataset loading.
5. Review the Appendices for the original data preparation, manual labeling, and validation checks.

The final metadata and photography labels are already prepared. The manual labeling process does not need to be repeated to reproduce model training and evaluation.

## Limitations

The dataset contains only 100 photographs labeled by one photographer. Results are preliminary, and the small Berlin test set does not establish reliable generalization to other locations.
