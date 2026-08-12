# 🛒 E-Commerce Customer Intelligence

An end-to-end Data Science and Machine Learning project that analyzes e-commerce customer behavior, segments customers based on purchasing patterns, and predicts the likelihood of repeat purchases.

---

## 📌 Project Overview

E-Commerce Customer Intelligence uses customer transaction data to understand purchasing behavior and generate useful customer insights.

The project follows a complete Data Science workflow:

Raw Data → Data Cleaning → Exploratory Data Analysis → Feature Engineering → Customer Segmentation → Machine Learning → Prediction → Evaluation → Visualization

The system analyzes customer behavior using features such as Recency, Frequency, Monetary value, Total Quantity, Unique Products, Average Order Value, and Customer Lifetime.

---

## 🎯 Objectives

- Analyze e-commerce customer purchasing behavior.
- Clean and preprocess transaction data.
- Perform Exploratory Data Analysis (EDA).
- Create meaningful customer-level features.
- Perform RFM-based customer analysis.
- Segment customers using K-Means Clustering.
- Predict whether a customer is likely to make a repeat purchase.
- Calculate purchase probability and purchase risk.
- Evaluate Machine Learning model performance.
- Visualize customer behavior and segmentation.
- Generate meaningful business insights.

---

## 📊 Dataset

The project uses an e-commerce transaction dataset containing customer purchase information.

Important transaction-level information includes:

- Customer ID
- Product information
- Quantity
- Price
- Invoice Date
- Country
- Transaction information

The transaction data is transformed into customer-level data for analysis and Machine Learning.

---

## 🔄 Data Science Workflow

### 1. Data Collection

The e-commerce transaction dataset is loaded into Python using Pandas.

### 2. Data Cleaning

The dataset is cleaned by:

- Handling missing values
- Removing duplicate records
- Removing invalid transactions
- Handling cancelled transactions
- Checking data types
- Removing unwanted records

### 3. Exploratory Data Analysis

EDA is performed to understand:

- Customer purchasing behavior
- Spending patterns
- Order frequency
- Product purchasing behavior
- Customer activity
- Relationships between numerical variables

### 4. Feature Engineering

Customer-level features are created:

| Feature | Description |
|---|---|
| Recency | Days since the customer's last purchase |
| Frequency | Number of purchases/orders |
| Monetary | Total amount spent |
| Total_Quantity | Total number of products purchased |
| Unique_Products | Number of different products purchased |
| Average_Order_Value | Average spending per order |
| Customer_Lifetime_Days | Days between first and last purchase |
| Purchase_Frequency | Purchasing activity over time |

---

## 👥 Customer Segments

After applying K-Means Clustering, customers are grouped according to their purchasing behavior. The clusters are then interpreted into meaningful business segments.

### 🟢 High Value Customer

- High spending
- High purchase frequency
- Recent purchases
- Valuable customers who are important for customer retention

### 🔵 Regular Customer

- Medium spending
- Medium purchase frequency
- Normal purchasing activity
- Customers with consistent purchasing behavior

### 🟠 At Risk Customer

- High Recency (long time since last purchase)
- Lower recent activity
- May need attention or targeted offers
- Potential customers to focus on for retention

### 🔴 Low Value Customer

- Low spending
- Low purchase frequency
- Low purchasing activity
- Customers with relatively lower contribution

## 🤖 Repeat Purchase Prediction

A supervised Machine Learning model is used to predict whether a customer is likely to make a repeat purchase.

The prediction stage produces:

- `Repeat_Purchase`
- `Purchase_Probability`
- `Purchase_Prediction`
- `Purchase_Risk`

Example:

```text
Purchase Probability : 87.6%
Purchase Prediction  : Likely to Purchase
Purchase Risk        : Low Risk
