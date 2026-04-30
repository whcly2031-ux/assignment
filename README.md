# 📊 Transaction Analysis and Visualisation Program

**UEEN1043 Assignment – Group 17 (P2)**

**Written By:**
* CHIEW WEI HENG (2304580)
* TAN POULNY (2303710)

---

## 📌 Overview
This project analyzes financial transaction data to identify patterns, detect fraud trends, and generate visualizations based on processed data.

The program performs:

* Data cleaning and preprocessing
* Merging multiple datasets
* Fraud classification and analysis
* Generation of visual insights through graphs

---
To use this program, several requirements must be met:
## 📁 Required Files
You are to ensure the following CSV files are in the same directory as the Python script:
* `transactions.csv` – Raw transaction data
* `merchant_codes.csv` – Merchant category mappings
* `fraud.csv` – Fraud status information

---
## ⚙️ Requirements
1. Install Anaconda Distribution (Python Toolkit including libraries)
   Link: https://www.anaconda.com/download
2. Install Spyder IDE
   Link: https://www.spyder-ide.org/download?os=windows&arch=x64
3. When download completes, follow the installer steps to complete setup
4. Launch Spyder IDE

## ▶️ How to Run
1. Place all required CSV files in the same folder as the script (suggested: Desktop)
2. In Spyder IDE, open and run this Python program.
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

The program generates **5 graphs in PNG format**:
1. `1_Average Transaction Per Date.png`
2. `2_Fraud Rate by Hour of Day.png`
3. `3_Fraud Distribution.png`
4. `4_Debit Credit by Fraud.png`
5. `5_Top 5 Fraud Business.png`

You may then find the respective image files at Desktop.
---

## 📈 Interpretation of Results

### 1. Average Transaction Amount per Date

* Shows spending trends over time
* Sudden spikes may indicate:
  * High-value transactions
  * Possible fraud increment

---

### 2. Fraud Rate (%) by Hour of Day

* Identifies the hours of highest risk

---

### 3. Overall Fraud Distribution

* Displays proportion of:
  * Fraudulent
  * Legitimate
  * and Unknown transactions

👉 High fraud percentage may indicate high system risk

---

### 4. Debit vs Credit by Fraud Status

* Compares fraud across different transaction types

---

### 5. Top 5 Business Types by Fraudulent Amount

* Highlights those industries most affected by fraud
* Indicates potentially vulnerable sectors

---

## ⚠️ Notes & Limitations
* Missing data is labeled as **"Unknown"**
* Results depend on the quality of dataset provided
* This is not a real time fraud detection system

---

