# Clustering-Project-Identify-optimal-location-to-startup-coaching-class-
To identify best possible locations in an particular area in Mumbai to startup new or open new branch of coaching class in Mumbai. Coaching classes for shool going and junior college(11th and 12th).

In this project we will try to find an optimal location to startup Tuition Classes or franchise of existing Classes. This analysis will be targeted to stakeholders interested in opening a private Tuition Classes or management of existing Classes to expand their business & revenue by opening new branch/franchise in Mumbai.
Using Data science powers to generate a few most promising Area based clusters so that best possible final location can be chosen by stakeholders.

There are lots of Classes in Mumbai, we will try to detect locations that are not already crowded with Classes and having good number of existing Schools & Colleges to ensure sufficient student admissions and less business competition. We will also consider Commercial Property Rates of the locations.
Use clustering algorithm to clusters the areas/locations so that different clusters are made for decision making to become easier.

Data Collection
* List of all Areas in Mumbai along with their geographical coordinates (latitude & longitude) & location is web-scraped from Wikipedia website.  
* Commercial property rates of each area is collected from major Indian online real estate platforms
* Neighborhood Schools, Colleges and Classes in each Area will be retrieved using Foursquare API.

- - - - 
Plot all Areas on Map showing respective Property Rates using python folium library.
- - - - 
Calculate Business Opportunity Index for each Area. A good Business Opportunity Index means there are more Schools/Colleges and less Classes in a Area.
Business Opportunity Index = (Total no. of Schools & Colleges) / [ (Total no. of Classes & Tutorials) + 1 ]
- - - - 
Cluster Areas using k-Means and DBScan clustering algorithm.
- - - - 
Select cluster of Areas having high number of Schools & college and less existing Classes and affordable property rates.
Now, for more short listing of Areas apply a limit on business opportunity index depending on the investing capacity and area preference of the stakeholder.
Plot the selected optimal areas of map using Folium library.
- - - -
RESULTS:
For Kmeans
![image](https://user-images.githubusercontent.com/55849395/201733745-be37bce7-12f7-4fee-b700-e3b81a2241e5.png)

For DBSCAN
![image](https://user-images.githubusercontent.com/55849395/201733821-dac8ff73-4ae6-4b52-b3a4-463fd4f77034.png)

![image](https://user-images.githubusercontent.com/55849395/201733844-03837f9e-9bcb-401f-8121-c07ef426f96c.png)

- - - - 
ANALYSIS:

* In KMeans clustering Cluster_2 has Medium to high Property rate, less classes or coaching centers and due to that a medium start-up opportunity index. Where as in cluster_1 opportunity index is very high because of very low classes but has very high property rates.
* In DBScan clustering cluster -1 has highest opportunity index but very high property prices. In cluster_1 the property rates are medium and opportunity index is also medium.
* We can recommend these locations from cluster_1 from DBScan algorithm as it more accurately determines clusters according to property rate and opportunity index .



