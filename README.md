# 🎯 Placement Prediction using Random Forest (Deployed on Render)

This project predicts whether a student is likely to be placed or not, based on academic and personal attributes. The model is deployed using **Render**, with a very basic user-facing web interface to interactively input data and get predictions.

## 🚀 Live App

🌐 **[Click here to try it](https://placement-prediction.onrender.com)**  
_(Replace with your actual Render URL if needed)_

---

## 🧠 Problem Statement

Predict placement outcomes based on student features using machine learning.

### 🔍 Input Features
- IQ Score (Numeric)
- 10th Percentage
- 12th Percentage
- CGPA (College GPA)
- Communication Skill (Numeric)

### 🧾 Output
- **Prediction**: Whether the student is placed or not.

---

## 🛠️ Machine Learning Model

- **Algorithm**: Random Forest Classifier
- **Preprocessing**: Standardization or basic scaling (if needed)
- **Training**: Offline using cleaned data
- **Serving**: Via API endpoint using Flask

---

## 💻 Frontend

- Very basic HTML form
- Accepts numeric inputs for each of the above features
- On submit, the form sends the data to the backend and displays prediction

---

## ⚙️ Deployment: Render

### 🧩 Stack Used
- **Backend**: Python (Flask)
- **Model**: Pickle-serialized Random Forest
- **Frontend**: HTML + basic CSS
- **Deployment**: [Render.com](https://render.com)

---

## 🧪 Issues Faced and Solutions

### 1. ❌ **Version Incompatibility**
- Some libraries (like `numpy`, `setuptools`) are not yet stable with **Python 3.13**
- ❗ **Render uses Python 3.13 by default**, causing dependency failures

✅ **Solution**:
- Explicitly specified the Python version **3.11.8** using a `runtime.txt` file in the root of the project:
  ```txt
  python-3.11.0
