# 🩺 Heart Disease Prediction Project

## 📘 Overview
This project predicts the likelihood of heart disease in patients using **Machine Learning**, provides a **web-based interface** built with **Django**, and visualizes key patterns using an **interactive Power BI dashboard**.

The system helps medical practitioners and users analyze heart health risk based on multiple medical attributes such as age, cholesterol level, blood pressure, and more.

---

## 🧠 Project Workflow

### 1️⃣ Data Preparation & Model Training (Python)
- Dataset: `heart.csv`
- Algorithms used:
  - **SVM (Support Vector Machine)** for classification
- Model training and evaluation done in `train_model.py` and `svc.ipynb`.
- Models are saved using **Joblib/Pickle** as:
  - `svm_model.pkl`
  - `scalar.pkl`

### 2️⃣ Web Application (Django)
- A simple web form built with **HTML + Django views** allows users to input their medical data.
- The trained ML model is loaded in Django’s backend to predict the presence of heart disease.
- Files include:
  - `views.py` – logic to handle prediction
  - `form.html` – user input page
  - `result.html` – displays prediction result (Heart Disease: Yes/No)
  - `urls.py`, `models.py`, `settings.py` – standard Django configuration

### 3️⃣ Data Visualization (Power BI)
- The Power BI dashboard visualizes:
  - Heart disease distribution by age and sex
  - Cholesterol and MaxHR trends
  - Chest pain type comparisons
- Dashboard name: **Heart Disease Prediction Dashboard**
- Example visuals:
  - Bar charts for age bins and sex ratio
  - Comparison of cholesterol and heart disease correlation

---

## ⚙️ How to Run the Project

### Step 1: Clone this repository
```bash
git clone https://github.com/mahammzahid/heart-disease-prediction.git
cd heart-disease-prediction
```

### Step 2: Create and activate a virtual environment
```bash
python -m venv venv
venv\Scripts\activate      # for Windows
```

### Step 3: Install dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Run the Django web server
```bash
python manage.py runserver
```
Open your browser and go to **http://127.0.0.1:8000/**  

### Step 5: View the Power BI Dashboard
Open the `.pbix` file in Power BI Desktop or view exported images (in the `/dashboard` folder if uploaded).

---

## 📊 Model Performance
| Algorithm | Accuracy | Description |
|------------|-----------|--------------|
| SVM        | ~85–90%   | Best performing classifier |

---

## 🧰 Tech Stack
- **Python** (Pandas, Scikit-learn, NumPy)
- **Django Framework**
- **HTML / CSS**
- **Power BI**
- **Git & GitHub**

---

## 💡 Future Improvements
- Integrate database storage for user inputs and predictions.  
- Add more features like blood sugar, ECG, and BMI.  
- Implement API-based model deployment for scalability.  

---


## 👩‍💻 Author
**Maham Zahid**  
Department of Computer Science,  
The Islamia University of Bahawalpur 
