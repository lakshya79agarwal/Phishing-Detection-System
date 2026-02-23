# Phishing-Detection-System

# 🛡️ Phishing Shield AI: Web-Based Detection System

## 📌 Project Overview

Phishing Shield AI is a full-stack Machine Learning application designed to identify fraudulent websites by analyzing their structural DNA. Unlike traditional blacklisting, this system uses **Random Forest Ensemble Learning** to detect "zero-day" phishing attacks based on 30 distinct URL features.

## 🚀 Key Features

* **High Accuracy:** Achieved **96.7% accuracy** using Random Forest Classifier.
* **Interactive UI:** Built with Streamlit for real-time security audits.
* **Explainable AI (XAI):** Provides tooltips and metrics to explain why a site was flagged.
* **Cloud Logging:** Integrated with **MongoDB Atlas** for persistent storage of scan history.
* **Real-time Confidence:** Displays probability scores for every prediction.

## 🛠️ Tech Stack

* **Language:** Python
* **ML Framework:** Scikit-Learn, Joblib, NumPy
* **Frontend:** Streamlit
* **Database:** MongoDB Atlas (NoSQL)
* **Deployment:** Streamlit Cloud & GitHub

## 📂 Project Structure

```text
├── app.py                   # Main Streamlit application
├── phishing_detector.pkl    # Trained Random Forest model (Pickle file)
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation

```

## 📊 How It Works

The system follows a 4-step pipeline:

1. **User Input:** The user provides a URL and specifies structural attributes (SSL, Traffic, etc.).
2. **Feature Processing:** Data is transformed into a 2D NumPy array compatible with the model.
3. **Inference:** The Random Forest model processes the input through multiple decision trees.
4. **Reporting:** Results are displayed instantly, and the audit is synced to the MongoDB cloud.

## 🛡️ Security & Privacy

This project uses **Streamlit Secrets** to manage MongoDB credentials, ensuring that sensitive database URIs are never exposed in the source code.

## 📝 Author

**Lakshya Agarwal** 
