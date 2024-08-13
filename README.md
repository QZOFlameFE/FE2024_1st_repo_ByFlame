<!-- 
<table>
<tr>
<th width=250>
CONTENT
</th>
</tr>
</table>
-->

<div style="display: flex; flex-direction: column; align-items: center; justify-content: center;"
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;">
<h1 align = center> Future Engineers 2024 </h1>
<h2 align = center> Team name: QYZYLORDA Flame </h2>
<h2 align = center> Team members: Sadu Yernur, Appaz Aldiyar </h2>
<h2 align = center> email: qzo.flame.fe2024@gmail.com </h2>
<div style="display: flex; flex-direction: column; align-items: center; justify-content: center;"
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;">
<div align = center>
  <img src=https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Team_photos/QZO_Logo12.png> 
</div>
</div>
</div>

# Contents 
`3D_models` contains 3D models of the project <br/>
`Team_photos` contains team photos and creating process photos <br/>
`Vehicle_photos` contains vehicle photos from every side, of an each model and process <br/>
`programms` contains the code and programms to run the robot <br/>
`videos` contains videos that demonstrates how robot works and runs, explanation of its basic principles <br/>
`ideas`
> [!NOTE]
> dadasdadas
# <hr/>
<!-- 



-->
# Mobility Management
  Our robot is designed by lego, especially we used LEGO MINDSTORMS Education Core Set(Serial number 45544) and other LEGO EV3 sets: EV3 Expansion Set, EV3 Homeschool Combo Pack and others. You can view all of the LEGO EV3 sets by this link: <a href="https://www.bricklink.com/catalogList.asp?catType=S&catString=166.59.800">https://www.bricklink.com/catalogList.asp?catType=S&catString=166.59.800</a>. Robot's wheels are taken from LEGO SPIKE Prime set and its expansion set(serial numbers 45678-1 and  45680-1). </br>
For better stability we used differential with two motors and steering control as required in the rules, our robot's size is 19.5cm (length); 13.5cm(width) and 27cm(height). We constructed the robot as small as possible to fit into the parking area by the situation below:
<div align=center>
<table>
<tr>
<th width=250>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/concepts/parking-situation.png) </br>
</th>
</tr>
</table>
</div>

## Chassis design
The basic of our chassis design comes from Ackerman model. It improves robot's stability during turns, 
<table>
<tr>
<th width=250>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/concepts/Ackermann_simple_design.png)
</th>
</tr>
</table>

<table>
<tr>
<th colspan=1 rowspan=1>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Building_Instructions/Steering_control.png)
Our robot's steering control construction
</th>
<th colspan=2 rowspan=1>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Building_Instructions/Differential.png)
Our robot's differential at rear axle

</th>
</tr>
</table>

## Usage of differential
  We used differential for making smoother turns and 
</div>
  The explanation of our construction design is on our youtube channel <a href="https://www.youtube.com/channel/UC0_5yZ2aPdJc0X5wtIw4ZcA">"QZO Flame" (tag: @QZOFlame)</a>.
   
   * [Building Instructions](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Building_Instructions/README.md)
   * [3D model of Pixy Camera_Case](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/3D_models/README.md)
# <hr/>
<!-- 



-->
# Power and Sense Management </br>
## Power Management </br>
  The core of our robot is <a href="#">EV3 Programmable Brick</a>, the power comes from a rechargable 10V Lithium Battery. 
</br>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/tree/main/Instructions/Power_and_Sense_Management/EV3_P-Brick.png)
* [Electroschemes of sensors](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Building_Instructions/README.md)
* 
<!-- 




-->
## Sense Management </br>
  UART sensors of LEGO EDUCATION MINDSTORMS EV3 Core Set such as color, ultrasonic and gyro sensors are used for sense management of our robot.
  * [Lego sensors, electroshemes]()
  Gyro sensor is used to save initial robot position in degrees and count the deviation from it. Ultrasonic sensor measures the distance from robot to wall. Color sensor is used to know the driving direction of the round. Encoders in medium motors are used to know the distance that robot moved. Our programm uses mix of this sensors to create the odometry of our robot, by the usage of encoders, gyro sensor and Pythagoras theorem we calculate the displacement that robot moves from initial positions and convert it to x and y coordinates. Before the first line in first lap the odometry is relative to the robot's initial position and after the color sensor views the line it recognizes robot direction and by specific math formulas it converts relative odometry to full odometry of the map, the center of the map is the center of odometry where x and y coordinates are equal to zero. Ultrasonic sensor and Gyro sensor in combine used to fix odometry also by Pythagoras theorem and exceptions for the situations when ultrasonic sensor view blocks. The detailed infprmation of sense management will be below.
  * [color sensor](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/color_sensor.md)
  * [ultrasonic sensor](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/ultrasonic_sensor.md)
  * [gyro_sensor sensor](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/gyro_sensor.md)
  * [Pixy2 camera](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/Pixy2_camera.md)
  * [encoders from motors](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/encoders_from_motors.md)
  * [odometry](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/odometry.md)
# <hr/>
<!-- 

























-->
# Obstacle Management
  For the obstacle detection we used Pixy2 camera and PixyMon v2 application to configure it. To use it in LEGO MINDSTORMS application you need to install special library. All of the downloads are able in official site of Pixy2 <a href="https://pixycam.com/downloads-pixy2/">https://pixycam.com/downloads-pixy2/</a>.
</br>
<div align = center style="display: flex; flex-direction: column; align-items: center; justify-content: center; color: gray">

<table>
<tr>
<th width=250>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_Management/ICON%20PIxyMon%20v2.png)
<p> 
PixyMon v2 application
</p>
</th>
</tr>
</table>

<table>
<tr>
<th width=250>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_Management/Pixy_Block.png)
<p>
Pixy block for LEGO MINDSTORMS
</p>
</th>
</tr>
</table>
</div>
  * [Pixy2 camera's configuration]()
  * [Programm part for obstacle detection]()
![alt text](?raw=true)
# <hr/>
<!-- 



ENDED





-->
# Pictures
## Robot Photos

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/front_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/right_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/back_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/left_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/top_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/down_side.png?raw=true)
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/Front_right_side.png?raw=true)
## Team Photos
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Team_photos/official-photos/Official_team_photo.jpeg?raw=true)
# <hr/>
<!-- 










-->
# Performance videos
## Open Challenge: https://www.youtube.com/watch?v=abwXTLdPtoA </br>
## Obstacle Challenge: https://www.youtube.com/watch?v=MrlbhuZwWcI </br>
# <hr/>
<!-- 







-->
# Engineering Factor
  For our construction we used LEGO MINDSTORMS Education Set and wheels from LEGO SPIKE Prime Set as it conducts simple platform LEGO MINDSTORMS application for code, logic and powerful UART sensors as Gyro, Ultrasonic and Colorsensor for sense management and EV3 programmable brick as a main controller. </br>
  Pixy2 camera is a powerful tool with I2C communication protocol. It is used to distinguish colors of red, green blocks and parking in obstacle challenge, their position by relative coordinates and their relative sizes. It also has its own programm <u>PixyMon v2</u> for configuration of Pixy2 camera, with interactive interface including various settings. </br>
  Optic Fibre cables </br>  
  * [electroschemes of sensors](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Engineering_factor/README.md)
# <hr/>
