## Assignment 2##

I have taken downloaded the zip file to current folder using the below command

```
wget http://thematicmapping.org/downloads/TM_WORLD_BORDERS-0.3.zip
```
Unzipped the file using the below command
```
unzip TM_WORLD_BORDERS-0.3.zip
```

```
ogr2ogr -f "MySQL" MySQL:"kbadana,host=localhost,user=kbadana,password=Changeme_1,port=3036" TM_WORLD_BORDERS-0.3.shp -nln World_Borders -update -overwrite -lco engine=MYISAM
```

This command imported the table into the database

###Table Structure###

``` SQL

CREATE TABLE IF NOT EXISTS `world_borders` (
  `OGR_FID` int(11) NOT NULL AUTO_INCREMENT,
  `SHAPE` geometry NOT NULL,
  `fips` varchar(2) DEFAULT NULL,
  `iso2` varchar(2) DEFAULT NULL,
  `iso3` varchar(3) DEFAULT NULL,
  `un` decimal(3,0) DEFAULT NULL,
  `name` varchar(50) DEFAULT NULL,
  `area` decimal(7,0) DEFAULT NULL,
  `pop2005` decimal(10,0) DEFAULT NULL,
  `region` decimal(3,0) DEFAULT NULL,
  `subregion` decimal(3,0) DEFAULT NULL,
  `lon` double(8,3) DEFAULT NULL,
  `lat` double(7,3) DEFAULT NULL,
  UNIQUE KEY `OGR_FID` (`OGR_FID`),
  SPATIAL KEY `SHAPE` (`SHAPE`)
) ENGINE=MyISAM  DEFAULT CHARSET=latin1 AUTO_INCREMENT=247 ;


```
