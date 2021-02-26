## Analysis of Airbnb Listings in Paris

### Date created
02/25/2021


### About the Project 
The objective of this project is to analyze data of Airbnb listings in Paris to determine the variables that impact listing price the most and allow us to create machine learning models to predict the price of listings and potential listings. With this information we can be better informed when selecting a potential or existing property to host on Airbnb in Paris. While Airbnb has 3 primary room types ("Entire place", "Private room", and "Shared room") this project focuses exclusively on "Entire place" listings since these categories represent vastly different types of listings and potentially have different variables that impact the listing price.

Questions explored are:
1. Can we create a model that accurately predicts the price or review score based on features in this dataset?
2. Which listing features have the strongest correlations to 'price'?
3. Which listing features have the strongest correlations to 'review_scores_rating'?
4. Which Paris neighborhoods have the highest average listing price?
5. Which Paris neighborhoods have the most/least amount of listings? Do the neighborhoods with fewer listings have higher average listing prices?  
6. Are there times of the year that listing prices increase or decrease?


### Installation Requirements
This project was created using Python 3.* and the common Python libraries such as Numpy, Pandas, Mathplotlib and Seaborn.


### Data Overview
Data was provided by [Inside Airbnb](http://insideairbnb.com/get-the-data.html) under a Creative Commons CC0 1.0 Universal (CC0 1.0) "Public Domain Dedication" license.

The three datasets that were used for this analysis of Airbnb listings in Paris were:

- **listings.csv** - General listing data for each listing ID currently available for rent on Airbnb in Paris.  
- **calendar.csv** - Calendars of availability for each listing in Paris over a one year period from the scrub date.  
- **reviews.csv** - All reviews left for all listing IDs currently available for rent on Airbnb in Paris.  


### Results
The main findings of this project can be found at the [blog post available here](https://medium.com/).  

An additional visualization of the dataset created above can be found in a Tableau dashboard [here](https://public.tableau.com/views/ParisAirbnbAnalysis/Eiffel?:language=en&:display_count=y&publish=yes&:origin=viz_share_link).


### Acknowledgements
The resources used to complete this project were:

How to create a new column that calculated the number of days between 2 dates:
https://stackoverflow.com/questions/33605514/how-to-extract-days-as-integers-from-a-timedelta64ns-object-in-python

How to strip $ and ',' from the 'price' column and convert it from dtype object:
https://stackoverflow.com/questions/25669588/convert-percent-string-to-float-in-pandas-read-csv

How to find the IQR for outlier detection using numpy.percentile:
https://www.geeksforgeeks.org/interquartile-range-and-quartile-deviation-using-numpy-and-scipy/

How to strip '%' from the host_response_rate column and convert it from dtype object:
https://stackoverflow.com/questions/25669588/convert-percent-string-to-float-in-pandas-read-csv

How to sort categorical data into Bins (used to handle NaN values:
- O'Reilly "Hands-On Machine Learning with Scikit-Learn, Keras, & TensorFlow" by Aurelien Geron page 54.

How to convert the host_is_superhost and instant_bookable columns to be bool dtype True/False:
https://pbpython.com/pandas_dtypes.html

Guidance to assist with use of Lasso Regression using Sklearn:
- "Machine Learning with Python Cookbook" by Chris Albon Section 13.4 pages 229-232

Guidance to assist with use of Elastic Net Regression using Sklearn:
https://machinelearningmastery.com/elastic-net-regression-in-python/