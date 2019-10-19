# Identify-commercial-centers-using-Points-of-Interest-POI-data
This project is emphasised on creating clusters of distinct commercial centres using points of interest (POI) data of a city . Points of interest (POI) data provides location information of different places along with their defining tags like hotels, type of shops, type of amenities,etc


Getting Data:

POI (OSM) data- https://www.openstreetmap.org/#map=11/28.6518/77.2219

You can use overpy (a python frontend for overpass API of OSM) to get OSM data for the desired city  
and  can use overpass-turbo to frame queries)
 
Save or Export the data as geojson file.

Query to extract a point or known as node, here below a shop.

Reading data :

Geopandas library is used to read the geojson file exported from osm.

GeoPandas is an open source project to make working with geospatial data in python easier. GeoPandas extends the datatypes used by pandas to allow spatial operations on geometric types. Geometric operations are performed by shapely. Geopandas further depends on fiona for file access and descartes and matplotlib for plotting.


Visualization of spatial data:

Folium:
A python library built upon leaflet, which is a Java Script based web library. It provides enough customization and options to play with interactive web map.

Clustering with Machine Learning
In Data Science and Machine Learning, KMeans and DBScan are two of the most popular clustering(unsupervised) algorithms.

While dealing with spatial clusters of different density, size and shape, it could be challenging to detect the cluster of points. The task can be even more complicated if the data contains noise and outliers. To deal with large spatial databases, Martin Ester and his co-authors proposed Density-Based Spatial Clustering of Applications with Noise (DBSCAN), which still remains as one of the highest cited science papers.

Density clustering algorithms use the concept of reachability i.e. how many neighbors has a point within a radius. DBScan is more lovely because it doesn’t need parameter, k, which is the number of clusters we are trying to find, which KMeans needs. When you don’t know the number of clusters hidden in the dataset and there’s no way to visualize your dataset, it’s a good decision to use DBScan. DBSCAN produces a varying number of clusters, based on the input data.
 

 
