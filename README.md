 
# Walmart Customer Analytics: RFM Segmentation & Churn Analysis

An end-to-end data analytics project simulating a real-world retail business intelligence workflow using **SQL Server**, **Python (Pandas)**, and **Power BI**.

---

## 📌 Project Overview
This project solves a critical business challenge for **Walmart**: identifying high-value customers, tracking revenue performance across time, and flagging customers at risk of churning. Instead of starting blindly with data, the project follows an industry-standard analyst workflow:
1. **Business Requirements Definition** (BRD scoping)
2. **Data Cleaning & Engineering** in SQL Server
3. **Behavioral Scoring & RFM Segmentation** in Python
4. **Interactive Dashboard Development** in Power BI

---

## 🛠️ Tech Stack & Tools
| Tool | Purpose in Project |
| :--- | :--- |
| **SQL Server (SSMS)** | Data ingestion, handling mixed date formats, deduplication, and exploratory data queries. |
| **Python (Pandas)** | Customer segmentation, Recency-Frequency-Monetary scoring, quantile splitting, and churn flagging. |
| **Power BI Desktop** | Building a 3-page interactive corporate report with custom DAX measures, bookmarks, and slicers. |
| **GitHub** | Version control and professional portfolio documentation. |

---

## 🔍 Key Business Questions Addressed
* **Customer Value:** Who are our core **Champions**, and what percentage of total revenue do they contribute?
* **Churn Risk:** What is the overall customer churn rate based on a 90-day inactivity threshold?
* **Temporal Trends:** How do customer acquisition, retention, and revenue trend across months, quarters, and years?
* **Strategic Targeting:** What precise retention actions should leadership take for 'At Risk' vs. 'Lost' customers?

---

## 📈 Key Insights & Findings
* **The 80/20 Rule:** **Champions** represent a core segment of the customer base while driving nearly **68% of total revenue**, highlighting a heavy revenue concentration.
* **Churn Sensitivity:** Overall churn sits around **50.86%** (90-day inactivity threshold), indicating that proactive retention campaigns are vital for long-term growth.
* **Seasonality:** Revenue exhibits strong behavioral spikes during Q4 periods, aligning with holiday retail trends.

---

## 🚀 Project Workflow & Execution

### Step 1 — SQL Data Cleaning & Validation
* Imported raw transaction datasets into SQL Server.
* Resolved complex data quality issues, including mixed date formats using `TRY_CONVERT` and `COALESCE`, and removed exact duplicate records.
* Validated row counts against benchmark totals to ensure data integrity.

### Step 2 — Python RFM Scoring Logic
* Loaded cleaned transactional records into Python via Pandas.
* Calculated **Recency** (days since last purchase), **Frequency** (total transactions), and **Monetary** (total spend) per customer.
* Assigned scores on a 1-to-5 scale using quantile functions (`qcut`) and mapped customers into distinct actionable groups (Champions, Loyal, At Risk, New, Lost).

### Step 3 — Power BI Interactive Dashboard
* Designed a 3-page report layout featuring a clean corporate theme matching Walmart's brand colors:
  * **Page 1 (Home):** Executive navigation hub with dynamic card links and metric glossaries.
  * **Page 2 (Business Overview):** High-level KPIs (Total Customers, Total Revenue, Churn %), dynamic revenue/customer toggles, and time-series line charts.
  * **Page 3 (RFM Analysis):** Deep-dive segmentation tables, average R/F/M scores, and customer value distributions.

---

