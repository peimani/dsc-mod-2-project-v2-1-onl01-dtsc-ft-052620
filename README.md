
# Module 2 K.C. Housing Prices


## Introduction

For this project we were tasked with taking housing data from King County, Washington and applying statistical analysis to see what affects housing prices.


## Project Summary

In this project we are going to use Object_Oriented Programming to Extract, Transform, and Load (ETL). Using what we have learned about statistics clean and analyze the relevant information to find strong correlations of the information that will give us what will affect the price of housing in King County. We will also take our work and analyze it for statistical significance so that we can have confidence in the information we are using. This will also help us with having more certainty in our analysis.

## Data Cleaning
The initial dataset that was loaded consisted of 21597 rows and 21 columns:

id - unique identified for a house
dateDate - house was sold
pricePrice - is prediction target
bedroomsNumber - of Bedrooms/House
bathroomsNumber - of bathrooms/bedrooms
sqft_livingsquare - footage of the home
sqft_lotsquare - footage of the lot
floorsTotal - floors (levels) in house
waterfront - House which has a view to a waterfront
view - Has been viewed
condition - How good the condition is ( Overall )
grade - overall grade given to the housing unit, based on King County grading system
sqft_above - square footage of house apart from basement
sqft_basement - square footage of the basement
yr_built - Built Year
yr_renovated - Year when house was renovated
zipcode - zip
lat - Latitude coordinate
long - Longitude coordinate
sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors
    
    1. The dataframe was checked for duplicates and missing values. This included taking a brief look at the data contained in each column as well as the type it was stored as. Null values were found and I got a description to get a statistical description of my dataset.
    2. A preliminary model was was made to evaluate the statistics of what we are working with.
    3. Using Exploratory Data Analysis I analyzed three questions:
        a. What affect does the condition of the house have on the price?
        b. Does Location affect house prices
        c. What is the effect of house size on it's price?
    4. Test the information for accuracy
       
Q1: What affect does the condition of the house have on the price?
    - There is a strong relationship with the house condition and it's price. Houses with a score of 3 and above show a large increase in price. According to the King County Assessors office, this means that houses that at minimum have been improved or need a normal amount of upkeep. If the home is need of many repairs and has much deferred maintenance the classification score of 1 or 2 are given. This causes the house value to drop. From this information we can use it to invest in houses at a condition of 1 or 2 and know that once it is updated we will see an increase in the price. It is flippable
    
Q2: Does Location affect House Price?
    - House prices are affected by location. To look at the correlation I made a density plot of housing sales, a cluster map of house sales as well as looking at the zipcodes with prices. When looking at all of this together we are able to see that certain areas will give you a higher price on a house sale. This will be helpful when we want find a house that needs work because we can see what it would be worth when it is fixed up in a specific area. 
    
Q3: What is the effect of house size on price?
    - This showed me that we could see that looking at the prices of the closest 15 neighbors will be helpfull in determining price. I also learned that a median square footage is where you can get the most for your money. The total square footage that was used in our data was a calculation of land and liveable square footage.

## Final Model

The final model was done after all the data cleaning, engineering and transformations. An R squared value of .930 was obtained. This was a significant increase from 0.662 (our baseline model). This means that around 93% of the variance in housing prices could be explained by this model. 93% of the variability of the data around the mean is explained by this model.

## Conclusion

This project was a steep learning curve. I feel like I had to first learn the many ways to analyze data with statistics. The next challenge was to learn how to manipulate the data and write the code in python. I did gain a lot of knowledge of new ways to visualize my information by creating maps and applying the appropriate graphs.

## Future Work

There is definitly more to learn. I feel like this was just the tip of the iceberg. I would like to look into other variables and also get more information on home renovation costs. I would like to fiqure out how to better analyze and compare zipcodes. I definitly could use more statistical analysis to learn more about my model. 

