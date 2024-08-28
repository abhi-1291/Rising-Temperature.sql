SELECT Next_Weather.id
<br>
FROM Weather AS Next_Weather, Weather AS Previous_Weather
<br>
WHERE 
<br>
Next_Weather.temperature > Previous_Weather.temperature
<br>
AND Next_Weather.recordDate > Previous_Weather.recordDate
<br>
AND Next_Weather.recordDate - Previous_Weather.recordDate = 1;
