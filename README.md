# DATA_MANAGEMENT_Assignment3
This project analyzes user-movie interactions using the MovieLens 100k dataset through Apache Zeppelin and Spark SQL. It addresses user behavior, movie ratings, and filtering logic to extract insights related to user age groups, genre preferences, and top-rated films.


## *1. Objective*

Using the MovieLens 100k dataset (`u.user`, `u.data`, `u.item`), this notebook answers the following five questions using **PySpark** and **Spark SQL**:

1. Calculate the average rating for each movie.
2. Identify the top ten movies with the highest average ratings.
3. Find the users who have rated at least 50 movies and identify their favourite movie.
4. Find all the users who are less than 20 years old.
5. Find all the users whose occupation is “scientist” and whose age is between 30 and 40 years old.

---

## *2. File Structure*

```
Assignment_3/  
├── assignment_3.json  
├── assignment_3.ipynb  
├── README.md   
├── image/  
       ├──user.png  
       ├──item.png  
       ├──rating.png  
       ├──Q1.png  
       ├──Q2.png  
       ├──Q3.png  
       ├──Q4.png  
       ├──Q5.png  
```

---
## *3. Tools Used*

- **Apache Zeppelin**
- **Apache Spark 2** (PySpark + Spark SQL)

---
## *4. Data Source*

- [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/)

---

## *5. Summary of Findings*

- Several high-scoring movies appear to be lesser-known titles, possibly reflecting the preferences of niche user segments.Several obscure movies (low popularity) hold high average ratings due to niche audiences.
- The majority of active users demonstrate a preference for drama and comedy genres.
- Users under the age of 20 form a distinct demographic cluster, with students comprising the dominant subgroup.
- Scientist users aged 30–40, based on results, appear to be geographically distributed rather than regionally concentrated.

---

## *6. Conclusion*

This study demonstrates the utility of Spark SQL within the Apache Zeppelin environment for the structured analysis of user–movie interaction data. All analytical queries adhere to the constraint of displaying the top 10 results, while user segmentation is implemented through well-defined SQL conditions. The modular and reproducible workflow facilitates systematic exploration of the MovieLens 100k dataset, supporting scalable and interpretable data analysis in a distributed computing context.




