# Amazon_Vine_Analysis

## Overview
An analysis of Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

### Purpose
The purpose of this project was to select a dataset out of approximately 50 datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. PySpark, Pandas, or SQL was used to determine if there were any bias toward favorable reviews from Vine members in your dataset; and a written report was provided to SellBy stakeholders.

### Project Requirements

Two technical analysis deliverables and a written report were required:

#### Deliverable 1: Perform ETL on Amazon Product Reviews

- Using knowledge of the cloud ETL process; an AWS RDS database with tables was created in pgAdmin, a dataset was selected from the Amazon Review datasets and extract into a DataFrame. The DataFrame was transformed into four separate DataFrames that matched the table schema in pgAdmin. The transformed data was uploaded into the appropriate tables and queries were run in pgAdmin to confirm the data has been uploaded.

#### Deliverable 2: Determine Bias of Vine Reviews

- Using knowledge of PySpark, Pandas, or SQL; the results of the analysis revealed whether there were any bias towards reviews that were written as part of the Vine program. The following results showed whether having a paid Vine review made a difference in the percentage of 5-star reviews.

## Results

The analysis addressed the following questions:

- How many Vine reviews and non-Vine reviews were there?
- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

## Summary

- The summary states whether or not there is bias, and the results support this statement (2 pt)
- An additional analysis is recommended to support the statement (2 pt)