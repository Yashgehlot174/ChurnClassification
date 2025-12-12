# 📉 Customer Churn Prediction Web App

A **machine learning–powered web application** that predicts whether a customer is likely to **churn** based on demographic, financial, and engagement features.  
The app is built using **TensorFlow, Scikit-learn, and Streamlit**, and is **fully deployed** for real-time predictions.

🚀 **Live Demo:**  
👉 https://churnclassification-zmhtcuzrhhhgzibbge48nh.streamlit.app/

---

## 📌 Project Overview

Customer churn is a critical business problem where companies lose customers over time.  
This project solves that problem by:

- Training a **binary classification neural network**
- Processing categorical and numerical features
- Providing **real-time churn probability predictions** via a Streamlit web app

The model outputs:
- **Churn Probability**
- **Final churn decision** (Likely / Not Likely)

---

## 🧠 Machine Learning Pipeline

1. **Data Collection**
   - Dataset: `Churn_Modelling.csv`

2. **Data Preprocessing**
   - Label Encoding → Gender  
   - One-Hot Encoding → Geography  
   - Feature Scaling → StandardScaler

3. **Model Training**
   - Deep Learning model using **TensorFlow / Keras**
   - Binary classification with sigmoid activation

4. **Model Persistence**
   - Saved trained model (`model.h5`)
   - Saved encoders & scaler (`.pkl` files)

5. **Deployment**
   - Streamlit web app
   - Hosted on Streamlit Cloud

---

## 🛠️ Tech Stack

- **Frontend / Deployment**
  - Streamlit

- **Machine Learning**
  - TensorFlow / Keras  
  - Scikit-learn

- **Data Handling**
  - Pandas  
  - NumPy

- **Model Serialization**
  - Pickle

---

## 📂 Project Structure

```
├── app.py
├── model.h5
├── scaler.pkl
├── label_encoder_gender.pkl
├── one_hot_encoder_geo.pkl
├── Churn_Modelling.csv
├── main.ipynb
├── prediction.ipynb
├── regression.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ How to Run Locally

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Streamlit App
```bash
streamlit run app.py
```

---

## 📊 Input Features Used

| Feature | Description |
|------|------------|
| CreditScore | Customer credit score |
| Geography | Country/region |
| Gender | Male/Female |
| Age | Customer age |
| Tenure | Years with the company |
| Balance | Account balance |
| NumOfProducts | Number of products used |
| HasCrCard | Credit card ownership |
| IsActiveMember | Active account status |
| EstimatedSalary | Estimated annual salary |

---

## 📈 Output

- **Churn Probability** (0–1)
- **Final Prediction**
  - ✅ Not Likely to Churn
  - ❌ Likely to Churn

---

## 🌐 Deployment

The application is deployed using **Streamlit Cloud**.

🔗 **Live App:**  
https://churnclassification-zmhtcuzrhhhgzibbge48nh.streamlit.app/

---

## 🚀 Future Improvements

- Add SHAP / feature importance visualizations
- Improve model accuracy with hyperparameter tuning
- Store predictions in a database
- Add authentication and user history tracking

---

## 👤 Author

**Yash Gehlot**  
Senior Undergraduate, **IIT Roorkee**  
Interests: Machine Learning, Data Analytics, AI Deployment
