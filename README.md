# GeoData_WS2020_II_Final_Group_J
GeoData_WS2020_II_Final_Group_J 

# GeoData_WS2020_II_Final_Group_J

## Introduction
Pan Hongqin is responsible for Exercise 4 and Exercise 5
Ding Yonghan is responsible for Exercise 3
Xiao Hanzhang is responsible for Exercise 1 & 2 & 6

## EX3. Compare the NDVI values of two different years (Yonghan Ding)

* First Creat two new layers from the Download files, and from the knowleadge of the NDVI calculation formular that should select the B4 and B8

![Creat new layers](https://user-images.githubusercontent.com/78090508/111850407-7cba5380-8910-11eb-907b-875571702f9a.png)












## EX4. Digitize the graves of uedemer hochwaldbuds (Pan)

### Task 1：
* Add the layer and open the raster - georeferencer. Here, I chose 10 intersections as the coordinates.

![](figures/EX4/T1-1.png)

* Choosing the same position on the map

![](figures/EX4/T1-2.png)

* Select transformation type - Thin plate spline(At first, l chose the transformation type as liner but it can’t match the original map. With the help from Mr. JonasZ, he found that changing the transformation type could solve the problem.)

![](figures/EX4/T1-3.png)

* If there is a black shadow at there, open the porperity and choose the transparency - adding 0 to additional no date value.

![](figures/EX4/T1-4.png)


* Georeferencered Map

![](figures/EX4/T1-5.png)


### Task 2:
* Change the transperency to 40%.

![](figures/EX4/T2-1.png)

* After the map was made, we can found that the burial mounds were nearly matched the map and the burial mounds were densely distributed. The location of the burial mounds in the picture corresponds to the larger burial mounds on the map and many smaller tombs scattered around which were not showed in the picture.  
(Tutorials reference: http://www.qgistutorials.com/en/docs/3/making_a_map.html )

![](figures/EX4/T2-2.png)


## Task 3:
* Choosing Render type - singleband pseudocolor and choosing the color ramp.

![](figures/EX4/T3-1.png)

* Color rendering - Blending mode - multply.

![](figures/EX4/T3-2.png)

* Properity - Transparency - 60% , the hillshade model was finished.

![](figures/EX4/T3-3.png)

### Task 4:
* Create a new point vector layer and point the burial mounds.
Here, l forgot how to measure the altitude. This task was not finished(l’m sorry for that)

![](figures/EX4/T4-1.png)

* With the point sampling tool you can sample these points and get the altitude.
Orthometric Height = Ellipsoidal Height - Geoid Height

![](figures/EX4/T4-2.png)

### Task 5:
* Create a new liner vector layer and digitize it.

![](figures/EX4/T5-1.png)


* We can see that there are many diameters that are parallel to the northeast. The origin of these patterns were supposed to be the farmland.

![](figures/EX4/T5-2.png)






## EX5.	Free exercise (Pan)

### Introduction:
This is a very interesting exercise I saw in the tutorial. lt introduces two methods of making contour plane, in order to master the visual expression of contour plane, to master the transformation of DEM data to contour line and the extraction, transformation, separation and color matching of contour line.

1. First way
Using DEM data to extract the contour
Raster - Extraction - contour line

![](figures/EX5/6.png)

Result:

![](figures/EX5/7.png)

After that, changing the contour line to ploygons
Vector - geometry tools - line to polygons

![](figures/EX5/8.png)

2. Second way
(Its a trick. We can directly use The contour data provided by the axismaps web site for making the Contour layer)

* Open Baidu coordinate pick system, pick up the coordinates you want to study the area of points (here, for example, Mount Everest)

![](figures/EX5/1.png)

* Change the URL according to the latitude and longitude, and wait for the contour to be drawn
When the system was loading, changing the unit of the contour to meter. After that , downloading  the geoJSON package.
Open the geoJson package in Qgis and export as shapefile.

![](figures/EX5/2.png)

3. Two different ways to get the contour plane, and the subsequent methods are the same

To symbolize the contour plane, set the layer to "Progressive" in the layer style, set the VALUE to ELEV, and then click "Categorize" to select the appropriate gradient for expression.Select Equa Count in the mode.

![](figures/EX5/9.png)


* To symbolize, change the stroke line width to 0.06

![](figures/EX5/4.png)

* The final result

![](figures/EX5/5.png)
