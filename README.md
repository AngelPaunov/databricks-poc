# Databricks DLT Pipeline: ELT for Machine Learning

## **Overview**
This project demonstrates a Delta Live Tables (DLT) pipeline in Databricks, designed to preprocess raw data into structured layers for machine learning (ML) workflows. It follows the **Medallion Architecture** (Bronze, Silver) to ensure scalable and high-quality data preparation.

## **Key Features**
- **Data Ingestion**: Loads raw data from `/databricks-datasets` in CSV and JSON formats.
- **Data Transformation**: Cleans and validates data with constraints and partitioning.
- **Layered Architecture**:
  - **Bronze**: Raw data with minimal processing.
  - **Silver**: Cleaned and structured data, ready for analysis or ML.

## **Use Cases**
- Customer segmentation, sales forecasting, and fraud detection.
- Preparing high-quality, structured data for ML model training.

## **How to Use**
1. **Import Notebook**: Upload `sample-DLT-pipeline-notebook.sql` to your Databricks workspace.
2. **Create Pipeline**:
   - Go to **Workflows** > **Delta Live Tables** and create a new pipeline.
   - Attach the notebook and configure the settings.
3. **Run and Query**:
   - Execute the pipeline to generate Bronze and Silver layers.
   - Query the results for downstream ML tasks.

## **Requirements**
- Databricks workspace with Delta Live Tables enabled.
