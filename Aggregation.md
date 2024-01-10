<h1>Weather Observation Station 15</h1>
<h3>Query the Western Longitude (LONG_W) for the largest Northern Latitude (LAT_N) in STATION that is less than 137.2345. Round your answer to 4 decimal places.</h3>
<pre>Select ROUND(LONG_W,4)
From STATION
Where LAT_N = (Select MAX(LAT_N)
              FROM Station
              Where LAT_N < 137.2345)</pre>
<br>
<br>

<h1>Weather Observation Station 16</h1>
<h3>Query the smallest Northern Latitude (LAT_N) from STATION that is greater than 38.7780. Round your answer to 4 decimal places.</h3>
<pre>
Select Round(Min(LAT_N),4)
From STATION
Where LAT_N > 38.7780
</pre>

<br><br>

<h1>Weather Observation Station 17</h1>
<h3>Query the Western Longitude (LONG_W)where the smallest Northern Latitude (LAT_N) in STATION is greater than 38.7780. Round your answer to 4 decimal places.</h3>
<pre>
Select Round(LONG_W,4)
From STATION
Where LAT_N = (Select Min(LAT_N)
               From Station
               Where LAT_N > 38.7780)
</pre>

<br><br>

<h1>Weather Observation Station 18</h1>
<h3>Query the Manhattan Distance between points P<sub>1</sub> and P<sub>2</sub> and round it to a scale of 4 decimal places.</h3>
<pre>
Select ROUND((MAX(LAT_N)-MIN(LAT_N)) + (MAX(LONG_W)-MIN(LONG_W)),4)
From STATION
</pre>

<br><br>

<h1>Weather Observation Station 19</h1>
<h3>Query the Euclidean Distance between points P<sub>1</sub> and P<sub>2</sub> and round it to a scale of 4 decimal places.</h3>
<pre>
Select ROUND(SQRT(POWER(MAX(LAT_N)-MIN(LAT_N),2) + POWER(MAX(LONG_W)-MIN(LONG_W),2)),4)
From STATION
</pre>

<br><br>

<h1>Weather Observation Station 20</h1>
<h3>A median is defined as a number separating the higher half of a data set from the lower half. Query the median of the Northern Latitudes (LAT_N) from STATION and round your answer to 4 decimal places.</h3>
<pre>

</pre>
