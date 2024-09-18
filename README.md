Automated Data Pipeline for Sales Data in Google Cloud
Project Overview
Welcome to the Automated Data Pipeline for Sales Data project! This project showcases the creation of an automated pipeline to handle sales data using Google Cloud Platform (GCP). It integrates multiple GCP services for seamless data upload, storage, processing, and visualization.

Key Features
Web Portal for Data Upload

Built using Python Flask to provide a user-friendly interface for uploading sales data files (CSV, Excel).
Google Cloud Storage (GCS) Integration

Uploaded files are stored in a GCS bucket for secure and scalable storage.
Automated Data Processing

A Google Cloud Function is triggered whenever a new file is uploaded. It processes and loads the sales data into BigQuery for analysis.
Data Visualization with Looker Studio

Interactive dashboards and insightful reports are created using Looker Studio, making it easy to analyze sales trends.
GCP Services Used
Google Cloud Storage (GCS): To store sales data files securely and accessibly.
Google Cloud Functions: Automatically triggered to process and load data into BigQuery.
BigQuery: Acts as the data warehouse to store and analyze sales data.
Looker Studio: Creates dynamic dashboards for sales data visualization.
Project Structure
bash
Copy code
📁 DE_SalesDataPipeline_GCP/
├── app.py               # Python Flask web app for uploading files
├── templates/
│   └── upload.html      # HTML file for the file upload interface
├── main.py              # Google Cloud Function code to process and load data
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
Setup Instructions
1. Flask Web App for Data Upload
The Python Flask web app allows users to upload sales data files (CSV/Excel) via a web interface.

Install dependencies:
bash
Copy code
pip install -r requirements.txt
Run the app:
bash
Copy code
python app.py
2. Google Cloud Storage (GCS)
Create a GCS bucket to store uploaded files.
Configure the Flask app to upload the files to this bucket.
3. Google Cloud Functions
Create a Google Cloud Function that triggers when a new file is uploaded to GCS.
The function processes the file and loads the sales data into BigQuery.
4. BigQuery
Set up a BigQuery dataset to store the processed sales data.
Ensure that the Cloud Function is set to load data into this dataset.
5. Looker Studio
Use Looker Studio to create reports and dashboards based on the data in BigQuery.
How It Works
The user uploads sales data via the Flask web app.
The uploaded file is stored in Google Cloud Storage (GCS).
A Google Cloud Function is triggered when a file is uploaded. It processes the data and inserts it into BigQuery.
The sales data in BigQuery is used to build dynamic reports in Looker Studio.
Conclusion
This project demonstrates a fully automated pipeline for handling sales data using GCP. The combination of Flask, GCS, Cloud Functions, BigQuery, and Looker Studio ensures a seamless, scalable, and insightful data processing experience.
