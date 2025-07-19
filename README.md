# Codtech-task-3
 🌼 Iris Flower Prediction API - CodTech Internship Task 3

This project is a complete end-to-end data science application that predicts the species of an iris flower using a machine learning model deployed as a web API using Flask.

## ✅ Project Objectives

- Train a classification model using the Iris dataset
- Build an API using Flask to serve the model
- Provide predictions based on user input
- Demonstrate a full ML pipeline: data → model → deployment

---

## 📊 Dataset Description

- **Source**: Built-in `sklearn.datasets.load_iris()`
- **Features**:
  - Sepal Length (cm)
  - Sepal Width (cm)
  - Petal Length (cm)
  - Petal Width (cm)
- **Target Classes**:
  - Setosa
  - Versicolor
  - Virginica

---

## 🛠️ Tech Stack

- Python
- Scikit-learn
- Flask
- NumPy
- Joblib

---

## 🧪 How to Run the Project Locally

### 1. Clone the Repository

```
git clone https://github.com/your-username/iris-flask-api.git
cd iris-flask-api
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

### 3. Start the Flask Server

```
python app.py
```

Server will start on: `http://127.0.0.1:5000`

---

## 🚀 API Usage

### Endpoint: `/predict`

- **Method**: POST
- **Content-Type**: `application/json`
- **Input JSON Format**:
```json
{
  "features": [5.1, 3.5, 1.4, 0.2]
}
```

- **Output JSON Format**:
```json
{
  "prediction": "setosa"
}
```

---

## 📁 Project Structure

```
iris-flask-api/
│
├── app.py              # Flask API
├── iris_model.pkl      # Trained ML model
├── requirements.txt    # Dependency file
└── README.md           # Project instructions and info
