# 🏠 House Price Prediction Model

This repository contains a Machine Learning model that predicts house price based on input features such as size and bedroom. The model has been trained and saved in `.pkl` format for reuse and deployment.

## 👥 Project Team
- Dipali Gantait
- Sudipta Singha
- Riyajul Saha

## 📁 Project Contents

- `house_price_prediction_model.pkl` – Trained ML model saved using `pickle`.
- `README.md` – Overview and instructions.
- `House_Price(ML).csv` – Dataset
- `House_Price_Model.ipynb` - Source Code

## 🧠 Model Information

- **Model Type**: Multilinear Regression
- **Purpose**: Predict House price.
- **Input Features**: Size in sqft and Bedrooms
- **Output**: Predicted Price

## 🧪 How to Use the Model

1. Clone this repository:
   ```bash
   git clone https://github.com/trio-rds-tensors/House_Price_Prediction_Model.git

2. Install required libraries:
   ```bash
   pip install numpy pandas scikit-learn
3. Load and use the model:
   ```bash
   import pickle
   # Load model
   with open('house_price_prediction_model.pkl','rb') as file:
      model = pickle.load(file)
   #Predict (example)
   predicted_price=model.predict([[size,bedroom_number]])
   print(predicted_price)

## ✅ Example
   ```bash
   # Predict price for 34 sqft size and 2 bedroom study hours
   model.predict([[34,2]])  # Output [101954.2590173] doller
```
## 📊 Performance
**Accuracy Metric:** R² Score = 0.9388153783546871

The model has been evaluated on test data and performs well on predicting continuous score values.

## 📜 License
This project is open-source and free to use for educational purposes.
