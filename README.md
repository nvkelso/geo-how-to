![Tile Previews](https://github.com/nvkelso/geo-how-to/raw/master/images/tile_providers_preview.png)

The tips and tricks here are oriented to BYOD (bring your down data) mapping and OpenStreetMap obliquely.

Presentation cartography and basic inventory mapping is the focus here. Spatial analytics is touched upon briefly but is not the main focus. This site makes assumptions that OpenSource GIS mostly means: PostGIS as a spatial data store and Mapnik as a rendering engine, a Mappy CSS styling language like Cascadenik or Carto to setup the layers and their appearance. Interactivity is briefly touched on. Actually embedding the resulting tile assets is briefly touched on.

_Looking for an overview of OSM instead? Check out the [Switch2osm](http://switch2osm.org/) site._


## Getting started

* [Software](https://github.com/nvkelso/geo-how-to/wiki/Getting-started:-SOFTWARE) - Install critical software and links to tutorials.

* [Data](https://github.com/nvkelso/geo-how-to/wiki/Getting-started:-DATA) - Download OSM and Natural Earth data.

* [Example workflow](https://github.com/nvkelso/geo-how-to/wiki/Getting-started:-WORKFLOW) - Start a project, import data, export data, create tiles.

* [Web mapping = API + tiles](https://github.com/nvkelso/geo-how-to/wiki/Getting-started:-OVERVIEW) - Slippy maps on the web have two parts: images tiles that make up the map, and an API framework that stitches tiles together and handles interactive panning and zooming.

* [Why go open source geo](https://github.com/nvkelso/geo-how-to/wiki/Why-go-open-source-geo) - Read what the community is saying.

* [Map examples](https://github.com/nvkelso/geo-how-to/wiki/Map-examples) - Pretty basemap tiles and compelling interactive maps.

* [When tiles aren't enough](https://github.com/nvkelso/geo-how-to/wiki/Print-and-big-map-images) - Use your web map stylesheet to render larger raster images and export to PDF, EPS, and SVG.


## Mapping

### Workflow:

* [Map Styling](https://github.com/nvkelso/geo-how-to/wiki/Map-Styling-in-cascadenik,-carto) - Color your map features using cascadenik or carto since raw Mapnik XML is hellish.

* [Rendering map tiles](https://github.com/nvkelso/geo-how-to/wiki/Rendering-map-tiles) - Once you're done designing your map, you'll need to render 10s of thousands of tiny image files, hundreds and thousands of megabytes in size.

* [Hosting Tiles](https://github.com/nvkelso/geo-how-to/wiki/Hosting tiles) - Publish your tiles so others can see them. Amazon S3, EC2, CloudFront, your own server, MapBox.com, etc.


### Upping your game:

* [Map Labels](https://github.com/nvkelso/geo-how-to/wiki/Labels) - Tips for labeling features. 

* [Style Hub](https://github.com/nvkelso/geo-how-to/wiki/Style-Hub) - Pre-baked stylesheets and icons for drawing OSM and Natural Earth data.

* [Adding interactivity](https://github.com/nvkelso/geo-how-to/wiki/Adding interactivity) - UTF-8 grids + hybrid tile vector maps

* [Is your map effective?](https://github.com/nvkelso/geo-how-to/wiki/Is your map effective) - Take a critical look at your work, evaluate it with a consistent rubric, and ask, "Is my map great?"

* [Viewing map tiles in desktop GIS apps](https://github.com/nvkelso/geo-how-to/wiki/Viewing map tiles in desktop GIS apps) - For QGIS, ArcGIS, and Manifold.

* [Map scales/zooms, coordinate systems](https://github.com/nvkelso/geo-how-to/wiki/Map-scales---zooms) - Web maps have 20 preset scales, learn these “zoom” levels and their natural scale equivelents.

* [Generalize your data](https://github.com/nvkelso/geo-how-to/wiki/Generalize your data) - Seriously. Your maps will look better and load faster.


### Tools of the trade:

* [QGIS](https://github.com/nvkelso/geo-how-to/wiki/QGIS) - The open source alternative to ArcMap, but not as industrial strength. It's a GUI for composing maps and doing simple analysis.

* [PostGIS](https://github.com/nvkelso/geo-how-to/wiki/PostGIS) - Store your geography in a spatial database (kinda the open source version of an Esri GeoDB). Faster than raw SHP files when speed matters. Storage default for OSM data.

* [OGR, GDAL](https://github.com/nvkelso/geo-how-to/wiki/OGR-to-reproject,-modify-Shapefiles) - Reproject, sort, filter and otherwise modify Shapefiles and other vector map data formats. GDAL for raster. These are amazingly powerful.

* [Mapnik](https://github.com/nvkelso/geo-how-to/wiki/Mapnik) - Draw web map tiles, industrial strength.

* [TileStache](https://github.com/nvkelso/geo-how-to/wiki/TileStache) - Cache web map tiles, from Stamen.

* [TileMill](http://mapbox.com/tilemill/) - Desktop "web" app with an easy installer, powered by Mapnik and Carto. From Development Seed / MapBox.

* [Dymo](https://github.com/nvkelso/geo-how-to/wiki/Dymo) - Create beautiful map labels, from Stamen. Like Annotation from ArcGIS.

* [Shapely](https://github.com/nvkelso/geo-how-to/wiki/Shapely) - Python library for geometric objects, predicates, and operations without requiring PostGIS.

* [pprepair](http://tudelft-gist.github.com/pprepair/) - Validate and automatically repair planar partitions.

* [Merge SHPs, GeoJSON, and more into single files](https://gist.github.com/3759113) - Good tool from Dane. [Alternative](https://gist.github.com/3759608) from Mike.

* [GeoJSON](https://github.com/nvkelso/geo-how-to/wiki/GeoJSON) - Make it smaller. Giving your data the precision it's accuracy deserves.

* [D3.js](http://www.smartjava.org/content/using-d3js-visualize-gis) - A robust data visualization library with built in geography support.

* [Kartograph](http://kartograph.org/) - Kartograph is a new framework for building interactive vector map applications without Google Maps or any other mapping service. It was created with the needs of designers and data journalists in mind. Tons of map projections, gracefully degrades to IE7. Great for thematic maps that are smaller scale than 1:250,000.

* [MaPublisher](https://github.com/nvkelso/geo-how-to/wiki/MaPublisher) - Make maps in Adobe Illustrator.

* [OpenStreetMap](https://github.com/nvkelso/geo-how-to/wiki/OpenStreetMap) - aka OSM. How to import it and explore the tag universe.

* [Geocoding](https://github.com/nvkelso/geo-how-to/wiki/Geocoding) - This is the one hard part about going open source geo.

* [Routing](https://github.com/nvkelso/geo-how-to/wiki/Routing) - The MapQuest Open API returns routing based on OSM data

* [Shaded relief](https://github.com/nvkelso/geo-how-to/wiki/Shaded relief) - set of utilities for processing DEM (digital elevation models, digital terrain models) and shading that to indicate the shape of mountains and other relief features. 

* [Land cover](https://github.com/nvkelso/geo-how-to/wiki/Land cover) - set of utilities for processing classified TIF images and colorizing techniques to indicate type (or presence) of vegetation and land use.


## Unix command line

* [Makefiles](https://github.com/nvkelso/geo-how-to/wiki/Make-files) - Key to organizing your workflow and making it repeatable.

* [Python](https://github.com/nvkelso/geo-how-to/wiki/Python) - tk tk tk

* [General Unix commands](https://github.com/nvkelso/geo-how-to/wiki/Unix-commands)

* [Download onto server using CURL](https://github.com/nvkelso/geo-how-to/wiki/Download-onto-server-using-CURL)

* [File permissions](https://github.com/nvkelso/geo-how-to/wiki/File-permissions)

* [GREP](https://github.com/nvkelso/geo-how-to/wiki/GREP) - Data formatting problems? Advanced text find-replace to the rescue.

* [SSH keys](https://github.com/nvkelso/geo-how-to/wiki/SSH-keys)

* [Shell scripts](https://github.com/nvkelso/geo-how-to/wiki/Shell-scripts)

* [ZIP on the server](https://github.com/nvkelso/geo-how-to/wiki/ZIP-on-the-server)

## Project management:

* [Git aka Github](https://github.com/nvkelso/geo-how-to/wiki/Github)

* [SVN aka Subversion](https://github.com/nvkelso/geo-how-to/wiki/SVN-aka-Subversion)


## Other

* [Markdown is the devil](https://github.com/nvkelso/geo-how-to/wiki/Markdown-is-evil) - Yet another random raw text formatting style without a GUI.