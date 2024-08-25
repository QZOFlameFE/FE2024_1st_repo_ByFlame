The Odomoetry is based in combine of all of the sensors that robot have. Ultrasonic measures distance to wall, gyro measures angle for math calculations, encoders measures the distance that robot moved, color sensor by specific math operations converts relative odometry to absolute odometry of the map.
# Relative Odometry
  Relative odometry is calculated by initial distance between robot and wall that measures by Ultrasonic sensor. That value is saved to variable named "fogX" and then, when the robot starts to move, encoders save the values of the distance that robot moved to the specific odometry loop that works in combine with gyro sensor. In this loop relatively previous value of the encoder is saved and compares with relatively current value of encoder and is substracted, lets name it "encoder change". The value that comes from gyro sensor lets name it "gyro angle" and the variable "gyro zero" that is the value that changes every time when robot turns. Number of turns named "Turn number" are calculated when the color sensor views a line, especially it counts only orange line numbers if the direction is clockwise and only blue line numbers if the direction is anticlockwise. "Gyro zero" is calculated like this: ["Turns number" * 90]. Then for comfortable calculations of odometry "gyro zero" substracts from "gyro angle". Now we can turn to odometry, the main formula for odometry is [("encoder change" * {sin or cos}("gyro angle" - "gyro zero"))/6.0770044]. 
  
## Explanation of the formula
  6.0770044 value comes from converting encoder's degrees and gear's cogs to centimeters. </br>
  the cos or sin is used for determinig x and y coordinates.
<table>
  <tr>
    <th width=400>

  ![odometry explanation](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/calculating_odometry.png) </br>
    </th>
  </tr>
</table>
<table>
  <tr>
    <th height=300>
    
  ![relative odometry programm part](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/relative_odometry.png) </br>
    </th>
  </tr>
  <tr>
    <th>
      
  ![relative odometry in programm](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/relative_odometry_programm.png) </br>
    </th>
  </tr>
</table>
</br>

# Absolute odometry
<table>
  <tr>
    <th width=1000>
      
![absolute odometry principle](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/absolute_odometry_principle.png) </br>
> [!NOTE]
> this is our XY coordinates for odometry

  </th>
  </tr>
</table>

<table>
  <tr>
    <th width=200>
      
![relative odometry to absolute odometry](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/relative_odometry_to_absolute_odometry.png) 
> [!NOTE]
> this is a part of programm where relative odometry transfers to absolute odometry

 </th>
  </tr>
</table>

<table>
  <tr>
    <th width=200>

![absolute odometry in programm](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/absolute_odometry_in_programm.png) </br>
> [!NOTE]
> part of programm where absolute odometry compiles

 </th>
  </tr>
</table>
When color sensor detects the line relative odometry transfers to absolute odometry with  coordinates center in center of the map. The principle is the x coordinate of the relative odometry by specific math operations transfers to full odometry. When the driving direction is clockwise we substract 100 from relative odometry's X coordinate and by linear function of the orange line in the map we transfer relative odometry to absolute odometry. If the driving direction is anticlockwise we sum 100 with relative odometry's X coordinate and with linear function of the blue line of the map we get absolute odometry.

## Usage of odometry in programm
### Aligning robot to the center
To align robot to the center of the straightforward zone. It is great to aligning robot to the center of the road for the Pixy2 camera to attach better view. 
### Avoid crash
Also we use odometry to detect the coordinates of pillars (red and green signs). If robot is too close to the pillars odometry helps to avoid accident and robot by gyro sensor and specific programm robot moves to the back. it works only between corner and straightforward zones to avoid collision with pillars in the back of the robot.
# Aligning odometry
<table>
  <tr>
    <th width=200>
      
![aligning odometry in the programm](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/aligning_odometry_in_programm.png)
    </th>
  </tr>
</table>
Odometry is a complex principle that can lose its accuracy over time, therefore, in order for our odometry to be accurate, we correct it with the help of ultrasonic and gyro sensor
