# 📊 AI-Driven Customer Segmentation in Marketing Analytics

This project applies **Machine Learning (PCA + K-Means Clustering + Decision Trees)** to segment online retail customers using real-world **UCI Online Retail II** transactional data.  
The purpose is to understand customer behavior using RFM-style features (Recency, Frequency, Monetary) and product diversity, enabling **data-driven marketing strategies, customer retention, and revenue optimization**.

---

## 🚀 Project Overview

This project performs end-to-end customer segmentation with:

- Data Cleaning & Preprocessing  
- RFM-style Feature Engineering  
- Outlier Treatment (99.5th percentile)  
- Log Transformation & Standardization  
- PCA (Principal Component Analysis)  
- K-Means Clustering (K = 4)  
- Cluster Profiling & Personas  
- Decision Tree Rules for Interpretability  
- Business Insights & Recommendations  

The final segmentation reveals **four meaningful groups**:

- **Cluster 0 — Power Buyers**  
- **Cluster 1 — Dormant Drifters**  
- **Cluster 2 — Value Seekers**  
- **Cluster 3 — High-Value Occasionals**

---

## 📦 Features in Detail

### **1. Data Cleaning**
- Removed missing Customer IDs  
- Removed cancelled invoices (Invoice starts with "C")  
- Removed negative quantities and prices  
- Created `Amount = Quantity × Price`  
- Treated outliers using the 99.5th percentile  

### **2. Feature Engineering**
Created customer-level metrics:

- `recency_days`  
- `num_orders`  
- `total_amount`  
- `avg_order_value`  
- `total_items`  
- `unique_products`  
- `avg_unit_price`  

### **3. PCA (Principal Component Analysis)**
Reduced dimensionality and highlighted key patterns:

- **PC1 → Spending power**  
- **PC2 → Recency behavior**  

### **4. K-Means Clustering**
- Elbow Method → Optimal K = **4**  
- Silhouette Score validated cluster separation  
- PCA components used for clustering  

### **5. Decision Tree Rules**
- Explains cluster assignments using simple decision rules  
- Provides interpretability for business users  

---

## 📸 Visualizations

Stored in `outputs/figures/`:

- Boxplots (before & after outlier removal)  
- Histograms (customer feature distributions)  
- Elbow Curve  
- Silhouette Score  
- PCA 2D Cluster Plot  
- Spending Boxplot per Cluster  
- Decision Tree Diagram  

---

## 🧠 Cluster Personas & Marketing Actions

### **Cluster 0 — Power Buyers**
- Highest spending, largest product variety  
- **Actions:** VIP perks, premium bundles, early access  

### **Cluster 1 — Dormant Drifters**
- Lowest spending, long recency  
- **Actions:** Win-back offers, reactivation campaigns  

### **Cluster 2 — Value Seekers**
- Moderate spending, price-conscious  
- **Actions:** Combo deals, reward programs, personalized recommendations  

### **Cluster 3 — High-Value Occasionals**
- Low frequency, high average order value  
- **Actions:** Seasonal reminders, curated lists, free shipping offers  

---

## 🛠 How to Reproduce the Project

### **1. Clone Repository**
```bash`
git clone https://github.com/Yogeshwaran0529/AI-Driven-Customer-Segmentation-in-Marketing-Analytics.git
cd <your-repo-name>

# 2. Install Dependencies
pip install -r requirements.txt

# 3. Run the Notebook
jupyter notebook Customer_Segmentation_Analysis_Using_AI.ipynb

---

## 📄 Report & Presentation

Full thesis-style report available as: report.pdf

Contains visualizations, methodology, insights, and cluster personas.

👤 Author

Yogeshwaran N 
AI & Data Analytics Enthusiast
