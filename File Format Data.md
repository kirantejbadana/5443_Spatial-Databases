##Homework 1##

###File Format Data###

####Shape File:####
This is a digital format of storing the information of the points which will contribute for making a figure. Shape files are simple because they store the primitive geometric data types of points, lines, and polygons. They are of limited use without any attributes to specify what they represent. These files are used for identifying the geometry and special positioning of the point.

####OSM File: #####
OSM file has a primitive data values like Nodes, Ways and relations. Nodes will be uniquely represented by the unique ID of the node. Location of the Nodes will be determined by the latitudes and longitudes. For evaluating the data present in the file we use the DTD Schema file which will make sure the file present is in a relevant format.

####Geo JSON: #####
Geo JSON is an open standard format for encoding collections of simple geographical feature along with their non-spatial attributes using JavaScript Object Notation. The features include points (therefore addresses and locations), line strings (therefore streets, highways and boundaries), polygons (countries, provinces, tracts of land), and multi-part collections of these types. Geo JSON features need not represent entities of the physical world only; mobile routing and navigation apps, for example, might describe their service coverage using Geo JSON.


#####GPX Format:#####
GPX, or GPS Exchange Format, is an XML Schema designed as a common GPS data format for software applications. It can be used to describe waypoints, tracks, and routes. The format is open and can be used without the need to pay license fees. Its tags store location, elevation, and time and can in this way be used to interchange data between GPS devices and software packages. Such computer programs allow users, for example, to view their tracks, project their tracks on satellite images or other maps, annotate maps, and tag photographs with the geolocation in the Exif metadata.

#####KML File Format:#####
You can create KML files with the Google Earth user interface, or you can use an XML or simple text editor to enter "raw" KML from scratch. KML files and their related images (if any) can be compressed using the ZIP format into KMZ archives. To share your KML and KMZ files, you can e-mail them, host them locally for sharing within a private internet, or host them publicly on a web server. Just as web browsers display HTML files, Earth browsers such as Google Earth display KML files. Once you've properly configured your server and shared the URL (address) of your KML files, anyone who's installed Google Earth can view the KML files hosted on your public web server.

####NMEA File Format:####
The National Marine Electronics Association (NMEA) has developed a specification that defines the interface between various pieces of marine electronic equipment. The standard permits marine electronics to send information to computers and to other marine equipment. The idea of NMEA is to send a line of data called a sentence that is totally self-contained and independent from other sentences. There are standard sentences for each device category and there is also the ability to define proprietary sentences for use by the individual company. All of the standard sentences have a two letter prefix that defines the device that uses that sentence type.

####CSV File Format:####
A comma-separated values (CSV) (also sometimes called character-separated values, because the separator character does not have to be a comma) file stores tabular data (numbers and text) in plain-text form. Plain text means that the file is a sequence of characters, with no data that has to be interpreted instead, as binary numbers. A CSV file consists of any number of records, separated by line breaks of some kind; each record consists of fields, separated by some other character or string, most commonly a literal comma or tab. Usually, all records have an identical sequence of fields.

####WKT File Format:#####
Well-known text (WKT) is a text markup language for representing vector geometry objects on a map, spatial reference systems of spatial objects and transformations between spatial reference systems. A binary equivalent, known as well-known binary (WKB) is used to transfer and store the same information on databases, such as PostGIS, Microsoft SQL Server and DB2. The formats were originally defined by the Open Geospatial Consortium (OGC) and described in their Simple Feature Access and Coordinate Transformation Service specifications.

####Software List:####

####ArcGis Software:####
ArcGis Software is used to create, share, and manage geographic data, maps, and analytical models using desktop and server applications. Deploy GIS across your organization and on the web.

##ArcGis Software Modules:##
GIS Professionals: GIS Professionals can create and manage data, maps and analytical models. They can then extend the reach of their work by sharing what they create across their organization.

Location Analytics: Location Analytics offers a way to add a geographic dimension to your business analytics systems. Make informed decisions by visualizing critical information on a map.

Developers: Developers can add mapping to web, mobile, and desktop applications using a choice of languages.


####QGIS Software:#####
QGIS is open source software package and QGIS offers many common GIS functionalities provided by core features and plugins. A short summary of six general categories of features and plugins is presented below, followed by first insights into the integrated Python console.

####GPSBABEL Software:####
GPSBabel is a cross-platform, free software to transfer routes, tracks, and waypoint data to and from consumer GPS unit, and to convert between over a hundred types of GPS data formats.[1] It has a command-line interface and a graphical interface for windows, OS X, and Linux users.

####GDAL Software:#####
GDAL(Geospatial Data Abstraction Library) is a translator library for raster and vector geospatial data formats that is released under an X/MIT style Open Source license by the Open Source Geospatial Foundation. As a library, it presents a single raster abstract data model and vector abstract data model to the calling application for all supported formats. It also comes with a variety of useful command line utilities for data translation and processing.

