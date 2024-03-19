# nosql-challenge
This module utilizes nosql to evaluate food ratings from the UK Food Standards Agency

# Instructions: 
You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data.

# Part 1: Database and Jupyter Notebook Set Up
Use NoSQL_setup_starter.ipynb for this section of the challenge.
  1. Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments
  2. Import PyMongo and Pretty Print (pprint).
  3. Create an instance of the Mongo Client.
  4. Confirm that you created the database and loaded the data properly.
  5. Assign the establishments collection to a variable.

# Part 2: Update the Database
Make the following changes to the establishments collection.
  1. Add the following information to the database:

{
    "BusinessName":"Penang Flavours",
    "BusinessType":"Restaurant/Cafe/Canteen",
    "BusinessTypeID":"",
    "AddressLine1":"Penang Flavours",
    "AddressLine2":"146A Plumstead Rd",
    "AddressLine3":"London",
    "AddressLine4":"",
    "PostCode":"SE18 7DY",
    "Phone":"",
    "LocalAuthorityCode":"511",
    "LocalAuthorityName":"Greenwich",
    "LocalAuthorityWebSite":"http://www.royalgreenwich.gov.uk",
    "LocalAuthorityEmailAddress":"health@royalgreenwich.gov.uk",
    "scores":{
        "Hygiene":"",
        "Structural":"",
        "ConfidenceInManagement":""
    },
    "SchemeType":"FHRS",
    "geocode":{
        "longitude":"0.08384000",
        "latitude":"51.49014200"
    },
    "RightToReply":"",
    "Distance":4623.9723280747176,
    "NewRatingPending":True
}
  2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
  3.Update the new restaurant with the BusinessTypeID you found.
  4. Remove any establishments within the Dover Local Authority from the database.
  5. Some of the number values are stored as strings, when they should be stored as numbers. Convert those. 

# Part 3: Exploratory Analysis
Use NoSQL_analysis_starter.ipynb for this section of the challenge.
Use the following questions to explore the database, and find the answers, so you can provide them to the magazine editors.
  1. Which establishments have a hygiene score equal to 20?
  2. Which establishments in London have a RatingValue greater than or equal to 4?
  3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

# Resources:
  Instructions provided by: Columbia Data Analytics Boot Camp, https://bootcampspot.instructure.com/courses/4737/assignments/68487?module_item_id=1162427
  Data: UK Food Standards AgencyLinks to an external site. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.

