# Physical Load Classification using IMU Sensor Data

## 📌 Project Overview
This project focuses on classifying **low vs high physical load** using **Inertial Measurement Unit (IMU)** sensor data.  
Unlike traditional Human Activity Recognition (HAR), which identifies *what* activity is being performed, this work aims to estimate **how physically demanding** a movement segment is using only accelerometer and gyroscope signals.

The project was developed as part of my MSc **Data Science and Computational Intelligence** coursework at **Coventry University**.

---

## 🎯 Objectives
- Quantify physical load from raw IMU signals  
- Engineer meaningful features from accelerometer and gyroscope data  
- Compare classical machine learning models for load classification  
- Evaluate model performance using robust validation techniques  

---

## 📂 Dataset
- IMU data consisting of **accelerometer and gyroscope signals**
- Signals segmented into fixed-length windows
- A proxy **physical load score** was computed using signal magnitudes
- Load scores were thresholded to create two classes:
  - **Low Load**
  - **High Load**

> Note: Dataset used is for academic and demonstration purposes.

---

## 🛠️ Feature Engineering
- Extracted **70+ statistical and signal-based features**, including:
  - Mean, standard deviation, variance
  - Signal magnitude area
  - Energy and peak-related features
- Features computed separately for accelerometer and gyroscope axes

---

## 🤖 Machine Learning Models
The following models were trained and evaluated:
- Logistic Regression
- Random Forest
- Support Vector Machine (RBF kernel)
- k-Nearest Neighbours (k-NN)
- Linear Discriminant Analysis (LDA)

---

## 📈 Results
- **Best-performing model:** Logistic Regression  
- **Classification accuracy:** ~**99.3%**  
- Strong and consistent performance across cross-validation and held-out test data

These results demonstrate that **classical machine learning models**, combined with effective feature engineering, can accurately distinguish physical load levels from IMU data.

---

## 🧰 Tech Stack
- **Programming:** Python  
- **Libraries:** pandas, NumPy, scikit-learn, matplotlib  
- **Techniques:**  
  - Data preprocessing  
  - Exploratory Data Analysis (EDA)  
  - Feature engineering  
  - Model training and evaluation  

---

## 📁 Project Structure
