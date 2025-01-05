# AQI_SNOWFLAKE_E2E


# Air Quality Index Monitoring Pipeline and Dashboard

## 🌟 Project Overview
This project is a comprehensive **end-to-end data engineering pipeline** and **interactive dashboard** designed to monitor and analyze **Air Quality Index (AQI)** data across India. The system processes real-time data from 500+ monitoring stations, offering automated workflows, efficient data modeling, and dynamic visualizations using **Snowflake** and **Streamlit**.

---

## 🚀 Key Features

### 1️⃣ **Robust Data Pipeline**
- **Multi-Layered Architecture**: 
  - **Stage Layer**: Captures raw, semi-structured JSON data from APIs.
  - **Clean Layer**: Deduplicates, normalizes, and processes data into structured tables.
  - **Consumption Layer**: Optimized for analytics and reporting.
- **Automation**: Fully automated data ingestion and processing with **GitHub Actions**, **Snowflake Tasks**, and **Dynamic Tables**.

### 2️⃣ **Dimensional Modeling**
- **Star Schema Design**: 
  - **Fact Table**: Captures hourly AQI and pollutant levels.
  - **Dimension Tables**: Includes **Location** and **Date** dimensions for hierarchical and descriptive context.
- **Aggregation**: Pre-computed hourly, city, and daily trends for optimized querying.

### 3️⃣ **Interactive Visualization Dashboard**
- Built with **Streamlit** and hosted directly on Snowflake.
- Key features:
  - **Hourly AQI Trends**: Line and bar charts for detailed analysis.
  - **Pollutant Analysis**: Highlights AQI levels and prominent pollutants.
  - **Map Integration**: Visualizes monitoring stations with latitude, longitude, and AQI values.
  - **Custom Filters**: Filter by state, city, station, and date for location-specific insights.

### 4️⃣ **Real-Time Updates**
- Integrated **GitHub Actions** for API-based real-time data ingestion.
- Fully automated workflows with no manual intervention.

---

## 📊 Architecture Diagram


<img width="1214" alt="Layered-Architecture" src="https://github.com/user-attachments/assets/0a291683-5b55-404d-9562-73833c2c3fac" />


---

## 🛠️ Tools and Technologies Used
- **Programming Languages**: Python, SQL
- **Data Warehouse**: Snowflake
- **Visualization**: Streamlit
- **Data Engineering**: Snowflake Dynamic Tables, Tasks, Virtual Warehouses
- **Data Modeling**: Star Schema (Fact and Dimension Tables)
- **APIs**: Ingested real-time data from public AQI sources

---

## 🔑 Challenges and Solutions
1. **Handling Semi-Structured JSON Data**: 
   - Transformed nested JSON data into structured tables using **Snowflake's FLATTEN function** and **VARIANT data type**.

2. **Ensuring Real-Time Automation**: 
   - Implemented **GitHub Actions** and integrated with **Snowflake Tasks** and **Dynamic Tables** to achieve seamless, fully automated workflows.

3. **Integrating Python with Snowflake**: 
   - Leveraged **Snowflake Snowpark**, optimized SQL queries, and used caching mechanisms to ensure low-latency performance in the **Streamlit dashboard**.

---

## 📷 Screenshots

### 1️⃣ **Dashboard Overview**
![Dashboard Overview](path-to-dashboard-overview.png)

### 2️⃣ **AQI Trends by Hour**
![AQI Trends](path-to-aqi-trends.png)

### 3️⃣ **Map View**
![Map View](path-to-map-view.png)

---


