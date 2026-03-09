# PySpark-DeltaLake-Project
A PySpark-based Data Lakehouse project implementing Medallion Architecture (Bronze → Silver → Gold)  using Delta Lake. 


![image_alt](https://github.com/Rio0294/PySpark-DeltaLake-Project/blob/e17850c08c5965aca9ff1ad09b9428962804ceb7/pyspark%20%20medallion%20draw.io.drawio.png)

## Results

### 🥉 Bronze Layer
- 12,575 records ingested from CSV
- Added ingestion timestamp column
- Saved as Parquet format

### 🥈 Silver Layer
- Schema enforced with correct data types (FloatType, DateType, TimestampType)
- Null values replaced with "Unknown" for string columns
- No duplicates found (12,575 records maintained)
- Data quality check passed - all transactions verified
- Saved as Delta Lake

### 🥇 Gold Layer
- Total revenue analysed by category
- Top 10 customers identified by spending
- Monthly revenue trend generated
- Online vs In-store sales compared
- Discount impact on revenue analysed
- All aggregations saved as Delta Lake
