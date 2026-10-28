# 🧠 ANN-Based Customer Churn Classification

An end-to-end deep learning project that predicts whether a bank customer is likely to leave the bank using an **Artificial Neural Network (ANN)**. The project combines customer data preprocessing, neural network training, and an interactive Streamlit application to generate churn predictions.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Dataset](#-dataset)
- [Machine Learning Workflow](#-machine-learning-workflow)
- [ANN Architecture](#-ann-architecture)
- [Installation](#-installation)
- [Running the Application](#-running-the-application)
- [Deployment](#-deployment)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 📖 Overview

Customer churn is a major challenge in the banking industry, as losing customers can affect revenue and long-term growth. This project uses an Artificial Neural Network to identify customers who may be likely to leave based on their demographic and banking information.

The trained model processes customer attributes and predicts the probability of churn. The prediction can help demonstrate how deep learning can support customer retention and data-driven decision-making.

---

## ✨ Features

- 🧠 Customer churn prediction using an Artificial Neural Network.
- 📊 Data preprocessing and feature engineering.
- 🔤 Encoding of categorical variables.
- 📏 Feature scaling for numerical inputs.
- 🎯 Binary classification of customer churn.
- 📈 Model training and performance evaluation.
- 🌐 Interactive interface for generating predictions.
- ☁️ Streamlit deployment for easy access.

---

## 🛠️ Tech Stack

| Component | Technologies |
|---|---|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Deep Learning | TensorFlow, Keras |
| Data Preprocessing | Scikit-learn |
| Model Evaluation | Scikit-learn |
| Development Environment | Jupyter Notebook |
| Web Application | Streamlit |

---

## 🗃️ Dataset

The project uses the bank customer churn dataset, commonly known as `Churn_Modelling.csv`.

The dataset contains customer demographic and account-related information that can be used to predict whether a customer exits the bank.

### Input features

| Feature | Description |
|---|---|
| `CreditScore` | Customer's credit score |
| `Geography` | Customer's country or region |
| `Gender` | Customer's gender |
| `Age` | Customer's age |
| `Tenure` | Number of years with the bank |
| `Balance` | Customer's account balance |
| `NumOfProducts` | Number of banking products held |
| `HasCrCard` | Whether the customer has a credit card |
| `IsActiveMember` | Whether the customer is an active member |
| `EstimatedSalary` | Estimated annual salary |

**Target variable:** `Exited`

- `0` — Customer did not leave the bank.
- `1` — Customer left the bank.

Identifier columns that do not contribute meaningfully to prediction, such as customer ID and surname, can be excluded during preprocessing.

---

## 🔄 Machine Learning Workflow

1. **Data Loading:** Load the customer churn dataset into a Pandas DataFrame.
2. **Data Preprocessing:** Separate input features and the target variable, and remove irrelevant identifiers.
3. **Categorical Encoding:** Convert categorical variables into numerical representations using suitable encoding techniques.
4. **Feature Scaling:** Standardize numerical features to help the neural network train effectively.
5. **Train-Test Split:** Divide the data into training and testing sets.
6. **ANN Development:** Build and train a neural network for binary classification.
7. **Model Evaluation:** Evaluate predictions using suitable classification metrics.
8. **Model Persistence:** Save the trained model and preprocessing objects for reuse.
9. **Prediction:** Generate churn predictions for customer inputs.
10. **Deployment:** Provide an interactive prediction interface through Streamlit.

---

## 🧠 ANN Architecture

An Artificial Neural Network consists of interconnected layers that learn patterns from customer data.

A typical binary classification architecture includes:

- **Input Layer:** Receives the preprocessed customer features.
- **Hidden Layers:** Learn complex relationships using neurons and activation functions such as ReLU.
- **Output Layer:** Uses a sigmoid activation function to produce a churn probability.

The predicted probability is converted into a binary class using a classification threshold.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Shilpa56721/ANN-Classification-Churn.git
cd ANN-Classification-Churn
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

If the repository contains a Streamlit entry point named `app.py`, run:

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal to access the application.

Enter the required customer details and submit them to receive a churn prediction.

---

## ☁️ Deployment

The application can be hosted using Streamlit Community Cloud.

1. Push the project to GitHub.
2. Ensure the dependency file and required model artifacts are available.
3. Open [Streamlit Community Cloud](https://share.streamlit.io/).
4. Connect the GitHub repository.
5. Select the application's main Python file.
6. Deploy the application.

---

## 🔮 Future Improvements

- Improve model performance through hyperparameter tuning.
- Add a confusion matrix and classification report.
- Evaluate precision, recall, F1-score, and ROC-AUC.
- Address class imbalance if required.
- Display churn probabilities alongside predicted classes.
- Add batch predictions for multiple customers.
- Improve the user interface and prediction explanations.

---

## 👩‍💻 Author

**Shilpa**

GitHub: [@Shilpa56721](https://github.com/Shilpa56721)

**Repository:** [ANN-Classification-Churn](https://github.com/Shilpa56721/ANN-Classification-Churn)

---

⭐ If you find this project useful, consider giving the repository a star!
