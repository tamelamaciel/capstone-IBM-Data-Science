# Coursera IBM Data Science Capstone Project
## Where to open an Indian restaurant in Ireland?  


By Tamela Maciel, June 2020

This jupyter notebook completes Coursera's IBM Data Science Professional Certificate capstone project.

It uses Irish census data (from the CSO data portal), the Foursquare API, BeautifulSoup for webscraping, k-Means clustering from scikit-learn, and various python libraries to clean, wrangle, and analyse the data.

![alt text](https://raw.githubusercontent.com/tamelamaciel/capstone-IBM-Data-Science/master/report/images/Indian_Spices.jpg "indian spices")

**The scenario**  

Our client runs several successful Indian restaurants in Leicester and throughout the UK, and is now seeking opportunities to expand into the Republic of Ireland. Ireland's economy is rapidly growing, especially in the tourism and food industry, and our client sees a gap in the Irish restaurant market for high-quality Indian food. 

The question is, where in Ireland should he open his new Indian restaurant? Where will the demand and relative scarcity of existing Indian restaurants be best served by a new venue?

Our client has three criteria which he believes will lead to a successful new Indian restaurant:
- A city in Ireland that is similar or larger in relative size compared to Leicester.
- A relative lack of Indian restaurants in that city.
- A relatively high proportion of residents who are Asian or Irish Asian.

Guided by these criteria, this notebook analyses a combination of census and venue location data in order to recommend the best location in Ireland for a new Indian restaurant. It clusters and profiles Irish cities based on types of restaurants, and uses this in combination with census data on population and demographics to identify the ideal new location for our client.

**Python libraries**

Pandas, Numpy, BeautifulSoup  
Shapely, Geopy  
KMeans from Sklearn.cluster  
Folium, Matplotlib, Seaborn  

**Key plots**

![alt text](https://raw.githubusercontent.com/tamelamaciel/capstone-IBM-Data-Science/master/report/images/percentage_asian_vs_indian_restaurants_scatterplot.png "scatter plot")

![alt text](https://raw.githubusercontent.com/tamelamaciel/capstone-IBM-Data-Science/master/report/images/final_cluster_map_inset.png "final choropleth")

**Results**

The cluster profiles combined with knowledge of the proportion of Asian residents in each city allows us to clearly identify those with a lack of current Indian restaurants but a relatively high Asian population. 

**These cities are our top three recommendations for locating a new Indian restaurant in Ireland:**

- **Dublin**: 2.8% Asian population, only 2 Indian restaurants out of 47 (4.3%), and no Indian restaurants in its most common 5 restaurants
- **Swords**: 3.2% Asian population, only 1 Indian restaurant out of 9 (11.1%), and no Indian restaurants in its most common 5 restaurants
- **Cork**: 2.1% Asian population, only 1 Indian restaurant out of 29 (3.4%), and no Indian restaurants in its most common 5 restaurants

**In addition, there are two additional cities that have good potential and would be worth considering by the client as strong runners-up:**

- **Galway**: 2.5% Asian population and only 3 Indian restaurants out of 39 (7.7%). However, its 3rd most common restaurant is an Indian restaurant, unlike our top three cities.
- **Limerick**: 1.8% Asian population (which is low but not far off of Cork), only 1 Indian restaurant out of 25 (4%), and no Indian restaurants in its most common 5 restaurants
