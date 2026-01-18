🚀 ChurnBuster – Customer Churn Prediction & Retention Dashboard
----------------------------------------------------------------------------------------------------------------------------------------

I built this project to help businesses predict customer churn before it happens. Most churn systems stop at a yes/no prediction, which isn’t enough for real decision-making. This project goes further by estimating churn probability, optimizing business intervention decisions, and explaining why customers are likely to leave.

It’s a hands-on, end-to-end project where I combined machine learning, business-driven optimization, explainable AI, interactive dashboards, and live deployment to build a practical churn analytics system.

🌐 Live Streamlit Dashboard (Deployed):
----------------------------------------------------------------------------------------------------------------------------------------

https://endurable-thwartedly-somer.ngrok-free.dev

🎯 Why I Built This
----------------------------------------------------------------------------------------------------------------------------------------

I wanted to move beyond basic churn classification and build something closer to how churn is handled in real businesses. With this project, I can:

Predict churn using probability scores, not just binary labels

Handle class imbalance properly

Optimize churn decisions using cost-based thresholding

Explain model predictions using Explainable AI (SHAP)

Visualize insights through a live interactive dashboard

🧠 Key Features
----------------------------------------------------------------------------------------------------------------------------------------

Churn prediction using XGBoost

Probability-based churn risk scoring

Cost-based threshold optimization for business decisions

Explainable AI with SHAP (global & individual explanations)

Interactive Streamlit dashboard

Publicly accessible deployment via Ngrok

Secure environment variable handling using .env

📊 Dataset
----------------------------------------------------------------------------------------------------------------------------------------

This project uses the Telco Customer Churn dataset, a publicly available, real-world–inspired dataset that simulates customer behavior in a telecommunications company.

🔗 Dataset Source:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

Dataset highlights:

~7,000 customer records

Combination of categorical and numerical features

Customer demographics, service usage, contract details, and billing data

Target variable: Churn (Yes / No)

Realistic class imbalance, suitable for applied machine learning

The dataset is widely used for churn prediction research and is ideal for demonstrating probability-based modeling, cost-sensitive decision-making, and explainable AI.

🛠️ Tech Stack I Used
----------------------------------------------------------------------------------------------------------------------------------------

Python – Core programming language

XGBoost – Gradient boosting model for churn prediction

Scikit-learn – Data preprocessing, evaluation, and metrics

SHAP – Model explainability and feature impact analysis

Streamlit – Interactive dashboard and UI

Ngrok – Public deployment via secure HTTPS tunnel

Pandas & NumPy – Data manipulation and analysis

Google Colab – Experimentation and development environment

🔐 Setting Up the Environment
----------------------------------------------------------------------------------------------------------------------------------------

I use Ngrok to deploy the Streamlit dashboard publicly, keeping the authentication token secure in a .env file.

Create a .env file:

NGROK_AUTH_TOKEN=my_ngrok_auth_token_here


Load it in Python:

from dotenv import load_dotenv
import os

load_dotenv()

NGROK_TOKEN = os.getenv("NGROK_AUTH_TOKEN")



📌 Dashboard Capabilities
----------------------------------------------------------------------------------------------------------------------------------------

The Streamlit dashboard allows users to:

View churn probability distribution

Adjust churn-risk threshold dynamically

Identify high-risk customers

Monitor total customers and churn-prone segments

Inspect top churn candidates in real time

🏗️ Architecture
----------------------------------------------------------------------------------------------------------------------------------------

Customer Churn Dataset (CSV)
 →
 Data Cleaning & Feature Encoding
 →
 XGBoost Churn Prediction Model
 →
 Probability Estimation
 →
 Cost-Based Threshold Optimization
 →
 Explainability with SHAP
 →
 Streamlit Dashboard
 →
 Public Access via Ngrok

🚀 Where I See It Being Useful
----------------------------------------------------------------------------------------------------------------------------------------

Customer retention analytics

Telecom, SaaS, and subscription-based businesses

Data-driven churn intervention strategies

Business decision support systems

Applied machine learning portfolios

🔮 What I Want to Add Next
----------------------------------------------------------------------------------------------------------------------------------------

Customer Lifetime Value (CLV) integration

Retention strategy simulation (offers, discounts, incentives)

FastAPI-based model serving

Cloud deployment (AWS / GCP)

User authentication and role-based dashboards
