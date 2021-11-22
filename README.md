# Amazon_Vine_Analysis

## Overview
An analysis of Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

### Purpose
The purpose of this project was to select a dataset out of approximately 50 datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. PySpark, Pandas, or SQL was used to determine if there were any bias toward favorable reviews from Vine members in your dataset; and a written report was provided to SellBy stakeholders.

### Resources

Apache Spark (Spark) is a unified analytics engine for large-scale data processing. Spark lets you write applications in code that can run on Hadoop. However, Spark doesn't have to run on Hadoop, as it can run in stand-alone mode or in the cloud. Spark can be 100 times faster than Hadoop. Just like Hadoop's MapReduce, Spark works with data spread across a cluster, or a group of computers that work together.

Spark uses in-memory computation instead of a disk-based solution, which means it doesn't need to talk to the HDFS each time and can retain as much as HDFS can in-memory. Spark uses lazy evaluation, which delays the evaluation of an expression or command until the value is needed.

Cloud-based notebooks provide a remote workspace with stronger resources than our local laptop might allow. Cloud notebooks permit us to share our work with others, such as coworkers, similar to GitHub. We'll use Google Colaboratory (Links to an external site.) (Colab), which are Google-hosted notebooks. Some setup is required, so we'll start there before getting back to the basics of PySpark.


### Project Requirements

Two technical analysis deliverables and a written report were required:

#### Deliverable 1: Perform ETL on Amazon Product Reviews

- Using knowledge of the cloud ETL process; an AWS RDS database with tables was created in pgAdmin, a dataset was selected from the Amazon Review datasets and extract into a DataFrame. The DataFrame was transformed into four separate DataFrames that matched the table schema in pgAdmin. The transformed data was uploaded into the appropriate tables and queries were run in pgAdmin to confirm the data has been uploaded.

Dataset selected: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz

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

Examples of summary

We can see that the percentage of 5-star reviews in Vine is very close to non-Vine reviews (51% to 50.5%).

Although the number of Vine reviews is pretty low, so far it can still represent the product. However, the average rating from Vine customers is 4.38 with std deviation of 0.78, and this is much higher than the 3.77 (std deviation: 1.51) from non-Vine customers. It is obvious that non-Vine reviews are more diverse than Vine reviews which got motivated to give higher ratings.

I believe the Vine customers tend to give higher ratings and pretty focusing on the higher ratings too. So reviews from Vine customers are not that trustworthy for me.

