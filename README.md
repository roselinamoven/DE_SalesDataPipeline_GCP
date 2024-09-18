# 🚀 **Automated Data Pipeline for Sales Data in Google Cloud** 🌩️

Welcome to the **Automated Data Pipeline for Sales Data** project! This repository demonstrates how to build a robust, automated data pipeline using Google Cloud Platform (GCP). It covers everything from uploading sales data files to visualizing insights through dashboards.

---

## 📋 **Project Overview**
This project automates the ingestion, storage, processing, and visualization of sales data using various GCP services.

### 🔹 **Key Features**
- **Web Portal for Data Upload** 🖥️  
   Built using **Python Flask** to upload sales data files (CSV, Excel) through an easy-to-use web interface.
   
- **Cloud Storage Integration** ☁️  
   Uploaded files are securely stored in a **Google Cloud Storage (GCS)** bucket.
   
- **Automated Data Processing** 🔄  
   A **Google Cloud Function** is triggered upon file upload, automatically processing and loading the sales data into **BigQuery** for analysis.

- **Data Visualization with Looker Studio** 📊  
   **Looker Studio** provides insightful dashboards and reports to help analyze sales trends and performance.

---

## 🛠️ **GCP Services Used**
- **Google Cloud Storage (GCS)**: Secure and scalable storage for sales data files.
- **Google Cloud Functions**: Automatically triggered to process and load data into BigQuery.
- **BigQuery**: Data warehouse for storing and analyzing sales data.
- **Looker Studio**: Dynamic dashboards for visualizing sales data.

---
## ⚙️ **Setup Instructions**

### 1️⃣ **Flask Web App for Data Upload**
- Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
- Run the app:
    ```bash
    python app.py
    ```
- Upload files via the Flask web interface.

### 2️⃣ **Google Cloud Storage (GCS)**
- Create a **GCS bucket** to store the uploaded files.
- Modify the Flask app to upload files to this bucket.

### 3️⃣ **Google Cloud Functions**
- Deploy a **Cloud Function** to trigger upon file uploads.
- The function processes the file and loads the sales data into **BigQuery**.

### 4️⃣ **BigQuery**
- Create a BigQuery dataset for storing the sales data.
- The Cloud Function will load processed data into this dataset.

### 5️⃣ **Looker Studio**
- Connect **Looker Studio** to BigQuery to create insightful dashboards and reports based on the sales data.

---

## 💡 **How It Works**
1. Users upload sales data via the **Flask web app**.
2. The file is stored in **Google Cloud Storage**.
3. A **Google Cloud Function** is triggered and processes the uploaded file.
4. The processed data is inserted into **BigQuery**.
5. Sales data is visualized in **Looker Studio** through dashboards.

---

## 🔍 **Conclusion**
This project builds a complete automated data pipeline using GCP, from file upload to data visualization. The integration of Flask, GCS, Cloud Functions, BigQuery, and Looker Studio creates a seamless experience for processing and analyzing sales data.

---

Feel free to contribute, open issues, or give feedback! 😊
