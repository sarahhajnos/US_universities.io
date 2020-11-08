[US_universities]
  	│index.html
    │readme.md
    ├─assets
    │      [us_colleges].geojson
    │      [us_urbanareas].geojson

For lab 3, I mapped the higher education schools in North Carolina per county. The schools dataset contained point data. Schools were categorized as: colleges, universities, and professional schools; technical and trade schools; and others. This data was from USGS, Science Base Catalog. I took this data and filtered it for higher education schools in NC, using select by attributes in QGIS (I later realized I could have found the same data from NC One Map). Then I found a shapefile of NC counties from NC One Map. I combined the two datasets in QGIS and then used the number of points calculator. I then exported this file in order to have the 'NUMPOINTS' attribute to count the number of schools per county.

I used ESRI World Gray Canvas as the basemap and centered the web map on the middle of North Carolina. I made the font Georgia in the serif family and used 'fas fa-university marker-color' for the symbol. The counties are various shades of green and categorized by number of secondary schools based on equal interval classifications. The university symbols were color coded using the Set3 scale.

Originally, I had the same map but I mapped every college and university for the entire country. The map was incredibly slow to load (I am assuming it was due to the amount of data that needed to be loaded), so I decided to alter my plan and map only North Carolina. This helped the map's performance and overall look. Before, the map was cluttered and wasn't asthetically pleasing. The end result looks much better, although I would have prefered using different colors for the symbols (I had trouble changing the third color so I opted to keep it). 
