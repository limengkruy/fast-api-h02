# Customer Churn Prediction with AI 🚀

## Overview
Welcome to the **Customer Churn Prediction Project**! 🎯 This AI-powered application uses the **Telco customer dataset** to predict whether a customer is likely to churn. We’ve built a robust machine learning model using **scikit-learn** and deployed it as a web API using **FastAPI**. Whether you’re an aspiring data scientist, a business analyst, or someone interested in customer retention strategies, this project is for you! 🔍

### 💡 **Why Customer Churn Prediction?**
Customer churn is one of the most important metrics for any business. Predicting which customers are at risk of leaving can help companies take action early—improving customer retention strategies, increasing revenue, and fostering long-term growth. This project applies machine learning to solve a real-world business problem.

---

## Tools & Technologies 🛠️

This project uses a collection of powerful tools to make the magic happen:

- **Git & GitHub**: For seamless version control and collaboration 🖥️
- **Scikit-learn**: A go-to library for machine learning in Python 📊
- **FastAPI**: To create an ultra-fast web API to deploy our AI model ⚡
- **Joblib**: To save and reload our trained model 💾
- **Uvicorn**: The lightning-fast ASGI server for running FastAPI ⚡
- **Pandas**: For all things data manipulation 🧑‍💻

---

## 🚀 How to Get Started

Follow these simple steps to get the project up and running locally:

### 1. Clone the repository:
    Start by cloning the repository to your local machine:
    ```bash
        git clone https://github.com/limengkruy/fast-api-h02.git
        cd fast-api-h02
    ```

### 2. Install the required dependencies:
    ```bash
        pip install -r requirements.txt
    ```

### 3. Train the model:
    Run the Python script to train the customer churn model and save it to a `.pkl` file:
    ```bash
    python train_model.py
    ```

### 4. Start the FastAPI server:
    ```bash
    uvicorn main:app --reload
    ```

### 5. To make predictions, send a POST request to `/predict` with the customer data in JSON format.

## API Endpoints

- **POST /predict**: Predict customer churn based on the input data.

    Example request:
    ```json
    {
        "seniorCitizen": 1,
        "partner": "Yes",
        "dependents": "No",
        "tenure": 25,
        "phoneService": "Yes",
        "multipleLines": "No",
        "internetService": "DSL",
        "onlineSecurity": "Yes",
        "onlineBackup": "No",
        "deviceProtection": "Yes",
        "techSupport": "No",
        "streamingTV": "Yes",
        "streamingMovies": "Yes",
        "contract": "One year",
        "paperlessBilling": "Yes",
        "paymentMethod": "Electronic check",
        "monthlyCharges": 89.45,
        "totalCharges": 2239.35,
        "churn": "Yes"
    }
    ```

    Example response:
    ```json
    {
        "prediction": "Yes"
    }
    ```

## Dependencies

This project requires the following Python packages:

- **scikit-learn**
- **fastapi**
- **joblib**
- **uvicorn**
- **pandas**

To install all dependencies, run:

```bash
pip install -r requirements.txt