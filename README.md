# MoviesETL_

**Project Overview**
The purpose of this project is to create an automated pipeline that takes in new movie data, performs the appropriate transformations, and loads the data into existing tables. The existing code is refactored into one function that performs the ETL process.
**Resources and Software**
    Wikipedia Movie Data
    Kaggle Movie Data: The file size of this data exceeds the maximum size allowed on GitHub. However, you may download it directly from Kaggle.
    In the zip file downloaded from Kaggle, only "movies_metadata.csv" and "ratings.csv" are used in this project. These files were added to the gitignore configuration (*.csv)
    Python 3.8
    pgAdmin 6.1
    PostgreSQL v14
    
**Results**
The new ETL function performs correctly and the data is successfuly added to a PostgreSQL database as seen in the images below. The final code output can be viewed below **Movie and Rating queries output in PNG**

![Movies_Query](https://user-images.githubusercontent.com/93059601/147427720-792049b9-958b-4467-a615-c7f8cb42dfae.PNG)

![Ratings_Query](https://user-images.githubusercontent.com/93059601/147427772-59e801c3-231c-4209-9199-a2b588d6265e.PNG)

These outputs were created with the following queries:

SELECT COUNT(*) AS "Number of Movies row" FROM movies;
SELECT COUNT(*) AS "Number of Ratings row" FROM ratings;

Exception to my code: I was unable to hide my postgres password due to system issues which delayed my work and output. I will continue to followup with resolution to the config(db_password). I used clear password to import the Movie and Rating data to my Test Postgres database to avoid delays in submission. I will change once my work is reviewed and marked. 
