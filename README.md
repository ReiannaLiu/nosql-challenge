# UK Food Hygiene Ratings Analysis

## Project Overview

Welcome to the UK Food Hygiene Ratings Analysis project! This initiative is designed to scrutinize the food hygiene ratings of various establishments across the United Kingdom. The data is sourced from the UK Food Standards Agency and aims to guide the editorial team of the food magazine, Eat Safe, Love, in selecting topics for their future articles.

## Table of Contents

1. [Database and Jupyter Notebook Setup](#database-setup)
2. [Database Updates](#database-updates)
3. [Exploratory Analysis](#exploratory-analysis)

---

## 1. Database and Jupyter Notebook Setup <a name="database-setup"></a>

### Instructions

#### Import Data
- Use the `NoSQL_setup_starter.ipynb` notebook to import the `establishments.json` file into your MongoDB database. The database should be named `uk_food` and the collection `establishments`.

#### Library Imports
- Import the necessary Python libraries, such as PyMongo and Pretty Print (`pprint`).

#### Initialize Mongo Client
- Create an instance of the Mongo Client to interact with your MongoDB database.

#### Data Verification
- Verify that the data has been imported correctly by listing all databases and collections, and displaying a sample document from the `establishments` collection.

---

## 2. Database Updates <a name="database-updates"></a>

### Instructions

#### Add New Restaurant
- Insert a new document for the recently opened halal restaurant, "Penang Flavours," located in Greenwich.

#### Update BusinessTypeID
- Identify the `BusinessTypeID` for "Restaurant/Cafe/Canteen" and update the new restaurant's document accordingly.

#### Remove Dover Establishments
- The magazine is not interested in establishments in Dover. Remove these from the database.

#### Data Type Corrections
- Some fields like latitude, longitude, and RatingValue are stored as strings. Convert these to their appropriate data types.

---

## 3. Exploratory Analysis <a name="exploratory-analysis"></a>

### Instructions

#### General Guidelines
- Use the `NoSQL_analysis_starter.ipynb` notebook for this section. Display the number of documents in the result set and convert the result to a Pandas DataFrame.

#### Questions to Answer
- Identify establishments with a hygiene score of 20.
- Locate establishments in London with a RatingValue of 4 or higher.
- Find the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score and proximity to "Penang Flavours."
- Determine the number of establishments in each Local Authority area with a hygiene score of 0, and list the top ten areas.

Feel free to dive in, and happy analyzing!