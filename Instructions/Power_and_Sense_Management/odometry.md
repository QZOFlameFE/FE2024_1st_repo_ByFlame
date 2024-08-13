The Odomoetry is based in combine of all of the sensors that robot have. Ultrasonic measures distance to wall, gyro measures angle for math calculations, encoders measures the distance that robot moved, color sensor by specific math operations converts relative odometry to absolute odometry of the map.
# Relative Odometry
  Relative odometry is calculated by initial distance between robot and wall that measures by Ultrasonic sensor. That value is saved to variable named "fogX" and then, when the robot starts to move, encoders save the values of the distance that robot moved to the specific odometry loop that works in combine with gyro sensor. In this loop relatively previous value of the encoder is saved and compares with relatively current value of encoder and is substracted, lets name it "encoder change". The value that comes from gyro sensor lets name it "gyro angle" and the variable "gyro zero" that is the value that changes every time when robot turns. Number of turns named "Turn number" are calculated when the color sensor views a line, especially it counts only orange line numbers if the direction is clockwise and only blue line numbers if the direction is anticlockwise. "Gyro zero" is calculated like this: ["Turns number" * 90]. Then for comfortable calculations of odometry "gyro zero" substracts from "gyro angle". Now we can turn to odometry, the main formula for odometry is [("encoder change" * {sin or cos}("gyro angle" - "gyro zero"))/6.0770044]. 
  
## Explanation of the formula


  and by the Pythagoras theorem is converted to coordinates change that is calculated as for x coordinate: "encoder change" multiplied to gyro sensor's angle substracted to angle that is calculated by the number of turns that robot made lets name it "gyro zero", for instance: if the robot made 1 turn "gyro zero" equals to 90, if the robot made 2 turns "gyro zero" equals to 180 and etc. Then the formula for x coordinate is: "encoder change" multipyied to gyro sensor's value substracted to "gyro zero" and all of that devided by 6.0770044 [("encoder change" * (gyro sensor's value - "gyro zero"))/6.0770044]. 




6.0770044 value comes to convert encoder's degrees to centimeters. 
