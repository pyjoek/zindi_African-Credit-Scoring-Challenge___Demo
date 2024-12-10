# Zindi African Credit Scoring Challenge

## Overview
This repository demonstrates a workflow for participating in the Zindi African Credit Scoring Challenge. It includes preprocessing steps, feature engineering, model training, and submission file generation. Specifically, the notebook `submission2.ipynb` focuses on refining predictions for the test set and generating a submission file.

---

## Repository Structure

- **`Train.csv`**: The training dataset with labeled examples for building the model.
- **`Test.csv`**: The test dataset for which predictions are made.
- **`VariableDefinitions.csv`**: Provides descriptions of the features in the datasets.
- **`submission2.ipynb`**: Jupyter notebook detailing the process for generating a submission file.
- **`SampleSubmission.csv`**: Example submission file format for the challenge.

---

## Workflow in `submission2.ipynb`

1. **Data Loading**:
   - Reads `Train.csv` and `Test.csv` using pandas.
   - Displays basic statistics and structures of the datasets.

2. **Data Cleaning**:
   - Handles missing values and irrelevant columns.
   - Encodes categorical variables.

3. **Feature Engineering**:
   - Creates new features to improve prediction accuracy.
   - Normalizes or scales numerical features.

4. **Model Training**:
   - Trains a machine learning model (e.g., Random Forest, XGBoost) on the training data.
   - Tunes hyperparameters for optimal performance.

5. **Prediction Generation**:
   - Predicts the likelihood of loan default on the test dataset.
   - Prepares a submission file with two columns: `ID` and `Defaulted`.

6. **Submission File**:
   - Saves the predictions to a CSV file named `submission.csv`.

---

## Instructions for Use

1. Clone this repository:
   ```bash
   git clone https://github.com/pyjoek/zindi_African-Credit-Scoring-Challenge___Demo.git
   ```

2. Install necessary Python packages (e.g., pandas, scikit-learn):
   ```bash
   pip install -r requirements.txt
   ```

3. Open `submission2.ipynb` in Jupyter Notebook:
   ```bash
   jupyter notebook submission2.ipynb
   ```

4. Follow the steps in the notebook to:
   - Preprocess the data.
   - Train the model.
   - Generate predictions.

5. Submit the generated `submission.csv` to Zindi for evaluation.

---

## Submission Format

The submission file must include two columns:
- **`ID`**: Unique identifier for each customer.
- **`Defaulted`**: Predicted likelihood of loan default.

Example:
```csv
ID,Defaulted
ID_001,0.23
ID_002,0.87
```

---

## Contributions
Feel free to raise issues or submit pull requests for improvements.

