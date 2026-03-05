# Asset Pricing Meta-Ensemble: Big Data Analytics & MLOps

## Project Overview
This project leverages Apache Spark, MLlib, and MLflow to forecast monthly stock excess returns. It addresses the failure of complex predictive models during market crashes by implementing a "Macro-Turbulence Gate" that dynamically routes capital between Gradient Boosted Trees and a safe Linear baseline.

## Architecture & Technologies
* **Data Ingestion:** PySpark & PyArrow (Databricks DBFS Volume)
* **Big Data Processing:** Spark SQL & Spark DataFrames
* **Machine Learning:** Spark MLlib (GBTRegressor, LinearRegression)
* **MLOps Tracking:** MLflow & Spark Pipelines
* **Evaluation:** Out-of-Sample RMSE & Mahalanobis Distance Gating

## Project Phases
1. **Problem Definition:** Predicting stock returns to build an "All-Weather" institutional strategy.
2. **Data Ingestion:** Processed gigabytes of partitioned Parquet data, handling legacy nanosecond timestamp schemas.
3. **Exploratory Data Analysis:** Distributed summary statistics and target distribution analysis.
4. **Predictive Modeling:** Spark Pipelines automating feature assembly into tree-based models.
5. **MLOps Best Practices:** End-to-end hyperparameter tuning tracked via MLflow.
6. **Business Insights:** Designed a real-time macroeconomic turbulence index for dynamic portfolio deleveraging.
