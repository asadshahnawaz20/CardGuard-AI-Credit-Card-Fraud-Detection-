# Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using **Machine Learning** techniques. Since fraudulent cases are rare compared to legitimate ones, the dataset is **highly imbalanced**, making fraud detection a challenging task.
An interactive **Streamlit web app** is developed for real-time prediction of transactions as *Legitimate* or *Fraudulent*.

---

## 📊 Dataset

* Source: [Kaggle – Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)

* Features:

  * **Time**: Seconds elapsed since the first transaction
  * **V1 – V28**: Anonymized PCA-transformed features
  * **Amount**: Transaction amount in USD
  * **Class**: Target variable → `0` = Legitimate, `1` = Fraudulent

* Total transactions: **284,807**

* Fraudulent transactions: **492** (≈0.17%)

---

## ⚙️ Project Workflow

1. **Data Preprocessing**

   * Handle class imbalance (undersampling)
   * Normalize transaction amounts
2. **Exploratory Data Analysis (EDA)**

   * Visualize class imbalance
   * Compare features for fraud vs legitimate cases
3. **Model Training**

   * Logistic Regression (binary classification)
   * Evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
4. **Deployment**

   * Streamlit app with user input for prediction

---

## 🚀 How to Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   .venv\Scripts\activate   # Windows
   source .venv/bin/activate  # Linux/Mac
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

---

## 🖥️ Streamlit App UI

* Enter transaction feature values (comma-separated).
* Click **Run Fraud Check**.
* Get instant prediction: ✅ Legitimate or ⚠️ Fraudulent.

---

## 📈 Results

* Model trained on balanced dataset of 492 fraud & 492 legit samples.
* Example performance (test data):

  * Accuracy: 0.934010152284264


---

## 🛠️ Tech Stack

* **Python**
* **Pandas, NumPy**
* **Scikit-learn**
* **Streamlit**

---

## 📌 Future Improvements

* Use advanced models (Random Forest, XGBoost, Neural Networks).
* Apply SMOTE/ADASYN for handling imbalance.
* Deploy on cloud (Heroku/AWS).
* Add visualization dashboard for transaction analytics.

---

## 🙌 Acknowledgments

* Dataset: ULB Machine Learning Group (Kaggle).
* Libraries: Scikit-learn, Streamlit.

---

