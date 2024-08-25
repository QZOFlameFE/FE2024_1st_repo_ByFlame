Pixy2 camera is a universal tool as it can work with EV3, arduino and raspberry. </br>
For the work in LEGO MINDSTORMS application you need to install "pixy block".
This block outputs: </br>
Signature id with the highest value of y coordinate </br>
camera's relative x coordinate of the object </br>
camera's relative y coordinate of the object </br>
relative width of the object </br>
relative height of the object </br>
angle of the object to camera </br>
<table>
<tr>
<th width=400>
  
![Pixy2 block](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Pixy2block.png)
</th>
</tr>
</table>

## Change of the driving direction
We use relative Y coordinate to detect if the last signature is green or red. If the robot views siqnature and it's y coordinate is high it is saved in variable named "last sign". 
## Parking position
To know where the parking is we also use pixy2 relative coordinates and odometry to know the parking zone's position.
## Bypassing obstacles
We use steering mechanism and pixy2 coordinates and connect them with linear function. So if the laps are close to robot linear function gives high values to steering mechanism's motor. 
