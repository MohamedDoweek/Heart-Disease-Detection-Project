# Heart Disease Detection Project

## Overview
This project predicts the likelihood of heart disease using clinical data.
The workflow covers data cleaning, preprocessing, feature engineering, exploratory analysis, model training, and saving a trained model.

## Project Files
- `Heart Disease (2).ipynb`: End-to-end notebook for data analysis, model training, and evaluation.
- `heart.csv`: Original heart disease dataset.
- `cleaned_data.csv`: Preprocessed dataset used for modeling.
- `decision_tree_model.pkl`: Saved trained Decision Tree model.

## What I Used

### Environment and Tools
- Python
- Jupyter Notebook / Google Colab style workflow
- Git + GitHub for version control and hosting

### Python Libraries
- `pandas` for loading, cleaning, and transforming data
- `numpy` for numerical operations
- `scikit-learn` for preprocessing and machine learning
- `matplotlib` for plots
- `seaborn` for data visualization

### Dataset Details
- Input dataset: `heart.csv`
- Original shape: `1025` rows x `14` columns
- Target column: `target` (heart disease prediction label)

### Features Used
- `age`, `sex`, `cp`, `trestbps`, `chol`, `fbs`, `restecg`, `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`

### Preprocessing Steps
1. Loaded data from `heart.csv`
2. Handled missing placeholders (`?`, `NA`, `N/A`, empty strings)
3. Converted columns to numeric where possible
4. Filled missing numeric values with median
5. Filled missing categorical values with mode
6. Encoded categorical features using one-hot encoding (`pd.get_dummies`)
7. Normalized feature values using `MinMaxScaler`
8. Created and saved cleaned data as `cleaned_data.csv`

### Feature Selection / Analysis
- Correlation analysis was used to inspect feature importance against `target`
- Example strong features observed in notebook output include:
  - `thal_2`
  - `thalach`
  - `slope_2`
  - `cp_2`
  - `cp_1`

### Model
- Trained model type: Decision Tree classifier
- Saved model artifact: `decision_tree_model.pkl`

### Outputs
- Cleaned dataset: `cleaned_data.csv` (shape shown in notebook: `1025 x 23`)
- Trained model file: `decision_tree_model.pkl`
- Notebook with all steps and outputs: `Heart Disease (2).ipynb`

## Project Screenshots
Add your screenshots in a folder named `screenshots` at the project root, then keep/update the image links below.

### 1) Dataset Preview
![Dataset Preview](screenshots/dataset-preview.png)
*Initial rows and structure of the heart disease dataset.*

### 2) Data Preprocessing Pipeline
![Preprocessing Pipeline](screenshots/preprocessing-pipeline.png)
*Missing value handling, encoding, and normalization steps.*

### 3) Feature Correlation with Target
![Feature Correlation](screenshots/feature-correlation.png)
*Most important features correlated with heart disease prediction.*

### 4) Model Training and Evaluation
![Model Training](screenshots/model-training.png)
*Decision Tree training output and evaluation metrics.*

### 5) Final Notebook Output
![Final Output](screenshots/final-output.png)
*Final project results and generated artifacts.*

## How to Run
1. Open `Heart Disease (2).ipynb` in Jupyter Notebook, VS Code, or Cursor.
2. Install the required libraries listed above.
3. Run all cells in order.
4. Use `decision_tree_model.pkl` for prediction/inference.

## Requirements
- Python 3.9+ (recommended)
- Jupyter Notebook
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## Notes
- Keep file paths unchanged to avoid notebook file-loading issues.
- If you retrain the model, replace `decision_tree_model.pkl` with the new exported model.
