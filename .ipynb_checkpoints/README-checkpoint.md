# Module_6_challenge

This assignment requires you to imagine you work for a proptech company. The company wants to offer an instant, one-click service for people to buy properties and then rent them. San Francisco data is used in this trial run. Your job is to use your data visualization skills, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

We begin by importing our technologies, dependencies, and data. 

CALCULATE AND PLOT THE HOUSING UNITS PER YEAR
This first section requires us to find the average housing units grouped by year. All other data is to be dropped. The housing units are then plotted by year in a bar chart. This chart demonstrates an increase of approximately 10,000 units in the six years shown. 

CALCULATE AND PLOT THE AVERAGE SALE PRICE PER SQUARE FOOT
This next section requires us to group by year the average sale price and gross rent. This data is plotted on a line chart. The line chart demonstrates a very gradual, slow increase in sale price per square foot but a rather steep increase in gross rent. In fact, gross rent almost quadrupled over the six years.

COMPARE THE AVERAGE SALE PRICE BY NEIGHBORHOOD
This section builds on the previous one. The difference is that the line chart has a drop-down menu allowing us to toggle between different neighborhoods. This added functionality allows us to analyze the growth in sale price per square foot and gross rent for each neighborhood individually. 

BUILD AN INTERACTIVE NEIGHBORHOOD MAP
In this section, we concatenate the previous dataframe with one that has longitudes and latitudes for each neighborhood. This new dataframe is cleaned and used to plot an interactive map displaying sale price and gross rent for each neighborhood. The size of the spot on the map correlates to the sale price per square foot. The color of the spot correlates to the gross rent; the spots get darker with higher rents. 

COMPOSE YOUR DATA STORY
Finally, this section requires us to use all the graphs previously created to create a story and make a recommendation. We copied the first two line graphs to have them together and avoid so much scrolling back and forth. We then took it a step further and created a new dataframe grouping the average sale price and gross rent by neighborhood. We excluded the year to analyze the average difference between sale price and rent in general, not in a trend over time. Once we plotted this data, we were able to visualize said differences. The chart allowed us to see which neighborhoods had the largest differences in one visual. Once the potential neighborhoods were identified, we went back to the second line graph and chose those neighborhoods in the drop-down menu. Seeing the trends of the specific neighborhoods over time either confirmed or denied our initial conclusions. 

We answered the following questions:

QUESTION: How does the trend in rental income growth compare to the trend in sales prices? Does this same trend hold true for all the neighborhoods across San Francisco?

ANSWER: As seen on "Sale Price per Square Foot and Gross Rent", the average trends across San Francisco's rental income and sales price are positive. Nonetheless, there is a large discrepancy between the growth rate of each. The Sale Price per Square Foot and Gross Rent graph above shows the sales price grew at a very slow pace while gross rent skyrocketed in the same timeframe.

The growth trend of gross rent for individual neighborhoods stays positive, but the sale price trend does not always stay positive. Alamo Square, for example, had sales price decline in 2016, which caused a rather horizontal trend. Still, other neighborhoods like Westwood Park have a negative correlation with sale prices very gradually lowering and gross rent rising linearly.


QUESTION: What insights can you share with your company about the potential one-click, buy-and-rent strategy that they're pursuing? Do neighborhoods exist that you would suggest for investment, and why?

ANSWER: The strategy works with some limitations taking into consideration some specifics. Overall, most neighborhoods will yield a return on investment because sale prices grow at a very gradual pace. Compare that growth with the rather steep gross rent growth. The disparity between these two metrics only increases with time.

Now, if you're trying to find the best bang for your buck and are trying to find the cheapest prices with the highest rent, then the options are much fewer depending on the disparity you seek. Take a look at the sfo_df hvplot below. Find the largest difference between price and rent on this plot and save yourself the time of clicking through the "Sale Price per Sq. ft. and Gross Rent grouped by Neighborhood'.



CODE SOURCE
All code was sourced or derived from the class activities. I had help from a "Slack tutor." I messaged the AskBCS Learning Assistant. Kimberly Rodriguez also shared how she concatenated the neighborhood locations with the existing dataframe, which shed some light on my issue with indexing; I kept producing numerical indexes which caused issues with my plotting. 



TECHNOLOGIES
This project used Pandas and hvplot. Python is the language used. The project was completed on a jupyter notebook. 