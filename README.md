## Zakariya Shafi 596

## ETL Project – Load Phase
# Overview

This project completes the Load stage of the ETL (Extract, Transform, Load) pipeline.
After extraction and transformation, the cleaned datasets are stored into SQLite and Parquet formats for efficient querying and long-term storage.

The workflow includes integrity checks, SQL validation, and organized data storage — ensuring reliable, reproducible ETL operations.

# Key Features

Loads transformed datasets into:

SQLite database (sales_data.db)

Parquet files (transformed_full.parquet, transformed_incremental.parquet)

Performs SQL verification queries to confirm successful loading.

Provides data previews for visual confirmation.

Demonstrates reproducible ETL structure and version-controlled workflow using GitHub.


# Technologies Used

Python (pandas, sqlite3, pyarrow)

SQLite3

Parquet Format

Jupyter Notebook / VS Code

Git & GitHub for version control

# How to Run

Clone the repository:

git clone https://github.com/<your-username>/ET_load.git
cd ET_load


Run the load script or notebook:

python load_data.py


or open the notebook in Jupyter/VS Code.

Verify loaded data in SQLite:

sqlite3 sales_data.db
SELECT * FROM sales_data LIMIT 5;

# Verification Steps

View the SQLite database tables.

Check Parquet file creation.

Confirm matching row counts with the transformed data.

Validate through sample queries and DataFrame previews.
