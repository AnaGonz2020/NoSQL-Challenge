# NoSQL-Challenge
* Module 12 
* Ana Gonzalez

## **Files**

Here you will find the completed files for this challenge:

* *NoSQL_setup_final.ipynb* - my jupyter notebook with the set-up code for the analysis.
* *NoSQL_analysis_final.ipynb* - my jupyter notebook with the analysis code for Eat Safe, Love, and answers to questions
* *Resources* folder with provided .json
    * establishments.json
    * hygiene_20.csv
    * London_RatingValue.csv
    * Top_establishments.csv
    * low_hygiene_score.csv

## **Results**

* *Part 1: Database and Jupyter Notebook Set Up*

    * In part 1 of this assignment, I was tasked to setup the data from an imported database from MongoDB. Using the provided json file, the document was imported into MongoDb, and then set up into a Jupyter notebook for easier querying. 

* *Part 2: Update the Database*

    * After importing the database, "Penang Flavours" was added to the establishments collection. The Business Type ID was also updated to reflect the Business Type of "Restaurant/Cafe/Canteen". In addition, all establishments with LocalAuthorityName of 'Dover' were removed from the data. Finally, using update_many(), I was able to update all 'latitude' and 'longitude' coordinates to a Decimal value.

* *Part 3: Exploratory Analysis*

    * **Which establishments have a hygiene score equal to 20?**
 There are a total of 41 establishments with a hygiene score equal to 20. The establishments are listed in the hygiene_20.csv file in the Resources folder.

    * **Which establishments in London have a RatingValue greater than or equal to 4?**
 The number of establishments with a Rating Value of 4 or greater. These are listed in the 'London_RatingValue.csv' file in the resources folder.

    * **What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?**
The top 5 establishments that are closes to the new establishment "Penang Flavours" are: Northall CPC, Roochi Ltd, Magic Wok, Sultan Kebab House, and Wolfe House Resid.Home. The results are also listed in the 'Top_establisments.csv' file in the Resources folder.

    * **How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.**
 There are 55 establishments that meet the search criteria being queryed. You can see the detailed information in the 'low_hygiene_score.csv' file in the Resources folder.
