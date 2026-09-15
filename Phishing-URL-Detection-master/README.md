# Phishing URL Detection

This is a machine learning project that detects whether a URL is **Phishing** or **Legitimate**.

The project takes a URL from the user, extracts some features from it, and uses a machine learning model to predict the result.

## Features

* Detects phishing and legitimate URLs
* Extracts URL and webpage features
* Uses machine learning for prediction
* Compares different machine learning models
* Has a simple Flask web application

## Machine Learning Models

The following models are used:

* Logistic Regression
* Decision Tree
* Random Forest
* SVM
* Gradient Boosting

After comparing the models, **Gradient Boosting** is used for the final prediction.

## Technologies Used

* Python
* Flask
* Pandas
* NumPy
* Scikit-learn
* BeautifulSoup
* HTML
* CSS

## How It Works

```text
Enter URL
   ↓
Extract URL features
   ↓
Machine Learning Model
   ↓
Prediction
   ↓
Phishing / Legitimate
```

## Project Files

```text
Phishing-URL-Detection/
│
├── pickle/
├── static/
├── templates/
├── app.py
├── feature.py
├── phishing.csv
├── requirements.txt
├── Procfile
├── Phishing URL Detection.ipynb
└── README.md
```

## How to Run

First, install the required packages:

```bash
pip install -r requirements.txt
```

Then run the application:

```bash
python app.py
```

Open the link shown in the terminal to use the application.

## Conclusion

This project uses machine learning to identify phishing URLs. It also shows how a machine learning model can be connected to a Flask web application.
