# Heart Disease Detection Project

## Overview
This project predicts the likelihood of heart disease using clinical data.
It includes a cleaned dataset, the original dataset, a trained Decision Tree model, and a Jupyter notebook with the full workflow.

## Project Files
- `Heart Disease (2).ipynb`: End-to-end notebook for data analysis, model training, and evaluation.
- `heart.csv`: Original heart disease dataset.
- `cleaned_data.csv`: Preprocessed dataset used for modeling.
- `decision_tree_model.pkl`: Saved trained Decision Tree model.

## How to Run
1. Open `Heart Disease (2).ipynb` in Jupyter Notebook or VS Code/Cursor.
2. Run all cells in order to reproduce preprocessing, training, and evaluation steps.
3. Use the saved model file (`decision_tree_model.pkl`) for inference if needed.

## Requirements
- Python 3.9+ (recommended)
- Jupyter Notebook
- Common data science libraries such as:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib` (if plots are used in notebook)

## Notes
- Keep file paths unchanged to avoid notebook file-loading issues.
- If you retrain the model, replace `decision_tree_model.pkl` with the new exported model.
