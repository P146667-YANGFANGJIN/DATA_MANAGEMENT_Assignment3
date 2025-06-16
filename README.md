# DATA_MANAGEMENT_Assignment3

<p align="center">
  <img src="image/pic.jpg" alt="Movie" width="800"/>
</p>

This project analyzes user-movie interactions using the MovieLens 100k dataset via PySpark, Spark SQL, and Cassandra. It focuses on extracting insights related to user demographics, genre preferences, and movie ratings by integrating Spark with a Cassandra NoSQL backend.

---

## *1. Objective*

Using the MovieLens 100k dataset (`u.user`, `u.data`, `u.item`), this notebook answers the following five questions using **PySpark**, **Spark SQL**, and **Apache Cassandra**:

1. Calculate the average rating for each movie.
2. Identify the top ten movies with the highest average ratings.
3. Find the users who have rated at least 50 movies and identify their favourite movie.
4. Find all the users who are less than 20 years old.
5. Find all the users whose occupation is “scientist” and whose age is between 30 and 40 years old.

---

## *2. File Structure*

```
Assignment_3/  
├── assignment_3.ipynb  
├── README.md   
├── image/  
       ├──user_df.png  
       ├──item_df.png  
       ├──rating_df.png  
       ├──Q1.png  
       ├──Q2.png  
       ├──Q3.png  
       ├──Q4.png  
       ├──Q5.png  
```

---
## *3. Tools Used*

- **Apache Spark 2** (PySpark + Spark SQL)
- **Apache Cassandra 3**
- **Jupyter Notebook (compiled from CLI-based PySpark execution)**

---
## *4. Data Source*

- [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/)

---

## *5. Summary of Findings*

- **Users under 20 years old** are predominantly students, based on the occupation field. This confirms that age filtering accurately highlights a student-heavy demographic.

- **Scientist users aged 30–40** are distributed across a wide range of zip codes, suggesting no geographic clustering and relatively sparse representation.

- **Movie average ratings** mostly fall in the 3.0–4.0 range, with a few titles scoring much lower or achieving exactly 4.0+, suggesting rating consistency but some polarization.

- **Top 10 highest-rated movies** all have a perfect average rating of 5.0, and include several lesser-known or documentary-style films, indicating niche audiences with strong preferences.

- **Most active users (rated ≥50 movies)** overwhelmingly favour the **drama** genre, followed distantly by **action**, showing drama's dominance among dedicated viewers.

---

## *6. Conclusion*

This project demonstrates the effectiveness of PySpark and Spark SQL in processing structured movie rating data, while leveraging Cassandra for distributed storage. All queries strictly adhere to the constraint of displaying the top 10 results. The integration of HDFS, Spark, and Cassandra supports reproducible and modular analysis of the MovieLens 100k dataset, enabling scalable insights on user behaviour and content preferences.
