# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program
In this project, I have had access to approximately 50 datasets. Each one contained reviews of a specific product, from clothing apparel to wireless products. I've needed to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I've used PySpark to determine if there is any bias toward favorable reviews from Vine members in my dataset. 

## Results
 - How many Vine reviews and non-Vine reviews were there?
  - After creating all the needed functions to do the calculations, we can see that non_vine reviews exceed the Vine reviews by more than 100 times. 

  - ![image](https://user-images.githubusercontent.com/80184581/128790748-ee6d1297-f175-4f6a-93a1-96bbfd3e13e8.png)

  - This explains that the company was very selective in choosing the best customers to express their honest feedback on its products. 

 - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? 
From the previous calculated data, I was able to use the count() function with the filter() function to get the number of the reviews which were 5 stars as we see in the following image. 

![image](https://user-images.githubusercontent.com/80184581/128790888-e96c6143-e477-438f-b327-9dfa4f0a75fa.png)

Here we see the large difference between the customers who put 5 starts as a review whether they got paid or not. These numbers doesn't explain much, so I've calculated the percentage of Vine and non-Vine reviews to get more insights about the results.

 - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
As a final step, we can say that this is the best part of the results because we are able now to understand the numbers and make effective conclusions. 

![image](https://user-images.githubusercontent.com/80184581/128791152-bdb178d0-32c3-4c18-a03f-3cbf2d892730.png)

In the previous image, we can see that 47.01% of the customers who didn't get paid to give their feedbacks put 5 stars for the products. However, 36.22% of paid reviews were 5 stars. 

## Summary
In brief, 
