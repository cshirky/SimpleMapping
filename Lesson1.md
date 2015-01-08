Google Maps #1: Basics of Location and Zoom

Ordinary Google maps put relevant location data right in the URL, allowing you to edit that URL in order to see how maps are positioned.

* Go to https://google.com/maps
* In the URL-bar of your browser, add the text in red onto the existing Maps URL:
	https://google.com/maps/@31,121,10z
	(Don’t neglect the leading slash. If your URL has a “%20” in it, you added a needless space.)
* Reload the map. You should get a map of eastern China, roughly centered on Shanghai:

* You can see there are three numbers after the @ sign, separated by commas, with the third ending in  z. What happens when you replace 5z with 3z and reload the map? 9z? 12z?

In 3D modeling, the Z axis is the vertical one, an extension into space of the familiar X and Y axes from graphing applications. For Google maps, z is both the vertical axis and specifies the zoom level. Possible zoom levels range from 1z (the globe) to 21z (the smallest area mapped.) Numbers below 1 are ignored, and fractional components are discarded.

* Go to https://google.com/maps/@31,121,12z. You should get a much more zoomed-in version of your first map, centered on southwest Shanghai. Now edit the first number to read 31.24, and the second number to 121.5, and reload the map. 

* You should now get a map showing downtown Pudong, centered almost exactly on the Pearl Tower. The first two numbers in the URL are Latitude (North/South location) and Longitude (East/West location.) These are the two essential numbers in geographic location, and are abbreviated lat and long, or sometimes lat/long or latlong.

* The 0° line for latitude is the equator. All latitudes north of the equator are positive numbers (Shanghai is around 31°, Beijing 40°, and so on.) The latitude of the North Pole (and thus the maximum latitude) is 90°. Latitudes south of the equator are negative numbers. The latitude of the South Pole is -90°. 

* The 0° line for longitude has no geographic logic. It is set by political convention as running through Greenwich, England. Longitudes to the east of Greenwich count up from 0. Longitudes to the west count down through negative numbers from 0. They meet on the opposite side of the world, in the Pacific Ocean. The International Date Line is at both 180° and -180° longitude.

* Turning the first number into 31.24 shifted the center of the map north by not quite a quarter of a degree. The length of 1° of latitude it is always close to 111 kilometers (it varies slightly, because the earth isn’t a perfect sphere), so adding .24 moved the center of the map about 26 kilometers.

* Turning the second number into 121.5 shifted the center of the map east half a degree. There is no standard length for longitude; 1° is close to 111 kilometers at the equator, but 0 at each pole. At Shanghai’s latitude, 1° is about 95.5 kilometers, so half a degree moved the center of the map about 48 kilometers. 

* Finally, familiarize yourself with basic map-moving operations: 
Click and drag to move the map
Double-click to zoom in a level
Double-right-click to zoom out a level
(The + and - buttons in the lower-left corner of the map also change the zoom level.)

Conclusion

Most mapping software does not allow you to edit latitude, longitude or zoom by hand. However, using Google maps, you can see the way all dynamic digital maps work, centering their maps around a point on the Earth’s surface, and using a zoom level to decide how to much area to show (with the obvious tradeoff of detail.)

No matter what mapping tools you use -- Google (Maps, My Maps, or Earth), CartoDB, Mapbox, or any of a host of others, the underlying data about points and views will always be expressed in lat/long and zoom, and all the data files stored and used by those applications rely on lat/long and zoom data.
