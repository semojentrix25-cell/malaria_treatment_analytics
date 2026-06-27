# SQL Folder

This project uses PostgreSQL as the backend database for storing cleaned and feature-engineered datasets.

SQL was primarily used to verify successful data loading and to support integration between Python and Power BI.

Example verification queries:

SELECT * FROM malaria_cleaned;
SELECT * FROM malaria_feature_engineered
LIMIT 10;
