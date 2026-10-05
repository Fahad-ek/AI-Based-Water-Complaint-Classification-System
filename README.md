# AI-Based-Water-Complaint-Classification-System
NLP-based water complaint classification system using TF-IDF and Logistic Regression to automatically categorize water-related complaints into different service categories.
# 💧 Smart Water AI

Smart Water AI is a machine learning-based water management project designed to support **water demand prediction, abnormal consumption detection, and water complaint classification** through an interactive Gradio application.

## 🚀 Project Overview

The system combines multiple machine learning and NLP modules to provide a simple AI-powered platform for analyzing water-related information.

### 1. 💧 Water Demand Prediction

The system predicts expected water consumption based on factors such as:

* Area/Ward
* Number of water connections
* Temperature
* Rainfall
* Day of the week
* Month
* Previous-day consumption
* 7-day average consumption
* 30-day average consumption
* Available water supply

The trained water demand model is loaded using **Joblib** and used to generate the predicted consumption in liters.

### 2. 🚨 Anomaly Detection

The project also identifies unusual water consumption patterns using an **Isolation Forest-based anomaly detection model**.

The anomaly detection module analyzes:

* Water consumption
* Previous-day consumption
* 7-day average consumption
* 30-day average consumption
* Demand ratio

The system classifies the consumption pattern as either **Normal** or **Abnormal**.

### 3. 📝 NLP Water Complaint Analysis

The NLP module automatically analyzes water-related complaints and classifies them into different categories:

* Leakage
* Low Water Supply
* High Consumption
* Water Quality
* Meter Problem
* Other

The text is cleaned using basic preprocessing techniques and converted into numerical features using **TF-IDF Vectorization** with unigram and bigram features.

A **Logistic Regression** classifier is then used to predict the complaint category and provide a confidence score.

The system supports both **English and Malayalam complaint examples**.

## 📊 Demand Risk Classification

Based on the predicted consumption and available water supply, the system calculates a **Demand Ratio** and classifies the water demand risk as:

* 🟢 LOW
* 🟠 MEDIUM
* 🔴 HIGH

This helps indicate whether the predicted demand is within the available water supply capacity.

## 🖥️ Interactive Web Application

The complete project is deployed as an interactive **Gradio web application** with separate sections for:

* Water Demand Prediction
* NLP Water Complaint Analysis
* About Project

The interface provides prediction results, demand ratio, risk level, anomaly status, complaint category, confidence score, and processed text.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* TF-IDF
* Logistic Regression
* Isolation Forest
* Joblib
* Gradio
* Regular Expressions (RE)
* Natural Language Processing (NLP)

## 🎯 Key Features

* Water demand prediction
* Consumption anomaly detection
* Water complaint classification
* Demand risk assessment
* English and Malayalam complaint support
* Confidence score for NLP predictions
* Interactive Gradio interface
* Pre-trained model integration

## 📌 Project Goal

The goal of Smart Water AI is to demonstrate how **Machine Learning and Natural Language Processing** can be combined to support smarter water-demand monitoring, identify unusual consumption patterns, and organize water-related complaints automatically.
