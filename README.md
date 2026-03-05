# Targeting Alpha: Big Data Analytics & MLOps

## Project Overview
This project leverages Apache Spark, MLlib, and MLflow to classify and identify high-performing stocks ("High-Alpha Winners"). It addresses the failure of traditional absolute price regression models by pivoting to event detection, successfully isolating the top 10% of monthly market performers to generate a projected Long-Short spread alpha of +2.51% monthly.

## Architecture & Technologies
* **Data Ingestion:** PySpark & PyArrow (Databricks DBFS Volume)
* **Big Data Processing:** Spark SQL & Spark DataFrames (Delta Tables)
* **Machine Learning:** Spark MLlib (GBTClassifier, StandardScaler)
* **MLOps Tracking:** MLflow & Spark Pipelines
* **Evaluation:** Out-of-Sample AUC-ROC & Precision-at-Top-1% (Decile Spread Analysis)

## Project Phases
1. **Problem Definition:** Reframed stock prediction as a classification problem to build a high-conviction institutional screening strategy.
2. **Data Ingestion:** Processed gigabytes of partitioned Parquet data, handling legacy nanosecond timestamp schemas using PyArrow.
3. **Exploratory Data Analysis:** Conducted distributed summary statistics, multicollinearity checks, and momentum signal variance analysis.
4. **Predictive Modeling:** Built Spark Pipelines to automate feature assembly, categorical encoding, scaling, and the training of Gradient Boosted Trees.
5. **MLOps Best Practices:** Managed end-to-end hyperparameter tuning, model serialization to Unity Catalog, and feature importance tracking via Databricks MLflow.
6. **Business Insights:** Designed a decile-based trading strategy yielding a 2.82x alpha edge and programmatically detected macroeconomic regime drift.
