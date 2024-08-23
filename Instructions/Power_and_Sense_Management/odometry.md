The Odomoetry is based in combine of all of the sensors that robot have. Ultrasonic measures distance to wall, gyro measures angle for math calculations, encoders measures the distance that robot moved, color sensor by specific math operations converts relative odometry to absolute odometry of the map.
# Relative Odometry
  Relative odometry is calculated by initial distance between robot and wall that measures by Ultrasonic sensor. That value is saved to variable named "fogX" and then, when the robot starts to move, encoders save the values of the distance that robot moved to the specific odometry loop that works in combine with gyro sensor. In this loop relatively previous value of the encoder is saved and compares with relatively current value of encoder and is substracted, lets name it "encoder change". The value that comes from gyro sensor lets name it "gyro angle" and the variable "gyro zero" that is the value that changes every time when robot turns. Number of turns named "Turn number" are calculated when the color sensor views a line, especially it counts only orange line numbers if the direction is clockwise and only blue line numbers if the direction is anticlockwise. "Gyro zero" is calculated like this: ["Turns number" * 90]. Then for comfortable calculations of odometry "gyro zero" substracts from "gyro angle". Now we can turn to odometry, the main formula for odometry is [("encoder change" * {sin or cos}("gyro angle" - "gyro zero"))/6.0770044]. 
  
## Explanation of the formula
  6.0770044 value comes from converting encoder's degrees and gear's cogs to centimeters. </br>
  the cos or sin is used for determinig x and y coordinates.
<table>
  <tr>
    <td width=400>
      
  ![odometry explanation](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/calculating_odometry.png)
    </td>
  </tr>
</table>
</br>

# Absolute odometry

![absolute odometry principle](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/absolute_odometry_principle.png) </br>
The relative odometry transfers to the absolute odometry when the color sensor views line. 
