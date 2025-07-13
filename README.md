# ✈️ Flight Fare Prediction Using Machine Learning

This project is a machine learning-based web application that predicts flight ticket prices based on various user inputs like date, time, stops, and airline. The project was developed as part of a 6-week summer internship under EESoc.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [Dataset](#-dataset)
- [Tech Stack](#-tech-stack)
- [Features](#-features)
- [Modeling](#-modeling)
- [Web Deployment](#-web-deployment)
- [How to Run](#-how-to-run)
- [Drawbacks](#-drawbacks)
- [Screenshots](#-screenshots)
- [License](#-license)

---

## 🔍 Overview

This project aims to predict the price of a flight ticket using machine learning regression models. The solution takes into account multiple factors such as departure/arrival time, total stops, airline, source, and destination.

---

## 📂 Dataset

- **Source:** [Kaggle - Flight Fare Dataset](https://www.kaggle.com/datasets)
- **Attributes Used:**
  - Date of Journey
  - Departure Time
  - Arrival Time
  - Duration
  - Total Stops
  - Airline
  - Source and Destination

---

## 🛠️ Tech Stack

- **Language:** Python
- **Framework:** Flask
- **ML Model:** Random Forest Regressor
- **Frontend:** HTML, CSS
- **Deployment:** Render
- **Libraries:**
  - Pandas
  - Numpy
  - Scikit-learn
  - Matplotlib & Seaborn (for EDA)

---

## ✅ Features

- Clean UI for user input
- Accepts airline, source, destination, journey date and time
- Predicts flight fare instantly
- Deployed on the web via Render

---

## 🧠 Modeling

- **Preprocessing:**
  - Converted date-time features
  - Label and one-hot encoding of categorical features
  - Feature engineering: duration (hours & minutes), departure/arrival components

- **Model Used:**
  - Random Forest Regressor
  - Trained and tested on Kaggle dataset

- **Performance:**
  - R² Score: ~0.83
  - MAE, RMSE calculated during evaluation

---

## 🌐 Web Deployment

- Trained model saved as `flight_rf.pkl`
- Deployed using Flask web server
- Render used for live deployment

🔗 [Live App](#) *(Add your Render link here)*

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/flight-price-predictor.git
cd flight-price-predictor

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py
