# 💳 Credit Risk Prediction App

A Streamlit web application that predicts **whether a loan should be granted to a customer** based on their financial and credit-related information. This project models **credit risk** by estimating the probability of default, calculating a credit score, and assigning a credit rating using a trained logistic regression model.

---

## 📌 Key Features

- 🧾 **Input Financial and Credit Information** of the customer
- 🔢 **Loan-to-Income Ratio** calculated on the fly
- 📉 Predicts the **probability of default**
- 🧮 Calculates a **credit score** (300–900 scale)
- ⭐ Classifies into **credit rating categories**: Poor, Average, Good, Excellent
- 🖥️ Interactive UI with **Streamlit**

---

## 🛠️ Tech Stack

| Component             | Technology Used                  |
|----------------------|----------------------------------|
| Frontend             | Streamlit                        |
| Backend              | Python                           |
| ML Model             | Logistic Regression (joblib)     |
| Feature Engineering  | Scikit-learn preprocessing       |
| DataFrame Handling   | pandas, numpy                    |
| Model Inference      | Manual logistic transformation   |

---

## 📁 File Structure

```plaintext
.
├── main.py                       # Streamlit app UI
├── prediction_helper.py         # Model logic and preprocessing
├── model_data.joblib          # (Assumed) Trained model with scaler and metadata
├── requirements.txt             # Required Python packages
├── README.md                    # You're reading it!

---
```

## 🚀 How to Run the App Locally

1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/credit-risk-analysis-app.git
cd credit-risk-analysis-app
```
2️⃣ Set up a Virtual Environment (Optional but Recommended)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3️⃣ Install the Required Packages
```
pip install -r requirements.txt

```
5️⃣ Run the Streamlit App
```
streamlit run main.py
```
## 💻 UI Overview

Once the app is running, you'll be able to:

Input features like:

-  Age

-  Income

-  Loan Amount

-  Delinquency Ratios

-  Loan Purpose, Type, Residence, etc.

**Click "Calculate Risk"**

See the predicted:

Default Probability

Credit Score (300–900)

Rating (Poor, Average, Good, Excellent)

###  📊 Credit Score Logic

Credit Score Range	Rating

- 300 - 499:	Poor

- 500 - 649:	Average

- 650 - 749:	Good

- 750 - 900:	Excellent

### 🧠 Model Explanation

-  Logistic Regression is used for classification.

📦 Requirements
-  Here are the key libraries used (add to requirements.txt):

**streamlit**

**pandas**

**numpy**

**scikit-learn**

**joblib**
