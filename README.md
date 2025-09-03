# Migraine Type Prediction Web App

This project is a Streamlit-based web application that predicts the type of migraine a user may be experiencing based on their symptoms. The app uses a trained Random Forest Classifier and provides personalized preventive recommendations alongside the prediction.

---

## Features

- Predicts migraine types using clinical features
- Displays detailed preventive measures
- Interactive Streamlit interface for easy user input
- Sidebar with educational content about migraines
- Includes model training, tuning, and persistence

---

## Dataset

The dataset includes various features like:

- Age, Duration, Frequency
- Symptoms: Nausea, Vomiting, Photophobia, Phonophobia, etc.
- Diagnostic labels: `Type` (e.g., "Migraine without aura", "Basilar-type aura", etc.)

> The dataset is loaded from a local CSV file:  
> `migraine_data.csv`

---

## Model

- **Algorithm**: Random Forest Classifier
- **Hyperparameter Tuning**: Performed using `GridSearchCV`
- **Preprocessing**:
  - Label Encoding for categorical features
  - MinMax Scaling for numerical features
- **Train-Test Split**: 80/20

The model is serialized using `pickle` for reusability.

---

## Tech Stack

- Python
- scikit-learn
- pandas / numpy
- Streamlit
- pickle
- matplotlib 

---
