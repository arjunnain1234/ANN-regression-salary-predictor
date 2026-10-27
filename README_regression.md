# Customer Salary Predictor 💰

An interactive web application built with **Streamlit** and an Artificial Neural Network (ANN) **regression** model that predicts a customer's **estimated salary** from demographic and banking features.

---

## 🌟 Features

* **Interactive User Interface:** Adjust customer parameters such as Geography, Age, Balance, Credit Score, Tenure, and Number of Products using dropdowns, sliders, and number inputs.
* **Real-time Prediction:** Instantly displays the predicted estimated salary (for example, `$140529.64`).
* **Regression Model:** Outputs a continuous numeric value instead of a category.
* **Pre-trained Model & Encoders:** The trained model, encoders, and scaler are saved as files and loaded by the app, so no retraining is needed to run it.

---

## 🛠️ Tech Stack

* **Frontend & UI:** [Streamlit](https://streamlit.io/)
* **Machine Learning:** ANN regression using TensorFlow/Keras
* **Preprocessing:** Scikit-Learn (label encoders, one-hot encoder, standard scaler)
* **Language:** Python

---

## 📁 Project Structure

```text
.
├── Churn_Modelling.csv          # Dataset used to train the model
├── salaryregression.ipynb       # Notebook: data preprocessing, model training, evaluation
├── regression_salary_pred.py    # Streamlit app (main file)
├── regression_model.h5          # Trained ANN regression model
├── label_encoder_gender.pkl     # Label encoder for Gender
├── label_encoder_yes_no.pkl     # Label encoder for Yes/No inputs
├── onehot_encoder_geo.pkl       # One-hot encoder for Geography
├── scaler.pkl                   # Scaler for numeric features
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## 🚀 Getting Started Locally

Follow these steps to set up and run the project on your machine.

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit App

```bash
streamlit run regression_salary_pred.py
```

---

## 📊 Input Features

The model uses the following customer attributes to predict the estimated salary:

* **Geography:** Customer's country of residence (e.g., France, Spain, Germany)
* **Gender:** Male or Female
* **Age:** Customer age (range: 18 - 90)
* **Balance:** Account balance
* **Credit Score:** Customer credit rating
* **Tenure:** Number of years the customer has been with the bank (range: 0 - 10)
* **Number of Products:** Number of bank products the customer uses (range: 1 - 4)
* **Has Credit Card:** Whether the customer holds a credit card (Yes/No)
* **Is Active Member:** Whether the customer is an active member (Yes/No)
* **Exited:** Whether the customer has left the bank (Yes/No)

---

## 🎯 Output

* **Predicted Estimated Salary:** A single numeric value in dollars, shown below the input form.

---

## ⚙️ How It Works

1. **Training (`salaryregression.ipynb`):** The notebook loads `Churn_Modelling.csv`, encodes categorical columns (Gender, Geography, Yes/No fields), scales numeric features, and trains an ANN regression model. The model and preprocessing objects are saved as `.h5` and `.pkl` files.
2. **Prediction (`regression_salary_pred.py`):** The Streamlit app loads those saved files, applies the same encoding and scaling to the user's inputs, and passes them to the model to get the predicted salary.

---

## 📸 Screenshot

<img width="1116" height="1334" alt="image" src="https://github.com/user-attachments/assets/569d0309-eb70-40c2-a238-7f4fa0e51b6f" />


## ☁️ Live Demo

Check out the live deployment of the app here: [Customer Salary Predictor Live App](https://your-app-name.streamlit.app/](https://salary-predictor-regression-based.streamlit.app)

---

## 🔍 Classification vs. Regression

This project is a **regression** problem because the target (estimated salary) is a continuous number. A classification problem, such as predicting whether a customer will churn, outputs a category (Yes/No) instead.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---

## 📝 License

This project is open source.
