# 🌧️ Rainfall Prediction Classifier using Python & MLflow  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)  
![MLflow](https://img.shields.io/badge/MLflow-Tracking%20%26%20Registry-brightgreen)  
![Flask](https://img.shields.io/badge/Flask-Web%20App-lightgrey)   

---

## 📌 Project Description  
The **Rainfall Prediction Classifier** is a machine learning project that predicts whether rainfall will occur based on meteorological parameters such as **pressure, dewpoint, humidity, cloud cover, sunshine, wind direction, and wind speed**.  

The project involves:  
- **Data Preprocessing & Cleaning** (handling missing values, outliers, and class imbalance with SMOTE)  
- **Exploratory Data Analysis (EDA)** with visualizations  
- **Model Training** using **Random Forest Classifier** with hyperparameter tuning  
- **Experiment Tracking & Model Registry** using **MLflow**  
- **Deployment** with a **Flask Web Application** for real-time predictions  

---

## ⚡ Key Features  
- ✅ Automated data preprocessing (missing values, outliers, SMOTE balancing)  
- ✅ EDA with plots (histograms, KDE, boxplots, correlation heatmaps)  
- ✅ Random Forest Classifier with GridSearchCV for best hyperparameters  
- ✅ Evaluation with **Accuracy, Recall, F1-score (macro average)**  
- ✅ MLflow for experiment tracking, model versioning, and registry  
- ✅ Flask web app for interactive rainfall predictions  
- ✅ Supports **Champion/Challenger** model promotion strategy with MLflow  

---

## 🛠️ Installation Instructions  

1. **Clone the Repository**  
```bash
git clone https://github.com/your-username/rainfall-prediction.git
cd rainfall-prediction
```

2. **Create and Activate Virtual Environment**  
```bash
# Create venv
python -m venv venv  

# Activate venv
# On Windows
venv\Scripts\activate  
# On Linux/Mac
source venv/bin/activate
```

3. **Install Dependencies**  
```bash
pip install -r requirements.txt
```

Typical dependencies include:  
- pandas, numpy, scikit-learn  
- matplotlib, seaborn  
- mlflow  
- flask  

4. **(Optional) Start MLflow Tracking Server**  
```bash
mlflow ui
```
MLflow UI will run at: [http://127.0.0.1:5000](http://127.0.0.1:5000)  

5. **Run Jupyter Notebook**  
```bash
jupyter notebook
```
Open `Rainfall Prediction Classifier.ipynb` to explore preprocessing, training, and MLflow experiments.  

6. **Run Flask App**  
```bash
python app.py
```
Then open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser to input weather parameters and get predictions.  

---

## 🚀 Usage  

### 1️⃣ Run the Model in Jupyter Notebook  
- Preprocess dataset  
- Train Random Forest Classifier  
- Track experiments with MLflow  
- Register models in MLflow Model Registry  
- Evaluate performance  

### 2️⃣ Use the Flask Web Application  
```bash
python app.py
```
- Enter weather parameters:  
  - Pressure  
  - Dewpoint  
  - Humidity  
  - Cloud cover  
  - Sunshine  
  - Wind direction  
  - Wind speed  
- Click **Predict** → Get **Rainfall** or **No Rainfall** instantly  

---

## 🧑‍💻 Technologies Used  
- **Python** – Core programming  
- **Jupyter Notebook** – Data preprocessing, training, experiments  
- **Scikit-learn** – Machine learning (Random Forest, metrics)  
- **Pandas & NumPy** – Data manipulation  
- **Matplotlib & Seaborn** – Visualization & EDA  
- **MLflow** – Experiment tracking & model registry  
- **Flask** – Web app deployment  

---

## 📊 Example Prediction  

```python
input_df = (1015.9, 19.9, 95, 81, 0.0, 40.0, 13.7)
input_df = pd.DataFrame([input_df], columns=['pressure', 'dewpoint', 'humidity', 'cloud', 'sunshine', 'winddirection', 'windspeed'])
prediction = loaded_model.predict(input_df)
print("Rainfall" if prediction[0] == 1 else "No Rainfall")
```

---

## ✅ Project Outcomes  
- Built and evaluated a **Random Forest Classifier** for rainfall prediction  
- Used **MLflow** for reproducibility, tracking, and model management  
- Deployed a **Flask web app** for real-time rainfall classification  

---

✨ Developed with Python, MLflow & Flask ✨  
