# Customer Segmentation using K-Means Clustering (RFM Analysis)

## 📌 Project Overview
This project performs **customer segmentation** on an e-commerce retail dataset using **K-Means clustering**.  
The goal is to group customers based on their purchasing behavior to support business decision-making such as targeted marketing and customer retention strategies.

---

## 📊 Dataset Description
The dataset contains transactional data from an online retail store.

**Columns:**
- InvoiceNo – Unique transaction ID
- StockCode – Product ID
- Description – Product description
- Quantity – Number of items purchased
- InvoiceDate – Date and time of purchase
- UnitPrice – Price per unit
- CustomerID – Unique customer identifier
- Country – Customer location

---

## 🧹 Data Cleaning & Preprocessing
- Removed rows with missing `CustomerID`
- Removed duplicate transactions
- Converted `InvoiceDate` to datetime format
- Created a new feature `TotalPrice = Quantity × UnitPrice`

---

## 🧠 Feature Engineering (RFM Analysis)

Customers were segmented using **RFM metrics**:

- **Recency** – Days since last purchase
- **Frequency** – Number of unique invoices
- **Monetary** – Total spending amount

An RFM table was created by aggregating transactional data at the customer level.

---

## ⚙️ Machine Learning Approach

### Algorithm Used:
- **K-Means Clustering**

### Steps:
1. Standardized RFM features using `StandardScaler`
2. Used the **Elbow Method (WCSS)** to determine optimal number of clusters
3. Applied **K-Means** clustering
4. Evaluated clustering quality using **Silhouette Score**

---

## 📈 Results & Insights
- Customers were successfully segmented into distinct groups
- Each cluster represents a different purchasing behavior:
  - High-value loyal customers
  - Regular customers
  - Low-spending or infrequent customers
  - Potentially lost customers

These insights can help businesses optimize marketing strategies and improve customer retention.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🚀 Future Improvements
- Handle returns by removing negative quantities
- Try advanced clustering algorithms (DBSCAN, Hierarchical Clustering)
- Visualize clusters using PCA or t-SNE
- Deploy results in a dashboard (Power BI / Streamlit)

---

## 📌 Conclusion
This project demonstrates a complete **unsupervised learning pipeline**, from raw transactional data to meaningful customer segmentation using K-Means clustering.

---

## 👤 Author
Devendra Kushwah
