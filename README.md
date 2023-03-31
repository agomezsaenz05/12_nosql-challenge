# 12_nosql-challenge
## Requirements
### Part 1: Database and Jupyter Notebook Set Up (15 points)
1. Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.

2. Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).

3. Create an instance of the Mongo Client.

4. Confirm that you created the database and loaded the data properly:
    - List the databases you have in MongoDB. Confirm that uk_food is listed.
    - List the collection(s) in the database to ensure that establishments is there.
    - Find and display one document in the establishments collection using find_one and display with pprint

5. Assign the establishments collection to a variable to prepare the collection for use.

*** Answers for part 1 are located in Starter_Code folder in NoSQL_setup_starter.ipynb ***

### Part 2: Update the Database (20 points)
Use NoSQL_setup_starter.ipynb for this section of the challenge.
The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:

1. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis.
2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3. Update the new restaurant with the BusinessTypeID you found.
4. The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
5. Some of the number values are stored as strings, when they should be stored as numbers. Use update_many to convert latitude and longitude to decimal numbers.

*** Answers for part 2 are located in Starter_Code folder in NoSQL_setup_starter.ipynb ***

### Part 3: Exploratory Analysis (55 points)
To receive all points, your Jupyter notebook analysis file must have all of the following:
- Question 1: Which establishments have a hygiene score equal to 20? (8 points)
- Question 2: Which establishments in London have a RatingValue greater than or equal to 4? (12 points)
- Question 3: What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"? (15 points)
- Question 4: How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas. (20 points)

*** Answers for part 3 are located in Starter_Code folder in NoSQL_analysis_starter.ipynb ***
