---
layout: post
title:  "An interactive, 3D Ordnance Survey map of Stroud"
date:   2016-04-04 
categories: maps
---

I made [a zoomable, draggable, 3D relief map of Stroud, using OS maps](/old/stroudviz/20160404144959.html).

![An Ordnance Survey map of the Five Valleys of Stroud, rendered in 3D with hills in high relief, viewed at an oblique angle](/assets/images/stroud0.png)


Sorry, reader: I didn't make detailed notes about how I did it, and it was a while ago. The brief version, as I recall it, is:

* I did it all with QGIS and plugins:
    * [Qgis2threejs](https://github.com/minorua/Qgis2threejs) to generate the visualisation
    * I can't remember how I got the LiDAR (DEM) models but it was [something like this](http://www.mjk2.net/waffle/misc/Lidar/lidar.htm)
    * I used Bing Maps with the [OpenLayers Plugin](https://plugins.qgis.org/plugins/openlayers_plugin/) to get the OS maps

It's interesting to see what Stroud would look like with a sea level of 60 meters (not that any climate models suggest sea levels going _that_ high):

![The same Ordnance Survey map of the Five Valleys of Stroud as the previous one on this page, as if it were flooded with water to the 60m contour](/assets/images/stroud1.png)


I also made one for a local historian, showing [the plan and height of now-demolished buildings in Badbrook](/old/stroudviz/20180226083305.html) (where the cinema complex currently stands):

![A small section of the Badbrook area of Stroud, Victorian map, with 3D shapes of different heights projected onto it](/assets/images/badbrook.png)

And one for my parents when they were taking part in a community project to survey the [historic landscape of Holmfirth](
/old/holmfirthviz2/20160408124243.html) (shows listed buildings, and trees)

![A 3D relief map of Holmfirth, 3D boxes representing listed buildings, green cones representing trees](/assets/images/holmfirth.png)

