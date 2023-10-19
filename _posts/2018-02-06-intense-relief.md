---
layout: post
title:  "Intense relief"
date:   2018-02-01 
categories: maps, history, stroud
---


Local archaeologist, Neil Baker (who I mentioned in [Mapping The Heavens]({% post_url 2018-02-01-the-heavens %})) has done a lot of fieldwork and documentary research about the area.

He's identified a few interesting lumps and bumps, and I wondered if any might be easy enough to interpret in [Lidar-derived DEM data from Defra](http://www.mjk2.net/waffle/misc/Lidar/lidar.htm).

A Digital Elevation Model (DEM) is like a 3D map that shows the height of the ground. LIDAR is a technology that uses laser beams to measure these heights from the air. In GIS software, you can use a DEM to create a _hillshade model_, which is a visual representation that shows how sunlight would cast shadows on the terrain. This helps to highlight the hills, valleys, and other features of the landscape. Effectively, it creates a picture that shows how the land looks from above, when the sun shines on it.

Here's a satelite view of The Heavens on the left, with a hillshade model of the same area on the right:

![Two maps of "The Heavens" overlaid on each other, the top one semi-transparent, rendered in 3D with hills in high relief, viewed at an oblique angle](/assets/images/dem.png)
<!--more-->
The "sun" is shining (approximately) from the west. It's really hard to interpret on this kind of scale. And when the "sun" is shining from different angles, you can pick out quite different features.

![Two maps of "The Heavens" overlaid on each other, the top one semi-transparent, rendered in 3D with hills in high relief, viewed at an oblique angle](/assets/images/compare-hillshade.png)

I thought it would be interesting to compile them into a movie clip that simulates a light revolving around the area (sorry for the rubbish sizing):
<video width="601" height="541" controls loop>
  <source src="{{ site.baseurl }}/assets/videos/heavens-hillshade.mp4" type="video/mp4">

  Your browser does not support the video tag.
</video>

It's _kind of intense_ to watch.


To make it a bit easier to "scrub" back and forward between interesting frames, I assembled it into a [little web page that allows you to step frame-by-frame through the sequence](/old/heavens/hillshade.html).

I'm not sure it's at all helpful, but it was fun.