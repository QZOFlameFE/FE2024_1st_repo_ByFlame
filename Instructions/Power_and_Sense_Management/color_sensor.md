<div align = center style="display: flex; flex-direction: column; align-items: center; justify-content: center;">

![Color Sensor](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/EV3_Color_Sensor.png)
<p>EV3 Color Sensor(Serial Number: 45506-1)</p>
<p>electroscheme: <a href="https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/schemes/95650%20Color%20sensor.pdf">https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/schemes/95650%20Color%20sensor.pdf</a> </p> 
<p>color sensor LEGO MINDSTORMS block instruction: <a href="https://ev3-help-online.api.education.lego.com/Education/en-us/page.html?Path=blocks%2FLEGO%2FColorSensor.html">https://ev3-help-online.api.education.lego.com/Education/en-us/page.html?Path=blocks%2FLEGO%2FColorSensor.html</a> </p>
[]()
</div>
Color sensor is used to determine driving direction of the round and robot's position in corner section or in straightforward section. It detects orange and blue colors of the lines, if the first color that robot viewed is orange the direction is clockwise and vice versa if the color is blue the direction is anticlockwise. For this purposes we used color sensor's rgb mode, if the color is white rgb is near to 255, 255, 255; if the color is blue the red value needs to be less than 120, if the color is orange blue and green values sum and subtracted by 40 needs to be lower than value of red. 
</br>
Also we use color sensor to convert relative odometry to absolute odometry that is limited by map size. Detailed information is in the <a href="https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/odometry.md">odometry</a> section.