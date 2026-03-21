# ❄️ Hotel Booking Data Engineering Project (Snowflake)

---

## 📖 Overview

This project demonstrates an end-to-end data engineering pipeline using Snowflake.
It follows the Medallion Architecture (Bronze → Silver → Gold) to transform raw hotel booking data into clean, structured, and analytics-ready datasets.

---

## 🎯 Objectives

* Ingest raw booking data into Snowflake
* Clean and validate data
* Perform data transformation
* Build aggregated tables for analysis
* Generate insights for business decision-making

---

## 🛠️ Tech Stack

* Snowflake (Cloud Data Warehouse)
* SQL
* GitHub

---

## 🏗️ Architecture

### 🥉 Bronze Layer

* Raw data loaded from CSV
* No transformations applied
* Table: `BRONZE_HOTEL_BOOKING`

---

### 🥈 Silver Layer

* Cleaned and validated data

* Applied transformations:

  * Data type conversions
  * Email validation
  * Date validation
  * Standardized text fields

* Table: `SILVER_HOTEL_BOOKINGS`

---

### 🥇 Gold Layer

* Aggregated and analytics-ready data

* Created business-level tables:

  * Daily bookings and revenue
  * Revenue by hotel city
  * Final clean dataset

* Tables:

  * `GOLD_AGG_DAILY_BOOKING`
  * `GOLD_AGG_HOTEL_CITY_SALES`
  * `GOLD_BOOKING_CLEAN`

---

## ⚙️ Project Workflow

1. Created database, file format, and stage in Snowflake
2. Loaded raw CSV data into Bronze table
3. Cleaned and transformed data into Silver layer
4. Built aggregated tables in Gold layer
5. Generated KPIs and analytical queries

---

## 📂 Project Structure

```
hotel-booking-snowflake-project/
│
├── README.md
├── sql/
├── data/
├── results/
```

---

## 📊 KPIs Generated

* Average Booking Value
* Total Guests
* Total Bookings
* Total Revenue

---

## 📈 Analysis Performed

* Revenue trends over time
* Booking trends
* Top cities by revenue
* Booking status distribution
* Room type analysis

---

## 📊 Results

📌 Detailed results and insights are available in the `/results` folder.

---

## 🚀 Future Improvements

* Build dashboard using Power BI or Tableau
* Automate pipeline using Snowflake Tasks & Streams
* Implement incremental data loading

---

## 👩‍💻 Author

Dharini Arumuga Vijeyakumar
B.Tech Computer Science and Business Systems

---

## ⭐ Conclusion

This project showcases how Snowflake can be used to build a structured and scalable data pipeline, transforming raw data into meaningful business insights.
