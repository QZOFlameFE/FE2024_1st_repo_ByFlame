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
  <img src="https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Team_photos/QZO_logoo.jpg">
</div>
</div>
</div>

# Contents 
* [**Mobility management**](#mobility-management)
  * [Chassis design and differential](#chassis-design-and-differential)
  * [Weight distribution](#weight-distribution)
  * [Camera position](#camera-position)
  * [Motor selection](#motor-selection)
* [**Power and Sense Management**](#power-and-sense-management)
  * [Sense Management](#sense-management)
  * [Power Management](#power-management)
* [**Obstacle management**](#obstacle-management)
* [**Pictures**](#pictures)
  * [Robot Photos](#robot-photos)
  * [Team Photos](#team-photos)
* [**Performance videos**](#performance-videos)
* [**Engineering factor**](#engineering-factor)
# <hr/>
<!-- 



-->
# Mobility Management
<p>   Our robot is designed by lego, especially we used LEGO MINDSTORMS Education Core Set(Serial number 45544) and other LEGO EV3 sets: EV3 Expansion Set, EV3 Homeschool Combo Pack and others. You can view all of the LEGO EV3 sets by this link: <a href="https://www.bricklink.com/catalogList.asp?catType=S&catString=166.59.800">https://www.bricklink.com/catalogList.asp?catType=S&catString=166.59.800</a>. Robot's wheels are taken from LEGO SPIKE Prime set and its expansion set(serial numbers 45678-1 and  45680-1). </p> </br>
  
<p>   For better stability we used differential with two motors at the rear axle and steering control as required in the rules, our robot's size is 19.5cm (length); 13.5cm(width) and 27cm(height). We constructed the robot as small as possible to fit into the parking area by the situation below: </p>

<div align=center>
<table>
<tr>
<th width=250>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/concepts/parking-situation.png) </br>
</th>
</tr>
</table>
</div>

### Chassis design and differential
The base of our chassis design comes from Ackerman steering model geometry. It improves maintainabiity of the robot as it controls the smoothness of the turns because of the maximum degrees of the steering can move
We have a differential in driving rear axle of our robot to make turns smoother. If robot turns one wheel will move slower than second and it reduces radius of the turn so our robot turn is controlled by 2 mechanisms: steering mechanism and differential.
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

### Weight distribution
  As our robot is a self-driving car with steering mechanism and differential in rear axle we need to make our robot slight heavy, and distribute weight a bit behind the center of our robot to prevent the wheels from slipping. The slipping of the wheels in rear axle impacts our odometry and the programm.
  
### Camera position
  Our camera places as much higher and behind as its possible for better view and obstacle control. It also inclined a bit down to view blocks that are close to robot and limit the view for better obstacle management.
</div>

### Motor selection
  We have a choice between 2 types of LEGO motors: large motor and medium motor, the large motor is powerful but the speed is lower, the medium motor is not that powerful but have a great speed. The comparison can be viewed by this link: <a href="https://www.eurobricks.com/forum/index.php?/forums/topic/87670-ev3-large-and-medium-motors-comparison/">https://www.eurobricks.com/forum/index.php?/forums/topic/87670-ev3-large-and-medium-motors-comparison/</a>. According to <a href="https://www.researchgate.net/publication/345182894_Dynamic_analysis_modeling_and_control_of_the_LEGO_EV3_modular_mobile_platform">research:</a> 
  
* Large servo motor (actuator) - maximum operating speed of 170 rpm, torque of 0.2 Nm and stopping torque of 0.4 Nm. It is positioned in the engine case an integrated encoder, a rotation meter, whose step is 1 degree of rotation and least sampling time 0.001 s.Also the power and speed is regulated by gear wheels and the size of the wheels. We choosed smaller wheels in steering mechanism because they do not move the robot, the only moves its trajectory.
* Medium-size servo motor - maximum speed of 250 rpm, running torque 0.08 Nm and stopping torque of 0.12 Nm, also with integrated encoder, identical to that of a large engine.
</br>
Also the wheels have low coefficient of friction to avoid loss of energy, but for wheels in the rear axles it will be better to choose wheels with a bit high cofficient of friction to avoid slipping of wheels. The rear wheels are bigger than wheels in front axle to have a better stability, movement control and the speed. It will be better to choose little smaller rear wheels than our. 
</br>
  The explanation of our construction design is on our youtube channel <a href="https://www.youtube.com/channel/UC0_5yZ2aPdJc0X5wtIw4ZcA">"QZO Flame" (tag: @QZOFlame)</a>.
   
   * [Building Instructions](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Building_Instructions/README.md)
   * [3D model of Pixy Camera_Case](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/3D_models/README.md)
# <hr/>
# Power and sense management </br>
## Power management </br>
  The core of our robot is <a href="#">EV3 Programmable Brick</a>, the power comes from a rechargable 10V Lithium Battery. EV3 P-Brick have 4 ports for motors and 4 ports for sensors.  Power consumption of motors and sensors: <a href="https://www.dexterindustries.com/ev3-current-consumption-measurement/">https://www.dexterindustries.com/ev3-current-consumption-measurement/</a>.
  <table>
<tr>
<th width=400>
  
  ![EV3 with ports for sensors and motors](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/EV3_P-Brick_demonstration.jpg)
</th>
</tr>
</table>

  * [Electroschemes/wiring diagrams](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/schemes/README.md)

  ### Comparison with other popular controllers
  
  <table>
    <tr>
      <th width=33%>
        
  ![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/EV3_P-Brick.png)
  
  EV3 P-Brick </th>
      <th width=33%>
        
  ![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/Arduino_UNO.jpeg)
        
  Arduino UNO 
      </th>
      <th width=33%> 
      
  ![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Power_and_Sense_Management/Raspberry_Pi_4B.png)
       
  Raspberry Pi </th>
    </tr> 
    <tr>
    <td colspan=3 align=center> processor </td>
    </tr>
    <tr>
      <td align=center> 300 MHz, 1 core </td>
      <td align=center> 16MHz </td>
      <td align=center> 1.5 GHz, 4 cores </td>
    </tr>
     <tr>
    <td colspan=3 align=center> ports </td>
    </tr>
    <tr>
      <td align=center> 4 ports for sensors, 4 ports for motors </td>
      <td align=center> 14 digital, 6 analog pins </td>
      <td align=center> 40 GPIO pins </td>
    </tr>
    <tr>
    <td colspan=3 align=center> programming </td>
    </tr>
    <tr>
      <td align=center> LEGO Mindstorms, limited Python and C++ </td>
      <td align=center> Arduino IDE (C, C++ based) </td>
      <td align=center> Multiple languages (Python, C++, Java, etc.) </td>
    </tr>
  </table>
  
  ### Limitations of LEGO Mindstorms
  <ul>
    <li> Block-programming makes hard to implement new features </li>
    <li>  </li>
  </ul>
  </br>
  </br>
  For the better Power and Sense management it would be better to switch on Raspberry Pi in spite of its abilities like more sensors and motors can be connected, unlimited programming and it does mot limit the choose in sensors and motors like LEGO EV3 P-Brick. 
   
## Sense management </br>
  UART sensors of LEGO EDUCATION MINDSTORMS EV3 Core Set such as color, ultrasonic and gyro sensors are used for sense management of our robot. </br>
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
# Obstacle management
  For the obstacle detection we used Pixy2 camera and PixyMon v2 application to configure it. To use it in LEGO MINDSTORMS application you need to install special library. All of the downloads are able in official site of Pixy2 <a href="https://pixycam.com/downloads-pixy2/">https://pixycam.com/downloads-pixy2/</a>. </br> </br>
<table>
<tr>
<th width=500>
  
  ![obstacle detection](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/obstacle_detection.png)
</th>
  <th width=500>
    
  ![obstacle detection](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Obstacle_detection1.png)
  </th>
  <tr>
    <th width=500>
      
  ![linear function](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/linear_function_convert.png)
</th>
  <th width=500>
    
  ![linear function](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/linear_function.png)
</table>
To calculate linear function we use this site: <a href="https://planetcalc.ru/8110/?ysclid=m0a3s77i4p794636345">https://planetcalc.ru/8110/?ysclid=m0a3s77i4p794636345</a>.
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
<th width=400>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_Management/Pixy_Block.png)
<p>
Pixy block for LEGO MINDSTORMS
</p>
</th>
</tr>
</table>
</div>

  * [Pixy2 camera's configuration](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/README.md)
  * [Programm part for obstacle detection](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Pixy_for_programm.md)

# <hr/>

# Pictures
### Robot photos

<table>
<tr>
  <th width=50%>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/forward.jpg)
  </th>
  <th width=50%>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/right.jpg)
  </th>
</tr>
<tr>
  <td width=50%>
    
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/back.jpg)
  </td>
  <td width=50%>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/left.jpg)
  </td>
</tr>
<tr>
  <td width=50%>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/down.jpg)
  </td>
  <td width=50%>

![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/top.jpg)
  </td>
</tr>
<tr>
  <td width=50%>
  
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Vehicle_photos/view.jpg)
  </td>
</tr>
</table>







## Team Photos
![alt text](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Team_photos/official-photos/Official_team_photo.jpeg?raw=true)
# <hr/>

<!-- 










-->
# Performance videos
### Open Challenge: https://www.youtube.com/watch?v=abwXTLdPtoA </br>
### Obstacle Challenge: https://www.youtube.com/watch?v=in7TNcsKKQ0 </br>
### Robot parts discussion: https://www.youtube.com/watch?v=4ONiXjtQosE </br>
# <hr/>



# Code explanation
The code is written in LEGO MINDSTORMS block programming and you can download and checl it <a href="#"> here</a>. 




# Conlusion
## Limitations

<table>
  <tr>
    <th align = center> Mobility Management </th>
    <td> 
    <ul>
      <li> LEGO motors, sensors and P-Brick are large in comparison with other electrical components </li>
      <li> LEGO EV3 set have limited opportunities like it is impossible to make Ackermann steering control geometry </li>
      <li> creating construction only by LEGO diminish </li>
    </ul>
    </td>
  </tr> 
    
  <tr>
    <th> Power and Sense Management </th>
    <td> <ul> 
      <li> 1 core CPU deprives multithreaded data processing and accuracy of sensor records. </li>
      <li> Only 4 ports for sensors and 4 ports for motors can be used. </li>
      <li> The Operating System of EV3 P-Brick is limited in functionality and flexibility. </li>
      <li> EV3 P-Brick have limited abilities in comparison with Raspberry Pi 4B that is a small computer. </li>
      <li> EV3 P-Brick is limited in source of motors and sensors since special firmware is needed for sensors and motors to interact with EV3 P-Brick. </li>
      <li> EV3 system has stopped in updates, and have some bugs like active bluetooth mode that sometimes interferes the operation of sensors </li> 
      <li> LEGO sensors are less accurate in comparison with other available sensors </li>
    </td>
  </tr>
      
  <tr>
    <th align = center> Obstacle Management </th>
    <td> <ul>
      <li> Pixy2 camera's quality is low (1.3 megapixels) </li>
      <li> Uses I2C that limits the sensor recordings to 60 times per second and lower </li>
      <li> Outputs only specified values </li>
      <li> Strong dependence on the lighting level </li>
    </td>
  </tr>
</table>

## Sugestions for further development
Since LEGO platform have numerous limitations it would be better to switch on Raspberry Pi's newest model. Raspberry Pi is a single board computer that affords the abilities to work with electronics. The main advantages by switching on Raspberry Pi would be the ability to use AI for detecting objects, using numerous and various sensors for better power and sense and obstacle managements. For the construction making it would be better to built own construction including the aspects of mechanical engineering, especially Ackermann Steering Geometry for smooth turns. Also it would be possible to make construction smaller and aerodynamic for better control and to fit into parking lot vertically as it is easier. Wheel selection is also an important factor, as better rubber on wheels prevents their slipping making the encoder values more accurate and improves traction. The smaller wheels for steering mechanism reduces the turn radius, and big wheels on rear axle improves the speed. Gears system regulates the torque and speed. For obstacle management choosing camera with greater resolution, better resistence to light changes and using AI technologies would improve the obtacle avoidance. Using more accurate sensors with more iterations per second would improve the sense management. Motors with more torque, RPM and damage resistance would improve the power and sense management.
<!-- 







-->
<!-- # Engineering Factor
### Construction making
  For our construction we used LEGO MINDSTORMS Education Set and wheels from LEGO SPIKE Prime Set as it conducts simple platform LEGO MINDSTORMS application for code, logic and powerful UART sensors as Gyro, Ultrasonic and Colorsensor for sense management and EV3 programmable brick as a main controller. </br>

  Pixy2 camera is a powerful tool with I2C communication protocol. It is used to distinguish colors of red, green blocks and parking in obstacle challenge, their position by relative coordinates and their relative sizes. It also has its own programm <u>PixyMon v2</u> for configuration of Pixy2 camera, with interactive interface including various settings. </br>
### Programming
  For the programming we used <a href="">LEGO MINDSTORMS</a> application. 
# <hr/>
