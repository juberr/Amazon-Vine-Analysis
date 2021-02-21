# Amazon Vine Program Analysis

## Overview

To better understand the impact of Amazon's Vine paid review program, this analysis presents the key summary statistics from a sample of video game reviews that have been split up by whether they are part of the Vine program or not.

## Resources Used

This analysis employs Apache Spark, the pySpark library, and Google Colabratory notebooks to perform the ETL process on raw review data, that is then uploaded to a Postgres SQL data base for future queries.

## Results

### Vine Reviews Results Table

Below are the summary statistics for reviews from the Vine program.

![vine program sum stats](https://github.com/juberr/Amazon-Vine-Analysis/blob/main/pics/vine%20sum%20stats.png?raw=true)

* From this sample, there were 94 Vine program reviews.
* of those 94 reviews, 48 were rated at 5 stars.
* 51.06% of the Vine program reviews were rated 5 stars.

### non-Vine Reviews Results Table

Below are the summary statistics for reviews not from the Vine program.

![no vine program sum stats](https://github.com/juberr/Amazon-Vine-Analysis/blob/main/pics/no%20vine%20sum%20stats.png?raw=true)

* From this sample, 40,471 were not in the Vine program.
* Of those 40,471, 15,663 were rated at 5 stars.
* 38.70% of the non-Vine program reviews were rated 5 stars.

## Summary

From this sample, there is a clear bias in 5 star reviews from the Vine program. There is a percentage difference of about 12% between Vine and non-Vine reviews. A key consideration is the difference in size between these two samples, because of this difference in sample size, statistical tests (e.g. ANOVA, t-test) should be ran to confirm the statistical significance of these findings.

Another analysis to consider is the average star rating across the Vine and non-Vine program samples. The below tables demonstrate the difference between both samples in terms of average star rating

### Average Vine program star rating

![avg vine program star rating](https://github.com/juberr/Amazon-Vine-Analysis/blob/main/pics/vine%20avg%20star.png?raw=true)

### Average non-Vine program star rating

![avg non-vine program star rating](https://github.com/juberr/Amazon-Vine-Analysis/blob/main/pics/no%20vine%20avg%20star.png?raw=true)

The high rating bias in Vine program reviews is not just for 5 star reviews alone! It appears even on average, there is about a points difference between the average Vine program review, and the average non-Vine program review.