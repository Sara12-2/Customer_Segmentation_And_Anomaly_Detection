# 🧠 Customer Segmentation & Anomaly Detection Dashboard

An interactive **Streamlit dashboard** that performs **customer segmentation using KMeans clustering** and detects anomalies using **Isolation Forest**.
This project is based on the **Marketing Campaign Dataset** and helps businesses analyze customer profiles, spending patterns, and detect unusual behaviors.

---

## 🚀 Features

* 📊 **Customer Segmentation** using KMeans clustering
* ⚡ **Elbow Method** visualization to choose optimal cluster count
* 🚨 **Anomaly Detection** with Isolation Forest (outlier customers)
* 🎨 Interactive **Streamlit Dashboard** with filters and charts
* 📥 Download filtered customer data as CSV

---

## 📂 Project Structure

```bash
CustomerSegmentation/
│── app.py                   # Main Streamlit app
│── marketing_campaign.csv    # Dataset (tab-separated)
│── requirements.txt          # Dependencies
│── README.md                 # Documentation
```

---

## 📊 Dataset

**File:** `marketing_campaign.csv` (tab-separated)

Columns include:

* **Demographics:** `Year_Birth`, `Education`, `Marital_Status`, `Income`, `Kidhome`, `Teenhome`
* **Purchases:** `MntWines`, `MntMeatProducts`, `MntFishProducts`, `MntSweetProducts`, `MntGoldProds`
* **Campaigns:** `Response`
* **Behavior:** `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases`, `NumWebVisitsMonth`, `Recency`
* **Customer Enrollment:** `Dt_Customer`

---

## ⚙️ How It Works

1. **Data Preprocessing**

   * Handle missing values
   * Convert dates
   * One-hot encode categorical features
   * Standardize numerical values

2. **Clustering (Segmentation)**

   * Apply **KMeans** (k=4 clusters by default)
   * Visualize cluster distribution

3. **Anomaly Detection**

   * Apply **Isolation Forest** to detect outliers
   * Mark anomalies in dataset

4. **Streamlit Dashboard**

   * Sidebar filters for clusters & anomalies
   * Metrics: Normal vs Anomaly count
   * Cluster averages table
   * Interactive bar charts
   * Download filtered dataset

---

## 💻 Installation

```bash
# Clone repo
git clone https://github.com/yourusername/CustomerSegmentation.git
cd CustomerSegmentation

# Create virtual environment
python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)

# Install requirements
pip install -r requirements.txt
```

---

## ▶️ Run App

```bash
streamlit run app.py
```

Then open 👉 [http://localhost:8501](http://localhost:8501) in your browser.

---

## 📌 Future Improvements

* 📉 Add PCA for dimensionality reduction visualization
* 🌐 Deploy on Streamlit Cloud
* 📈 Add more anomaly detection models (LOF, DBSCAN)
* 🖼 Visualize cluster profiles with radar charts

---

## 🛠️ Tech Stack

* **Python**
* **Pandas, NumPy**
* **Scikit-learn** (KMeans, Isolation Forest)
* **Matplotlib**
* **Streamlit**

---

✨ With this project, businesses can **identify customer groups**, **detect unusual patterns**, and **take data-driven decisions** for targeted marketing.
