# Amazon_Vine_Analysis
by using Google Colab,  Pyspark, Postgres/pgAdmin, AWS RDS and SQL

## overview
#### the purpose of this module is to analyze the Amazon reviews written by members of paid Amazon vine program, companies will receive a common review of vine members in order to determine if there is any trend. however, this this case we will get the data from  
website server rather than a csv or any document, and also we will connect our result from pyspark to pgadmin or postgres, using by AWS and RDS. so that we could cook our data from online and then move them to the local environment. then we will present that all to our client or other companies.


## Results
#### Deliverable 1

#### the result in the below picture. in the pyspark and also see 4 table in the pgadmin.

<img width="1605" alt="Screen Shot 2022-09-12 at 10 14 21 PM" src="https://user-images.githubusercontent.com/106010498/190323596-b5a2695a-380d-4f47-a732-482651c93855.png">
<img width="1634" alt="Screen Shot 2022-09-12 at 10 14 24 PM" src="https://user-images.githubusercontent.com/106010498/190323601-dafcae8a-3dab-4117-9e5c-dc2aa7e2eb6a.png">


<img width="1728" alt="customers table" src="https://user-images.githubusercontent.com/106010498/190323612-cec855d4-9ef0-41cd-b312-049171533449.png">

<img width="1728" alt="products_table" src="https://user-images.githubusercontent.com/106010498/190323624-cb4d38b9-5a36-46d1-8feb-ec92c58ed668.png">

<img width="1728" alt="vine table" src="https://user-images.githubusercontent.com/106010498/190323644-7d2ce41d-447a-4012-a541-85a70d78967d.png">



<img width="1728" alt="review id table" src="https://user-images.githubusercontent.com/106010498/190323632-13ff3e67-7558-4b70-a25e-3d66cfe99553.png">


#### Deliverable 2
#### i will answer three question base on the follow picture 

<img width="984" alt="Screen Shot 2022-09-14 at 7 31 28 PM" src="https://user-images.githubusercontent.com/106010498/190324218-d294802f-fa22-4cb7-be84-aba6e0795d0b.png">

#### 1.How many Vine reviews and non-Vine reviews were there?
###### Vine members made up only 49 of the reviews whereas the Non-Vine members is 40471.


#### 2.How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
###### Vine members gave 48 out of 49 reviews a 5 star rating.
###### Non-Vine members gave 15663 out of 40471 reviews a 5 star rating.

#### 3.What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
###### 51.06% of the reviews for Vine members were rated 5 stars.
###### 38.7% of the reviews for Non-Vine members were rated 5 stars.

The dataset had over 3 million reviews recorded. In order to focus on reviews that would be considered more likely to be helpful, we needed to filter the dataset by:


## Summary
#### we will the Vine members don't have show bias when rating their products based on that the number of 5-star rating was about 10% more than Non-Vine members, there is many reason to cause that, we can assume that the Vine customers are more critical about thier rating and None-Vine customers are more indifferent when they submitting their review. However, to support this assumption. we need to focus on all of the data rather than just filtering it to a percentage of helpful or total votes as we did. review the data as is would give more different result and it will might make us to support our assumption.

## additional analysis that non-filtered-total dataset to support above statement.

![Screen Shot 2022-09-14 at 11 15 55 PM (2)](https://user-images.githubusercontent.com/106010498/190328565-b35552e4-0a9e-48b9-a7c6-dee1e796d07c.png)
