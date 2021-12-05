# Amazon_Vine_Analysis


## Overview & Purpose

The overall purpose of the project is to analyze and review Amazon reviews by paid members of Amazon Vine service. This allows the manufacturers and the publishers to obtain reviews for the products and determine if there are any biases in between the Vine members and non-Vine members. The Vine reviews are made publicly available in S3 site. We should use Spark and AWS to accomodate the capacity of the large dataset. We'll need to pick one of the datasets (out of 50) and use PySpark to perform the ETL process to extract the dataset, connect to AWD RDS Instance. We'll use Pyspark Pandas or SQL to determine if there are any biases. 

Of the various datasets, the Electronics section was analyzed for the reviews. 

## Results
Using bulleted lists and images of DataFrames as support, address the following questions:


There were over 3MM reviews, and in order to sort out meaningful dataset, the dataset was resorted by showing total votes equal or greater than 20 reviews, and helpful votes / total votes to have percentage 50%+. 
![helpfulvotes](https://user-images.githubusercontent.com/89154507/144763659-d389eb67-4b44-4b1c-a3bf-1582d874c31c.jpg)

Overall, the dataset would review around 50,000 reviews. 

**How many Vine reviews and non-Vine reviews were there?**

Overall, vine members took up 2.1%~ (1,080 reviews) and compared to this, non-Vine members were 97.9%~, 49,659. 

![Totalreviews](https://user-images.githubusercontent.com/89154507/144763689-d7b453a1-6667-4ddd-9dfd-9a4e050f8a7c.jpg)



**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

454 / 1080 reviews had 5 star rating for Vine members. 
23034 / 49659 reviews had 5 star ratings for non-Vine members

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

Vine members = 42% (approx)
Non-Vine members = 46% (approx) 


## Overall Conclusion
The given results presents that Vine members did not have any special biases when giving ratings in the reviews. When comparing the reviews between Vine members and non-Vine members, the proportion or the ratio was actually 4% lower when comparing the Vine members (42%) to non-Vine members (46%). The lower 5 star rating ratio shows that Vine members aren't just randomly giving out more 5 star ratings, but they tend to give equal & critical reviews on the platform when compared to non-Vine members. 

**Additional Research**

We can also run a similar analysis on different categories for Vine members vs non-Vine members to see if there are big difference when looking at the reviews & by analyzing whether Vine members give out easy 5 star ratings compared to non-Vine members. 
