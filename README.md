# PySpark IMDb Movie Reviews Analysis

Data processing and exploratory storytelling pipeline built with **Apache Spark (PySpark)** on the Kaggle 50K IMDb Movie Reviews dataset.

## Pipeline Tasks Completed
1. **Data Ingestion:** Loaded the CSV dataset into a Spark DataFrame with multi-line quote escaping enabled.
2. **Schema & Exploration:** Inspected inferred column data types (`review`, `sentiment`) and previewed sample records.
3. **Data Cleaning:** Filtered out null and whitespace-only review entries.
4. **Sentiment Aggregation:** Computed total valid review counts and grouped sentiment distribution (`positive` vs. `negative`).
5. **Feature Transformation & Filtering:** Engineered a `review_length` character-count column using `pyspark.sql.functions.length` and isolated long-form reviews (`> 500` characters).
6. **Export:** Saved the cleaned and transformed DataFrame with headers to CSV.

## Data Sources & Reproducibility
* **Raw Input Dataset:** [IMDb Dataset of 50K Movie Reviews (Kaggle)](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
