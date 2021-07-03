# Amazon Vine Analysis

## Overview of Project

### Background
Some companies pay a small fee to Amazon to provide products to Amazon Vine members who are then required to publish a review.  Concerns have come up, however, as to whether there is review bias of Vine members.

## Analysis 

### Overview of Analysis
The purpose of this analysis is to assess whether there is bias towards favorable reviews from Vine members in a dataset related to watch purchases.  Using PySpark, dataframes were created to separate reviews of Vine vs non-Vine members to then calculate the percentage of each group that gave 5-star ratings.

### Results
1.	 In total there were 47 and 8,362 Vine and non-Vine reviews, respectively.


![Total Reviews](https://user-images.githubusercontent.com/80165223/124360346-ed029180-dbee-11eb-9c01-6251ecb9c3e6.png)



2.	There were 15 and 4,332 5-star Vine and non-Vine reviews, respectively.


![Five-Star Reviews](https://user-images.githubusercontent.com/80165223/124360350-f12eaf00-dbee-11eb-89dd-4deac24b4dc6.png)



3.	The percentage of 5-star reviews were 32% and 52% for Vine and non-Vine members, respectively.



![percentage 5 stars](https://user-images.githubusercontent.com/80165223/124360354-f55acc80-dbee-11eb-9b16-fee17b696ed6.png)




## Summary

In the dataset pertaining to watch purchases there was no positivity bias towards paid Vine members.  Positivity skewed toward the unpaid members as displayed in the analysis section.  The sample size is quite low for paid members which skews the overall dataset results heavily towards unpaid members.  More data from the paid members may prove beneficial in answering this overall question.

To better understand the question a two-way t-test could be run to see if the rating averages for both groups have statistically different means.  If there is a significant difference, a multiple linear regression could then be run to see what variables are predicting rating for each group, if significant.
