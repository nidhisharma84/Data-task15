# 📊 Customer Segmentation using RFM Analysis

## 📌 Project Overview

This project performs Customer Segmentation using the RFM (Recency, Frequency, Monetary) model on an E-commerce Online Retail dataset.

RFM analysis helps businesses identify valuable customers based on their purchasing behavior and design targeted marketing strategies.

---

## 📂 Dataset Used

Online Retail Dataset (E-commerce transactional data)

Columns include:
- InvoiceNo
- StockCode
- Description
- Quantity
- InvoiceDate
- UnitPrice
- CustomerID
- Country

---

## 🛠 Tools & Technologies

- Python
- Google Colab
- pandas
- numpy
- matplotlib

---

## 🔍 Steps Performed

### 1️⃣ Data Cleaning
- Removed missing CustomerID values
- Removed cancelled invoices (InvoiceNo starting with "C")
- Converted InvoiceDate to datetime format
- Created a new column:
  
  TotalAmount = Quantity × UnitPrice

---

### 2️⃣ RFM Calculation

For each CustomerID:

- Recency → Days since last purchase
- Frequency → Number of unique invoices
- Monetary → Total amount spent

---

### 3️⃣ RFM Scoring

- Applied quartile-based scoring (1–4 scale)
- Created R_score, F_score, M_score
- Combined them into a final RFM_Score

Example:
444 → High-value customer

---

### 4️⃣ Customer Segmentation

Customers were categorized into:

- Champions
- Loyal Customers
- At Risk
- New Customers
- Others

---

### 5️⃣ Visualization

- Created a bar chart to show distribution of customer segments.

---

## 📈 Business Insights

- Champions generate the highest revenue and should be retained with loyalty programs.
- Loyal Customers are ideal targets for cross-selling.
- At Risk customers need re-engagement campaigns.
- New Customers should receive onboarding offers.
- Others can be targeted through general promotions.

---

## 📤 Project Deliverables

- task15_rfm.ipynb
- rfm_segments.csv
- segment_actions.txt

---

## 🎯 Conclusion

This project demonstrates:

- Data cleaning and preprocessing
- Feature engineering
- Customer behavior analysis
- Marketing-driven segmentation
- Business strategy thinking
