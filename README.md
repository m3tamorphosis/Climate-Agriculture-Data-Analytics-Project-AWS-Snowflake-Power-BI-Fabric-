# 🌦️ Climate & Agriculture Data Analytics Project (AWS → Snowflake → Power BI Fabric)

**AWS | Snowflake | Power BI | Power BI Fabric | Data Engineering**

![AWS](https://img.shields.io/badge/AWS-S3-orange?style=flat\&logo=amazonaws\&logoColor=white)
![AWS IAM](https://img.shields.io/badge/AWS-IAM-orange?style=flat\&logo=amazonaws\&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat\&logo=snowflake\&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat\&logo=powerbi\&logoColor=black)
![Microsoft Fabric](https://img.shields.io/badge/Microsoft-Fabric-0078D4?style=flat\&logo=microsoft\&logoColor=white)

## 📌 Project Overview

This project demonstrates an **end-to-end data analytics pipeline** using **AWS, Snowflake, and Power BI Fabric**. The goal is to ingest a CSV dataset stored in AWS, integrate it with Snowflake using secure role-based access, perform data transformation and categorization, and finally build interactive analytical reports in Power BI, which are published to **Power BI Fabric**.

The project focuses on analyzing **Rainfall, Temperature, and Humidity** trends and their relationship with agricultural factors such as crop type, soil type, irrigation, and yields.

---

## 🛠️ Tools & Technologies Used

**AWS | Snowflake | Power BI | Power BI Fabric | Data Engineering**

![AWS](https://img.shields.io/badge/AWS-S3-orange?style=flat\&logo=amazonaws\&logoColor=white)
![AWS IAM](https://img.shields.io/badge/AWS-IAM-orange?style=flat\&logo=amazonaws\&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat\&logo=snowflake\&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat\&logo=powerbi\&logoColor=black)
![Microsoft Fabric](https://img.shields.io/badge/Microsoft-Fabric-0078D4?style=flat\&logo=microsoft\&logoColor=white)

* **AWS S3** – CSV file storage
* **AWS IAM** – Role creation for secure access
* **Snowflake** – Data warehouse and transformation
* **Power BI Desktop** – Data modeling & visualization
* **Power BI Fabric** – Report publishing & sharing

---

## 📂 Dataset Description

The dataset is stored as a **CSV file** and contains the following fields:

| Column Name | Description                 |
| ----------- | --------------------------- |
| Year        | Year of record              |
| Location    | Geographic location         |
| Area        | Agricultural area           |
| Rainfall    | Annual rainfall measurement |
| Temperature | Average temperature         |
| Soil type   | Type of soil                |
| Irrigation  | Irrigation method           |
| Yields      | Crop yield output           |
| Humidity    | Humidity level              |
| Crops       | Crop type                   |
| Price       | Crop price                  |
| Season      | Agricultural season         |

---

## 🔄 Data Pipeline Workflow

### 1️⃣ Upload CSV File to AWS S3

* The raw CSV dataset is uploaded to an **AWS S3 bucket**.

### 2️⃣ Create AWS IAM Role for Power BI & Snowflake

* An IAM role is created to allow **secure access** between AWS S3 and Snowflake.
* The role is configured with proper permissions for reading CSV data from S3.

### 3️⃣ Integrate AWS S3 with Snowflake

* A Snowflake **storage integration** is created using the AWS IAM role.
* The CSV file from S3 is loaded into Snowflake tables.

### 4️⃣ Data Transformation in Snowflake

The following transformations and categorizations are applied:

#### 📅 Year Grouping

* **Year 2004 – 2009** → `Y1`
* **Year 2010 – 2015** → `Y2`
* **Year 2016 – 2019** → `Y3`

#### 🌧️ Rainfall Classification

* **Rainfall 255 – 1200** → `Low`
* **Rainfall 2800 – 4103** → `High`

These transformations help simplify analysis and improve report readability.

---

## 📊 Power BI Reporting

Power BI is connected directly to **Snowflake** as the data source.

Across all report pages, the following common KPIs are included:

* **Average value by Year**
* **Average value by Season**
* **Average value by Crop**
* **Average value by Location**

### 📄 Report Pages

#### 📘 Page 1 – Rainfall Analysis

* Average value by Year
* Average value by Season
* Average value by Crop
* Average value by Location

#### 📕 Page 2 – Temperature Analysis

* Average value by Year
* Average value by Season
* Average value by Crop
* Average value by Location

#### 📗 Page 3 – Humidity Analysis

* Average value by Year
* Average value by Season
* Average value by Crop
* Average value by Location

#### 📙 Page 4 – Humidity Analysis (Advanced)

* Average value by Year
* Average value by Season
* Average value by Crop
* Average value by Location

---

## 🚀 Deployment to Power BI Fabric

* The completed Power BI report is **published to Power BI Fabric**.
* This allows cloud-based access, sharing, and collaboration.

---

## ✅ Key Learnings

* Secure data integration using **AWS IAM Roles**
* External data loading into **Snowflake**
* Data transformation and categorization for analytics
* Building multi-page analytical reports in **Power BI**
* Publishing and managing reports in **Power BI Fabric**

---

## 📎 Project Use Case

This project is ideal for:

* Data analytics portfolios
* Cloud data engineering demonstrations
* Agricultural and climate data analysis
* Power BI + Snowflake integration examples

---

📌 *This repository contains the dataset, SQL scripts, and Power BI report files used in this project.*
