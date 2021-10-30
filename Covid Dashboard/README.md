
# Covid19 Dashboard
![Screenshot (606)](https://user-images.githubusercontent.com/39759685/133439977-b198cae5-7f51-4f77-b79f-cf4cc6fc4194.png)


The Following project aims on Collecting The data from different sources, then **GEO-TAG** them, and finall present them in a Dyanmic Way and Responsive way.



## Data Collection
The Data is collected from this [link!](https://github.com/covid19india/api)

This dataset is not geo-tagged i.e. it does not contain the latitude and longitude for the registered Covid Case, But it do have the Address of that patient. So `Data collection.ipynb`
is the file that feteches the Latitde and Longitude from the Internet using `Google Maps API`.

## GeoJSON File

I have used the GeoJSON file for the Plotting My state, Jhanrknad and WestBengal. Following is one example:

![jharkhnad](https://user-images.githubusercontent.com/39759685/133441208-f6378ea0-aa63-42be-9dd2-48dd22df1494.png)

## Developing a Dynamic Dashsboard, That has Three colors of labels, 
 - Red : Region That have cases greated than 500
 - Blue : Region that have case greater than 200 and less than 500
 - Green : Region that have cases less than 200
 Following Video Demostrated the Dynamic map
 
 https://user-images.githubusercontent.com/39759685/133437693-757fa9e1-7ece-40c7-a11b-8ab2151c3330.mp4
 
 ## Developing a Time Series Map (BONUS)
 
 I have created a time series map that show the number of Cases in a region. For example, when the Color of one region is darker that the other that means that area has higher Corona Pateients at that time
 
 
 

https://user-images.githubusercontent.com/39759685/133442766-e806be44-68ce-400c-880c-eb3856029c30.mp4

## Professional bar plot



https://user-images.githubusercontent.com/39759685/139533427-e6aacb37-99a5-4e23-86aa-a5766464cad0.mp4



https://user-images.githubusercontent.com/39759685/139533430-193c4b1f-68c3-4e8c-ba23-dbd34e4e7e82.mp4



https://user-images.githubusercontent.com/39759685/139533433-892314d5-b8aa-4e3f-9ec2-836dee515ef4.mp4



https://user-images.githubusercontent.com/39759685/139533436-dcb86efc-42bb-4b8d-8ecf-cccf62b7d06c.mp4



https://user-images.githubusercontent.com/39759685/139533439-f3523e24-1652-459a-8ac2-4e01c39e953e.mp4



https://user-images.githubusercontent.com/39759685/139533440-b30c72cc-c45d-46e1-8570-a1e53f2da1c8.mp4





