# 📊 Transaction Analysis and Visualisation

**UEEN1043 Assignment – Group 17 (P2)**

**Authors:**

* CHIEW WEI HENG (2304580)
* TAN POULNY (2303710)

---

## 📌 Overview

This project analyzes financial transaction data to identify patterns, detect fraud trends, and visualize key insights.

The program performs:

* Data cleaning and preprocessing
* Merging multiple datasets
* Fraud classification and analysis
* Generation of visual insights through graphs

---

## 📁 Required Files

Ensure the following CSV files are in the same directory as the Python script:

* `transactions.csv` – Raw transaction data
* `merchant_codes.csv` – Merchant category mappings
* `fraud.csv` – Fraud status information

---

## ⚙️ Requirements

Install the required Python libraries before running:

```bash
pip install pandas matplotlib
```

---

## ▶️ How to Run

1. Place all required CSV files in the same folder as the script
2. Run the Python program:

```bash
python your_script_name.py
```

3. If files are missing, the program will display:

```text
File Not Found! Please insert the files in the same folder with this program.
```

---

## 🔄 Program Workflow

### 1. Data Loading

* Reads all CSV files into pandas DataFrames

### 2. Data Cleaning

* Removes rows with errors
* Handles missing values
* Converts transaction amounts into numeric format
* Removes zero-value transactions
* Sorts and removes duplicates

### 3. Data Merging

* Combines transaction, merchant, and fraud datasets
* Labels missing values as **"Unknown"**
* Classifies:

  * Transaction Type → Debit / Credit
  * Fraud Status → Fraud / Legitimate / Unknown

### 4. Analysis & Summary

Displays:

* Total transactions
* Debit vs Credit counts
* Fraud distribution
* Business category insights

### 5. Visualisation Output

The program generates **5 PNG graphs**:

1. `1_Average Transaction Per Date.png`
2. `2_Fraud Rate by Hour of Day.png`
3. `3_Fraud Distribution.png`
4. `4_Debit Credit by Fraud.png`
5. `5_Top 5 Fraud Business.png`

---

## 📈 Interpretation of Results

### 1. Average Transaction Amount per Date

* Shows spending trends over time
* Sudden spikes may indicate:

  * High-value transactions
  * Possible fraud bursts

---

### 2. Fraud Rate (%) by Hour of Day

* Identifies high-risk hours
* Fraud often occurs during **late-night or low-activity hours**

---

### 3. Overall Fraud Distribution

* Displays proportion of:

  * Fraudulent
  * Legitimate
  * Unknown transactions

👉 High fraud percentage may indicate system risk

---

### 4. Debit vs Credit by Fraud Status

* Compares fraud across transaction types
* Fraud is often more common in **debit transactions**

---

### 5. Top 5 Business Types by Fraudulent Amount

* Highlights industries most affected by fraud
* Indicates potentially vulnerable sectors

---

## ⚠️ Notes & Limitations

* Missing data is labeled as **"Unknown"**
* Results depend on dataset quality
* Not a real-time fraud detection system

---

## ✅ Conclusion

This project demonstrates how transaction data can be:

* Cleaned and structured
* Analyzed for fraud detection
* Visualized for decision-making

---

## 📌 Future Improvements

* Add machine learning for fraud prediction
* Real-time monitoring system
* Interactive dashboards (e.g., Plotly, Streamlit)
