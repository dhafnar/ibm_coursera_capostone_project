# Final Report

## Introduction/Business Problem

Belgian capital Brussels is the administrative seat of European Union. People who want to work for one of the european institutions often have to move there. It is something that quite some people I know - and are also from the european country of Slovenia - decided to do. 

Moving to a capital of another country is a big step, so one might want to move to a similar neighbourhood that he lived in his home country.

##Data

For the project, I will take Bežigrad, one of Ljubljana’s (capital of Slovenia) representative districts and compare it to the 19 municipalities of the Brussels-Capital Region. The goal is to find a municipality (or municipalities) that is the most similar in terms of venues to the Ljubljana’s representative district.

I will make the comparison based on the type of venues that are the most common in the district and municipalities. I will then perform a grouping using machine learning to determine which of the municipalities are the most similar to Bežigrad district.

Foursquare enables us to search for specific venues at a certain location. Venues are places like coffee shops, restaurants and shops. I will focus on types of venues, which are comparable across different locations.

For example, if the district is residential, you expect there to be a lot of small grocery stores, some coffee places etc. If the district is industrial, touristy or business oriented, the types of venues that are most frequent will be different. We will use the data and compare it with machine learning techniques to determine the most similar municipality.

The data used will be the list of 19 municipalities of the Brussels-Capital Region from Wikipedia. I will add the name of Bežigrad district to the generated list. From there, I will use Google Geocoding API data to get the coordinates of the district and municipalities. That will give me a dataframe I can use to get the data from Foursquare. I will then use k-means (machine learning technique for grouping) with different amount of centroids to determine one or more Brussels districts that is the closest to the Ljubljana’s Bežigrad district.
