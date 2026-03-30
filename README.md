### Scalable Sales Analytics Pipeline using PySpark

Overview:
This project presents a **scalable end-to-end data analytics pipeline** built using **Apache PySpark** on the *Global Superstore dataset*. It demonstrates how large-scale datasets can be processed efficiently using distributed computing, following industry-standard data engineering and analytics practices.

The pipeline simulates a real-world workflow, including:
* Data ingestion
* Data cleaning & transformation
* Distributed processing
* Exploratory Data Analysis (EDA)
* Visualization of insights
  
Objectives:

* Build a **scalable data processing pipeline** using PySpark
* Perform **distributed analytics on large datasets**
* Extract **business insights from sales data**
* Demonstrate **real-world data engineering workflow**

Dataset:

* **Source:** Global Superstore Dataset
* **Records:** ~51,000+ rows
* **Features:** 20+ columns

Key Columns:
* Order ID
* Order Date
* Customer Name
* Country
* Category & Sub-Category
* Product Name
* Sales, Quantity, Discount, Profit
* Shipping Cost

 Project Structure:
Bigdata-PySpark-Sales-Analysis/
dataset/
Global_Superstore2.csv

notebooks/
pyspark_bigdata_analysis.ipynb

scripts/
analysis_pipeline.py

images/
charts.png

README.md

Tech Stack:
* **Apache PySpark** – Distributed data processing
* **Python** – Core programming
* **Pandas** – Data manipulation
* **Matplotlib & Seaborn** – Visualization
* **Google Colab** – Execution environment

Workflow:

### 1️⃣ Environment Setup

* Configured PySpark in Google Colab
* Installed required libraries:

bash
pyspark
pandas
matplotlib
seaborn

### 2️⃣ Data Ingestion

* Loaded dataset using PySpark DataFrame API
* Enabled:

  * Schema inference
  * Efficient CSV parsing
  * Distributed data loading

### 3️⃣ Data Understanding

* Schema inspection
* Descriptive statistics
* Missing value analysis
* Column-level exploration

### 4️⃣ Data Cleaning

* Removed duplicates
* Handled missing/null values
* Converted data types
* Fixed malformed numeric fields

### 5️⃣ Distributed Data Processing

Used PySpark transformations:
python
groupBy()
agg()
filter()
orderBy()

### 📊 Key Analyses
* Total Sales by Category
* Profit by Region
* Top Products by Revenue
* Sales by Market

### 6️⃣ Exploratory Data Analysis (EDA)

* Customer segment performance
* Discount vs Profit relationship
* Shipping cost patterns
* Regional sales trends

### 7️⃣ Visualization
Converted PySpark DataFrames → Pandas for visualization:
* Sales by Category
* Profit by Region
* Top Products
* Correlation Heatmap

## ⚡ Scalability Demonstration
PySpark enables distributed processing through partitioning:
python
df = df.repartition(8)

### Benefits:
* Parallel computation
* Efficient aggregation
* Lazy evaluation
* Scalable to millions of records

## 📈 Key Insights

### 💡 Category Performance

* Technology category generates highest revenue

### 🌍 Regional Profitability

* Some regions have high sales but low profit → heavy discounting

### 💸 Discount Impact

* Increased discounts → reduced profitability

### 🏆 Product Analysis

* Few products contribute to majority of sales (Pareto effect)

### 📊 Market Trends

* Distinct purchasing behavior across global markets

## ✅ Results

* Built a **scalable analytics pipeline**
* Demonstrated **distributed data processing**
* Extracted **actionable business insights**
* Visualized large-scale analytics effectively

## 🔮 Future Enhancements

* Spark SQL optimization
* Window functions for advanced analytics
* Machine Learning with Spark MLlib
* Workflow orchestration using Apache Airflow
* Deployment on cloud platforms (AWS / GCP / Azure)

## 👨‍💻 Author

**Pran Wasnik**
Aspiring Data Engineer | Big Data Enthusiast
