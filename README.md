# Amazon Vine Program Analysis

## Overview

To better understand the impact of Amazon's Vine paid review program, this analysis presents the key summary statistics from a sample of video game reviews that has been split up by whether they are part of the Vine program or not.

#### Resources Used
This analysis employs Apache Spark, the pySpark library, and Google Colabratory notebooks to perform the ETL process on raw review data, that is then uploaded to a Postgres SQL data base for future queries.

## Results

#### Vine Reviews Results Table

Below are the summary statistics for reviews from the Vine program.

(INSERT VINE REVIEWS TABLE HERE)

* From this sample, there were 94 Vine program reviews.
* of those 94 reviews, 48 were rated at 5 stars.
* 51.06% of the Vine program reviews were rated 5 stars.

#### non-Vine Reviews Results Table

Below are the summary statistics for reviews not from the Vine program.

(INSERT NON VINE REVIEWS HERE)

* From this sample, 40,471 were not in the Vine program.
* Of those 40,471, 15,663 were rated at 5 stars.
* 38.70% of the non-Vine program reviews were rated 5 stars.

## Summary

From this sample, there is a clear bias in 5 star reviews from the Vine program. There is a percentage difference of about 12% between Vine and non-Vine reviews. A key consideration is the difference in size between these two samples, because of this difference in sample size, statistical tests (ANOVA) should be ran to confirm the statistical significance of these findings.

Another analysis to consider is the average star rating across the Vine and non-Vine program samples. The below tables demonstrate the difference between both samples in terms of average star rating

### Average Vine program star rating

(INSERT PICTURE HERE)

### Average non-Vine program star rating

(INSERT PICTURE HERE)
