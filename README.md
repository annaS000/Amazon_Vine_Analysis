# **Amazon Vine Analysis**

## **Overview**
> For this project we are looking at a dataset of Amazon reviews for video games written by members of the paid Amazon Vine program. The Amazon Vine program allows manufacturers and publishers to acquire reviews for their products. Additionally, companies such as SellBy pay a fee to Amazon and provide products to Amazon Vine members, who, in return, will publish a review. We must analyze the data to determine if this program has any impact on whether these members provide positive reviews for the products. To do this we will be using PySpark,perform the ETL process, connect to an AWS RDS instance, and load the cleaned data into pgAdmin. Finally, we will use use Pandas to determine if there is any bias for these reviews.

---

## **Code**
[Amazon_Reviews_ETL](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)

[Vine_Review_Analysis](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)

---

## **Results** 
* How many Vine reviews and non-Vine reviews were there?

    Vine Reviews
    ![](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/images/paid_table.png?raw=true)
    * There were only 94 reviews by members of the paid Amazon Vine program.

    non-Vine Reviews
    ![](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/images/unpaid_table.png?raw=true)
    * There were 40471 reviews from non-Vine members.

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

    5 Star Vine Reviews

    ![](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/images/paid5star.png?raw=true)
    * There were only 48 five star reviews by members of the paid Amazon Vine program. Which makes up 51.06% of the five star reviews.


    5 Star non-Vine Reviews

    ![](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/images/unpaid5star.png?raw=true)
    
    * There were 15663 five star reviews from non-Vine members. Which makes up 38.7% of the five star reviews.


* **One Star Reviews**
![](https://github.com/annaS000/Amazon_Vine_Analysis/blob/main/images/onestar1.png?raw=true)

---

## **Summary** 
Based on the results of our Vine review analysis, we can see that the factor of being paid or not may have an impact on Amazon members leaving positive reviews on video games. While majority of the reviews came from non-Vine members, of the portion of reviews that came from Vine members only one gave a one star review and about 51% of these members gave five star reviews. As for the non-Vine members, only about 38% of these customers gave a five star review and about 25% of them gave a one star review. These results should be considered when determining how well a video game actually did, since it seems there is a slight bias when a customer leaves a review and is apart of the Vine program but, these members were only a small proportion of these reviews so we can say that most of these reviews were genuine in terms of the game's performance.