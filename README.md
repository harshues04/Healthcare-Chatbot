# HealthCare ChatBot using Machine Learning

This is a console-based HealthCare ChatBot that uses machine learning models to predict diseases based on user-input symptoms. It also provides descriptions, precautions, and severity analysis for the predicted conditions.

## Features

- Disease prediction using Decision Tree and SVM models
- Interactive symptom input with pattern matching
- Severity analysis based on symptoms and duration
- Description and precaution suggestion for the predicted diseases
- Secondary prediction for increased reliability



## Input Files

- `Training.csv`: Contains symptoms and disease labels used to train the models.
- `Testing.csv`: Used to evaluate model performance.
- `symptom_severity.csv`: Maps symptoms to severity scores (used for risk assessment).
- `symptom_Description.csv`: Provides disease descriptions.
- `symptom_precaution.csv`: Lists precautions for each disease.

## How It Works

1. The chatbot trains a Decision Tree and SVM model on symptom-disease mapping.
2. The user inputs a symptom, which is matched using pattern recognition to suggest accurate symptom names.
3. The chatbot asks the user for the duration of symptoms.
4. Based on the Decision Tree model, the chatbot predicts the most likely disease.
5. The user is asked about additional symptoms associated with the predicted disease.
6. A secondary prediction is made with these confirmed symptoms to verify the diagnosis.
7. The chatbot outputs:
   - Predicted disease(s)
   - Description(s) from the database
   - Suggested precautionary measures
   - Severity-based consultation recommendation

## Installation & Requirements

### Prerequisites

- Python 3.x
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `pyttsx3` (optional for voice output)
  - `csv`

You can install the necessary libraries with:

```bash
pip install pandas numpy scikit-learn pyttsx3
