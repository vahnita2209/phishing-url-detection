# Phishing URL Detection

A machine learning-based web application that analyzes URLs and predicts whether they are **legitimate or potentially phishing URLs**.

The project extracts multiple URL and webpage-based features and compares different machine learning algorithms to identify the model that performs best for phishing URL classification. A Flask web application is used to provide a simple interface where users can enter a URL and receive a prediction.

## Features

* Detects potentially phishing and legitimate URLs
* Extracts **30 URL and webpage-based features**
* Compares multiple machine learning classification models
* Displays prediction results through a Flask web application
* Uses the best-performing trained model for prediction
* Provides model evaluation using accuracy, precision, recall, and F1-score
* Includes feature importance analysis for understanding important phishing indicators

## Machine Learning Models

The following models are evaluated in the project:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* Gradient Boosting Classifier

The models are compared using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Gradient Boosting is used as the final prediction model after comparing the performance of the selected models.

## Technologies Used

* **Python**
* **Flask**
* **Scikit-learn**
* **Pandas**
* **NumPy**
* **BeautifulSoup**
* **Requests**
* **Whois**
* **Matplotlib**
* **HTML/CSS**

## How It Works

The system follows these main steps:

```text
User enters URL
       ↓
URL and webpage feature extraction
       ↓
30 features generated
       ↓
Trained ML model
       ↓
Phishing / Legitimate prediction
       ↓
Result displayed in Flask web application
```

## Feature Extraction

The system extracts characteristics from the URL and webpage, including:

* IP address usage
* URL length
* URL shortening
* `@` symbol usage
* Redirection patterns
* Prefix/suffix usage
* Number of subdomains
* HTTPS usage
* Domain registration information
* Favicon information
* Non-standard ports
* External requests
* Anchor links
* Script and link information
* Form handling
* Email information
* Website forwarding
* Popup usage
* Iframe usage
* Domain age
* DNS information
* Links on the webpage
* Other URL and webpage characteristics

These features are converted into numerical values and passed to the machine learning model.

## Project Structure

```text
Phishing-URL-Detection/
│
├── pickle/
│   └── model.pkl
│
├── static/
│   └── styles.css
│
├── templates/
│   └── index.html
│
├── Phishing URL Detection.ipynb
├── phishing.csv
├── feature.py
├── app.py
├── requirements.txt
├── Procfile
└── README.md
```

## Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Phishing-URL-Detection
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Flask application

```bash
python app.py
```

The application will start locally and can be accessed through the URL shown in the terminal.

## Model Evaluation

The project compares five machine learning models and evaluates their performance on the phishing URL dataset.

The final results should be updated below using the results obtained from the current version of the notebook:

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |        — |         — |      — |        — |
| Decision Tree       |        — |         — |      — |        — |
| Random Forest       |        — |         — |      — |        — |
| SVM                 |        — |         — |      — |        — |
| Gradient Boosting   |        — |         — |      — |        — |

> **Note:** The values above should be replaced with the results generated from the current notebook rather than using results from the original project.

## Feature Importance

Feature importance is analyzed using the trained Gradient Boosting model to understand which URL and webpage characteristics contribute most to the classification.

This helps identify patterns commonly associated with phishing URLs and provides better interpretability of the machine learning model.

## Conclusion

This project demonstrates how machine learning can be applied to detect potentially phishing URLs based on URL and webpage characteristics.

Five classification algorithms are compared to understand their performance on the dataset. The best-performing model is then used in a Flask-based web application to provide predictions for newly entered URLs.

The project also demonstrates the complete machine learning workflow, including:

* Data exploration
* Feature extraction
* Data preprocessing
* Model training
* Model comparison
* Performance evaluation
* Feature importance analysis
* Model deployment using Flask

## Future Improvements

* Add a larger and more recent phishing URL dataset
* Improve feature extraction using modern URL-based features
* Add real-time threat intelligence APIs
* Improve the web interface
* Deploy the application using a cloud platform
* Add confidence-based warnings for suspicious URLs

## Disclaimer

This project is intended for **educational and research purposes**. The prediction should not be treated as a guaranteed indication that a website is safe or malicious.
