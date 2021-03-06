# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program
In this project, I have had access to approximately 50 datasets. Each one contained reviews of a specific product, from clothing apparel to wireless products. I've needed to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I've used PySpark to determine if there is any bias toward favorable reviews from Vine members in my dataset. 

## Results
 - **How many Vine reviews and non-Vine reviews were there?**
   After creating all the needed functions like *count()* to do the calculations and get the number of reviews, we can see that non_vine reviews exceed the Vine reviews by more than 100 times. This explains that the company was very selective in choosing the best customers to express their honest feedback on its products. 

   ![image](https://user-images.githubusercontent.com/80184581/128790748-ee6d1297-f175-4f6a-93a1-96bbfd3e13e8.png)

 - **How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
From the previous calculated data, I was able to use the *count()* function with the *filter()* function to get the number of the reviews which were 5 stars as we see in the following image. Here we see the large difference between the customers who put 5 starts as a review whether they got paid or not. These numbers doesn't explain much, so I've calculated the percentage of Vine and non-Vine reviews to get more insights about the results.

   ![image](https://user-images.githubusercontent.com/80184581/128790888-e96c6143-e477-438f-b327-9dfa4f0a75fa.png)

 - **What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
As a final step and using a simple mathematical formula which divides the number of 5-stars Vine reviews and non-Vine reviews by the total number of Vine reviews, we can say that this is the best part of the results because we are able now to understand the numbers and make effective conclusions. In the following image, we can see that 47.01% of the customers who didn't get paid to give their feedbacks put 5 stars for the products. However, 36.22% of paid reviews were 5 stars.

   ![image](https://user-images.githubusercontent.com/80184581/128791152-bdb178d0-32c3-4c18-a03f-3cbf2d892730.png)

## Summary
In brief, since the percentage of Vine reviews which were 5 stars is lower than the percentage of non-Vine reviews by almost 10%, we can say that there is an advantage for the company to get more honest and clear reviews on its products from the people who get paid on their surveys. Although it's costly, it encourges the customers to give honest reviews and helps the companies to improve themselves and their products. Finally, we can also get the most recent reviews by creaing a new dataframe which sorts the data in descending order. This will help the companies to know the customers' feedback on its most recent organizational structure and updated products.
