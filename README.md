# Heart Disease Prediction Using Machine Learning

A web-based machine learning application that predicts the possibility of heart disease using a **Decision Tree Classification model**.

The project combines a trained machine learning model with a **Flask backend** and an **HTML frontend**, allowing users to enter patient-related information through a simple web interface and receive a prediction.

## Project Overview

Heart disease prediction is a classification problem where machine learning can be used to identify patterns in patient data.

In this project, a **Decision Tree Classifier** is trained on a heart disease dataset and integrated into a Flask web application.

The application allows users to enter the required health-related values through a web form. The Flask backend processes the input, passes it to the trained model, and displays the prediction on the webpage.

> **Note:** This project is developed for educational and machine learning purposes only. It is not a medical diagnostic tool and should not replace professional medical advice.

## Features

* User-friendly web interface
* Heart disease prediction using Machine Learning
* Decision Tree Classification
* Flask-based backend
* HTML-based frontend
* Pre-trained model stored using Pickle
* Real-time prediction through the web form
* Simple and easy-to-use interface

## Machine Learning Model

The project uses a **Decision Tree Classifier**.

The notebook includes:

* Data loading and exploration
* Exploratory Data Analysis (EDA)
* Feature analysis
* Training and testing data split
* Decision Tree model training
* Model evaluation
* Confusion Matrix
* Classification Report
* ROC Curve and ROC-AUC analysis
* Decision Tree visualization
* Decision rule extraction
* Feature importance analysis
* Tree depth analysis
* Gini vs Entropy comparison

### Model Results

The Decision Tree model using the **Gini Index** achieved:

**Test Accuracy: 78.69%**

The notebook also compares Gini Index with Entropy:

| Criterion | Test Accuracy |
| --------- | ------------: |
| Gini      |        78.69% |
| Entropy   |        80.33% |

These results are specific to the train-test split and configuration used in this project.

## Technologies Used

* **Python**
* **Flask**
* **HTML**
* **CSS**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Pickle**
* **Google Colab**

## Project Structure

```text
heart-disease-prediction/
│
├── app.py
│       Flask backend application
│
├── DTModel.pkl
│       Trained Decision Tree machine learning model
│
├── requirements.txt
│       Required Python libraries
│
├── README.md
│       Project documentation
│
└── templates/
    │
    └── index.html
            Frontend user interface
```

## How the Application Works

```text
User Input
    ↓
HTML Frontend
    ↓
Flask Backend
    ↓
Pre-trained Decision Tree Model
    ↓
Prediction
    ↓
Result Displayed on Webpage
```

## Flask Backend

The `app.py` file handles the backend functionality of the application.

It:

1. Loads the trained Decision Tree model.
2. Starts the Flask application.
3. Receives input from the frontend.
4. Processes the user input.
5. Passes the input to the machine learning model.
6. Generates the prediction.
7. Sends the prediction back to the frontend.

## Frontend

The frontend is created using **HTML** and is located inside the `templates` folder.

```text
templates/
└── index.html
```

The `index.html` file provides the interface where users can enter the required patient information and view the prediction result.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/heart-disease-prediction.git
```

### 2. Open the project folder

```bash
cd heart-disease-prediction
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Flask application

```bash
python app.py
```

### 5. Open the application

After starting the Flask server, open the local URL shown in the terminal, usually:

```text
http://127.0.0.1:5000/
```

## Requirements

The main libraries required for this project are:

```text
Flask
numpy
pandas
scikit-learn
matplotlib
seaborn
```

## Machine Learning Workflow

```text
Dataset
   ↓
Data Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Train-Test Split
   ↓
Decision Tree Classifier
   ↓
Model Evaluation
   ↓
Model Saving
   ↓
Flask Integration
   ↓
Web Application
```

## Model File

The trained model is stored as:

```text
DTModel.pkl
```

The Flask application loads this saved model and uses it to generate predictions from user-provided input.

## Dataset

The machine learning model is trained using a heart disease dataset containing patient-related features and a target variable representing the presence or absence of heart disease.

The notebook used for model development and analysis is included separately as part of the project.

## Future Improvements

* Improve the frontend design
* Add better input validation
* Add additional machine learning models
* Compare multiple classification algorithms
* Deploy the Flask application online
* Add more detailed prediction information
* Improve model performance using hyperparameter tuning

## Disclaimer

This project is intended **only for educational and demonstration purposes**.

The predictions generated by this application should not be considered medical advice or a medical diagnosis. Users should consult a qualified healthcare professional for medical decisions.

## Author

**Yogesh Ankam**

Computer Science & Engineering (AI & ML)
DY Patil College of Engineering & Technology, Kolhapur
