
# 🚗 Car Price Prediction – Machine Learning Project

## 📌 Project Overview
This project predicts the selling price of a used car based on features like:
- Car brand
- Year
- Present price
- KM driven
- Fuel type
- Seller type
- Transmission

Dataset used: **car_data.csv** (inside `data/` folder)

Model used: **Linear Regression**

This project performs:
✔ Data Cleaning  
✔ Exploratory Data Analysis (EDA)  
✔ Feature Engineering  
✔ Model Training  
✔ Evaluation  
✔ Saving Trained Model (`joblib`)  


## 📁 Project Structure
```
car_price_prediction/
│
├── data/
│   └── car_data.csv
│
├── notebooks/
│   └── 01_eda_and_model.ipynb
│
├── src/
│   ├── __init__.py
│   ├── data_loader.py
│   ├── preprocess.py
│   ├── train.py
│   ├── predict.py
│
├── models/
│   ├── car_price_model.joblib
│   └── scaler.joblib
│
├── app/
│   ├── flask_app.py
│   └── streamlit_app.py
│
├── tests/
│   └── test_data.py
│
├── requirements.txt
└── README.md
```

---

## 🛠 Installation & Setup

### ✅ 1. Clone the repository
```
git clone https://github.com/your-username/car_price_prediction.git
cd car_price_prediction
```

### ✅ 2. Create virtual environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows
```

### ✅ 3. Install dependencies
```
pip install -r requirements.txt
```

---

## 🚀 Train the Model
```
python src/train.py
```

This generates:
```
models/car_price_model.joblib
models/scaler.joblib
```

---

## 🔮 Run Prediction
```
python src/predict.py
```

---

## 🌐 Run Streamlit App (UI)
```
streamlit run app/streamlit_app.py
```

---

## 🔥 Run Flask API (Backend)
```
python app/flask_app.py
```

Endpoint:
```
http://localhost:5000/predict
```

Example JSON body:
```json
{
  "car_features": [2016, 12.5, 50000, "Petrol", "Dealer", "Manual"]
}
```

---

## 📈 Model Evaluation Metrics
```
RMSE: ...
R² Score: ...
```

---

## 📚 Open Notebook
```
jupyter notebook notebooks/01_eda_and_model.ipynb
```

---

## 🤝 Contribution
Pull requests are welcome!

## 📄 License
Free & open source.
