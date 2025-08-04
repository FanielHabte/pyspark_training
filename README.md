# 🚀 PySpark Projects for Hands-On Learning

This guide contains two end-to-end projects, each focused on a different aspect of Spark — **PySpark (with MLlib + DataFrames)** and **Spark SQL** — using **two distinct real-world datasets**. Both projects are built to help you master the Spark ecosystem through practical, engaging work.

---

## 📘 Project 1: Customer Behavior & Segmentation Engine (Using PySpark + MLlib + Plotly)

### 🧠 Focus Areas
- PySpark DataFrame API
- Parquet transformations
- Feature engineering
- MLlib clustering (e.g., KMeans)
- Visualizing output with Plotly

### 📦 Dataset
- **Source**: [E-Commerce Behavior Data (Kaggle)](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store)
- **Rows**: ~10 million
- **Fields**: `event_time`, `user_id`, `event_type`, `product_id`, `category_code`, `brand`, `price`, `user_session`

### 🔨 Tasks
1. **Data Ingestion & Storage**
   - Load CSV → Clean → Convert and save as Parquet
   - Handle nulls, cast data types

2. **Feature Engineering**
   - Count views, carts, purchases per user/session
   - Compute average session duration, conversion ratio
   - Create session-based behavior profiles

3. **MLlib Clustering**
   - Normalize features
   - Apply KMeans or BisectingKMeans
   - Tag users with behavioral cluster labels

4. **Plotly Visualizations**
   - View cluster distribution (scatter, 3D plots)
   - Show funnel completion per cluster
   - Compare session features across clusters

5. **Deliverables**
   - A behavioral segmentation notebook
   - Insights into how users interact with the platform

---

## 📘 Project 2: Spark SQL Analytics Hub (Using Spark SQL + NYC Taxi Data)

### 🧠 Focus Areas
- Spark SQL syntax mastery
- Analytical query building
- Time-based analysis and window functions
- Rolling metrics and retention tracking

### 📦 Dataset
- **Source**: [NYC Yellow Taxi Trip Data](https://www.nyc.gov/assets/tlc/downloads/pdf/2023_yellow_tripdata.csv)
- **Rows**: 1M+ per month
- **Fields**: `pickup_datetime`, `dropoff_datetime`, `passenger_count`, `trip_distance`, `fare_amount`, `payment_type`, etc.

### 🔨 Tasks
1. **Register SQL View**
   - Load CSV or Parquet
   - Create temp or global views using `.createOrReplaceTempView()`

2. **Analytics Use Cases**
   - Daily trip count and revenue
   - Top pickup/dropoff locations
   - Average trip duration by hour
   - Passenger behavior by time of day

3. **Advanced SQL Techniques**
   - Rolling 7-day revenue (window functions)
   - Detecting repeat riders (LAG/LEAD)
   - Revenue heatmap by hour + weekday
   - Aggregations with `ROLLUP`, `CUBE`, `GROUPING SETS`

4. **Interactive Query Dashboard (Optional)**
   - Use Spark SQL results to populate a dashboard (Plotly or BI tool)
   - Export materialized views as Parquet or CSV

5. **Deliverables**
   - Set of analytical views answering key business questions
   - Query notebook or dashboard visualizations

---

## 🔁 Summary

| Project | Dataset | Skills Covered | Tools |
|--------|---------|----------------|-------|
| **1. Behavior Segmentation** | E-Commerce (Kaggle) | PySpark, MLlib, Plotly | Spark DataFrames, Clustering |
| **2. Analytics Hub** | NYC Taxi Data | Spark SQL, SQL Windows, BI Prep | SQL Views, Aggregations, Time Series |

---

## 🧰 Recommended Tools & Environment
- Apache Spark 3.x (locally or Databricks)
- Jupyter Notebook or VSCode
- Plotly or Tableau for visualization
- Parquet as storage format
