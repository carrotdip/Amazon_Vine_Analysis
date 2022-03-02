# Amazon Vine Analysis
## Overview
The purpose of this analysis was to perform the ETL process on a large dataset, specifically Vine reviews for beauty products on Amazon. Due to the large amount of data, Spark and AWS was utilized to analyze the data "in the cloud". The Amazon Vine reviews dataset was uploaded onto Amazon's Relational Database Service (RDS) and PySpark was utilized to perform the analyses. 
## Results
![txt](https://github.com/carrotdip/Amazon_Vine_Analysis/blob/65c7c21ffec5e45bf07c0a6241a91566e531fba6/vine_table_values.png)\
As shown in the screenshot, there is a total of 497 Vine (paid) reviews and 120,863 non-Vine (unpaid) reviews for beauty products on Amazon. Of the 497 paid reviews, 220 were 5 stars, creating a percentage of 44.3% 5-star paid reviews. Of the 120,863 unpaid reviews, 74,470 were 5 stars, creating a percentage of 61.6% of 5-star unpaid reviews. 
It may be presumed that Vine reviews, because they are paid, may lead to a bias of higher reviews. However, our analysis showed that this was not the case. There is a significantly higher percentage of 5-star unpaid reviews at 61.6% vs. paid reviews at 44.3%. This analysis shows that Vine reviews do not cause a bias among the star ratings. 
To further test, I would recommend performing a two-sample t-Test to confirm that there is a statistical difference between the two samples (Vine vs. non-Vine reviews). 
