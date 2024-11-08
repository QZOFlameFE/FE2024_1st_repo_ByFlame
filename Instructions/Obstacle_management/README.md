<table>
<tr>
<th width=800>

![PixyMon configuration](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Pixy2_configuration.png)
</th>
</tr>
</table>

<table>
<tr>
<th width=800>

![PixyMon settings](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Settings_Pix2.png) 
</th>
</tr>
</table>
Every Pixy2 camera is unique, so the parameters that we have can be not relative to any other pixy2 camera. Also, the parameters need to be changed in different lighting conditions.

To set the pixy we click to "action" panel and "set signature" mode.

The main parameters of the Pixymon are signature range, camera brightness, max blocks, max blocks per signature, min block area. 

To view how Pixy2 camera track the block we click to "View" panel and then choose "blocks, video, detected pixels" mode. 

Also it is important to set "Block Filtering" to zero, and remove "Saturation" tick in "Camera" panel because it slows down block detection
<table>
<tr>
<th width=800>
  
![PixyMon view](https://github.com/QZOFlameFE/FE2024_1st_repo_ByFlame/blob/main/Instructions/Obstacle_management/Pixy2_view.png)
</th>
</tr>
</table>


</br> </br>
Pixy2 is a camera that can detect and view colors of the objects and their relative position and size. It is a powerful tool for obstacle detection as it recognizes road signs and parking in the obstacle challenge. To set it you need to follow this steps:
1) Download Pixymon v2
2) Set the "camera brightness" in settings
3) Set the signatures in "Action" field
4) Set the "View" field to "blocks, video, detected pixels"
5) Regulate "signature range" for every signature you have
6) Regulate "min block area"
