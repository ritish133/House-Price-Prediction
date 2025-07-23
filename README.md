🏡 House Price Prediction using Machine Learning

This project implements a **House Price Prediction** model trained on California housing data. It leverages preprocessing pipelines, feature engineering, and a **Random Forest Regressor** to estimate housing prices based on location, demographics, and proximity to the ocean.

---

🚀 Features

- Data preprocessing with `scikit-learn` pipelines
- Stratified sampling based on income categories
- Handling of missing values and categorical features
- Model training using Random Forest
- Inference pipeline to predict house prices from unseen data
- Model and pipeline serialization with `joblib`

---

📁 Project Structure
├── housing.csv           # Dataset (California Housing)
├── input.csv             # Auto-generated test input (for inference)
├── output.csv            # Predictions saved after inference
├── model.pkl             # Trained Random Forest model
├── pipeline.pkl          # Preprocessing pipeline
├── house_price_predictor.py # Main training/inference script
└── README.md             # Project documentation

---

🧠 Model Overview

- **Model Used**: Random Forest Regressor
- **Evaluation Metric**: Root Mean Squared Error (RMSE) via cross-validation
- **Preprocessing Techniques**:
  - Imputation using median strategy
  - Feature scaling with `StandardScaler`
  - One-hot encoding of categorical features
  - ColumnTransformer to combine numeric and categorical pipelines

---

📦 Dependencies

Install the required libraries:
pip install pandas numpy scikit-learn joblib

---

📝 How to Run
1. Train the Model : Simply run the script. If the model and pipeline do not exist, it will train and save them automatically.
2. Predict on New Data : Once the model is trained, running the script again will perform inference on the auto-generated input.csv

  Command to run:
      python main.py

---

📌 Notes
	•	The first time you run the script, it creates a stratified test set from the full dataset and saves it as input.csv.
	•	Make sure housing.csv is present in the same directory before running.

---

License
This project is licensed under the MIT License
Use, modify, and distribute freely.

---

🙌 Acknowledgments
This project was inspired by hands-on machine learning best practices and the California Housing dataset.
Powered by scikit-learn and pandas.


For questions or improvements, feel free to open an issue or submit a pull request!

