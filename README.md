# 🏠 Real Estate Price Prediction App

This is an end-to-end machine learning project that predicts real estate prices based on user inputs such as square footage, number of bedrooms, and location. It consists of a **machine learning model**, a **Flask backend server**, and a **client-side web application**.

---

## 🎯 Project Overview

This project walks through the entire lifecycle of building a machine learning-powered web application:

1. 📊 **Model Building**: Train a linear regression model using the Banglore house price dataset from Kaggle.
2. 🔌 **Backend API**: Deploy the trained model via a Flask API server to serve real-time predictions.
3. 🌐 **Frontend Website**: A simple HTML/CSS/JavaScript interface to input data and fetch predictions.

---

## 🧠 Technologies & Tools Used

- **Python** for scripting and modeling
- **NumPy** and **Pandas** for data processing
- **Matplotlib** for data visualization
- **Scikit-learn (sklearn)** for model training
- **Jupyter Notebook** for experimentation
- **Flask** for the backend server
- **HTML/CSS/JavaScript** for frontend UI
- **VS Code / PyCharm** as IDEs

---

## 🗃️ Folder Structure

```
Real-Estate-Price-Prediction/
│
├── client/
│ ├── app.html # UI for user input
│ ├── app.css # Styles
│ └── app.js # JS logic for API call
│
├── model/
│ ├── banglore_home_prices_final.ipynb # Notebook with full model pipeline
│ ├── banglore_home_prices_model.pickle # Trained sklearn model
│ ├── bengaluru_house_prices.csv # Dataset from Kaggle
│ └── columns.json # Feature/column data for prediction
│
├── server/
│ ├── artifacts/ # Saved intermediate files (if any)
│ ├── server.py # Flask app for backend API
│ └── util.py # Helper functions for model loading & prediction
│
├── README.md
```

---

## 🚀 How It Works

1. User opens the web UI (HTML form).
2. Enters home details like area (sqft), number of bedrooms, and location.
3. Client-side JS sends a POST request to Flask API (`/predict_home_price`).
4. Flask server loads the model and returns the predicted price.
5. Price is displayed dynamically in the UI.

---

## 🔧 Setup Instructions

### ⚙️ Step 1: Clone the Repo

```bash
git clone https://github.com/SwedeshnaMishra/Real-Estate-Price-Prediction.git
cd Real-Estate-Price-Prediction
```

### 🧠 Step 2: Setup Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt  # Create this if missing
```

### 🔥 Step 3: Run Flask Server
```bash
cd server
python server.py
```

### 🌐 Step 4: Run Frontend
Open `client/app.html` in your browser. Ensure the server is running at `http://127.0.0.1:5000/`.

---

## 🧪 Model Pipeline
- Data loading and preprocessing
- Outlier detection and removal
- Feature engineering (location encoding)
- Dimensionality reduction
- Train/test split
- GridSearchCV for hyperparameter tuning
- K-Fold Cross-Validation

---

## For Contributing
If you want to contribute to this project, please follow these steps:
- `Fork` the repository.
- Create a new branch `(git checkout -b feature/your-feature-name)`.
- Make your changes and commit them `(git commit -m 'Add some feature')`.
- Push to the branch `(git push origin feature/your-feature-name)`.
- Open a pull request.

---

## Project Maintainer
**Github:** [Swedeshna Mishra](https://github.com/SwedeshnaMishra)
