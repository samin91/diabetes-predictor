# Diabetes Progression Predictor

A REST API built with **FastAPI** to predict diabetes progression based on patient data.  
The application is **Dockerized** for easy deployment and reproducibility.  
The prediction model is trained using **scikit-learn**.

---
I am just testing the github actions 

## 🛠 Tools & Technologies

- **Python 3.11** – core programming language  
- **FastAPI** – web framework for building REST APIs  
- **Uvicorn** – ASGI server to run the FastAPI app  
- **scikit-learn** – machine learning model training and prediction  
- **Docker** – containerization for consistent deployment  
- **Pydantic** – data validation for API input  

## 📁 Project Structure
```
diabetes-predictor/
├── app/
│ ├── main.py # FastAPI application
│ ├── __init__.py 
├── models/
│ └── diabetes_model.pkl
├── requirements.txt # Python dependencies
├── Dockerfile # Docker build instructions
├── README.md
```

## ⚡ Features

- Health check endpoint (`GET /`)  
- Model prediction endpoint (`POST /predict`)  
- Validates input data using Pydantic schemas  
- Returns predicted diabetes progression  
- Fully Dockerized for deployment  

---

## 🚀 Installation & Running Locally

Clone the repository:

```
git clone https://github.com/<your-username>/diabetes-predictor.git
cd diabetes-predictor
```
Create a virtual environment and install dependencies:

```
python -m venv venv
source venv/bin/activate      # On macOS/Linux
venv\Scripts\activate         # On Windows
pip install --upgrade pip
pip install -r requirements.txt
```

Run the FastAPI app:

```
python -m uvicorn app.main:app --reload --port 8000
```

Visit in browser:
```
Health check: http://127.0.0.1:8000/

Interactive docs: http://127.0.0.1:8000/docs
```


