# VerticalFarmingAutomation

A two semester capstone project. <br>


Our team is building a robot that traverse vertical farming environment to pollinate and harvest tomatotes.<br>
I was responsible for manipulation and project management in the Spring 22 semester. <br>
>* Use head camera to detect ArUco marker
>* Subscribe to the ArUco marker topic, which is a twist coordinate published
>* Extract a constant coordinate from the subscribed ArUco marker coordinates 
>* Implement inverse kinematics using move_to_pose() Stretch ROS package by
>    * Use TF2 to conduct homogeneous transformation for the coordinate viewed at the base link of the robot
>    * measure the distance between the base link of the robot and the end of the fully retracted telescopic armlink at its lowest lift height to calculate the offset
>    * Add the offset to the desired goal positions
>* Conudct direct offset calibration to improve in positional accuracy

I will be focusing on perception part in the Fall 22 semester. <br>

**Manipulation**<br>
![Manipulation](https://user-images.githubusercontent.com/92174982/182002189-2031ef27-5600-404f-bc1f-c63e55b1242c.gif)
