# Food hygiene ratings analysis
## **Goal**:

Import a JSON file to MongoDB and use PyMongo to update  and explore the data to answer a number of questions. This particular dataset contains a list of various establishments across the UK with location details and ratings data.  

## **Tools**:
MongoDB
## **Language**:
Python(Pandas, PyMongo)

## **Steps**:
1. Used *mongoimport* to import a JSON file and assigned the *establishments* collection to a variable.
2. Updated the *establishments* collection by inserting data for a new restaurant.
3. Performed a query to delete all the documents in the collection where "Dover Local Authority" is the value for LocalAuthorityName.
4. Performed a query to change the data type for 3 fields.
5. Performed a series of queries to answer the following questions:
- *Which establishments have a hygiene score equal to 20?*
- *Which establishments in London have a RatingValue greater than or equal to 4?*
- *What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?*
6. Built an aggregation pipeline to include a match query, group, and sort to answer the following question:
- *How many establishments in each Local Authority area have a hygiene score of 0,sorted from highest to lowest?*
6. Converted all the results to Pandas data frames.

### **References**
UK Food Standards AgencyLinks to an external site. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).


 

