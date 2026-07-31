# 🏠 Bangalore Home Price Prediction

A Machine Learning web application that predicts **Bangalore house prices** based on property details such as **area, BHK, bathrooms, and location**. The project uses a trained **Linear Regression** model served through a **Flask API** with a simple and interactive web interface.

## 🚀 Live Demo

🌐 **Try the application here:**

**https://property-prediction-5.onrender.com/**

---

## 📌 Features

* 📍 Predict house prices in Bangalore
* 🏡 Enter Area (Square Feet), BHK, Bathrooms, and Location
* 🤖 Machine Learning model trained using Scikit-learn
* 🌐 Flask REST API
* 🎨 Responsive frontend using HTML, CSS, JavaScript, and jQuery
* 📋 Dynamic location dropdown loaded from the trained dataset

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* jQuery

### Backend

* Python
* Flask

### Machine Learning

* Scikit-learn
* NumPy
* Pandas

### Model Serialization

* Pickle

---

## 📂 Project Structure

```text
Bangalore-Home-Price-Prediction/
│
├── artifacts/
│   ├── columns.json
│   └── property_prediction.pickle
│
├── static/
│   ├── app.css
│   └── app.js
│
├── templates/
│   └── app.html
│
├── server.py
├── util.py
├── requirements.txt
├── README.md
└── Bengaluru_House_Data.csv
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Bangalore-Home-Price-Prediction.git
```

### Navigate to the project

```bash
cd Bangalore-Home-Price-Prediction
```

### Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
python server.py
```

Open your browser and visit:

```
http://127.0.0.1:5000/
```

---

## 🧠 Machine Learning Pipeline

* Data Cleaning
* Feature Engineering
* Outlier Removal
* One-Hot Encoding
* Model Training
* Model Evaluation
* Model Serialization (Pickle)
* Flask API Integration

---

## 📡 API Endpoints

### Get Available Locations

**GET**

```
/get_location_names
```

Example Response

```json
{
  "locations": [
    "1st block jayanagar",
    "electronic city",
    "whitefield"
  ]
}
```

---

### Predict Home Price

**POST**

```
/predict_home_price
```

Parameters

| Parameter  | Type    |
| ---------- | ------- |
| total_sqft | float   |
| bhk        | integer |
| bath       | integer |
| location   | string  |

Example Response

```json
{
    "estimated_price": 82.45
}
```

---

## 📸 Application Preview

The application allows users to:

* Enter the property area
* Select the number of bedrooms (BHK)
* Select the number of bathrooms
* Choose a location
* Click **Estimate Price**
* Instantly view the predicted house price

---

## 💡 Future Improvements

* Improve UI/UX
* Deploy with Docker
* Add confidence score for predictions
* Support multiple regression models
* Add property image upload
* Integrate maps for location selection
* Store prediction history
* Add user authentication

---

## 📊 Dataset

The model is trained using the **Bengaluru House Price Dataset**, which contains:

* Location
* Total Square Feet
* Number of Bedrooms
* Number of Bathrooms
* Price

---

## 🌐 Live Website

**https://property-prediction-5.onrender.com/**

---

## 👨‍💻 Author

**Rishabh Jha**

If you found this project useful, consider giving it a ⭐ on GitHub!

---

## 📄 License

This project is licensed under the MIT License.
