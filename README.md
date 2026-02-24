# World Layoffs Data Cleaning Project

## Project Overview
This project involves a thorough data cleaning process of a raw layoffs dataset using MySQL. The goal was to transform messy, inconsistent data into a structured format suitable for analysis.

## Steps Performed
1. **Staging Table Creation**: Created a staging environment to protect the raw data.
2. **Duplicate Removal**: Utilized `ROW_NUMBER()` and CTEs to identify and delete 100% identical records.
3. **Standardization**: 
   - Trimmed whitespace from company names.
   - Standardized industry labels (e.g., merging "Crypto" variations).
   - Fixed trailing punctuation in country names.
4. **Data Type Conversion**: Converted text-based date strings into the `DATE` format for time-series analysis.
5. **Null Handling**: Used self-joins to populate missing values in the `industry` column based on existing company records.

## Tools Used
* MySQL Workbench
* SQL (CTEs, Window Functions, Joins, DDL/DML)