## 📂 Repository Structure
```text
Walmart-Customer-Analytics/
│
├── 01_sql/
│   ├── 01_data_cleaning.sql          # Mixed dates & cleaning scripts
│   └── 02_exploratory_queries.sql    # Business requirement queries
│
├── 02_python/
│   ├── rfm_segmentation.ipynb        # Pandas RFM scoring & churn logic
│   └── cleaned_walmart_data.csv      # Processed dataset output
│
├── 03_powerbi/
│   ├── Walmart_Customer_Dashboard.pbix # Interactive 3-page report
│   └── Walmart_Theme.json            # Custom corporate color theme
│
├── Documents/
│   └── Walmart_BRD.docx              # Business Requirements Document
│
└── README.md                         # Project documentation
# Walmart Customer Analytics: RFM Segmentation & Churn Analysis

An end-to-end data analytics project simulating a real-world retail business intelligence workflow using **SQL Server**, **Python (Pandas)**, and **Power BI**. 

---

## 📌 Project Overview
This project solves a critical business challenge for **Walmart**: identifying high-value customers, tracking revenue performance across time, and flagging customers at risk of churning. Instead of starting blindly with data, the project follows an industry-standard analyst workflow:
1. **Business Requirements Definition** (BRD scoping)
2. **Data Cleaning & Engineering** in SQL Server
3. **Behavioral Scoring & RFM Segmentation** in Python
4. **Interactive Dashboard Development** in Power BI

---

## 🛠️ Tech Stack & Tools
| Tool | Purpose in Project |
| :--- | :--- |
| **SQL Server (SSMS)** | Data ingestion, handling mixed date formats, deduplication, and exploratory data queries. |
| **Python (Pandas)** | Customer segmentation, Recency-Frequency-Monetary scoring, quantile splitting, and churn flagging. |
| **Power BI Desktop** | Building a 3-page interactive corporate report with custom DAX measures, bookmarks, and slicers. |
| **GitHub** | Version control and professional portfolio documentation. |

---

## 🔍 Key Business Questions Addressed
* **Customer Value:** Who are our core **Champions**, and what percentage of total revenue do they contribute?
* **Churn Risk:** What is the overall customer churn rate based on a 90-day inactivity threshold?
* **Temporal Trends:** How do customer acquisition, retention, and revenue trend across months, quarters, and years?
* **Strategic Targeting:** What precise retention actions should leadership take for 'At Risk' vs. 'Lost' customers?

---

## 📈 Key Insights & Findings
* **The 80/20 Rule:** **Champions** represent a core segment of the customer base while driving nearly **68% of total revenue**, highlighting a heavy revenue concentration.
* **Churn Sensitivity:** Overall churn sits around **50.86%** (90-day inactivity threshold), indicating that proactive retention campaigns are vital for long-term growth.
* **Seasonality:** Revenue exhibits strong behavioral spikes during Q4 periods, aligning with holiday retail trends.

---

## 🚀 Project Workflow & Execution

### Step 1 — SQL Data Cleaning & Validation
* Imported raw transaction datasets into SQL Server.
* Resolved complex data quality issues, including mixed date formats using `TRY_CONVERT` and `COALESCE`, and removed exact duplicate records.
* Validated row counts against benchmark totals to ensure data integrity.

### Step 2 — Python RFM Scoring Logic
* Loaded cleaned transactional records into Python via Pandas.
* Calculated **Recency** (days since last purchase), **Frequency** (total transactions), and **Monetary** (total spend) per customer.
* Assigned scores on a 1-to-5 scale using quantile functions (`qcut`) and mapped customers into distinct actionable groups (Champions, Loyal, At Risk, New, Lost).

### Step 3 — Power BI Interactive Dashboard
* Designed a 3-page report layout featuring a clean corporate theme matching Walmart's brand colors:
  * **Page 1 (Home):** Executive navigation hub with dynamic card links and metric glossaries.
  * **Page 2 (Business Overview):** High-level KPIs (Total Customers, Total Revenue, Churn %), dynamic revenue/customer toggles, and time-series line charts.
  * **Page 3 (RFM Analysis):** Deep-dive segmentation tables, average R/F/M scores, and customer value distributions.

---

## 📂 Repository Structure
* `01_sql/`: Contains database scripts for cleaning and exploratory analysis.
* `02_python/`: Jupyter notebook containing the complete RFM calculation pipeline.
* `03_powerbi/`: Contains the `.pbix` report file and custom theme JSON.
* `Documents/`: Project Business Requirements Document (BRD).

---

## 👤 Connect & Author
**Ankit Joshi**  
*B.Tech Computer Science Engineering (2023 Graduate)*[cite: 1]  
[LinkedIn Profile](#) | [GitHub Portfolio](https://github.com/ajoshi222)
