# Customer Salary Predictor 💰

An interactive web application built with **Streamlit** and a machine learning model (Artificial Neural Network for **regression**) that predicts a customer's **estimated salary** based on demographic and banking features.

---

## 🌟 Features

* **Interactive User Interface:** Easily adjust customer parameters such as Geography, Age, Balance, Credit Score, Tenure, and Number of Products using intuitive sliders, number inputs, and dropdowns.
* **Real-time Prediction:** Instantly calculates and displays the predicted estimated salary (for example, `$140529.64`).
* **Regression Model:** Unlike a classification model that outputs a category (Yes/No), this model outputs a continuous numeric value.
* **Built with Streamlit:** Fast, lightweight, and responsive web framework for data-driven applications.

---

## 🛠️ Tech Stack

* **Frontend & UI:** [Streamlit](https://streamlit.io/)
* **Machine Learning:** Artificial Neural Network (ANN) regression using TensorFlow/Keras and Scikit-Learn
* **Language:** Python

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
streamlit run app.py
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

## 📸 Screenshot

Add a screenshot of the app to your repository (for example, in a `images/` folder) and link it here:

```markdown
![App Screenshot](images/app-screenshot.png)
```

---

## ☁️ Live Demo

Check out the live deployment of the app here: [Customer Salary Predictor Live App](https://your-app-name.streamlit.app/)

---

## 🔍 Classification vs. Regression

This project is a **regression** problem because the target (estimated salary) is a continuous number. Its companion project, the Customer Retention Predictor, is a **binary classification** problem that predicts whether a customer will churn.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---

## 📝 License

This project is open source.
