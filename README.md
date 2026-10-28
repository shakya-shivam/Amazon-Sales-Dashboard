# 📊 Amazon Sales Dashboard - Power BI & Figma

## 🎯 Project Overview
An interactive and performance-optimized Power BI dashboard designed to analyze Amazon sales data. This project focuses on tracking core business metrics, customer behavior, and revenue trends to empower data-driven decision-making. 

## 🎥 Visual Proof & Live Demo

All live demo files, including a full interactive video recording and high-resolution layout images, are securely stored in the `Assets` folder of this repository. 

To explore the real-time dashboard interaction, dynamic DAX filtering, and the complete UI/UX flow, please navigate to the `Assets` folder and download the media files directly for an uncompressed, high-quality experience.


## 🛠️ Tech Stack & Tools
* **Data Visualization & Modeling:** Power BI Desktop
* **UI/UX Design:** Figma (Custom background canvases and layouts)
* **Languages:** DAX (Data Analysis Expressions)
* **Version Control:** Git & GitHub

## 🧠 Data Modeling & Architecture
To ensure enterprise-grade performance, the raw dataset (`Amazon.csv`) was transformed into a robust **Star Schema**. 
* **Core Fact Table:** Utilized the primary raw data as the central Fact table.
* **Custom Date Dimension:** Instead of relying on Power BI's auto-date feature, I engineered a dynamic `Dim_Date` table using DAX to handle complex time-intelligence calculations efficiently. 

## 🚧 Challenges & Solutions
**The Privacy & Offline Reliability Challenge:** 
Initially, the dashboard required geographical mapping for regional sales. However, relying on Power BI's default Map visuals involves sending data to Bing/external servers. 
* **Solution:** To ensure 100% client data privacy (compliance with European data standards) and complete offline reliability, I replaced the external Map visual with a custom-configured **Scatter Chart**. This allowed for geographical data representation processed entirely on the local machine without any external server pings.

## 📈 Key Insights & Metrics (DAX Measures)
Optimized DAX formulas were used to extract high-level KPIs:
1. **Total Revenue** 
2. **Total Quantity Sold**
3. **Total Orders** 
4. **Total Customers**
5. **Average Order Value (AOV)**

*(The explicit DAX code for these measures is documented in the `DAX_Measures.txt` file within this repository).*

---
**🤖 Transparency Note:** 
*The core business logic, Figma UI/UX conceptualization, and data modeling were independently designed and developed. AI tools were leveraged strictly as a co-pilot for optimizing code efficiency, troubleshooting technical bottlenecks, and refining documentation.*
