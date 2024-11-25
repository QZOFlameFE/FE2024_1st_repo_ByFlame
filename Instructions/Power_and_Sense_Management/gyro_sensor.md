<div align = center style="display: flex; flex-direction: column; align-items: center; justify-content: center;">

![Color Sensor](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/EV3_Gyro_Sensor.png)
<p>EV3 Gyro Sensor(Serial Number: 45505-1)</p>
<p>electroscheme: <a href="https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/schemes/99380%20Gyro%20sensor.pdf">https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/schemes/99380%20Gyro%20sensor.pdf</a> </p> 
<p>Gyro sensor LEGO MINDSTORMS block instruction: <a href="https://ev3-help-online.api.education.lego.com/Education/en-us/page.html?Path=blocks%2FLEGO%2FGyro.html">https://ev3-help-online.api.education.lego.com/Education/en-us/page.html?Path=blocks%2FLEGO%2FGyro.html</a> </p>
</div>
We use gyro sensor to save robot's initial(starting) position and count its deviation in degrees. Its features for precise angular motion detection and orientation measurement. Its key characteristics include angular velocity measurement, allowing real-time detection of rotational movement in degrees per second (°/s), and cumulative angle tracking, which provides continuous and accurate measurement of changes in orientation. Its high responsiveness enables the detection of even minute rotational changes, making it suitable for applications requiring sensitivity to directional shifts. This sensor enables real-time data transmission and processing for advanced control algorithms.
In programm we use gyro sensor for tracing the robot position, and control the drive of the robot like turns and correction of the straight ride by PD and PID regulators. Especially it place specific role in steering control that is performed by PID regulator. The PD regulator traces robot's position in angles in comparison with robot's initial (starting) position.
</br>
Gyro sensor have a significant role in odometry, especially in math constructions when the angles are needed. Detailed information is in the <a href="https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/odometry.md">odometry</a> section.
