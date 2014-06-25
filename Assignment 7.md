## Assignment 7 ##

I have used within function to check out if the latitude and longitude in the volcanoes or earth_quakes table 
in shape of state_borders table. I have used Right outer join for displaying the data 

```SQL
SELECT state,sb.shape as Location,Vol.shape FROM `state_borders` as sb right outer join `volcanoes` as Vol ON contains(sb.shape,Vol.shape) where sb.state='California'
```


ouput:

Total Number of output rows displayed: 20


```SQL
SELECT state,sb.shape as Location,Vol.shape FROM `state_borders` as sb right outer join `earth_quakes` as Vol ON contains(sb.shape,Vol.shape) where sb.state='California'
```

ouput:

Total Number of output rows displayed: 2,210

Cross verification: 

I have checked these points in the maps and I have identified that all the points are centered in California

http://itouchmap.com/latlong.html


