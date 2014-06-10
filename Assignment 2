##Assignment 2##

I have written below code to test the database connectivity

``` php

<?php
$con=mysqli_connect("localhost","kbadana","Changeme_1","kbadana");
// Check connection
if (mysqli_connect_errno()) {
  echo "Failed to connect to MySQL: " . mysqli_connect_error();
}

$result = mysqli_query($con,"SELECT * FROM Planets");

while($row = mysqli_fetch_array($result)) {
  echo $row['Name'] . "   " . $row['NumMoons'] . "   " . $row['Type'] . "   " . $row['LengthOfYear'];
  echo "<br>";
}

mysqli_close($con);
?>

```

Link to be checked for output of the database

```
http://cs2.mwsu.edu/~kbadana/DBTest/DBTest.php

```

###Output Displayed###

Mercury 0 Rocy 0.24
Venus 0 Rocy 0.62
Earth 1 Rocy 1.00
Mars 2 Rocy 1.88
Jupiter 16 Gas 11.86
Saturn 18 Gas 29.46
Pluto 1 Rocy 247.70