### Definitions: ###

####Point:####
A point is an exact position or location on a plane surface. It is important to understand that a point is not a thing, but a place. Here we represent the point using latitude and longitude and time zone. 

####Curve:####
A curve (also called a curved line in older texts) is, generally speaking, an object similar to a line but which is not required to be straight. This entails that a line is a special case of curve, namely a curve with null curvature.

#####LineString:####
A LineString is a one-dimensional object representing a sequence of points and the line segments connecting them.

####Multi-Curve:####
A Multi-Curve is a 1-dimensional Geometry Collection whose elements are Curves. 

####MultiLineStrings:####
A string literal is the representation of a string value within the source code of a computer program. Most often in modern languages this is a quoted sequence of characters (formally "bracketed delimiters"), as in x = "foo", where "foo" is a string literal with value foo – the quotes are not part of the value, and one must use escape characters to allow the delimiters themselves to be embedded in the string.

####Surface Polygon:####
In the general case it allows to specify a list of arbitrary polygons (convex or concave) with optional holes using any number of vertices and edges. The polygons may be connected by shared vertices to form a mesh. Materials can be assigned to the whole mesh or per polygon. It is possible to attach any kind of extra data on a per vertex basis, like texture coordinates or user values. The source description of polygon surfaces is subject to tessellation and displacement for rendering.

####Multi polygon:####
A multipolygon relation can have any number of ways in the role outer (the outline) and any number of ways in the role inner (the holes), and these must somehow form valid rings to build a multipolygon.

####Touches####
- If the neighbor polygon is an overlapping neighbor and the Include area overlaps check box is checked
  - Add the AREA field to the output table.
  - Calculate the area of the overlap.
  - Record the calculated area for use in the output table AREA field.
  - Record 0 for use in the output table LENGTH field.
  - Record 0 for use in the output table NODE_COUNT field.
  - Overlapping neighbor analysis is complete. Analyze the next neighbor polygon.
- If the neighbor polygon is an edge neighbor
  - Calculate the length of the coincident boundary.
  - Record the calculated length for use in the LENGTH field.
  - Record 0 for use in the NODE_COUNT field.
  - Edge neighbor analysis is complete. Analyze the next neighbor polygon.
- If the neighbor polygon is a node neighbor
  - Find the number of times the neighbor polygon crosses and touches the source polygon at a point.
  - Record this count value for use in the NODE_COUNT field.
  - Record 0 for use in the LENGTH field.
  - Node neighbor analysis is complete. Analyze the next neighbor polygon.

####Crosses####
- Using polygon 1 as the source polygon for an example, three neighbor polygons are found, and the following information is reported in the output table below:
  - Polygon 2 overlaps polygon 1; the area of overlap, 1600, is written in the AREA field. The analysis of edge and node neighbors is skipped even though polygon 2 has a coincident edge with polygon 1 and crosses it at a point. Therefore, the fields LENGTH and NODE_COUNT get a value of 0.
  - Polygon 4 has a coincident edge with polygon 1; the coincident length of the edge, 100, is written in the LENGTH field.
  - Polygon 5 has a coincident edge with polygon 1; the length of the coincident edge, 20, is written in the LENGTH field. The node neighbor analysis is skipped even though it crosses polygon 1 at a point. The field NODE_COUNT gets a value of 0.

####Within#####
Among the following four polygons, overlapping, edge, or node neighbors occur only once between any two polygons. The tool only looks for edge and node neighbors (in that order) and the output does not contain the field AREA. Using polygon 1 as the source polygon for an example, three neighbor polygons are found, and the following information is reported in the output table below:
- Each of polygons 2 and 5 has a coincident edge with polygon 1; the length of the edge, 20, is written in the LENGTH field. The node neighbor analysis is skipped even though polygon 2 crosses polygon 1 at a point. The field NODE_COUNT gets a value of 0.
- Polygon 4 has a coincident edge with polygon 1; the length of the coincident edge, 100, is written in the LENGTH field.

####Overlaps#####
- A polygon covering the hole of another polygon
  - In this case, polygon 2 has a hole which is covered by polygon 1. Notice the two polygons do not overlap, so the analysis for overlapping neighbors is unnecessary. When polygon 1 is the source polygon and polygon 2 has a coincident edge of 200 with polygon 1, this value is written to the LENGTH field. The NODE_COUNT field value is 0. Similarly, when polygon 2 is the source polygon, polygon 1 has a coincident edge of 200 with polygon 2, which results in the same values in the LENGTH field for each record.

- A polygon completely overlapping another polygon
  - In this case, polygons 1 and 2 overlap each other. You need to check the Include area overlap check box in order for this neighboring relationship to be found in the analysis. For both polygon 1, being the source, and polygon 2, being the neighbor, and vice versa, the overlapping area of 2500 is reported in the output table below.
