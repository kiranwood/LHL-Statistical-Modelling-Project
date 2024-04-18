# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

This project is focused on API's, using python to clean and create a database, as well as perform an EDA and interpret statistical models. 

The goals of this project is to:
- Connect and compare multiple API's
- Join, clean and transform data
- Create a database using python
- Use visualization to explore data
- Build a statistical model

## Process

### Step 1 - Connect to API (city_bikes.ipynb)

Send a request to Citybikes (https://citybik.es/). Recieve all the information for bike stations in Siena Italy into a json format. Organize the data to grab longitude, latitude, station name and number of bikes. Turn the json file into a dataframe and save as a csv file (bike_stations.csv).

### Step 2 - Connect to multiple API's (yelp_foursquare_EDA.ipnb)

Connect to Foursquare API ((https://developer.foursquare.com/places) and Yelp Api (https://docs.developer.yelp.com/docs/fusion-intro). Using the longitude and latitude from each station in previous step, to get information on resturants within 1000m of station. From the data grab the resturant name, categories, address, distance from station, review count and ratings if applicable. Move this data into a dataframe and save as csv file(foursquare_restaurants.csv, yelp_restaurants). Compare the results of the two API's.

### Step 3 - Join Data (joining_data.ipynb)

Join the data from each of the API's into one dataframe. Save this dataframe as a csv(bike_and_restaurants.csv).

### Step 4 - Validate Join (joining_data.ipynb)

Inspect the data from before and after the join to validate that it was done correctly.

### Step 5 - EDA (joining_data.ipynb)

Using the newly joined dataframe, create graphs and visualization to explore the data. Interpret the results and turn the graphs into jpgs(scatter_and_his.jpg, boxplots.jpg).

### Step 6 - Database (joining_data.ipynb)

Turn the joined dataframe into an Database. Create the tables. Clean the dataframes and add data into the database.

### Step 7 - Regression Model (model_building.ipynb)

Use the database and SQL to create a dataframe to make a regression model thats based on the number of bikes in a station and the review counts and ratings from locations nearby that station. Interpert the results.

### Step 8 - Classification Model (model_building.ipynb)

Create an outline for how to turn the regression model from the previous step into a classification model.

### Step 9 - Final Touches

Move all the csv files and database into the data folder. As well as move the jpgs into the images file. Clean code for easy readability.

## Results

It was discovered that the Yelp API had more coverage compared to the Foursquare API as it not only included more detailed data (columns) but also more restaurants (rows).

The model showed that there was a positive correlation between the number of bikes in a station and the average rating of nearby resturants. The model showed a very good fit with low p values, high R-squared and F statistic. But the model may not be as reliable due to the low sample size.

## Challenges 

One of the biggest challenges was to decide which graphs and visualization to use since there were so many options. It was also difficult to figure out how each of the API's worked. As well as work out how to use the keys for the API's.

## Future Goals

With more time it is possible to look into alternate tests or methods instead of a regression model to provide a more reliable result. Another goal would be to create a classification model from the outline that was made in the project. It would also be interesting to explore the other ways to analyze the data of bike stations and nearby restaurants with the other unused data. 

